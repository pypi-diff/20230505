# Comparing `tmp/autora-workflow-0.2.1.tar.gz` & `tmp/autora-workflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.2.1.tar", last modified: Mon May  1 16:03:43 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.0.tar", last modified: Fri May  5 13:30:34 2023, max compression
```

## Comparing `autora-workflow-0.2.1.tar` & `autora-workflow-0.3.0.tar`

### file list

```diff
@@ -1,105 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/basic-usage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/controller/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/basic-usage/controller.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/regressor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/variables.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   253381 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/basic-usage/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    75537 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-conda/lib/python/func0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-pip/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.597746 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000001-PARAMS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/interactive/using-alternative-planners-and-executors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.593746 autora-workflow-0.3.0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 13:30:34.000000 autora-workflow-0.3.0/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:30:34.601746 autora-workflow-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 13:30:17.000000 autora-workflow-0.3.0/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.2.1/.github/workflows/python-publish.yml` & `autora-workflow-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/.gitignore` & `autora-workflow-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/.idea/autora-workflow.iml` & `autora-workflow-0.3.0/.idea/autora-workflow.iml`

 * *Files 16% similar despite different names*

#### Comparing `autora-workflow-0.2.1/.idea/autora-workflow.iml` & `autora-workflow-0.3.0/.idea/autora-workflow.iml`

```diff
@@ -8,15 +8,14 @@
       <excludeFolder url="file://$MODULE_DIR$/.mypy_cache"/>
       <excludeFolder url="file://$MODULE_DIR$/.venv"/>
       <excludeFolder url="file://$MODULE_DIR$/.vscode"/>
       <excludeFolder url="file://$MODULE_DIR$/site"/>
       <excludeFolder url="file://$MODULE_DIR$/venv"/>
       <excludeFolder url="file://$MODULE_DIR$/venv3.10"/>
     </content>
-    <orderEntry type="jdk" jdkName="Python 3.10 (autora-workflow)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PackageRequirementsSettings">
     <option name="requirementsPath" value=""/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="GOOGLE"/>
```

### Comparing `autora-workflow-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.0/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/.pre-commit-config.yaml` & `autora-workflow-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/LICENSE.md` & `autora-workflow-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/PKG-INFO` & `autora-workflow-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.2.1
+Version: 0.3.0
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE.md
 
 # AutoRA Workflow
```

### Comparing `autora-workflow-0.2.1/docs/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.3.0/docs/interactive/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/basic-usage.ipynb` & `autora-workflow-0.3.0/docs/interactive/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/cli/controller/custom-function/controller.yml` & `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/controller.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 !!python/object:autora.controller.controller.Controller
-_experiment_runner_callable: &id002 !!python/name:func.plus_1 ''
+_experiment_runner_callable: &id002 !!python/name:func1.plus_1 ''
 _experimentalist_pipeline: &id004 !!python/object:autora.experimentalist.pipeline.Pipeline
   params: {}
   steps:
   - !!python/tuple
     - ten_random_samples
-    - !!python/name:func.ten_random_samples ''
+    - !!python/name:func1.ten_random_samples ''
 _theorist_estimator: &id006 !!python/object:sklearn.linear_model._base.LinearRegression
   _sklearn_version: 1.2.2
   copy_X: true
   fit_intercept: true
   n_jobs: null
   positive: false
 executor_collection:
```

### Comparing `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/flow.cylc` & `autora-workflow-0.3.0/docs/cli/with-cylc-conda/flow.cylc`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 [runtime]
     [[setup]]
         script = """
-            cp $CYLC_WORKFLOW_RUN_DIR/controller.yml $CYLC_WORKFLOW_SHARE_DIR;
-            cp -R $CYLC_WORKFLOW_RUN_DIR/history $CYLC_WORKFLOW_SHARE_DIR/history
+            cp $CYLC_WORKFLOW_RUN_DIR/controller.dill $CYLC_WORKFLOW_SHARE_DIR;
             conda create -p $CYLC_WORKFLOW_SHARE_DIR/env --clone autora-cylc
         """
     [[experimentalist]]
-        script = $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=experimentalist --verbose --debug
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                experimentalist \
+                --debug
+        """
     [[experiment_runner]]
-        script = /$CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=experiment_runner --verbose --debug
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                experiment_runner \
+                --debug
+        """
     [[theorist]]
-        script = $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.controller "$CYLC_WORKFLOW_SHARE_DIR/controller.yml" "$CYLC_WORKFLOW_SHARE_DIR/history/." --step-name=theorist --verbose --debug
+        script = """
+            $CYLC_WORKFLOW_SHARE_DIR/env/bin/python -m autora.workflow \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                "$CYLC_WORKFLOW_SHARE_DIR/controller.dill" \
+                theorist \
+                --debug
+        """
 
 [scheduling]
     cycling mode = integer
     initial cycle point = 1
+    final cycle point = 3
     [[graph]]
         R1 = """
         setup => experimentalist
         """
         P1 = """
             experimentalist => experiment_runner => theorist
             theorist[-P1] => experimentalist
```

### Comparing `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml` & `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml` & `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/environment.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc` & `autora-workflow-0.3.0/docs/cli/with-cylc-slurm/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/passing-static-parameters.ipynb` & `autora-workflow-0.3.0/docs/interactive/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/docs/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.0/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/mkdocs/base.yml` & `autora-workflow-0.3.0/mkdocs/base.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 # yaml-language-server: $schema=https://squidfunk.github.io/mkdocs-material/schema.json
 
 # Shared configuration matching the rest of the AutoRA documentation.
 theme:
   name: material
 
 plugins:
-  multirepo: {}
-  gen-files:
-    scripts: [ "mkdocs/gen_ref_pages.py" ]
-  literate-nav:
-    nav_file: SUMMARY.md
-  section-index: {}
-  mkdocstrings:
-      handlers:
-        python: 
-          import: ["https://scikit-learn.org/stable/objects.inv"]
   mkdocs-jupyter:  # required to convert Jupyter notebooks
     include_source: true
     execute: false
     ignore_h1_titles: true
 
 markdown_extensions:
   admonition: {}
   pymdownx.details: {}
   pymdownx.superfences: {}
   pymdownx.arithmatex: # required for equation display
     generic: true
+  pymdownx.snippets: {}
 
 extra_javascript: [ 
   # requirements for pymdownx.arithmetex:
   "javascripts/mathjax.js",                                 
   "https://polyfill.io/v3/polyfill.min.js?features=es6", 
   "https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"
 ]
```

### Comparing `autora-workflow-0.2.1/pyproject.toml` & `autora-workflow-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
 
 dependencies = [
     "autora-core",
-    "typer",
-    "rich",
-    "shellingham",
-    "pyyaml"
+    "typer[all]",
+    "dill",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "autora-core[dev]"
+    "autora-core[dev]",
+    "autora-workflow[docs]",
+]
+docs = [
+    "mkdocs-include-markdown-plugin",
 ]
 
 [project.urls]
 homepage = "http://www.empiricalresearch.ai/"
 repository = "https://github.com/AutoResearch/autora-workflow"
 documentation = "https://hollandjg.github.io/autora-workflow/"
```

### Comparing `autora-workflow-0.2.1/src/autora/workflow/__init__.py` & `autora-workflow-0.3.0/src/autora/workflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,21 +493,24 @@
     >>> f"m = {tfitted.coef_[0][0]:.2f}, c = {tfitted.intercept_[0]:.2f}"
     'm = 3.50, c = 1.04'
 
     This seems to work fine.
 
     Now we can define the executor component. We'll use a factory method to generate the
     collection:
-    >>> from autora.workflow.executor import make_online_executor_collection
-    >>> executor_collection = make_online_executor_collection([
-    ...     ("seed_experimentalist", "experimentalist", experimentalist_which_needs_no_data),
-    ...     ("main_experimentalist", "experimentalist", experimentalist_which_needs_a_model),
-    ...     ("theorist", "theorist", LinearRegression()),
-    ...     ("experiment_runner", "experiment_runner", experiment_runner),
-    ... ])
+    >>> from autora.workflow.executor import (ChainedFunctionMapping, from_experimentalist_pipeline,
+    ...     from_experiment_runner_callable, from_theorist_estimator)
+    >>> executor_collection = ChainedFunctionMapping(
+    ...     seed_experimentalist=
+    ...         [from_experimentalist_pipeline, experimentalist_which_needs_no_data],
+    ...     main_experimentalist=
+    ...         [from_experimentalist_pipeline, experimentalist_which_needs_a_model],
+    ...     experiment_runner=[from_experiment_runner_callable, experiment_runner],
+    ...     theorist=[from_theorist_estimator, LinearRegression()],
+    ... )
 
     We need some special parameters to handle the main experimentalist, so we specify those:
     >>> params = {"main_experimentalist": {"sampler": {"models": "%models%"}}}
 
     We now instantiate the controller:
     >>> from autora.workflow.base import BaseController
     >>> from autora.workflow.state import History
```

### Comparing `autora-workflow-0.2.1/src/autora/workflow/controller.py` & `autora-workflow-0.3.0/src/autora/workflow/controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
-import pathlib
 from typing import Callable, Dict, Optional
 
 from autora.experimentalist.pipeline import Pipeline
 from autora.variable import VariableCollection
 from sklearn.base import BaseEstimator
 
 from .base import BaseController
-from .executor import make_online_executor_collection
+from .executor import (
+    ChainedFunctionMapping,
+    from_experiment_runner_callable,
+    from_experimentalist_pipeline,
+    from_theorist_estimator,
+)
 from .planner import last_result_kind_planner
-from .serializer import HistorySerializer
 from .state import History
 
 _logger = logging.getLogger(__name__)
 
 
 class Controller(BaseController[History]):
     """
@@ -56,62 +59,31 @@
                 E.g. if the experimentalist had a step named "pool" which took an argument "n",
                 which you wanted to set to the value 30, then params would be set to this:
                 `{"experimentalist": {"pool": {"n": 30}}}`
             planner: a function which maps from the state to the next ExecutorName. The default
                 is to map from the last result in the state's history to the next logical step.
         """
 
-        if params is None:
-            params = {}
         state = History(
             variables=variables,
+            params=params,
             conditions=[],
             observations=[],
             models=[],
-            params=params,
         )
 
-        self._experimentalist_pipeline = experimentalist
-        self._experiment_runner_callable = experiment_runner
-        self._theorist_estimator = theorist
-
-        executor_collection = make_online_executor_collection(
-            [
-                (
-                    "experimentalist",
-                    "experimentalist",
-                    self._experimentalist_pipeline,
-                ),
-                (
-                    "experiment_runner",
-                    "experiment_runner",
-                    self._experiment_runner_callable,
-                ),
-                (
-                    "theorist",
-                    "theorist",
-                    self._theorist_estimator,
-                ),
-            ]
+        executor_collection = ChainedFunctionMapping(
+            experimentalist=[from_experimentalist_pipeline, experimentalist],
+            experiment_runner=[from_experiment_runner_callable, experiment_runner],
+            theorist=[from_theorist_estimator, theorist],
         )
 
         super().__init__(
             state=state,
             planner=planner,
             executor_collection=executor_collection,
             monitor=monitor,
         )
 
     def seed(self, **kwargs):
         for key, value in kwargs.items():
             self.state = self.state.update(**{key: value})
-
-    def load(self, directory: pathlib.Path):
-        serializer = HistorySerializer(directory)
-        state = serializer.load()
-        self.state = state
-        return
-
-    def dump(self, directory: pathlib.Path):
-        serializer = HistorySerializer(directory)
-        serializer.dump(self.state)
-        return
```

### Comparing `autora-workflow-0.2.1/src/autora/workflow/cycle.py` & `autora-workflow-0.3.0/src/autora/workflow/cycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Callable, Dict, Optional
 
 from autora.experimentalist.pipeline import Pipeline
 from autora.variable import VariableCollection
 from sklearn.base import BaseEstimator
 
 from .base import BaseController
-from .executor import make_default_online_executor_collection
+from .executor import full_cycle_wrapper
 from .planner import full_cycle_planner
 from .state import Snapshot
 
 _logger = logging.getLogger(__name__)
 
 
 class Cycle(BaseController):
@@ -60,18 +60,18 @@
         )
         planner = full_cycle_planner
 
         self._experimentalist_pipeline = experimentalist
         self._experiment_runner_callable = experiment_runner
         self._theorist_estimator = theorist
 
-        executor_collection = make_default_online_executor_collection(
-            experimentalist_pipeline=self._experimentalist_pipeline,
-            experiment_runner_callable=self._experiment_runner_callable,
-            theorist_estimator=self._theorist_estimator,
+        executor_collection = _executor_collection_factory(
+            experimentalist=self._experimentalist_pipeline,
+            experiment_runner=self._experiment_runner_callable,
+            theorist=self._theorist_estimator,
         )
 
         super().__init__(
             state=state,
             planner=planner,
             executor_collection=executor_collection,
             monitor=monitor,
@@ -194,13 +194,23 @@
 
     @experiment_runner.setter
     def experiment_runner(self, value):
         self._experiment_runner_callable = value
         self.executor_collection = self._updated_executor_collection()
 
     def _updated_executor_collection(self):
-        executor_collection = make_default_online_executor_collection(
-            experimentalist_pipeline=self._experimentalist_pipeline,
-            experiment_runner_callable=self._experiment_runner_callable,
-            theorist_estimator=self._theorist_estimator,
+        return _executor_collection_factory(
+            experimentalist=self._experimentalist_pipeline,
+            experiment_runner=self._experiment_runner_callable,
+            theorist=self._theorist_estimator,
         )
-        return executor_collection
+
+
+def _executor_collection_factory(experimentalist, experiment_runner, theorist):
+    executor_collection = {
+        "full_cycle": full_cycle_wrapper(
+            experimentalist_pipeline=experimentalist,
+            experiment_runner_callable=experiment_runner,
+            theorist_estimator=theorist,
+        )
+    }
+    return executor_collection
```

### Comparing `autora-workflow-0.2.1/src/autora/workflow/planner.py` & `autora-workflow-0.3.0/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora/workflow/plotting.py` & `autora-workflow-0.3.0/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora/workflow/protocol.py` & `autora-workflow-0.3.0/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.0/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora/workflow/state/history.py` & `autora-workflow-0.3.0/src/autora/workflow/state/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,22 +72,22 @@
                                     Result(data='c1', kind=ResultKind.CONDITION),
                                     Result(data='c2', kind=ResultKind.CONDITION),
                                     Result(data='o1', kind=ResultKind.OBSERVATION),
                                     Result(data='o2', kind=ResultKind.OBSERVATION),
                                     Result(data='m1', kind=ResultKind.MODEL),
                                     Result(data='m2', kind=ResultKind.MODEL)])
         """
-        self._history: List
+        self.data: List
 
         if history is not None:
-            self._history = list(history)
+            self.data = list(history)
         else:
-            self._history = []
+            self.data = []
 
-        self._history += _init_result_list(
+        self.data += _init_result_list(
             variables=variables,
             params=params,
             conditions=conditions,
             observations=observations,
             models=models,
         )
 
@@ -215,24 +215,24 @@
         history_extension += _init_result_list(
             variables=variables,
             params=params,
             conditions=conditions,
             observations=observations,
             models=models,
         )
-        new_full_history = self._history + history_extension
+        new_full_history = self.data + history_extension
 
         return History(history=new_full_history)
 
     def __repr__(self):
         return f"{type(self).__name__}({self.history})"
 
     @property
     def _by_kind(self):
-        return _history_to_kind(self._history)
+        return _history_to_kind(self.data)
 
     @property
     def variables(self) -> VariableCollection:
         """
 
         Examples:
             The initial object is empty:
@@ -367,15 +367,15 @@
             If we add a new value, like the params object, the updated value is added to the
             end of the history:
             >>> h = h.update(params={'new': 'param'})
             >>> h.history  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             [..., Result(data={'new': 'param'}, kind=ResultKind.PARAMS)]
 
         """
-        return self._history
+        return self.data
 
     def filter_by(self, kind: Optional[Set[Union[str, ResultKind]]] = None) -> History:
         """
         Return a copy of the object with only data belonging to the specified kinds.
 
         Examples:
             >>> h = History(models=['m1', 'm2'], conditions=['c1', 'c2'],
@@ -404,15 +404,15 @@
                      Result(data='m2', kind=ResultKind.MODEL)])
 
         """
         if kind is None:
             return self
         else:
             kind_ = {ResultKind(s) for s in kind}
-            filtered_history = _filter_history(self._history, kind_)
+            filtered_history = _filter_history(self.data, kind_)
             new_object = History(history=filtered_history)
             return new_object
 
 
 @dataclass(frozen=True)
 class Result(SupportsDataKind):
     """
```

### Comparing `autora-workflow-0.2.1/src/autora/workflow/state/param.py` & `autora-workflow-0.3.0/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.0/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.1/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.3.0/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.2.1
+Version: 0.3.0
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE.md
 
 # AutoRA Workflow
```

### Comparing `autora-workflow-0.2.1/tests/test_controller_plots.py` & `autora-workflow-0.3.0/tests/test_controller_plots.py`

 * *Files identical despite different names*

