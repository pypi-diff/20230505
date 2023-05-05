# Comparing `tmp/autora-workflow-0.3.0.tar.gz` & `tmp/autora-workflow-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.0.tar", last modified: Fri May  5 13:30:34 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.1.tar", last modified: Fri May  5 13:34:18 2023, max compression
```

## Comparing `autora-workflow-0.3.0.tar` & `autora-workflow-0.3.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/basic-usage/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/python/func0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-pip/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/saving-and-loading-dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/using-alternative-planners-and-executors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.811180 autora-workflow-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/basic-usage/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/func0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-pip/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/interactive/using-alternative-planners-and-executors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.815180 autora-workflow-0.3.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.819180 autora-workflow-0.3.1/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:34:18.000000 autora-workflow-0.3.1/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:34:18.823180 autora-workflow-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:34:07.000000 autora-workflow-0.3.1/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.0/.github/workflows/python-publish.yml` & `autora-workflow-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.github/workflows/test-pytest.yml` & `autora-workflow-0.3.1/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.gitignore` & `autora-workflow-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.idea/autora-workflow.iml` & `autora-workflow-0.3.1/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.1/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/.pre-commit-config.yaml` & `autora-workflow-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/LICENSE.md` & `autora-workflow-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/PKG-INFO` & `autora-workflow-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.3.0/docs/cli/basic-usage/index.ipynb` & `autora-workflow-0.3.1/docs/cli/basic-usage/index.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/basic-usage/lib.py` & `autora-workflow-0.3.1/docs/cli/basic-usage/lib.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-conda/example.ipynb` & `autora-workflow-0.3.1/docs/cli/with-cylc-conda/index.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-conda/flow.cylc` & `autora-workflow-0.3.1/docs/cli/with-cylc-conda/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/python/func0.py` & `autora-workflow-0.3.1/docs/cli/with-cylc-conda/lib/python/func0.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/controller.yml` & `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/environment.yml` & `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/environment.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/flow.cylc` & `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml` & `autora-workflow-0.3.1/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/interactive/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.3.1/docs/interactive/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/interactive/basic-usage.ipynb` & `autora-workflow-0.3.1/docs/interactive/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/interactive/passing-static-parameters.ipynb` & `autora-workflow-0.3.1/docs/interactive/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/interactive/saving-and-loading-dill.ipynb` & `autora-workflow-0.3.1/docs/interactive/saving-and-loading-dill.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/docs/interactive/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.1/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/mkdocs/base.yml` & `autora-workflow-0.3.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/mkdocs.yml` & `autora-workflow-0.3.1/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 - Interactive:
     - 'interactive/basic-usage.ipynb'
     - 'interactive/passing-static-parameters.ipynb'
     - "interactive/accessing-state-dependent-properties.ipynb"
     - "interactive/using-alternative-planners-and-executors.ipynb"
     - "interactive/saving-and-loading-dill.ipynb"
 - Command line:
-    - "cli/basic-usage/example.ipynb"
+    - "Basic Usage": "cli/basic-usage/index.ipynb"
+    - "With Cylc and Conda": "cli/with-cylc-conda/index.ipynb"
```

### Comparing `autora-workflow-0.3.0/pyproject.toml` & `autora-workflow-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/__init__.py` & `autora-workflow-0.3.1/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/__main__.py` & `autora-workflow-0.3.1/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/base.py` & `autora-workflow-0.3.1/src/autora/workflow/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         if self.monitor is not None:
             self.monitor(self.state)
         return self
 
     def run(self, num_steps: int = 1):
         """Run the next num_steps planned steps in the workflow."""
         for i in range(num_steps):
-            self.run_once(self)
+            self.run_once()
         return self
 
     def __next__(self):
         """Run the next planned step in the workflow."""
         return self.run_once()
 
     def __iter__(self):
```

### Comparing `autora-workflow-0.3.0/src/autora/workflow/controller.py` & `autora-workflow-0.3.1/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/cycle.py` & `autora-workflow-0.3.1/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/executor.py` & `autora-workflow-0.3.1/src/autora/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/planner.py` & `autora-workflow-0.3.1/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/plotting.py` & `autora-workflow-0.3.1/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/protocol.py` & `autora-workflow-0.3.1/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.1/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/state/history.py` & `autora-workflow-0.3.1/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/state/param.py` & `autora-workflow-0.3.1/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.1/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.0/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.3.1/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.3.0/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.3.1/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 .vscode/launch.json
 docs/index.md
 docs/quickstart.md
 docs/cli/basic-usage/index.ipynb
 docs/cli/basic-usage/lib.py
 docs/cli/with-cylc-conda/.gitignore
 docs/cli/with-cylc-conda/environment.yml
-docs/cli/with-cylc-conda/example.ipynb
 docs/cli/with-cylc-conda/flow.cylc
+docs/cli/with-cylc-conda/index.ipynb
 docs/cli/with-cylc-conda/lib/python/func0.py
 docs/cli/with-cylc-pip/TODO
 docs/cli/with-cylc-slurm/README.md
 docs/cli/with-cylc-slurm/controller.yml
 docs/cli/with-cylc-slurm/environment.yml
 docs/cli/with-cylc-slurm/flow.cylc
 docs/cli/with-cylc-slurm/global.cylc
```

### Comparing `autora-workflow-0.3.0/tests/test_controller_plots.py` & `autora-workflow-0.3.1/tests/test_controller_plots.py`

 * *Files identical despite different names*

