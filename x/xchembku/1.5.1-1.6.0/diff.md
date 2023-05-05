# Comparing `tmp/xchembku-1.5.1.tar.gz` & `tmp/xchembku-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.5.1.tar", last modified: Wed May  3 05:00:35 2023, max compression
+gzip compressed data, was "xchembku-1.6.0.tar", last modified: Fri May  5 11:38:07 2023, max compression
```

## Comparing `xchembku-1.5.1.tar` & `xchembku-1.6.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 05:00:25.000000 xchembku-1.5.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-03 05:00:25.000000 xchembku-1.5.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.386099 xchembku-1.5.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-03 05:00:25.000000 xchembku-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-03 05:00:25.000000 xchembku-1.5.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 05:00:25.000000 xchembku-1.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 05:00:25.000000 xchembku-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-03 05:00:35.402099 xchembku-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-03 05:00:25.000000 xchembku-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 05:00:25.000000 xchembku-1.5.1/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.386099 xchembku-1.5.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-03 05:00:25.000000 xchembku-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:00:35.402099 xchembku-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_well_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_soakdb3_crystal_well.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 11:37:56.000000 xchembku-1.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-05 11:37:56.000000 xchembku-1.6.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.056967 xchembku-1.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 11:37:56.000000 xchembku-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-05 11:37:56.000000 xchembku-1.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:37:56.000000 xchembku-1.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:37:56.000000 xchembku-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-05 11:38:07.072968 xchembku-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 11:37:56.000000 xchembku-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 11:37:56.000000 xchembku-1.6.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-05 11:37:56.000000 xchembku-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:38:07.072968 xchembku-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:38:06.000000 xchembku-1.6.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_droplocation1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_droplocation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_soakdb3_crystal_well.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_swiss3.py
```

### Comparing `xchembku-1.5.1/.dae-devops/Makefile` & `xchembku-1.6.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/conventions.rst` & `xchembku-1.6.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/developing.rst` & `xchembku-1.6.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/devops.rst` & `xchembku-1.6.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/docs_structure.rst` & `xchembku-1.6.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/installing.rst` & `xchembku-1.6.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/docs/testing.rst` & `xchembku-1.6.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.dae-devops/project.yaml` & `xchembku-1.6.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.devcontainer/Dockerfile` & `xchembku-1.6.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.devcontainer/devcontainer.json` & `xchembku-1.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/CONTRIBUTING.rst` & `xchembku-1.6.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/actions/install_requirements/action.yml` & `xchembku-1.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/dependabot.yml` & `xchembku-1.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/pages/make_switcher.py` & `xchembku-1.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/workflows/code.yml` & `xchembku-1.6.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/workflows/docs.yml` & `xchembku-1.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/workflows/docs_clean.yml` & `xchembku-1.6.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.github/workflows/linkcheck.yml` & `xchembku-1.6.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.gitignore` & `xchembku-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.gitlab-ci.yml` & `xchembku-1.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/.vscode/launch.json` & `xchembku-1.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/LICENSE` & `xchembku-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/PKG-INFO` & `xchembku-1.6.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.5.1
+Version: 1.6.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.5.1/README.rst` & `xchembku-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/configurations/development.yaml` & `xchembku-1.6.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/conf.py` & `xchembku-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/images/dls-favicon.ico` & `xchembku-1.6.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/images/dls-logo.svg` & `xchembku-1.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/index.rst` & `xchembku-1.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.6.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/docs/user/index.rst` & `xchembku-1.6.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/pyproject.toml` & `xchembku-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.6.0/src/xchembku.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.5.1
+Version: 1.6.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.5.1/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.6.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,12 +106,13 @@
 src/xchembku_lib/datafaces/direct_crystal_wells.py
 src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_crystal_plate.py
 tests/test_crystal_well_autolocation.py
-tests/test_crystal_well_droplocation.py
+tests/test_crystal_well_droplocation1.py
+tests/test_crystal_well_droplocation2.py
 tests/test_soakdb3_crystal_well.py
 tests/test_swiss3.py
 tests/configurations/direct.yaml
 tests/configurations/service.yaml
```

### Comparing `xchembku-1.5.1/src/xchembku_api/context_base.py` & `xchembku-1.6.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/interface.py` & `xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/interface.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.6.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/datafaces/context.py` & `xchembku-1.6.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.6.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/exceptions.py` & `xchembku-1.6.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.6.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.6.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.6.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.6.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.6.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Model containing well information formed from a composite query of droplocation information.
 
     Typically this structure is returned by queries.
     """
 
     # Stuff from the original record.
     uuid: str
+    crystal_plate_uuid: str
     position: str
     filename: str
     width: Optional[int]
     height: Optional[int]
     error: Optional[str]
     created_on: str
```

### Comparing `xchembku-1.5.1/src/xchembku_cli/main.py` & `xchembku-1.6.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_cli/subcommands/base.py` & `xchembku-1.6.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_cli/subcommands/service.py` & `xchembku-1.6.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_cli/version.py` & `xchembku-1.6.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/__main__.py` & `xchembku-1.6.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/contexts/base.py` & `xchembku-1.6.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/swiss3.py` & `xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/swiss3.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.6.0/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/databases/databases.py` & `xchembku-1.6.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/databases/normsql.py` & `xchembku-1.6.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.6.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
                 self.fields[field_name] = {"type": sql_type}
 
         # Remove attribute of the model that doesn't get stored in the database.
         self.fields.pop("crystal_coordinates")
 
         # Add indexes.
         self.fields["crystal_well_uuid"]["index"] = True
+        self.fields["number_of_crystals"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellDroplocationsTable(TableDefinition):
     # ----------------------------------------------------------------------------------------
     def __init__(self):
```

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/context.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,19 @@
             where = "AND"
 
         if filter.barcode is not None:
             query += f"\n{where} barcode = ?"
             subs.append(filter.barcode)
             where = "AND"
 
+        if filter.visit is not None:
+            query += f"\n{where} visit = ?"
+            subs.append(filter.visit)
+            where = "AND"
+
         if filter.from_formulatrix__plate__id is not None:
             if filter.direction == -1:
                 query += f"\n{where} formulatrix__plate__id < ?"
             else:
                 query += f"\n{where} formulatrix__plate__id > ?"
             subs.append(filter.from_formulatrix__plate__id)
             where = "AND"
```

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import copy
 import logging
 from typing import Any, Dict, List
 
 from dls_normsql.constants import CommonFieldnames
 
-from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
+from xchembku_api.models.crystal_well_filter_model import (
+    CrystalWellFilterModel,
+    CrystalWellFilterSortbyEnum,
+)
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 from xchembku_api.models.crystal_well_needing_droplocation_model import (
     CrystalWellNeedingDroplocationModel,
 )
 from xchembku_lib.datafaces.direct_base import DirectBase
 
 logger = logging.getLogger(__name__)
@@ -173,127 +176,262 @@
         return records
 
     # ----------------------------------------------------------------------------------------
     async def fetch_crystal_wells_needing_droplocation(
         self, filter: CrystalWellFilterModel, why=None
     ) -> List[CrystalWellNeedingDroplocationModel]:
         """
-        Wells need a droplocation if they have an autolocation but no droplocation.
+        Wells need a droplocation if they have an autolocation.
+        """
+
+        # Caller wants results relative to anchor?
+        if filter.anchor is not None and filter.direction is not None:
+            return await self.__fetch_crystal_wells_needing_droplocation_hard(
+                filter, why=why
+            )
+        # Query can be made easier if there is no anchor with direction involved.
+        else:
+            return await self.__fetch_crystal_wells_needing_droplocation_easy(
+                filter, why=why
+            )
+
+    # ----------------------------------------------------------------------------------------
+    async def __fetch_crystal_wells_needing_droplocation_easy(
+        self, filter: CrystalWellFilterModel, why=None
+    ) -> List[CrystalWellNeedingDroplocationModel]:
+        """
+        Wells need a droplocation if they have an autolocation.
         """
 
+        if why is None:
+            why = "API fetch_crystal_wells_needing_droplocation"
+
+        # Build the individual pieces of the SQL query.
         subs: List[Any] = []
+        orderby = self.__build_orderby(filter)
+        where = self.__build_where(filter, subs)
+        fields = self.__build_fields(filter)
+        joins = self.__build_joins(filter)
 
-        created_on = CommonFieldnames.CREATED_ON
+        # Glue them together.
+        main_query = "\nSELECT" + fields + joins + where + "\n" + orderby
 
-        where = "WHERE"
+        if filter.limit is not None:
+            main_query += f"\nLIMIT {filter.limit}"
+
+        # Query the database.
+        records = await self.query(main_query, subs=subs, why=why)
+
+        # Parse the records returned by sql into models.
+        models = [CrystalWellNeedingDroplocationModel(**record) for record in records]
+
+        return models
+
+    # ----------------------------------------------------------------------------------------
+    async def __fetch_crystal_wells_needing_droplocation_hard(
+        self, filter: CrystalWellFilterModel, why=None
+    ) -> List[CrystalWellNeedingDroplocationModel]:
+        """
+        This is the query when we want records relative from an anchor record.
+
+        Since this involves complex subqueries, we limit use of this
+        to when we're looking only at records in a specific visit or plate.
+        """
+
+        if filter.visit is None:
+            raise RuntimeError(
+                "programming error: no visit supplied with relative crystal well filter"
+            )
 
         if why is None:
             why = "API fetch_crystal_wells_needing_droplocation"
 
-        query = (
-            "\nSELECT crystal_wells.*,"
+        # Build the individual pieces of the SQL query.
+        subs: List[Any] = []
+        orderby = self.__build_orderby(filter)
+        where = self.__build_where(filter, subs)
+        fields = self.__build_fields(filter)
+        joins = self.__build_joins(filter)
+
+        # We need the row number to be in both the main and sub query.
+        row_number = f"\n  ROW_NUMBER() OVER ({orderby}) AS ordered_row_number"
+        fields = row_number + "," + fields
+
+        # Main query gets the actual results.
+        main_query = "SELECT" + fields + joins + where
+
+        # Build another "where" since it may add subs.
+        where = self.__build_where(filter, subs)
+
+        # Sub query computes row_numbers under the same filter in the same order as the main query.
+        sub_query = "\nSELECT\n  crystal_wells.uuid," + row_number + joins + where
+
+        # Do the main query, but filter the results by the subquery based on matching row numbers.
+        full_query = (
+            f"\nSELECT * FROM (\n{main_query}\n) AS main_query"
+            f"\n/* Match row_numbers starting from the anchor {filter.anchor}. */"
+            "\nWHERE ordered_row_number >"
+            f"\n  (SELECT ordered_row_number FROM ({sub_query}\n) AS sub_query"
+            f"\n    WHERE sub_query.uuid = ?)"
+            f"\n    ORDER BY ordered_row_number"
+        )
+        subs.append(filter.anchor)
+
+        if filter.limit is not None:
+            full_query += f"\nLIMIT {filter.limit}"
+
+        # Do the actual query.
+        records = await self.query(full_query, subs=subs, why=why)
+
+        # Parse the records returned by sql into models.
+        models = [CrystalWellNeedingDroplocationModel(**record) for record in records]
+
+        return models
+
+    # ----------------------------------------------------------------------------------------
+    def __build_fields(
+        self,
+        filter: CrystalWellFilterModel,
+    ) -> str:
+        """
+        Wells need a droplocation if they have an autolocation.
+        """
+
+        fields = (
+            "\n  crystal_wells.*,"
             "\n  crystal_well_autolocations.auto_target_x,"
             "\n  crystal_well_autolocations.auto_target_y,"
             "\n  crystal_well_autolocations.well_centroid_x,"
             "\n  crystal_well_autolocations.well_centroid_y,"
             "\n  crystal_well_autolocations.drop_detected,"
             "\n  crystal_well_autolocations.number_of_crystals,"
             "\n  crystal_well_droplocations.confirmed_target_x,"
             "\n  crystal_well_droplocations.confirmed_target_y,"
             "\n  crystal_well_droplocations.confirmed_microns_x,"
             "\n  crystal_well_droplocations.confirmed_microns_y,"
             "\n  crystal_well_droplocations.is_usable,"
             "\n  crystal_plates.visit,"
             "\n  crystal_plates.thing_type AS crystal_plate_thing_type"
+        )
+
+        return fields
+
+    # ----------------------------------------------------------------------------------------
+    def __build_joins(
+        self,
+        filter: CrystalWellFilterModel,
+    ) -> str:
+        """
+        Wells need a droplocation if they have an autolocation.
+        """
+
+        joins = (
             "\nFROM crystal_wells"
             "\nJOIN crystal_well_autolocations ON crystal_well_autolocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_well_droplocations ON crystal_well_droplocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_plates ON crystal_plates.uuid = crystal_wells.crystal_plate_uuid"
         )
 
+        return joins
+
+    # ----------------------------------------------------------------------------------------
+    def __build_where(
+        self,
+        filter: CrystalWellFilterModel,
+        subs: List[Any],
+    ) -> str:
+        """
+        Wells need a droplocation if they have an autolocation.
+        """
+
+        where = "WHERE"
+        sql = ""
+
         # Caller wants a glob of file?
         if filter.filename_pattern is not None:
-            query += (
+            sql += (
                 "\n/* Just certain filenames. */"
                 f"\n{where} crystal_wells.filename GLOB ?"
             )
             subs.append(filter.filename_pattern)
             where = "AND"
 
         # Caller wants specific barcode?
         if filter.barcode is not None:
-            query += (
-                f"\n/* Just a wells on plates with barcode '{filter.barcode}'. */"
+            sql += (
+                f"\n/* Just wells on plate with barcode '{filter.barcode}'. */"
                 f"\n{where} crystal_plates.barcode = ?"
             )
             subs.append(filter.barcode)
             where = "AND"
 
         # Caller wants specific visit?
         if filter.visit is not None:
-            query += (
-                f"\n/* Just a wells on plates with visit '{filter.visit}'. */"
+            sql += (
+                f"\n/* Just wells on plates with visit '{filter.visit}'. */"
                 f"\n{where} crystal_plates.visit = ?"
             )
             subs.append(filter.visit)
             where = "AND"
 
         # Caller wants only those not yet decided?
         if filter.is_decided is False:
-            query += (
+            sql += (
                 "\n/* Include only crystal wells which have not had a decision made. */"
                 f"\n{where} crystal_well_droplocations.is_usable IS NULL"
             )
             where = "AND"
 
         # Caller wants only those which are decided?
         # Confirmed means a droplocation record has been created at all (though might not have usable coordinates).
         if filter.is_decided is True:
-            query += (
+            sql += (
                 "\n/* Include only crystal wells which have a decision made. */"
                 f"\n{where} crystal_well_droplocations.is_usable IS NOT NULL"
             )
             where = "AND"
 
         # Caller wants only those which are decided but do or don't have usable coordinates?
         if filter.is_usable is not None:
-            query += (
+            sql += (
                 f"\n/* Include only crystal wells which have filter.is_usable = {filter.is_usable}. */"
                 f"\n{where} crystal_well_droplocations.is_usable = ?"
             )
             subs.append(filter.is_usable)
             where = "AND"
 
-        # Caller wants results relative to anchor?
-        if filter.anchor is not None:
-            # Caller wants the anchor itself?
-            if filter.direction is None:
-                query += (
-                    "\n/* Get the crystal well at the anchor. */"
-                    f"\n{where} crystal_wells.uuid = ?"
-                )
-            # Not the anchor itself, but either side of the anchor?
-            else:
-                op = ">"
-                if filter.direction == -1:
-                    op = "<"
-                query += (
-                    f"\n/* Get the crystal well(s) starting from the anchor {filter.anchor}. */"
-                    f"\n{where} crystal_wells.created_on {op} (SELECT {created_on} FROM crystal_wells WHERE uuid = ?)"
-                )
+        # Caller wants just the anchor record?
+        if filter.anchor is not None and filter.direction is None:
+            sql += (
+                "\n/* Get the crystal well at the anchor. */"
+                f"\n{where} crystal_wells.uuid = ?"
+            )
             subs.append(filter.anchor)
 
-        sql_direction = "ASC"
-        if filter.direction == -1:
-            sql_direction = "DESC"
+        return sql
 
-        query += f"\nORDER BY crystal_wells.{created_on} {sql_direction}"
+    # ----------------------------------------------------------------------------------------
+    def __build_orderby(
+        self,
+        filter: CrystalWellFilterModel,
+    ) -> str:
 
-        if filter.limit is not None:
-            query += f"\nLIMIT {filter.limit}"
+        sql = ""
 
-        records = await self.query(query, subs=subs, why=why)
+        position_direction = "ASC"
+        if filter.direction == -1:
+            position_direction = "DESC"
 
-        # Parse the records returned by sql into models.
-        models = [CrystalWellNeedingDroplocationModel(**record) for record in records]
+        # Filter says order by number of crystals?
+        if filter.sortby == CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS:
+            crystals_direction = "DESC"
+            if filter.direction == -1:
+                crystals_direction = "ASC"
+
+            # If duplicate crystals, use position as tie breaker.
+            order_by = f"crystal_well_autolocations.number_of_crystals {crystals_direction}, crystal_wells.position {position_direction}"
+        else:
+            order_by = f"crystal_wells.position {position_direction}"
 
-        return models
+        sql += f"ORDER BY {order_by}"
+
+        return sql
```

### Comparing `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/src/xchembku_lib/version.py` & `xchembku-1.6.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/base.py` & `xchembku-1.6.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/configurations/direct.yaml` & `xchembku-1.6.0/tests/configurations/direct.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/configurations/service.yaml` & `xchembku-1.6.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/conftest.py` & `xchembku-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/test_crystal_plate.py` & `xchembku-1.6.0/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/test_crystal_well_autolocation.py` & `xchembku-1.6.0/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/test_crystal_well_droplocation.py` & `xchembku-1.6.0/tests/test_crystal_well_droplocation1.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,53 +28,53 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocationDirect:
+class TestCrystalWellDroplocation1Direct:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         configuration_file = "tests/configurations/direct.yaml"
-        CrystalWellDroplocationTester().main(
+        CrystalWellDroplocation1Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocationService:
+class TestCrystalWellDroplocation1Service:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
         configuration_file = "tests/configurations/service.yaml"
-        CrystalWellDroplocationTester().main(
+        CrystalWellDroplocation1Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
-class CrystalWellDroplocationTester(Base):
+class CrystalWellDroplocation1Tester(Base):
     """
     Class to test the dataface droplocation-related endpoints.
     """
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
         self.__injected_count = 0
@@ -139,14 +139,33 @@
         models.append(await self.__inject(dataface, False, False))
         models.append(await self.__inject(dataface, True, True))
         models.append(await self.__inject(dataface, True, False))
         models.append(await self.__inject(dataface, True, True))
         models.append(await self.__inject(dataface, True, True))
         models.append(await self.__inject(dataface, True, False))
 
+        # --------------------------------------------------------------------------
+        # Query for list from filename glob.
+        crystal_well_models = await self.__check(
+            dataface,
+            CrystalWellFilterModel(filename_pattern="*A_1.jpg"),
+            3,
+            "filename glob",
+            filename="02A_1.jpg",
+        )
+
+        assert (
+            crystal_well_models[1].filename == "03A_1.jpg"
+        ), "filename glob, second response"
+        assert (
+            crystal_well_models[2].filename == "04A_1.jpg"
+        ), "filename glob, third response"
+
+        # --------------------------------------------------------------------------
+
         # Check the filtered queries.
         await self.__check(dataface, CrystalWellFilterModel(), 5, "no limit, all")
 
         # Upsert all with the same values to make sure it doesn't make new records.
         records = await dataface.query(
             "SELECT * FROM crystal_well_droplocations",
             why="[UPSCHK] direct query all drop locations",
@@ -177,77 +196,89 @@
         await self.__check(
             dataface, CrystalWellFilterModel(is_decided=False), 2, "unconfirmed only"
         )
 
         # Check the anchor query forward.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(anchor=models[3].uuid, direction=1, limit=1),
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                anchor=models[3].uuid,
+                direction=1,
+                limit=1,
+            ),
             1,
             "anchored forward",
-            filename="004b.jpg",
+            filename="05B_1.jpg",
         )
 
         # Check the anchor query forward at the end of the list.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(anchor=models[5].uuid, direction=1),
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                anchor=models[5].uuid,
+                direction=1,
+            ),
             0,
             "anchored forward at the end of the list",
         )
 
         # Check the anchor query backward.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(anchor=models[2].uuid, direction=-1),
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                anchor=models[2].uuid,
+                direction=-1,
+                limit=1,
+            ),
             1,
             "anchored backward",
-            filename="001a.jpg",
+            filename="02A_1.jpg",
         )
 
         # Check the anchor query backward at the start of the list.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(anchor=models[1].uuid, direction=-1),
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                anchor=models[1].uuid,
+                direction=-1,
+            ),
             0,
             "anchored at the start of the list",
         )
 
         # Check the anchor query backward at the start of the list of those unconfirmed.
         await self.__check(
             dataface,
             CrystalWellFilterModel(
-                is_decided=False, anchor=models[1].uuid, direction=-1
+                is_decided=False,
+                visit=self.__visit,
+                anchor=models[1].uuid,
+                direction=-1,
             ),
             0,
             "anchored at the start of the list, backward, unconfirmed",
         )
 
         # Check the anchor query backward at the start of the list of those unconfirmed.
         await self.__check(
             dataface,
             CrystalWellFilterModel(
-                is_decided=False, anchor=models[2].uuid, direction=-1
+                is_decided=False,
+                visit=self.__visit,
+                anchor=models[2].uuid,
+                direction=-1,
             ),
             0,
             "anchored at the start of the list, forward unconfirmed",
         )
 
-        # Query for list from filename glob.
-        crystal_well_models = await self.__check(
-            dataface,
-            CrystalWellFilterModel(filename_pattern="*a.jpg"),
-            3,
-            "filename glob",
-            filename="001a.jpg",
-        )
-
-        assert crystal_well_models[1].filename == "002a.jpg"
-        assert crystal_well_models[2].filename == "003a.jpg"
-
         # --------------------------------------------------------------------------
         # Check the usable queries.
         await self.__check(
             dataface,
             CrystalWellFilterModel(is_decided=True, is_usable=False),
             0,
             "confirmed but unusable only (1)",
@@ -299,37 +330,38 @@
         )
 
     # ----------------------------------------------------------------------------------------
 
     async def __inject(self, dataface, autolocation: bool, droplocation: bool):
         """ """
 
-        letter = "a"
+        letter = "A"
         if self.__injected_count > 3:
-            letter = "b"
+            letter = "B"
 
-        filename = "%03d%s.jpg" % (self.__injected_count, letter)
         self.__injected_count += 1
+        filename = "%02d%s_1.jpg" % (self.__injected_count, letter)
+        position = "%s%02da" % (letter, self.__injected_count)
 
         # Create the well object.
         m = CrystalWellModel(
-            position="01A_1",
+            position=position,
             crystal_plate_uuid=self.__crystal_plate_model.uuid,
             crystal_plate_thing_type=self.__crystal_plate_model.thing_type,
             filename=filename,
         )
 
         # Write well record.
         await dataface.upsert_crystal_wells([m])
 
         if autolocation:
             # Add a crystal well autolocation.
             ta = CrystalWellAutolocationModel(
                 crystal_well_uuid=m.uuid,
-                number_of_crystals=10,
+                number_of_crystals=self.__injected_count,
                 well_centroid_x=100,
                 well_centroid_y=100,
             )
 
             await dataface.originate_crystal_well_autolocations([ta])
 
         if droplocation:
@@ -361,14 +393,17 @@
         crystal_well_models = await dataface.fetch_crystal_wells_needing_droplocation(
             filter
         )
 
         # Make sure we got enough.
         assert len(crystal_well_models) == expected, note
 
+        if filename is not None:
+            assert crystal_well_models[0].filename == filename, f"{note} filename"
+
         for crystal_well_model in crystal_well_models:
             # All wells should belong to the visit.
             assert crystal_well_model.visit == self.__visit, f"{note} visit"
 
             # All present confirmed drop locations should be consistent.
             if (
                 crystal_well_model.well_centroid_x is not None
@@ -385,11 +420,8 @@
                     crystal_well_model.dict()
                 )
                 assert crystal_well_model.confirmed_target_x == 150
                 assert crystal_well_model.confirmed_microns_x == microns_x
                 assert crystal_well_model.confirmed_target_y == 50
                 assert crystal_well_model.confirmed_microns_y == microns_y
 
-        if filename is not None:
-            assert crystal_well_models[0].filename == filename, f"{note} filename"
-
         return crystal_well_models
```

### Comparing `xchembku-1.5.1/tests/test_soakdb3_crystal_well.py` & `xchembku-1.6.0/tests/test_soakdb3_crystal_well.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.1/tests/test_swiss3.py` & `xchembku-1.6.0/tests/test_swiss3.py`

 * *Files identical despite different names*

