# Comparing `tmp/autora-3.0.0a7.tar.gz` & `tmp/autora-3.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0a7.tar", last modified: Wed May  3 17:11:35 2023, max compression
+gzip compressed data, was "autora-3.0.0a8.tar", last modified: Thu May  4 16:56:06 2023, max compression
```

## Comparing `autora-3.0.0a7.tar` & `autora-3.0.0a8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 17:11:24.000000 autora-3.0.0a7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.819201 autora-3.0.0a7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.819201 autora-3.0.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/publish-package-anaconda-org.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/test-conda-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/test-poetry-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-03 17:11:24.000000 autora-3.0.0a7/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-03 17:11:24.000000 autora-3.0.0a7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.819201 autora-3.0.0a7/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 17:11:24.000000 autora-3.0.0a7/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-03 17:11:24.000000 autora-3.0.0a7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:24.000000 autora-3.0.0a7/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 17:11:24.000000 autora-3.0.0a7/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 17:11:24.000000 autora-3.0.0a7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 17:11:24.000000 autora-3.0.0a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-03 17:11:35.823201 autora-3.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-05-03 17:11:24.000000 autora-3.0.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.819201 autora-3.0.0a7/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 17:11:24.000000 autora-3.0.0a7/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 17:11:24.000000 autora-3.0.0a7/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/experiment-runner/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/experimentalists/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 17:11:24.000000 autora-3.0.0a7/docs/theorist/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-03 17:11:24.000000 autora-3.0.0a7/mkdocs/base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 17:11:24.000000 autora-3.0.0a7/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-03 17:11:24.000000 autora-3.0.0a7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-03 17:11:24.000000 autora-3.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:11:35.823201 autora-3.0.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 17:11:24.000000 autora-3.0.0a7/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:11:35.823201 autora-3.0.0a7/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-03 17:11:35.000000 autora-3.0.0a7/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-03 17:11:35.000000 autora-3.0.0a7/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:11:35.000000 autora-3.0.0a7/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 17:11:35.000000 autora-3.0.0a7/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:11:35.000000 autora-3.0.0a7/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 16:55:38.000000 autora-3.0.0a8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-package-anaconda-org.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-conda-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-poetry-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 16:55:38.000000 autora-3.0.0a8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-04 16:55:38.000000 autora-3.0.0a8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-04 16:55:38.000000 autora-3.0.0a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-04 16:56:06.494232 autora-3.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-05-04 16:55:38.000000 autora-3.0.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.486232 autora-3.0.0a8/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 16:55:38.000000 autora-3.0.0a8/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 16:55:38.000000 autora-3.0.0a8/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/experiment-runner/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/experimentalists/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/theorist/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs/base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-04 16:55:38.000000 autora-3.0.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:56:06.494232 autora-3.0.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 16:55:38.000000 autora-3.0.0a8/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/top_level.txt
```

### Comparing `autora-3.0.0a7/.github/pull_request_template.md` & `autora-3.0.0a8/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/publish-documentation-gh-pages.yml` & `autora-3.0.0a8/.github/workflows/publish-documentation-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/publish-package-anaconda-org.yml` & `autora-3.0.0a8/.github/workflows/publish-package-anaconda-org.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/publish-package-pypi.yml` & `autora-3.0.0a8/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/test-conda-build.yml` & `autora-3.0.0a8/.github/workflows/test-conda-build.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.0.0a8/.github/workflows/test-pre-commit-hooks.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.github/workflows/test-pytest.yml` & `autora-3.0.0a8/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.gitignore` & `autora-3.0.0a8/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.idea/autora.iml` & `autora-3.0.0a8/.idea/autora.iml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml` & `autora-3.0.0a8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.idea/modules.xml` & `autora-3.0.0a8/.idea/modules.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/.pre-commit-config.yaml` & `autora-3.0.0a8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/LICENSE.md` & `autora-3.0.0a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/PKG-INFO` & `autora-3.0.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a7
+Version: 3.0.0a8
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -28,14 +28,15 @@
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
 Provides-Extra: theorist-darts
 Provides-Extra: all-experimentalists
+Provides-Extra: experimentalist-novelty-sampler
 Provides-Extra: experimentalist-inequality-sampler
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
```

### Comparing `autora-3.0.0a7/README.md` & `autora-3.0.0a8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -419,14 +419,43 @@
     with the content of the release.
   - Select whether this is a pre-release or a new "latest" release. It's a "pre-release" if there's an alpha, 
     beta, or release candidate number in the tag name, otherwise it's a new "latest" release.
   - Click on "Publish release"
 - GitHub actions will run to create and publish the PyPI and Anaconda packages, and publish the documentation. Check in 
   GitHub actions whether they run without errors and fix any errors which occur.
 
+# How to add new packages
+
+This demonstrates how to add a package published under autora-theorist-example in pyPI in the GitHub repository 
+example-contributor/contributor-theorist
+
+## Add the package as optional dependency
+In the `pyorject.toml` file add an optional dependency for the package in the [project.optional-dependencies] section:
+```toml
+example-theorist = ["autora-theorits-example"]
+```
+Add the example-theorist to be part of the all-theorists dependency:
+```toml
+all-theorists = [
+    ...
+    "autora[example-theorist]",
+    ...
+]
+```
+
+## Import documentation from the package repository
+Import the documentation in the `mkdocs.yml` file:
+```yml
+- User Guide:
+  - Theorists:
+    - Overview: 'theorist/overview.md'
+    ...
+    - Example Theorist: '!import https://github.com/example-contributor/contributor-theorist/?branch=main&extra_imports=["mkdocs/base.yml"]'
+    ...
+```
 
 # How to Develop
 
 Install this in an environment using your chosen package manager. 
 
 ## Using `virtualenv`
```

### Comparing `autora-3.0.0a7/conda/autora/meta.yaml` & `autora-3.0.0a8/conda/autora/meta.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/docs/experimentalists/overview.md` & `autora-3.0.0a8/docs/experimentalists/overview.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/docs/img/logo.png` & `autora-3.0.0a8/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/docs/img/overview.png` & `autora-3.0.0a8/docs/img/overview.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/docs/index.md` & `autora-3.0.0a8/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/docs/theorist/overview.md` & `autora-3.0.0a8/docs/theorist/overview.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/mkdocs/base.yml` & `autora-3.0.0a8/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a7/mkdocs.yml` & `autora-3.0.0a8/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   custom_dir: mkdocs/overrides
   features:
     - content.action.edit
     - content.action.view
+    - navigation.indexes
 
 nav:
 - Introduction: 'index.md'
 - Tutorials:
   - Automated Theorist
   - Automated Experimentalist
   - Closed-Loop Discovery
@@ -40,14 +41,15 @@
   - Theorists:
     - Overview: 'theorist/overview.md'
     - DARTS: '!import https://github.com/autoresearch/autora-theorist-darts/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - BSR
     - BMS
   - Experimentalists:
     - Overview: 'experimentalists/overview.md'
+    - Novelty Sampler: '!import https://github.com/autoresearch/autora-novelty-sampler/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - Inequality Sampler: '!import https://github.com/autoresearch/autora-experimentalist-inequality-sampler/?branch=main&extra_imports=["mkdocs/base.yml"]'
   - Experiment Runners:
     - Overview: 'experiment-runner/overview.md'
   - Synthetic Datasets: '!import https://github.com/autoresearch/autora-synthetic-data/?branch=main&extra_imports=["mkdocs/base.yml"]'
   - Workflow: '!import https://github.com/autoresearch/autora-workflow/?branch=main&extra_imports=["mkdocs/base.yml"]'
 - Contributor Guide:
   - Module Contributions
```

### Comparing `autora-3.0.0a7/pyproject.toml` & `autora-3.0.0a8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,18 @@
   "autora[theorist-darts]",
 ]
 theorist-darts = [
   "autora-theorist-darts",
 ]
 all-experimentalists = [
   "autora[experimentalist-inequality-sampler]",
+  "autora[experimentalist-novelty-sampler]",
+]
+experimentalist-novelty-sampler =[
+  "autora-novelty-sampler"
 ]
 experimentalist-inequality-sampler =[
   "autora-experimentalist-inequality-sampler"
 ]
 all-experiment-runners = [
 ]
 synthetic-experiments = [
```

### Comparing `autora-3.0.0a7/src/autora.egg-info/PKG-INFO` & `autora-3.0.0a8/src/autora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a7
+Version: 3.0.0a8
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -28,14 +28,15 @@
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
 Provides-Extra: theorist-darts
 Provides-Extra: all-experimentalists
+Provides-Extra: experimentalist-novelty-sampler
 Provides-Extra: experimentalist-inequality-sampler
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
```

### Comparing `autora-3.0.0a7/src/autora.egg-info/SOURCES.txt` & `autora-3.0.0a8/src/autora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

