# Comparing `tmp/autora-workflow-0.3.2.tar.gz` & `tmp/autora-workflow-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.2.tar", last modified: Fri May  5 13:43:51 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.3.tar", last modified: Fri May  5 21:05:47 2023, max compression
```

## Comparing `autora-workflow-0.3.2.tar` & `autora-workflow-0.3.3.tar`

### file list

```diff
@@ -1,95 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.543181 autora-workflow-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.551181 autora-workflow-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.555181 autora-workflow-0.3.2/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/basic-usage/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/func0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.559181 autora-workflow-0.3.2/docs/cli/with-cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-pip/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.563181 autora-workflow-0.3.2/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/saving-and-loading-dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/docs/interactive/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:43:51.575181 autora-workflow-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.551181 autora-workflow-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.547181 autora-workflow-0.3.2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.567181 autora-workflow-0.3.2/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:43:51.000000 autora-workflow-0.3.2/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.571181 autora-workflow-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:43:40.000000 autora-workflow-0.3.2/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.031272 autora-workflow-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.043272 autora-workflow-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   253372 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/basic-usage/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/dump_initial_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.059272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.059272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.039272 autora-workflow-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.039272 autora-workflow-0.3.3/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 21:05:47.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.2/.github/workflows/python-publish.yml` & `autora-workflow-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/.github/workflows/test-pytest.yml` & `autora-workflow-0.3.3/.github/workflows/test-pytest.yml`

 * *Files 16% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: "pip"
     - run: pip install ".[dev]"
-    - run: pytest --doctest-modules
+    - run: pytest --doctest-modules --ignore docs/cli/
```

### Comparing `autora-workflow-0.3.2/.gitignore` & `autora-workflow-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/.idea/autora-workflow.iml` & `autora-workflow-0.3.3/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.3/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/.pre-commit-config.yaml` & `autora-workflow-0.3.3/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -16,9 +16,10 @@
         - "--per-file-ignores=__init__.py:F401"
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.2.0"
     hooks:
       - id: mypy
         additional_dependencies: [types-requests,types-PyYAML]
         language_version: python3.8
+        exclude: ^docs/
 default_language_version:
   python: python3
```

### Comparing `autora-workflow-0.3.2/LICENSE.md` & `autora-workflow-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/PKG-INFO` & `autora-workflow-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.2
+Version: 0.3.3
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: cylc
 License-File: LICENSE.md
 
 # Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
```

### Comparing `autora-workflow-0.3.2/docs/cli/basic-usage/index.ipynb` & `autora-workflow-0.3.3/docs/cli/basic-usage/README.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988368055555555%*

 * *Differences: {"'cells'": "{3: {'execution_count': 1, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2023-05-05T19:09:32.724377Z', 'start_time': '2023-05-05T19:09:31.597456Z'}}}, 24: "*

 * *            "{'source': ['If we run the experiment for another 3 cycles, we can get results closer "*

 * *            'to the ground truth. In this example, we overwrite the results file each time the CLI '*

 * *            "is called.']}}"}*

```diff
@@ -95,19 +95,19 @@
                 "Then, before we start the experiment, we\n",
                 "- load the controller from the file\n",
                 "- save its state to a `.dill` file."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-05-04T21:18:25.014597Z",
-                    "start_time": "2023-05-04T21:18:24.379286Z"
+                    "end_time": "2023-05-05T19:09:32.724377Z",
+                    "start_time": "2023-05-05T19:09:31.597456Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from lib import controller\n",
                 "import dill\n",
@@ -608,16 +608,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "If we run the experiment for another 3 cycles, we can get results closer to the ground truth. In this example, we\n",
-                "overwrite the results file each time the CLI is called."
+                "If we run the experiment for another 3 cycles, we can get results closer to the ground truth. In this example, we overwrite the results file each time the CLI is called."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "ExecuteTime": {
```

### Comparing `autora-workflow-0.3.2/docs/cli/basic-usage/lib.py` & `autora-workflow-0.3.3/docs/cli/basic-usage/lib.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/cli/with-cylc-conda/flow.cylc` & `autora-workflow-0.3.3/docs/cli/with-cylc-pip/flow.cylc`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+[scheduling]
+    cycling mode = integer
+    initial cycle point = 1
+    final cycle point = 3
+    [[graph]]
+        R1 = """
+        setup_python => initialize_controller => experimentalist
+        """
+        P1 = """
+            experimentalist => experiment_runner => theorist
+            theorist[-P1] => experimentalist
+        """
+
 [runtime]
-    [[setup]]
+    [[setup_python]]
         script = """
-            cp $CYLC_WORKFLOW_RUN_DIR/controller.dill $CYLC_WORKFLOW_SHARE_DIR;
-            conda create -p $CYLC_WORKFLOW_SHARE_DIR/env --clone autora-cylc
+            virtualenv "$CYLC_WORKFLOW_SHARE_DIR/env" -p python3.10
+            source "$CYLC_WORKFLOW_SHARE_DIR/env/bin/activate"
+            pip install --upgrade pip
+            pip install -r "$CYLC_WORKFLOW_RUN_DIR/requirements.txt"
+        """
+    [[initialize_controller]]
+    script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python \
+                -m dump_initial_controller \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill"
         """
     [[experimentalist]]
         script = """
             $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
-                experimentalist \
-                --debug
+                experimentalist
         """
     [[experiment_runner]]
         script = """
             $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
-                experiment_runner \
-                --debug
+                experiment_runner
         """
     [[theorist]]
         script = """
             $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
                 "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
-                theorist \
-                --debug
+                theorist
         """
 
-[scheduling]
-    cycling mode = integer
-    initial cycle point = 1
-    final cycle point = 3
-    [[graph]]
-        R1 = """
-        setup => experimentalist
-        """
-        P1 = """
-            experimentalist => experiment_runner => theorist
-            theorist[-P1] => experimentalist
-        """
+
```

### Comparing `autora-workflow-0.3.2/docs/cli/with-cylc-conda/lib/python/func0.py` & `autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/cli/with-cylc-slurm/flow.cylc` & `autora-workflow-0.3.3/docs/cli/with-cylc-slurm/flow.cylc`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,59 @@
-[runtime]
-    [[setup]]
-        script = """
-            cp $CYLC_WORKFLOW_RUN_DIR/controller.yml $CYLC_WORKFLOW_SHARE_DIR;
-            cp -R $CYLC_WORKFLOW_RUN_DIR/history $CYLC_WORKFLOW_SHARE_DIR/history
-            conda create -p $CYLC_WORKFLOW_SHARE_DIR/env --clone /users/jholla10/anaconda/autora-cylc
-        """
-    [[experimentalist]]
-        script = $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=experimentalist --verbose --debug
-        platform = oscar
-    [[experiment_runner]]
-        script = /$CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=experiment_runner --verbose --debug
-        platform = oscar
-    [[theorist]]
-        script = $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=theorist --verbose --debug
-        platform = oscar
-
 [scheduling]
     cycling mode = integer
     initial cycle point = 1
+    final cycle point = 3
     [[graph]]
         R1 = """
-        setup => experimentalist
+        setup_python => initialize_controller => experimentalist
         """
         P1 = """
             experimentalist => experiment_runner => theorist
             theorist[-P1] => experimentalist
         """
+
+[runtime]
+    [[setup_python]]
+        script = """
+            virtualenv "$CYLC_WORKFLOW_SHARE_DIR/env" -p python3.9
+            source "$CYLC_WORKFLOW_SHARE_DIR/env/bin/activate"
+            pip install --upgrade pip
+            pip install -r "$CYLC_WORKFLOW_RUN_DIR/requirements.txt"
+        """
+        platform = oscar
+    
+    [[initialize_controller]]
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python \
+                -m dump_initial_controller \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill"
+        """
+        platform = oscar
+    
+    [[experimentalist]]
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                experimentalist
+        """
+        platform = oscar
+    
+    [[experiment_runner]]
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                experiment_runner
+        """
+        platform = oscar
+    
+    [[theorist]]
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                theorist
+        """
+        platform = oscar
+
+
```

### Comparing `autora-workflow-0.3.2/docs/interactive/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.3.3/docs/interactive/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/interactive/basic-usage.ipynb` & `autora-workflow-0.3.3/docs/interactive/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/interactive/passing-static-parameters.ipynb` & `autora-workflow-0.3.3/docs/interactive/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/interactive/saving-and-loading-dill.ipynb` & `autora-workflow-0.3.3/docs/interactive/saving-and-loading-dill.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/docs/interactive/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.3/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/mkdocs/base.yml` & `autora-workflow-0.3.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/mkdocs.yml` & `autora-workflow-0.3.3/mkdocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 - Interactive:
     - 'interactive/basic-usage.ipynb'
     - 'interactive/passing-static-parameters.ipynb'
     - "interactive/accessing-state-dependent-properties.ipynb"
     - "interactive/using-alternative-planners-and-executors.ipynb"
     - "interactive/saving-and-loading-dill.ipynb"
 - Command line:
-    - "Basic Usage": "cli/basic-usage/index.ipynb"
-    - "With Cylc and Conda": "cli/with-cylc-conda/index.ipynb"
+    - "Basic Usage": "cli/basic-usage/README.ipynb"
+    - "With Cylc, Virtualenv and Pip": "cli/with-cylc-pip/README.md"
+    - "With Cylc and Conda": "cli/with-cylc-conda/README.md"
+    - "With Cylc and Slurm": "cli/with-cylc-slurm/README.md"
```

### Comparing `autora-workflow-0.3.2/pyproject.toml` & `autora-workflow-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 dev = [
     "autora-core[dev]",
     "autora-workflow[docs]",
 ]
 docs = [
     "mkdocs-include-markdown-plugin",
 ]
+cylc = [
+    "cylc-flow",
+    "cylc-uiserver"
+]
 
 [project.urls]
 homepage = "http://www.empiricalresearch.ai/"
 repository = "https://github.com/AutoResearch/autora-workflow"
 documentation = "https://hollandjg.github.io/autora-workflow/"
 
 [build-system]
```

### Comparing `autora-workflow-0.3.2/src/autora/workflow/__init__.py` & `autora-workflow-0.3.3/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/__main__.py` & `autora-workflow-0.3.3/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/base.py` & `autora-workflow-0.3.3/src/autora/workflow/base.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/controller.py` & `autora-workflow-0.3.3/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/cycle.py` & `autora-workflow-0.3.3/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/executor.py` & `autora-workflow-0.3.3/src/autora/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/planner.py` & `autora-workflow-0.3.3/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/plotting.py` & `autora-workflow-0.3.3/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/protocol.py` & `autora-workflow-0.3.3/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.3/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/state/history.py` & `autora-workflow-0.3.3/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/state/param.py` & `autora-workflow-0.3.3/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.3/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.2/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.3.3/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.2
+Version: 0.3.3
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: cylc
 License-File: LICENSE.md
 
 # Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
```

### Comparing `autora-workflow-0.3.2/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.3.3/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,29 +19,35 @@
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
 .idea/runConfigurations/pytest_in_tests.xml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 docs/index.md
-docs/cli/basic-usage/index.ipynb
+docs/cli/basic-usage/README.ipynb
 docs/cli/basic-usage/lib.py
 docs/cli/with-cylc-conda/.gitignore
+docs/cli/with-cylc-conda/README.md
 docs/cli/with-cylc-conda/environment.yml
 docs/cli/with-cylc-conda/flow.cylc
-docs/cli/with-cylc-conda/index.ipynb
-docs/cli/with-cylc-conda/lib/python/func0.py
-docs/cli/with-cylc-pip/TODO
+docs/cli/with-cylc-conda/lib/python/controller_setup.py
+docs/cli/with-cylc-conda/lib/python/dump_initial_controller.py
+docs/cli/with-cylc-pip/.gitignore
+docs/cli/with-cylc-pip/README.md
+docs/cli/with-cylc-pip/flow.cylc
+docs/cli/with-cylc-pip/requirements.txt
+docs/cli/with-cylc-pip/lib/python/controller_setup.py
+docs/cli/with-cylc-pip/lib/python/dump_initial_controller.py
+docs/cli/with-cylc-slurm/.gitignore
 docs/cli/with-cylc-slurm/README.md
-docs/cli/with-cylc-slurm/controller.yml
-docs/cli/with-cylc-slurm/environment.yml
 docs/cli/with-cylc-slurm/flow.cylc
 docs/cli/with-cylc-slurm/global.cylc
-docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
-docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
+docs/cli/with-cylc-slurm/requirements.txt
+docs/cli/with-cylc-slurm/lib/python/controller_setup.py
+docs/cli/with-cylc-slurm/lib/python/dump_initial_controller.py
 docs/interactive/accessing-state-dependent-properties.ipynb
 docs/interactive/basic-usage.ipynb
 docs/interactive/passing-static-parameters.ipynb
 docs/interactive/saving-and-loading-dill.ipynb
 docs/interactive/using-alternative-planners-and-executors.ipynb
 mkdocs/base.yml
 src/autora/workflow/__init__.py
```

### Comparing `autora-workflow-0.3.2/tests/test_controller_plots.py` & `autora-workflow-0.3.3/tests/test_controller_plots.py`

 * *Files identical despite different names*

