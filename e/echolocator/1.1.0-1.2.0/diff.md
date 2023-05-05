# Comparing `tmp/echolocator-1.1.0.tar.gz` & `tmp/echolocator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.1.0.tar", last modified: Tue May  2 11:09:31 2023, max compression
+gzip compressed data, was "echolocator-1.2.0.tar", last modified: Fri May  5 11:50:45 2023, max compression
```

## Comparing `echolocator-1.1.0.tar` & `echolocator-1.2.0.tar`

### file list

```diff
@@ -1,228 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-02 11:09:23.000000 echolocator-1.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-02 11:09:23.000000 echolocator-1.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 11:09:23.000000 echolocator-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-02 11:09:23.000000 echolocator-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 11:09:23.000000 echolocator-1.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:09:23.000000 echolocator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-02 11:09:23.000000 echolocator-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-02 11:09:31.688869 echolocator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 11:09:23.000000 echolocator-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-02 11:09:23.000000 echolocator-1.1.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/diagrams/3drop_texrank_coordinates.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-02 11:09:23.000000 echolocator-1.1.0/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-02 11:09:23.000000 echolocator-1.1.0/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-02 11:09:23.000000 echolocator-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:09:31.688869 echolocator-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/box/
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/image_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.html
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_fetch_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 11:50:37.000000 echolocator-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-05 11:50:37.000000 echolocator-1.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.769450 echolocator-1.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 11:50:37.000000 echolocator-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 11:50:37.000000 echolocator-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:50:37.000000 echolocator-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:50:37.000000 echolocator-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-05 11:50:37.000000 echolocator-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-05 11:50:45.789451 echolocator-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 11:50:37.000000 echolocator-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-05 11:50:37.000000 echolocator-1.2.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/1_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials/101_run_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials/102_update_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/2_how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/2_how-to/201_add_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/2_how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/3_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations/301_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations/302_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/4_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/4_reference/402_building_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/4_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/diagrams/3drop_texrank_coordinates.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/image_details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/image_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/swiss3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-05 11:50:37.000000 echolocator-1.2.0/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 11:50:37.000000 echolocator-1.2.0/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-05 11:50:37.000000 echolocator-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:50:45.789451 echolocator-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.769450 echolocator-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_export_to_soakdb3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_fetch_images.py
```

### Comparing `echolocator-1.1.0/.dae-devops/Makefile` & `echolocator-1.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/conventions.rst` & `echolocator-1.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/developing.rst` & `echolocator-1.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/devops.rst` & `echolocator-1.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/docs_structure.rst` & `echolocator-1.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/installing.rst` & `echolocator-1.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/docs/testing.rst` & `echolocator-1.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.dae-devops/project.yaml` & `echolocator-1.2.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.devcontainer/Dockerfile` & `echolocator-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.devcontainer/devcontainer.json` & `echolocator-1.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/CONTRIBUTING.rst` & `echolocator-1.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/actions/install_requirements/action.yml` & `echolocator-1.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/dependabot.yml` & `echolocator-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/pages/make_switcher.py` & `echolocator-1.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/workflows/code.yml` & `echolocator-1.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/workflows/docs.yml` & `echolocator-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/workflows/docs_clean.yml` & `echolocator-1.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.github/workflows/linkcheck.yml` & `echolocator-1.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.gitignore` & `echolocator-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.gitlab-ci.yml` & `echolocator-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/.vscode/launch.json` & `echolocator-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/LICENSE` & `echolocator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/Makefile` & `echolocator-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/PKG-INFO` & `echolocator-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.1.0
+Version: 1.2.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.1.0/README.rst` & `echolocator-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/configurations/development.yaml` & `echolocator-1.2.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/1_tutorials/101_run_conda.rst` & `echolocator-1.2.0/docs/1_tutorials/101_run_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/1_tutorials/102_update_image.rst` & `echolocator-1.2.0/docs/1_tutorials/102_update_image.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/2_how-to/201_add_fields.rst` & `echolocator-1.2.0/docs/2_how-to/201_add_fields.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/3_explanations/301_naming_conventions.rst` & `echolocator-1.2.0/docs/3_explanations/301_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/3_explanations/302_process.rst` & `echolocator-1.2.0/docs/3_explanations/302_process.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/4_reference/402_building_conda.rst` & `echolocator-1.2.0/docs/4_reference/402_building_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/_static/theme_overrides.css` & `echolocator-1.2.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/conf.py` & `echolocator-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/diagrams/3drop_texrank_coordinates.drawio` & `echolocator-1.2.0/docs/diagrams/3drop_texrank_coordinates.drawio`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/dls-favicon.ico` & `echolocator-1.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/dls-logo.svg` & `echolocator-1.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/excalidraw-example.svg` & `echolocator-1.2.0/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/git_merge.png` & `echolocator-1.2.0/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/image_details.png` & `echolocator-1.2.0/docs/images/image_details.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/image_list.png` & `echolocator-1.2.0/docs/images/image_list.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/docs/images/swiss3.png` & `echolocator-1.2.0/docs/images/swiss3.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/modulefiles/conda` & `echolocator-1.2.0/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/pyproject.toml` & `echolocator-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.2.0/src/echolocator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.1.0
+Version: 1.2.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.1.0/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.2.0/src/echolocator.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,14 @@
 src/echolocator_lib/guis/aiohttp.py
 src/echolocator_lib/guis/base.py
 src/echolocator_lib/guis/constants.py
 src/echolocator_lib/guis/context.py
 src/echolocator_lib/guis/guis.py
 src/echolocator_lib/guis/html/index.html
 src/echolocator_lib/guis/html/index.js
-src/echolocator_lib/guis/html/targeting.html
-src/echolocator_lib/guis/html/targeting.js
 src/echolocator_lib/guis/html/css/image_edit_ux.css
 src/echolocator_lib/guis/html/css/image_list_ux.css
 src/echolocator_lib/guis/html/css/pixel_ux.css
 src/echolocator_lib/guis/html/css/styles.css
 src/echolocator_lib/guis/html/css/system_health_ux.css
 src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
 src/echolocator_lib/guis/html/images/green_dot_crosshair.png
@@ -134,29 +132,23 @@
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
 src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
 src/echolocator_lib/guis/html/javascript/webviz/spreader.js
 src/echolocator_lib/guis/html/javascript/webviz/transformer.js
-src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
-src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
 src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
 src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
-src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
-src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
-src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
-src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
-src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
-src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
+src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_droplocation.py
-tests/test_export.py
+tests/test_export_to_csv.py
+tests/test_export_to_soakdb3.py
 tests/test_fetch_image.py
 tests/test_fetch_images.py
 tests/configurations/service.yaml
 tests/example_images/1.jpg
 tests/example_images/2.jpg
 tests/example_images/3.jpg
 tests/example_images/4.png
```

### Comparing `echolocator-1.1.0/src/echolocator_api/context_base.py` & `echolocator-1.2.0/src/echolocator_api/context_base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_api/databases/constants.py` & `echolocator-1.2.0/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_api/exceptions.py` & `echolocator-1.2.0/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.2.0/src/echolocator_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_api/guis/context.py` & `echolocator-1.2.0/src/echolocator_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_api/guis/guis.py` & `echolocator-1.2.0/src/echolocator_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_cli/main.py` & `echolocator-1.2.0/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_cli/subcommands/base.py` & `echolocator-1.2.0/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_cli/subcommands/service.py` & `echolocator-1.2.0/src/echolocator_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_cli/version.py` & `echolocator-1.2.0/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/__main__.py` & `echolocator-1.2.0/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/composers/composers.py` & `echolocator-1.2.0/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/composers/html.py` & `echolocator-1.2.0/src/echolocator_lib/composers/html.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.2.0/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/composers/text.py` & `echolocator-1.2.0/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/contexts/base.py` & `echolocator-1.2.0/src/echolocator_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/envvar.py` & `echolocator-1.2.0/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.2.0/src/echolocator_lib/guis/aiohttp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import csv
 import logging
 import multiprocessing
 import threading
 from pathlib import Path
+from typing import List
 
 from dls_servbase_api.constants import Keywords as ProtocoljKeywords
 
 # Utilities.
 from dls_utilpack.callsign import callsign
-from dls_utilpack.describe import describe
 from dls_utilpack.require import require
 
 # Basic things.
 from dls_utilpack.thing import Thing
 from dls_utilpack.visit import get_xchem_directory
 
 # The model which describes the crystal wells to be injected into soakdb3.
@@ -22,15 +22,21 @@
 
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 from xchembku_api.models.crystal_well_droplocation_model import (
     CrystalWellDroplocationModel,
 )
-from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
+from xchembku_api.models.crystal_well_filter_model import (
+    CrystalWellFilterModel,
+    CrystalWellFilterSortbyEnum,
+)
+from xchembku_api.models.crystal_well_needing_droplocation_model import (
+    CrystalWellNeedingDroplocationModel,
+)
 
 # Base class for an aiohttp server.
 from echolocator_lib.base_aiohttp import BaseAiohttp
 
 # Object managing echolocator_composers.
 from echolocator_lib.composers.composers import (
     Composers,
@@ -185,82 +191,97 @@
         if self.__xchembku is None:
             raise RuntimeError(
                 "refusing to execute command %s because server is shutting down"
                 % (command)
             )
 
         if command == Commands.LOAD_TABS:
-            return await self._load_tabs(opaque, request_dict)
+            return await self.__load_tabs(opaque, request_dict)
 
         if command == Commands.SELECT_TAB:
-            return await self._select_tab(opaque, request_dict)
+            return await self.__select_tab(opaque, request_dict)
 
         if command == Commands.FETCH_IMAGE:
-            return await self._fetch_image(opaque, request_dict)
+            return await self.__fetch_image(opaque, request_dict)
 
         elif command == Commands.FETCH_IMAGE_LIST:
-            return await self._fetch_image_list(opaque, request_dict)
+            return await self.__fetch_image_list(opaque, request_dict)
 
-        elif command == Commands.EXPORT:
-            return await self._export(opaque, request_dict)
+        elif command == Commands.EXPORT_TO_SOAKDB3:
+            return await self.__export_to_soakdb3(opaque, request_dict)
+
+        elif command == Commands.EXPORT_TO_CSV:
+            return await self.__export_to_csv(opaque, request_dict)
 
         elif command == Commands.UPDATE:
-            return await self._update(opaque, request_dict)
+            return await self.__update(opaque, request_dict)
 
         else:
             raise RuntimeError("invalid command %s" % (command))
 
     # ----------------------------------------------------------------------------------------
-    async def _load_tabs(self, opaque, request_dict):
+    async def __load_tabs(self, opaque, request_dict):
 
         tab_id = await self.get_cookie_content(
             opaque, Cookies.TABS_MANAGER, Keywords.TAB_ID
         )
         logger.debug(f"[GUITABS] tab_id from cookie content is {tab_id}")
 
         # Reply with tabs.
         response = {Keywords.TAB_ID: tab_id}
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def _select_tab(self, opaque, request_dict):
+    async def __select_tab(self, opaque, request_dict):
         tab_id = require("request json", request_dict, Keywords.TAB_ID)
 
         logger.debug(f"[GUITABS] tab_id in request is {tab_id}")
 
         # Put the tab_id into the cookie.
         self.set_cookie_content(opaque, Cookies.TABS_MANAGER, Keywords.TAB_ID, tab_id)
 
         response = {}
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def _fetch_image(self, opaque, request_dict):
+    async def __fetch_image(self, opaque, request_dict):
 
         # Get uuid from the cookie if it's not being posted here.
         crystal_well_uuid = await self.set_or_get_cookie_content(
             opaque,
             Cookies.IMAGE_EDIT_UX,
             "crystal_well_uuid",
             request_dict.get("crystal_well_uuid"),
             "",
         )
 
-        logger.info(f"fetching image for crystal_well_uuid {crystal_well_uuid}")
+        logger.info(
+            f"fetching image from crystal_well_uuid {crystal_well_uuid}"
+            f" direction {request_dict.get('direction')}"
+        )
 
         # Not able to get an image from posted value or cookie?
         # Usually first time visiting Image Details tab when no image picked from list.
         if crystal_well_uuid == "":
             response = {"record": None}
             return response
 
         # Start a filter where we anchor on the given well.
-        filter = CrystalWellFilterModel(anchor=crystal_well_uuid, limit=1)
+        filter = CrystalWellFilterModel(
+            anchor=crystal_well_uuid,
+            limit=1,
+            sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
+        )
+
+        # Caller is providing visit?
+        visit = request_dict.get("visit")
+        if visit is not None:
+            filter.visit = visit
 
         # Image previous or next?
         direction = request_dict.get("direction", 0)
         if direction != 0:
             filter.direction = direction
 
         should_show_only_undecided = await self.set_or_get_cookie_content(
@@ -287,110 +308,124 @@
         record = crystal_well_models[0].dict()
         record["filename"] = "filestore" + record["filename"]
         response = {"record": record}
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def _fetch_image_list(self, opaque, request_dict):
+    async def __fetch_image_list(self, opaque, request_dict):
 
         # Remember last posted value for auto_update_enabled.
         auto_update_enabled = await self._handle_auto_update(
             opaque, request_dict, Cookies.IMAGE_LIST_UX
         )
 
-        visit = await self.set_or_get_cookie_content(
-            opaque,
-            Cookies.IMAGE_LIST_UX,
-            "visit",
-            request_dict.get("visit"),
-            None,
-        )
-
-        barcode_filter = await self.set_or_get_cookie_content(
+        visit_filter = await self.set_or_get_cookie_content(
             opaque,
             Cookies.IMAGE_LIST_UX,
-            "barcode_filter",
-            request_dict.get("barcode_filter"),
+            "visit_filter",
+            request_dict.get("visit_filter"),
             None,
         )
-        should_show_only_undecided = await self.set_or_get_cookie_content(
-            opaque,
-            Cookies.IMAGE_LIST_UX,
-            "should_show_only_undecided",
-            request_dict.get("should_show_only_undecided"),
-            False,
-        )
-
-        logger.debug(
-            f"fetching image records, barcode_filter is '{barcode_filter}' and "
-            f" should_show_only_undecided is '{should_show_only_undecided}'"
-        )
-
-        # Start a filter where we anchor on the given image.
-        filter = CrystalWellFilterModel(barcode=barcode_filter)
 
         should_show_only_undecided = await self.set_or_get_cookie_content(
             opaque,
             Cookies.IMAGE_LIST_UX,
             "should_show_only_undecided",
             request_dict.get("should_show_only_undecided"),
             False,
         )
-        if should_show_only_undecided:
-            filter.is_decided = False
 
-        # Fetch the list from the xchembku.
-        crystal_well_models = (
-            await self.__xchembku.fetch_crystal_wells_needing_droplocation(filter)
-        )
+        if visit_filter is None:
+            visit_filter = ""
+        visit_filter = visit_filter.strip()
 
-        html = echolocator_composers_get_default().compose_image_list(
-            crystal_well_models
-        )
         filters = {
-            "visit": visit,
-            "barcode_filter": barcode_filter,
+            "visit_filter": visit_filter,
             "should_show_only_undecided": should_show_only_undecided,
         }
+
+        if visit_filter == "":
+            html = "please enter a visit"
+
+        else:
+            logger.debug(
+                f"fetching image records, visit_filter is '{visit_filter}' and "
+                f" should_show_only_undecided is '{should_show_only_undecided}'"
+            )
+
+            # Start a filter where we anchor on the given image.
+            filter = CrystalWellFilterModel(
+                visit=visit_filter,
+                sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
+            )
+
+            should_show_only_undecided = await self.set_or_get_cookie_content(
+                opaque,
+                Cookies.IMAGE_LIST_UX,
+                "should_show_only_undecided",
+                request_dict.get("should_show_only_undecided"),
+                False,
+            )
+            if should_show_only_undecided:
+                filter.is_decided = False
+
+            # Fetch the list from the xchembku.
+            crystal_well_models = (
+                await self.__xchembku.fetch_crystal_wells_needing_droplocation(filter)
+            )
+
+            html = echolocator_composers_get_default().compose_image_list(
+                crystal_well_models
+            )
+
         response = {
             "html": html,
             "filters": filters,
             "auto_update_enabled": auto_update_enabled,
         }
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def _update(self, opaque, request_dict):
+    async def __update(self, opaque, request_dict):
 
         t = require("ajax request", request_dict, "crystal_well_droplocation_model")
 
         # Wrap a model around the posted fields.
         crystal_well_droplocation_model = CrystalWellDroplocationModel(**t)
 
         # Update the database record.
         await self.__xchembku.upsert_crystal_well_droplocations(
             [crystal_well_droplocation_model],
             only_fields=list(t.keys()),
         )
 
         # Caller wants to select the next image automatically?
         if request_dict.get(Keywords.SHOULD_ADVANCE, False):
+
+            # Caller must provide a visit in order to automatically advance.
+            visit = request_dict.get("visit")
+            if visit is None:
+                raise RuntimeError(
+                    "programming error: visit not submitted with request to advance after update"
+                )
+
             # Advance by fetching the next image record after the update.
             next_request_dict = {
                 ProtocoljKeywords.ENABLE_COOKIES: [
                     Cookies.IMAGE_EDIT_UX,
                     Cookies.IMAGE_LIST_UX,
                 ],
                 Keywords.COMMAND: Commands.FETCH_IMAGE,
                 "crystal_well_uuid": crystal_well_droplocation_model.crystal_well_uuid,
                 "direction": 1,
+                "visit": visit,
             }
-            response = await self._fetch_image(opaque, next_request_dict)
+            response = await self.__fetch_image(opaque, next_request_dict)
 
             if response.get("record") is not None:
                 response[
                     "confirmation"
                 ] = "drop location has been updated and view advanced to next image"
             else:
                 response[
@@ -398,119 +433,194 @@
                 ] = "drop location has been updated and there are no more images in the list"
         else:
             response = {"confirmation": "drop location has been updated"}
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def _export(self, opaque, request_dict):
-
-        visit = request_dict.get("visit")
+    async def __export_to_soakdb3(self, opaque, request_dict):
 
-        if visit is None:
-            raise RuntimeError("visit not submitted with request (programming error)")
-
-        visit = visit.strip()
-        if visit == "":
+        # Caller must provide a visit.
+        visit_filter = request_dict.get("visit_filter")
+        if visit_filter is None:
+            raise RuntimeError("programming error: visit not submitted with request")
+
+        # Visit must not be blank.
+        visit_filter = visit_filter.strip()
+        if visit_filter == "":
             response = {"error": "blank visit was given"}
             return response
 
-        # Get the barcode string submitted from the html form.
-        barcode_filter = request_dict.get("barcode_filter")
+        # Get a filter for wells we want to export.
+        crystal_well_filter = CrystalWellFilterModel(
+            visit=visit_filter,
+            is_decided=True,
+            is_usable=True,
+            sortby=CrystalWellFilterSortbyEnum.POSITION,
+        )
+
+        # Fetch the list of wells according to the filter.
+        crystal_well_models: List[
+            CrystalWellNeedingDroplocationModel
+        ] = await self.__xchembku.fetch_crystal_wells_needing_droplocation(
+            crystal_well_filter
+        )
+
+        # Export the crystal wells to the appropriate soakdb3 visit.
+        await self.__export_to_soakdb3_visit(visit_filter, crystal_well_models)
+
+        response = {
+            "confirmation": f"exported {len(crystal_well_models)} rows to soakdb3 visit {visit_filter}"
+        }
+
+        return response
+
+    # ----------------------------------------------------------------------------------------
+    async def __export_to_soakdb3_visit(
+        self,
+        visit,
+        crystal_well_models: List[CrystalWellNeedingDroplocationModel],
+    ) -> None:
 
-        if barcode_filter is None:
+        # Fetch the plate record for visit.
+        crystal_plate_filter = CrystalPlateFilterModel(visit=visit)
+        crystal_plate_models = await self.__xchembku.fetch_crystal_plates(
+            crystal_plate_filter
+        )
+
+        if len(crystal_plate_models) == 0:
             raise RuntimeError(
-                "barcode_filter not submitted with request (programming error)"
+                f'database integrity error: no crystal plate for visit "{visit}"'
             )
+        crystal_plate_model = crystal_plate_models[0]
 
-        barcode_filter = barcode_filter.strip()
-        if barcode_filter == "":
-            response = {"error": "blank barcode was given"}
+        soakdb3_crystal_well_models = []
+        for m in crystal_well_models:
+            soakdb3_crystal_well_models.append(
+                Soakdb3CrystalWellModel(
+                    LabVisit=visit,
+                    CrystalPlate=crystal_plate_model.rockminer_collected_stem,
+                    CrystalWell=m.position,
+                    EchoX=m.confirmed_microns_x,
+                    EchoY=m.confirmed_microns_y,
+                )
+            )
+
+        visit_directory = Path(get_xchem_directory(self.__export_directory, visit))
+
+        logger.debug(
+            f"exporting {len(soakdb3_crystal_well_models)} to {str(visit_directory)}"
+        )
+        # Append well records to soakdb3 database.
+        # Soakdb3 wants the "/processing" to be on the end of the visitid.
+        await self.__xchembku.inject_soakdb3_crystal_wells(
+            str(visit_directory / "processing"), soakdb3_crystal_well_models
+        )
+
+    # ----------------------------------------------------------------------------------------
+    async def __export_to_csv(self, opaque, request_dict):
+
+        # Caller must provide a visit.
+        visit_filter = request_dict.get("visit_filter")
+        if visit_filter is None:
+            raise RuntimeError("visit not submitted with request (programming error)")
+
+        # Visit must not be blank.
+        visit_filter = visit_filter.strip()
+        if visit_filter == "":
+            response = {"error": "blank visit was given"}
             return response
 
-        # Get a filter for wells on the plate with this barcode.
+        # Get a filter for wells we want to export.
         crystal_well_filter = CrystalWellFilterModel(
-            barcode=barcode_filter,
+            visit=visit_filter,
             is_decided=True,
             is_usable=True,
+            sortby=CrystalWellFilterSortbyEnum.POSITION,
         )
 
-        # Fetch the list of wells for this barcode.
-        crystal_well_models = (
-            await self.__xchembku.fetch_crystal_wells_needing_droplocation(
-                crystal_well_filter
-            )
+        # Fetch the list of wells according to the filter.
+        crystal_well_models: List[
+            CrystalWellNeedingDroplocationModel
+        ] = await self.__xchembku.fetch_crystal_wells_needing_droplocation(
+            crystal_well_filter
         )
 
-        # Fetch the plate record for barcode.
-        crystal_plate_filter = CrystalPlateFilterModel(barcode=barcode_filter)
+        # Group the wells by the plate they belong to.
+        plates_crystal_well_models = {}
+        for crystal_well_model in crystal_well_models:
+            crystal_plate_uuid = crystal_well_model.crystal_plate_uuid
+            if crystal_plate_uuid not in plates_crystal_well_models:
+                plates_crystal_well_models[crystal_plate_uuid] = []
+            plates_crystal_well_models[crystal_plate_uuid].append(crystal_well_model)
+
+        # Keep a list of the confirmations we will get from exporting the plates.
+        confirmations = []
+
+        # Go through each plate separately.
+        for (
+            crystal_plate_uuid,
+            plate_crystal_well_models,
+        ) in plates_crystal_well_models.items():
+            # Export the crystal wells for this plate to the appropriate csv file named for the plate.
+            filename = await self.__export_to_csv_plate(
+                visit_filter, crystal_plate_uuid, plate_crystal_well_models
+            )
+
+            confirmations.append(
+                f"exported {len(plate_crystal_well_models)} rows to {filename}"
+            )
+
+        response = {"confirmation": "\n".join(confirmations)}
+
+        return response
+
+    # ----------------------------------------------------------------------------------------
+    async def __export_to_csv_plate(
+        self,
+        visit,
+        crystal_plate_uuid,
+        crystal_well_models: List[CrystalWellNeedingDroplocationModel],
+    ):
+
+        # Fetch the plate record for visit.
+        crystal_plate_filter = CrystalPlateFilterModel(uuid=crystal_plate_uuid)
         crystal_plate_models = await self.__xchembku.fetch_crystal_plates(
             crystal_plate_filter
         )
 
         if len(crystal_plate_models) == 0:
             raise RuntimeError(
-                f"no plate for barcode {barcode_filter} (database integrity error)"
+                f'database integrity error: no crystal plate for uuid "{crystal_plate_uuid}"'
             )
-
         crystal_plate_model = crystal_plate_models[0]
 
         # Use the stem from the rockmaker Luigi pipeline to form the csv filename.
-        logger.debug(describe("self.__export_directory", self.__export_directory))
-        logger.debug(describe("self.__export_subdirectory", self.__export_subdirectory))
-        logger.debug(describe("visit", visit))
         visit_directory = Path(get_xchem_directory(self.__export_directory, visit))
-        logger.debug(describe("xchem_directory", visit_directory))
         targets_directory = visit_directory / self.__export_subdirectory
-        logger.debug(describe("targets_directory", targets_directory))
 
         filename = (
             targets_directory
             / f"{crystal_plate_model.rockminer_collected_stem}_targets.csv"
         )
-        logger.debug(describe("filename", filename))
 
         if not filename.parent.is_dir():
             raise RuntimeError(f"the directory does not exist: {str(filename.parent)}")
 
-        # directory.mkdir(parents=True, exist_ok=True)
-
         with open(filename, "w", newline="") as f:
             writer = csv.writer(f)
 
             for m in crystal_well_models:
                 row = []
                 row.append(m.position)
                 row.append(m.confirmed_microns_x or "")
                 row.append(m.confirmed_microns_y or "")
                 writer.writerow(row)
 
-        response = {
-            "confirmation": f"exported {len(crystal_well_models)} rows to {filename}"
-        }
-
-        soakdb3_crystal_well_models = []
-        for m in crystal_well_models:
-            soakdb3_crystal_well_models.append(
-                Soakdb3CrystalWellModel(
-                    LabVisit=visit,
-                    CrystalPlate=crystal_plate_model.rockminer_collected_stem,
-                    CrystalWell=m.position,
-                    EchoX=m.confirmed_microns_x,
-                    EchoY=m.confirmed_microns_y,
-                )
-            )
-
-            # Append well records to soakdb3 database.
-            # Soakdb3 wants the "/processing" to be on the end of the visitid.
-            await self.__xchembku.inject_soakdb3_crystal_wells(
-                str(visit_directory / "processing"), soakdb3_crystal_well_models
-            )
-
-        return response
+        return filename
 
     # ----------------------------------------------------------------------------------------
     async def _handle_auto_update(self, opaque, request_dict, cookie_name):
 
         # Remember last posted value for auto_update_enabled.
         auto_update_enabled = request_dict.get("auto_update_enabled")
         # logger.debug(
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/constants.py` & `echolocator-1.2.0/src/echolocator_lib/guis/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     SHOULD_ADVANCE = "echolocator_guis::keywords::should_advance"
 
 
 class Commands:
     UPDATE = "echolocator_guis::commands::update"
     FETCH_IMAGE = "echolocator_guis::commands::fetch_image"
     FETCH_IMAGE_LIST = "echolocator_guis::commands::fetch_image_list"
-    EXPORT = "echolocator_guis::commands::export"
+    EXPORT_TO_SOAKDB3 = "echolocator_guis::commands::export_to_soakdb3"
+    EXPORT_TO_CSV = "echolocator_guis::commands::export_to_csv"
     LOAD_TABS = "echolocator_guis::commands::load_tabs"
     SELECT_TAB = "echolocator_guis::commands::select_tab"
 
 
 class Cookies:
     TABS_MANAGER = "TABS_MANAGER"
     IMAGE_LIST_UX = "IMAGE_LIST_UX"
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/context.py` & `echolocator-1.2.0/src/echolocator_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/guis.py` & `echolocator-1.2.0/src/echolocator_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.2.0/src/echolocator_lib/guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/index.html` & `echolocator-1.2.0/src/echolocator_lib/guis/html/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     <link rel="stylesheet" href="javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css">
 
     <!-- Common javascript classes. -->
     <script src="javascript/common/base.js"></script>
 
     <!-- Classes for screen interaction. -->
     <script src="javascript/raphael/raphael-2.1.4/raphael.min.js"></script>
-    <script src="javascript/webviz/sprite/shape.js"></script>
+    <script src="javascript/webviz/sprite/ring.js"></script>
     <script src="javascript/webviz/hair/guide2.js"></script>
     <script src="javascript/webviz/spreader.js"></script>
     <script src="javascript/webviz/transformer.js"></script>
 
     <!-- Support for all echolocator pages. -->
     <script src="javascript/version.js"></script>
     <script src="javascript/runtime.js"></script>
@@ -64,26 +64,25 @@
                     <div class="T_auto_update">
                         <div class="T_toggle">AUTO</div>
                         <div class="T_status">-</div>
                     </div>
                     <div class="T_buttons" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
                             <div class="T_prompt">visit</div>
-                            <div class="T_input"><input type="text" class="T_visit"></div>
+                            <div class="T_input"><input type="text" class="T_visit_filter"></div>
                             <div class="T_separator"></div>
-                            <button class="T_export_button" title="export">Export</button>
+                            <button class="T_export_to_soakdb3_button" title="export to soakdb3 database">Export to
+                                Soakdb3</button>
+                            <div class="T_separator"></div>
+                            <button class="T_export_to_csv_button" title="export to csv file">Export to CSV</button>
                         </div>
                     </div>
-                    <div class="T_help">Exports all images on the plate which have been decided.</div>
                     <div class="T_inputs" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_row">
                             <div class="T_field">
-                                <div class="T_prompt">barcode</div>
-                                <div class="T_input"><input type="text" class="T_barcode_filter"></div>
-                                <div class="T_separator"></div>
                                 <div class="T_prompt">show only undecided</div>
                                 <div class="T_input"><input type="checkbox" class="T_should_show_only_undecided"></div>
                             </div>
                         </div>
                     </div>
                     <div class="T_section">
                         <div class="T_title" title="image list">Image List</div>
@@ -102,15 +101,14 @@
                         <button class="T_reject_button" title="reject image">Not Usable<span class="T_hint"> (right
                                 click or X)</span></button>
                         <button class="T_reset_button" title="reset image">Undecided<span class="T_hint"></span>
                             (-)</span></button>
                         <button class="T_next_button" title="next image">Next<span class="T_hint"> (right
                                 arrow)</span></button>
                     </div>
-                    <div class="T_help T_hide_when_no_image">Right-click in the image to mark as not usable.</div>
 
                     <div class="T_image_info T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
                             <div class="T_prompt">filename:</div>
                             <div class="T_input">
                                 <div class="T_filename"></div>
                             </div>
```

#### html2text {}

```diff
@@ -13,22 +13,19 @@
 
     * Image_List
     * Image_Details
 AUTO
 -
 visit
 [                    ]
-Export
-Exports all images on the plate which have been decided.
-barcode
-[                    ]
+Export to Soakdb3
+Export to CSV
 show only undecided
 ⁰
 Image List
 -
 Previous (left arrow) Usable (space bar) Not Usable (right click or X)
 Undecided (-) Next (right arrow)
-Right-click in the image to mark as not usable.
 filename:
 Num crystals:
 is usable?
 [images/radial1.666.png]
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/index.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/index.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
         this.#raphael = raphael;
 
         // TODO: Try to use raphael normal transformation instead of transformer class.
         this.#transformer = this.#raphael.webviz_transformer;
 
         var that = this;
 
-        this.#shape = new webviz__sprite__Shape(this, this.plugin_link_name);
+        this.#shape = new webviz__sprite__Ring(this, this.plugin_link_name);
 
         this.#shape.activate(this.#raphael, this.#color);
 
         // Set box to appear guaranteed on-screen somewhere.
         this.#shape.set({
             position: {
                 x: 220,
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -244,14 +244,17 @@
             }
 
             json_object["crystal_well_droplocation_model"] = model;
 
             // Tell server to add response["html"] for next image in series.
             json_object[this.SHOULD_ADVANCE] = true;
 
+            // Server needs to know the visit as its limiting window in the advancement logic.
+            json_object["visit"] = this.#record.visit;
+
             // Send request to update database immediately.
             this.send(json_object);
 
             // Move to next image.
             this.request_update(1);
         }
 
@@ -323,15 +326,19 @@
     request_update(direction = 0) {
 
         var json_object = {}
         // TODO: Remove hardcoded "IMAGE_LIST_UX" in image edit's cookie list.
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME, "IMAGE_LIST_UX"]
         json_object[this.COMMAND] = this.FETCH_IMAGE;
         json_object["crystal_well_uuid"] = this.#crystal_well_uuid;
-        json_object["direction"] = direction;
+
+        if (direction !== 0) {
+            json_object["direction"] = direction;
+            json_object["visit"] = this.#record.visit;
+        }
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle an error response.
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 // Class backing the actions ux.
 
 class echolocator__ImageListUx extends echolocator__UxAutoUpdate {
     COOKIE_NAME = "IMAGE_LIST_UX";
     FETCH_IMAGE_LIST = "echolocator_guis::commands::fetch_image_list";
-    EXPORT = "echolocator_guis::commands::export";
+    EXPORT_TO_SOAKDB3 = "echolocator_guis::commands::export_to_soakdb3";
+    EXPORT_TO_CSV = "echolocator_guis::commands::export_to_csv";
 
     #jquery_objects = {};
-    #visit = "undefined";
-    #barcode_filter = "undefined";
+    #visit_filter = "undefined";
     #should_show_only_undecided = "undefined";
 
     constructor(runtime, plugin_link_name, $interaction_parent) {
         super(runtime);
 
         this.plugin_link_name = plugin_link_name;
         this.$interaction_parent = $interaction_parent;
@@ -21,53 +21,52 @@
     // -------------------------------------------------------------
     // Activate things on the UX.
 
     activate() {
         super.activate()
 
         this.#jquery_objects.$div = $(".T_composed", this.$interaction_parent);
-        this.#jquery_objects.$visit = $(".T_visit", this.$interaction_parent);
-        this.#jquery_objects.$barcode_filter = $(".T_barcode_filter", this.$interaction_parent);
+        this.#jquery_objects.$visit_filter = $(".T_visit_filter", this.$interaction_parent);
         this.#jquery_objects.$should_show_only_undecided = $(".T_should_show_only_undecided", this.$interaction_parent);
-        this.#jquery_objects.$export_button = $(".T_export_button", this.$interaction_parent);
+        this.#jquery_objects.$export_to_soakdb3_button = $(".T_export_to_soakdb3_button", this.$interaction_parent);
+        this.#jquery_objects.$export_to_csv_button = $(".T_export_to_csv_button", this.$interaction_parent);
 
         var that = this;
-        this.#jquery_objects.$visit.change(
+        this.#jquery_objects.$visit_filter.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
-        this.#jquery_objects.$barcode_filter.change(
+        this.#jquery_objects.$should_show_only_undecided.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
-        this.#jquery_objects.$should_show_only_undecided.change(
+        this.#jquery_objects.$export_to_soakdb3_button.click(
             function(jquery_event_object) {
-                that._handle_filter_change(jquery_event_object);
+                that._handle_export_to_soakdb3_clicked(jquery_event_object);
             });
 
-        this.#jquery_objects.$export_button.click(
+        this.#jquery_objects.$export_to_csv_button.click(
             function(jquery_event_object) {
-                that._handle_export_clicked(jquery_event_object);
+                that._handle_export_to_csv_clicked(jquery_event_object);
             });
 
     } // end method
 
     // -------------------------------------------------------------
     // Request update from database.
 
     request_update() {
 
         var json_object = {}
         json_object[this.COMMAND] = this.FETCH_IMAGE_LIST;
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME];
 
-        json_object["visit"] = this.#visit;
-        json_object["barcode_filter"] = this.#barcode_filter;
+        json_object["visit_filter"] = this.#visit_filter;
         json_object["should_show_only_undecided"] = this.#should_show_only_undecided;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
@@ -78,22 +77,20 @@
 
         // Let the base class have a look at the response.
         super.handle_ajax_success(response, status, jqXHR);
 
         var filters = response.filters;
         if (filters !== undefined) {
             var t;
-            t = filters["visit"];
-            if (t === undefined)
-                t = "";
-            this.#jquery_objects.$visit.val(t);
-            t = filters["barcode_filter"];
+
+            t = filters["visit_filter"];
             if (t === undefined)
                 t = "";
-            this.#jquery_objects.$barcode_filter.val(t);
+            this.#jquery_objects.$visit_filter.val(t);
+
             t = filters["should_show_only_undecided"];
             if (t === undefined)
                 t = false;
             this.#jquery_objects.$should_show_only_undecided.prop("checked", t);
         }
 
         var html = response.html;
@@ -106,35 +103,49 @@
     }
 
     // -------------------------------------------------------------
 
     _handle_filter_change(jquery_event_object) {
         var F = "echolocator__ImageListUx::_handle_filter_change"
 
-        this.#visit = this.#jquery_objects.$visit.val()
-        this.#barcode_filter = this.#jquery_objects.$barcode_filter.val()
+        this.#visit_filter = this.#jquery_objects.$visit_filter.val()
         this.#should_show_only_undecided = this.#jquery_objects.$should_show_only_undecided.prop("checked")
         this.request_update()
 
     } // end method
 
     // -------------------------------------------------------------
 
-    _handle_export_clicked(jquery_event_object) {
-        var F = "echolocator__ImageListUx::_handle_export_clicked"
+    _handle_export_to_soakdb3_clicked(jquery_event_object) {
+        var F = "echolocator__ImageListUx::_handle_export_to_soakdb3_clicked"
+
+        this.#visit_filter = this.#jquery_objects.$visit_filter.val()
+
+        // Enable no cookie for this request.
+        var json_object = {}
+        json_object[this.COMMAND] = this.EXPORT_TO_SOAKDB3;
+
+        json_object["visit_filter"] = this.#visit_filter;
+
+        this.send(json_object);
+
+    } // end method
+
+    // -------------------------------------------------------------
+
+    _handle_export_to_csv_clicked(jquery_event_object) {
+        var F = "echolocator__ImageListUx::_handle_export_to_csv_clicked"
 
-        this.#visit = this.#jquery_objects.$visit.val()
-        this.#barcode_filter = this.#jquery_objects.$barcode_filter.val()
+        this.#visit_filter = this.#jquery_objects.$visit_filter.val()
 
         // Enable no cookie for this request.
         var json_object = {}
-        json_object[this.COMMAND] = this.EXPORT;
+        json_object[this.COMMAND] = this.EXPORT_TO_CSV;
 
-        json_object["visit"] = this.#visit;
-        json_object["barcode_filter"] = this.#barcode_filter;
+        json_object["visit_filter"] = this.#visit_filter;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -40,15 +40,15 @@
     activate_confirmation_message() {
 
         var cm_class = "T_ajax_confirmation_message";
         var $cm_container = $("." + cm_class + "_container", this.$interaction_parent);
         var $cm = $("." + cm_class, this.$interaction_parent);
 
         if ($cm_container.length == 0) {
-            this.$interaction_parent.prepend("<div class='" + cm_class + "_container'><div class='" + cm_class + "'></div></div>");
+            this.$interaction_parent.prepend("<div class='" + cm_class + "_container'><xmp class='" + cm_class + "'></xmp></div>");
             $cm_container = $("." + cm_class + "_container", this.$interaction_parent);
             $cm = $("." + cm_class, this.$interaction_parent);
         }
 
         $cm_container.hide();
         this.#jquery_objects.$confirmation_message_container = $cm_container;
         this.#jquery_objects.$confirmation_message = $cm;
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,63 +1,68 @@
-class webviz__sprite__Shape extends common__Base {
+class webviz__sprite__Ring extends common__Base {
 
     constructor(page, name, classname, precisionLine = false) {
         super(page.runtime);
 
         this.page = page;
         this.name = name;
         this.debug_identifier = name;
         this.precisionLine = precisionLine;
     } // end constructor
 
     // -------------------------------------------------------------
 
     activate(raphael, color) {
-        var F = "webviz__sprite__Shape[" + this.name + "]::activate";
+        var F = "webviz__sprite__Ring[" + this.name + "]::activate";
 
         this._raphael = raphael
 
         raphael.setStart();
 
-        // this._perimeter = this._raphael.path("M0,0:L10,0:L0,10:L0,0").attr({ 
+        // this._group = this._raphael.path("M0,0:L10,0:L0,10:L0,0").attr({ 
         //     fill: "#FF0000", 
         //     stroke: "#000000", 
         //     "stroke-width": 1 
         // }); 
 
-        this._center = this._raphael.circle(0, 0, 5).attr({
-            fill: color,
-            stroke: "black",
-            "stroke-width": 1
+        // Dot at the center.
+        // this._center = this._raphael.circle(0, 0, 5).attr({
+        //     fill: color,
+        //     stroke: "black",
+        //     "stroke-width": 1
+        // });
+
+        this._raphael.circle(0, 0, 1).attr({
+            fill: "transparent",
+            stroke: "white",
+            "stroke-width": 5,
+            "stroke-dasharray": "--",
         });
 
-        this._perimeter = this._raphael.circle(0, 0, 1).attr({
+        this._raphael.circle(0, 0, 1).attr({
             fill: "transparent",
-            stroke: color,
-            "stroke-width": 4
+            stroke: "black",
+            "stroke-width": 2,
+            "stroke-dasharray": "--",
         });
 
         // matrix = Raphael.matrix(1, 0, 0, 1, 0, 0, 0, 0, 0);
         // matrix.translate(0, 0)
         // console.log(F + " raphael matrix is \"" + matrix.toTransformString() + "\"")
-        // this._perimeter.translate(1, 1);
-        // console.log(F + " ball matrix is \"" + this._perimeter.matrix.toTransformString() + "\"")
+        // this._group.translate(1, 1);
+        // console.log(F + " ball matrix is \"" + this._group.matrix.toTransformString() + "\"")
 
         this._group = this._raphael.setFinish()
-        this._group._parent_object = this;
-
-        this._perimeter._group = this._group;
-        this._perimeter._parent_object = this;
 
         console.log(F + ": activated")
     } // end method
 
     // -------------------------------------------------------------
     set(settings) {
-        var F = "webviz__sprite__Shape[" + this.name + "]::set";
+        var F = "webviz__sprite__Ring[" + this.name + "]::set";
 
         for (var k in settings) {
             var setting = settings[k];
 
             if (k == "position") {
                 // console.log(F + ": [CENTPO] setting position [" + setting.x + ", " + setting.y + "]");
 
@@ -70,15 +75,15 @@
                 }
             }
             if (k == "scale") {
                 // console.log(F + ": [CENTPO] setting scale " + setting)
 
                 // Something wrong with settings?
                 if (!isNaN(setting)) {
-                    this._perimeter.scale(setting);
+                    this._group.scale(setting);
                 } else {
                     console.log(F + ": [CENTPO] something is wrong with the scale setting")
                 }
             }
             // The setting is for visibility?
             else if (k == "visible") {
                 if (setting)
@@ -90,21 +95,21 @@
         }
     } // end method
 
     // -------------------------------------------------------------
     // Returns the currents settings in a JSON-serializable structure.
 
     get() {
-        var F = "webviz__sprite__Shape[" + this.name + "]::get";
+        var F = "webviz__sprite__Ring[" + this.name + "]::get";
 
         var settings = {};
 
         // Position to where the group's anchor point has been moved.
-        var x = this._perimeter.matrix.x(0, 0);
-        var y = this._perimeter.matrix.y(0, 0);
+        var x = this._group.matrix.x(0, 0);
+        var y = this._group.matrix.y(0, 0);
 
         settings.position = {
             x: x,
             y: y
         };
 
         return settings;
```

### Comparing `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/src/echolocator_lib/version.py` & `echolocator-1.2.0/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/base.py` & `echolocator-1.2.0/tests/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,21 @@
 
     def __init__(self):
         self.tasks_execution_outputs = {}
         self.residuals = ["stdout.txt", "stderr.txt", "main.log"]
 
         self.injected_count = 0
         self.visit = "cm00001-1"
-        self.barcode = "98ab"
+        self.__barcode_template = "98a%d"
         self.crystal_plate_uuid = None
-        self.rockminer_collected_stem = "98ab_2021-09-14_RI1000-0276-3drop"
+        self.__rockminer_collected_stem_template = "98a%d_2021-09-14_RI1000-0276-3drop"
+
+        self.crystal_plate_models = []
+
+        self.__formulatrix_plate_id = 0
 
     def main(self, constants, configuration_file, output_directory):
         """
         This is the main program which calls the test using asyncio.
         """
 
         # Save these for when the configuration is loaded.
@@ -95,26 +99,34 @@
         return rockingest_multiconf
 
     # ----------------------------------------------------------------------------------------
 
     async def inject_plate(self, xchembku):
         """ """
 
+        self.__formulatrix_plate_id += 1
+        self.barcode = self.__barcode_template % (self.__formulatrix_plate_id)
+        rockminer_collected_stem = self.__rockminer_collected_stem_template % (
+            self.__formulatrix_plate_id
+        )
+
         # Make the plate on which the wells reside.
         crystal_plate_model = CrystalPlateModel(
-            formulatrix__plate__id=10,
+            formulatrix__plate__id=self.__formulatrix_plate_id,
             barcode=self.barcode,
-            rockminer_collected_stem=self.rockminer_collected_stem,
+            rockminer_collected_stem=rockminer_collected_stem,
             visit=self.visit,
             thing_type=CrystalPlateObjectThingTypes.SWISS3,
         )
 
         await xchembku.upsert_crystal_plates([crystal_plate_model])
         self.crystal_plate_uuid = crystal_plate_model.uuid
 
+        self.crystal_plate_models.append(crystal_plate_model)
+
     # ----------------------------------------------------------------------------------------
 
     async def inject(self, xchembku, autolocation: bool, droplocation: bool):
         """ """
 
         if self.crystal_plate_uuid is None:
             await self.inject_plate(xchembku)
```

### Comparing `echolocator-1.1.0/tests/configurations/service.yaml` & `echolocator-1.2.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/conftest.py` & `echolocator-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/example_images/1.jpg` & `echolocator-1.2.0/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/example_images/2.jpg` & `echolocator-1.2.0/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/example_images/3.jpg` & `echolocator-1.2.0/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/example_images/4.png` & `echolocator-1.2.0/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/images/1.jpg` & `echolocator-1.2.0/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/images/2.jpg` & `echolocator-1.2.0/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/images/3.jpg` & `echolocator-1.2.0/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.1.0/tests/test_droplocation.py` & `echolocator-1.2.0/tests/test_droplocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,77 +103,80 @@
 
         self.__cookies = {}
         # Inject some wells.
         crystal_wells.append(await self.inject(xchembku, True, False))
         crystal_wells.append(await self.inject(xchembku, True, False))
         crystal_wells.append(await self.inject(xchembku, True, False))
 
-        await self.__set_confirmed_target(xchembku, crystal_wells, 0, 1)
-        await self.__set_confirmed_target(xchembku, crystal_wells, 1, 2)
-        await self.__set_confirmed_target(xchembku, crystal_wells, 2, None)
+        # The crystal count increases with each one added, so they are sorted in reverse order of adding.
+        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 2, 1)
+        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 1, 0)
+        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 0, None)
 
-        await self.__set_is_usable(xchembku, crystal_wells, 0, False)
-        await self.__set_is_usable(xchembku, crystal_wells, 0, True)
+        await self.__set_is_usable_and_dont_advance(xchembku, crystal_wells, 0, False)
+        await self.__set_is_usable_and_dont_advance(xchembku, crystal_wells, 0, True)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __set_confirmed_target(
+    async def __set_confirmed_target_and_advance(
         self, xchembku, crystal_well_models, index1, index2
     ):
         """ """
 
         x = 100 + index1
         y = 200 + index1
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.UPDATE,
             Keywords.SHOULD_ADVANCE: True,
+            "visit": self.visit,
             "crystal_well_droplocation_model": {
                 "crystal_well_uuid": crystal_well_models[index1].uuid,
                 "confirmed_target_x": x,
                 "confirmed_target_y": y,
                 "is_usable": True,
             },
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies=self.__cookies
         )
 
         self.__cookies = response["__cookies"]
 
-        logger.debug(describe("first set_target response", response))
+        note = f"advance from {index1} to {index2}"
+        logger.debug(describe(f"set_target response, {note}", response))
 
-        assert "record" in response
+        assert "record" in response, note
         record = response["record"]
-        assert "confirmation" in response
-        assert "has been updated" in response["confirmation"]
+        assert "confirmation" in response, note
+        assert "has been updated" in response["confirmation"], note
         if index2 is not None:
-            assert record is not None, f"index {index1}"
-            assert record["uuid"] == crystal_well_models[index2].uuid, f"index {index1}"
-            assert "advanced" in response["confirmation"]
+            assert record is not None, note
+            assert record["uuid"] == crystal_well_models[index2].uuid, note
+            assert "advanced" in response["confirmation"], note
         else:
-            assert record is None
-            assert "no more images" in response["confirmation"]
+            assert record is None, note
+            assert "no more images" in response["confirmation"], note
 
         # Fetch the record which should have been updated.
         fetched_models = await xchembku.fetch_crystal_wells_needing_droplocation(
             CrystalWellFilterModel(anchor=crystal_well_models[index1].uuid)
         )
 
-        assert fetched_models[0].confirmed_target_x == x, f"index {index1}"
-        assert fetched_models[0].confirmed_target_y == y, f"index {index1}"
-        assert fetched_models[0].is_usable is True, f"index {index1}"
+        assert fetched_models[0].confirmed_target_x == x, note
+        assert fetched_models[0].confirmed_target_y == y, note
+        assert fetched_models[0].is_usable is True, note
 
     # ----------------------------------------------------------------------------------------
 
-    async def __set_is_usable(
+    async def __set_is_usable_and_dont_advance(
         self,
         xchembku,
         crystal_well_models,
         index1,
         is_usable,
     ):
         """ """
```

### Comparing `echolocator-1.1.0/tests/test_export.py` & `echolocator-1.2.0/tests/test_export_to_soakdb3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import csv
 import logging
 from pathlib import Path
 
 # API constants.
 from dls_servbase_lib.datafaces.context import Context as DlsServbaseDatafaceContext
 from dls_utilpack.visit import get_xchem_subdirectory
 
@@ -37,28 +36,28 @@
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestExport:
+class TestExportToSoakdb3:
     def test(self, constants, logging_setup, output_directory):
         """ """
 
         configuration_file = "tests/configurations/service.yaml"
-        ExportTester().main(
+        ExportToSoakdb3Tester().main(
             constants,
             configuration_file,
             output_directory,
         )
 
 
 # ----------------------------------------------------------------------------------------
-class ExportTester(Base):
+class ExportToSoakdb3Tester(Base):
     """
     Class to test the gui fetch_image endpoint.
     """
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
@@ -135,23 +134,19 @@
 
         self.__visit_directory = (
             Path(self.__output_directory)
             / "labxchem"
             / get_xchem_subdirectory(self.visit)
         )
 
-        # Soakdb3 expects visitid to be a visit directory.
+        # Soakdb3 expects visitid to be a visit directory with processing tacked onto the end.
         # This is because of how the soadkb3 VBA in the Excel works.
         visitid = str(self.__visit_directory / "processing")
 
-        self.__crystal_targets_directory = (
-            self.__visit_directory / "processing/lab36/crystal-targets"
-        )
-
-        self.__crystal_targets_directory.mkdir(parents=True)
+        (Path(visitid)).mkdir(parents=True)
 
         # ----------------------------------------------------------------
         # Seed the necessary fields in the head table.
 
         protein = "P1"
         drop_volume = 3.1
 
@@ -165,113 +160,51 @@
             visitid,
             Tablenames.HEAD,
             [head_record],
         )
 
         # ----------------------------------------------------------------
 
-        await self.__export_initial()
-
         crystal_wells = []
 
         # Inject some wells.
         crystal_wells.append(await self.inject(self.__xchembku, False, False))
         crystal_wells.append(await self.inject(self.__xchembku, True, True))
         crystal_wells.append(await self.inject(self.__xchembku, True, False))
         crystal_wells.append(await self.inject(self.__xchembku, True, True))
         crystal_wells.append(await self.inject(self.__xchembku, True, True))
         crystal_wells.append(await self.inject(self.__xchembku, True, False))
 
         await self.__export_wells(crystal_wells)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __export_initial(self):
-        """ """
-
-        request = {
-            Keywords.COMMAND: Commands.EXPORT,
-            "visit": self.visit,
-            "barcode_filter": self.barcode,
-        }
-
-        response = await echolocator_guis_get_default().client_protocolj(
-            request, cookies={}
-        )
-
-        # Expect confirmation message in response.
-        assert "confirmation" in response
-        assert "exported 0" in response["confirmation"]
-
-        # Check the csv file got written with no lines.
-        csv = (
-            self.__crystal_targets_directory
-            / f"{self.rockminer_collected_stem}_targets.csv"
-        )
-
-        assert csv.exists()
-        assert csv.stat().st_size == 0
-
-    # ----------------------------------------------------------------------------------------
-
     async def __export_wells(self, crystal_wells):
         """ """
 
         request = {
-            Keywords.COMMAND: Commands.EXPORT,
-            "visit": self.visit,
-            "barcode_filter": self.barcode,
+            Keywords.COMMAND: Commands.EXPORT_TO_SOAKDB3,
+            "visit_filter": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
         # Expect confirmation message in response.
         assert "confirmation" in response
-        assert "exported 3" in response["confirmation"]
-
-        # Check the csv file got written.
-        csv_path = (
-            self.__crystal_targets_directory
-            / f"{self.rockminer_collected_stem}_targets.csv"
-        )
-        assert csv_path.exists()
-
-        # Read the csv file into an array.
-        rows = []
-        with open(csv_path, "r", newline="") as csv_file:
-            reader = csv.reader(csv_file)
-            for row in reader:
-                rows.append(row)
-
-        # Check row count we read.
-        assert len(rows) == 3
-
-        # Check each row has 3 parts.
-        for row in rows:
-            assert len(row) == 3
-
-        # Check the well positions are those that are considered "confirmed".
-        # The position constants are fromt the Swiss3 microns computation.
-        assert rows[0][0] == "02A_1"
-        assert int(rows[0][1]) == -561
-        assert int(rows[0][2]) == -842
-        assert rows[1][0] == "04A_1"
-        assert int(rows[1][1]) == 6
-        assert int(rows[1][2]) == -274
-        assert rows[2][0] == "05A_1"
-        assert int(rows[2][1]) == 289
-        assert int(rows[2][2]) == 9
+        assert "exported" in response["confirmation"]
 
         # Check the results stored in soakdbb3, there should be no change to the first ones.
         queried_models = await self.__xchembku.fetch_soakdb3_crystal_wells(
             str(self.__visit_directory / "processing")
         )
         assert len(queried_models) == 3
+
+        # The position constants are fromt the Swiss3 microns computation.
         assert queried_models[0].CrystalWell == "02A_1"
         assert int(queried_models[0].EchoX) == -561
         assert int(queried_models[0].EchoY) == -842
         assert queried_models[1].CrystalWell == "04A_1"
         assert int(queried_models[1].EchoX) == 6
         assert int(queried_models[1].EchoY) == -274
         assert queried_models[2].CrystalWell == "05A_1"
```

### Comparing `echolocator-1.1.0/tests/test_fetch_image.py` & `echolocator-1.2.0/tests/test_fetch_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,74 +175,78 @@
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.FETCH_IMAGE,
             "crystal_well_uuid": crystal_wells[2].uuid,
             "direction": 1,
+            "visit": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
         logger.debug(describe("fetch_image response", response))
 
         record = response["record"]
-        assert record["uuid"] == crystal_wells[3].uuid
+        assert record["position"] == crystal_wells[1].position
+        assert record["uuid"] == crystal_wells[1].uuid
         assert record["confirmed_target_x"] is not None
 
         # -------------------------------------------------------------------------------------
         # Same query again, but rely on cookies for values.
         request.pop("crystal_well_uuid")
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies=response["__cookies"]
         )
 
         logger.debug(describe("fetch_image response", response))
 
         record = response["record"]
-        assert record["uuid"] == crystal_wells[3].uuid
+        assert record["position"] == crystal_wells[1].position
+        assert record["uuid"] == crystal_wells[1].uuid
         assert record["confirmed_target_x"] is not None
 
     # ----------------------------------------------------------------------------------------
 
     async def __request_forward_undecided(self, crystal_wells):
         """ """
 
         # Get next image in forward direction, anchored on 2, ignoring those decided.
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.FETCH_IMAGE,
-            "crystal_well_uuid": crystal_wells[2].uuid,
+            "crystal_well_uuid": crystal_wells[5].uuid,
             "direction": 1,
+            "visit": self.visit,
             "should_show_only_undecided": True,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
         logger.debug(describe("__request_forward_undecided response 1", response))
 
         record = response["record"]
-        assert record["uuid"] == crystal_wells[5].uuid
+        assert record["uuid"] == crystal_wells[2].uuid
         assert record["confirmed_target_x"] is None
 
         # -------------------------------------------------------------------------------------
         # Same query again, but rely on cookies for values.
         request.pop("crystal_well_uuid")
         request.pop("should_show_only_undecided")
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies=response["__cookies"]
         )
 
         logger.debug(describe("__request_forward_undecided response 2", response))
 
         record = response["record"]
-        assert record["uuid"] == crystal_wells[5].uuid
+        assert record["uuid"] == crystal_wells[2].uuid
         assert record["confirmed_target_x"] is None
```

### Comparing `echolocator-1.1.0/tests/test_fetch_images.py` & `echolocator-1.2.0/tests/test_fetch_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         """ """
 
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.FETCH_IMAGE_LIST,
+            "visit_filter": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
         logger.debug(describe("first fetch_image response", response))
@@ -147,14 +148,15 @@
         """ """
 
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.FETCH_IMAGE_LIST,
+            "visit_filter": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
         logger.debug(describe("fetch_image response", response))
@@ -167,17 +169,19 @@
         # Count the number of rows in the table.
         rows = table.find_all("tr")
 
         # Assert that the row count is equal to the expected value.
         assert len(rows) == 1 + 5
 
         # Check the first row's filename.
+        # Remember fiels are injected with increasing crystal counts,
+        # so default sorting is in reverse order.
         row = rows[1]
         columns = row.find_all(class_="T_filename")
         assert len(columns) == 1
-        assert columns[0].get_text() == Path(crystal_wells[1].filename).stem
+        assert columns[0].get_text() == Path(crystal_wells[5].filename).stem
 
         # Check the last row's filename.
         row = rows[5]
         columns = row.find_all(class_="T_filename")
         assert len(columns) == 1
-        assert columns[0].get_text() == Path(crystal_wells[5].filename).stem
+        assert columns[0].get_text() == Path(crystal_wells[1].filename).stem
```

