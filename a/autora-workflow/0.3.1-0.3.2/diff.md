# Comparing `tmp/autora-workflow-0.3.1.tar.gz` & `tmp/autora-workflow-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.1.tar", last modified: Fri May  5 13:34:18 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.2.tar", last modified: Fri May  5 13:43:51 2023, max compression
```

## Comparing `autora-workflow-0.3.1.tar` & `autora-workflow-0.3.2.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.811180 autora-workflow-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/basic-usage/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/func0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-pip/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/saving-and-loading-dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/using-alternative-planners-and-executors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.543181 autora-workflow-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.551181 autora-workflow-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/basic-usage/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/func0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-pip/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:43:51.575181 autora-workflow-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.551181 autora-workflow-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.1/.github/workflows/python-publish.yml` & `autora-workflow-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.github/workflows/test-pytest.yml` & `autora-workflow-0.3.2/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.gitignore` & `autora-workflow-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.idea/autora-workflow.iml` & `autora-workflow-0.3.2/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.2/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/.pre-commit-config.yaml` & `autora-workflow-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/LICENSE.md` & `autora-workflow-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/basic-usage/index.ipynb` & `autora-workflow-0.3.2/docs/cli/basic-usage/index.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/basic-usage/lib.py` & `autora-workflow-0.3.2/docs/cli/basic-usage/lib.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-conda/flow.cylc` & `autora-workflow-0.3.2/docs/cli/with-cylc-conda/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-conda/index.ipynb` & `autora-workflow-0.3.2/docs/cli/with-cylc-conda/index.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/func0.py` & `autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/func0.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/controller.yml` & `autora-workflow-0.3.2/docs/cli/with-cylc-slurm/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/environment.yml` & `autora-workflow-0.3.2/docs/cli/with-cylc-slurm/environment.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/flow.cylc` & `autora-workflow-0.3.2/docs/cli/with-cylc-slurm/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml` & `autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/interactive/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.3.2/docs/interactive/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/interactive/basic-usage.ipynb` & `autora-workflow-0.3.2/docs/interactive/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/interactive/passing-static-parameters.ipynb` & `autora-workflow-0.3.2/docs/interactive/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/interactive/saving-and-loading-dill.ipynb` & `autora-workflow-0.3.2/docs/interactive/saving-and-loading-dill.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/docs/interactive/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.2/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/mkdocs/base.yml` & `autora-workflow-0.3.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/mkdocs.yml` & `autora-workflow-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/pyproject.toml` & `autora-workflow-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "autora-workflow"
 description = "Workflow tools for the Autonomous Research Assistant (AutoRA) package."
 authors = [
     { name = "John Gerrard Holland", email = "john_holland1@brown.edu" }
 ]
 dynamic = ["version"]
 
-readme = "README.md"
+readme = "docs/index.md"
 license = { text = "MIT License" }
 
 dependencies = [
     "autora-core",
     "typer[all]",
     "dill",
 ]
```

### Comparing `autora-workflow-0.3.1/src/autora/workflow/__init__.py` & `autora-workflow-0.3.2/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/__main__.py` & `autora-workflow-0.3.2/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/base.py` & `autora-workflow-0.3.2/src/autora/workflow/base.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/controller.py` & `autora-workflow-0.3.2/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/cycle.py` & `autora-workflow-0.3.2/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/executor.py` & `autora-workflow-0.3.2/src/autora/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/planner.py` & `autora-workflow-0.3.2/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/plotting.py` & `autora-workflow-0.3.2/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/protocol.py` & `autora-workflow-0.3.2/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.2/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/state/history.py` & `autora-workflow-0.3.2/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/state/param.py` & `autora-workflow-0.3.2/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.2/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.1/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.3.2/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
 .idea/runConfigurations/pytest_in_tests.xml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 docs/index.md
-docs/quickstart.md
 docs/cli/basic-usage/index.ipynb
 docs/cli/basic-usage/lib.py
 docs/cli/with-cylc-conda/.gitignore
 docs/cli/with-cylc-conda/environment.yml
 docs/cli/with-cylc-conda/flow.cylc
 docs/cli/with-cylc-conda/index.ipynb
 docs/cli/with-cylc-conda/lib/python/func0.py
```

### Comparing `autora-workflow-0.3.1/tests/test_controller_plots.py` & `autora-workflow-0.3.2/tests/test_controller_plots.py`

 * *Files identical despite different names*

