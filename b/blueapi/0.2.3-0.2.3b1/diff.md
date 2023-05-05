# Comparing `tmp/blueapi-0.2.3.tar.gz` & `tmp/blueapi-0.2.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.2.3.tar", last modified: Fri May  5 09:29:25 2023, max compression
+gzip compressed data, was "blueapi-0.2.3b1.tar", last modified: Mon Apr 24 15:19:11 2023, max compression
```

## Comparing `blueapi-0.2.3.tar` & `blueapi-0.2.3b1.tar`

### file list

```diff
@@ -1,180 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.771493 blueapi-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.747493 blueapi-0.2.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-05 09:29:15.000000 blueapi-0.2.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-05 09:29:15.000000 blueapi-0.2.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.747493 blueapi-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.739493 blueapi-0.2.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.747493 blueapi-0.2.3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.747493 blueapi-0.2.3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.747493 blueapi-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 09:29:15.000000 blueapi-0.2.3/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 09:29:15.000000 blueapi-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-05 09:29:15.000000 blueapi-0.2.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 09:29:15.000000 blueapi-0.2.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-05 09:29:15.000000 blueapi-0.2.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 09:29:15.000000 blueapi-0.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 09:29:15.000000 blueapi-0.2.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 09:29:15.000000 blueapi-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-05 09:29:25.771493 blueapi-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-05 09:29:15.000000 blueapi-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-05 09:29:15.000000 blueapi-0.2.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/config/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 09:29:15.000000 blueapi-0.2.3/config/adsim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 09:29:15.000000 blueapi-0.2.3/config/bl45p.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/explanations/type_validators.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.751493 blueapi-0.2.3/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/developer/tutorials/dev-run.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/images/debug-vscode.png
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/reference/asyncapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/reference/asyncapi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 09:29:15.000000 blueapi-0.2.3/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.743493 blueapi-0.2.3/helm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.755493 blueapi-0.2.3/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.759493 blueapi-0.2.3/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.759493 blueapi-0.2.3/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 09:29:15.000000 blueapi-0.2.3/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-05 09:29:15.000000 blueapi-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:29:25.771493 blueapi-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.743493 blueapi-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.759493 blueapi-0.2.3/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.759493 blueapi-0.2.3/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.763493 blueapi-0.2.3/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/bluesky_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.763493 blueapi-0.2.3/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.763493 blueapi-0.2.3/src/blueapi/plans/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/plans/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/plans/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.763493 blueapi-0.2.3/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/service/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/startup/adsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/startup/bl45p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/startup/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-05 09:29:15.000000 blueapi-0.2.3/src/blueapi/worker/worker_busy_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.759493 blueapi-0.2.3/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 09:29:25.000000 blueapi-0.2.3/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.767493 blueapi-0.2.3/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.771493 blueapi-0.2.3/tests/plans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/plans/test_scanspec_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.771493 blueapi-0.2.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/utils/test_thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:29:25.771493 blueapi-0.2.3/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-05 09:29:15.000000 blueapi-0.2.3/tests/worker/test_reworker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/config/adsim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/config/bl45p.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/type_validators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/bl45p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/plans/test_scanspec_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.2.3/.devcontainer/Dockerfile` & `blueapi-0.2.3b1/.devcontainer/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 # Add apt-get system dependecies for runtime here if needed
 
 # copy the virtual environment from the build stage and put it in PATH
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
-ENTRYPOINT ["blueapi"]
+ENTRYPOINT ["bluesky"]
 CMD ["worker"]
```

### Comparing `blueapi-0.2.3/.devcontainer/devcontainer.json` & `blueapi-0.2.3b1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/CONTRIBUTING.rst` & `blueapi-0.2.3b1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/actions/install_requirements/action.yml` & `blueapi-0.2.3b1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/dependabot.yml` & `blueapi-0.2.3b1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/pages/make_switcher.py` & `blueapi-0.2.3b1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/workflows/code.yml` & `blueapi-0.2.3b1/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,20 @@
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
         python: ["3.9", "3.10", "3.11"]
-        install: [".[dev]", "-e .[dev]"]
+        install: ["-e .[dev]"]
+        # Make one version be non-editable to test both paths of version code
+        include:
+          - os: "ubuntu-latest"
+            python: "3.8"
+            install: ".[dev]"
 
     services:
       activemq:
         image: rmohr/activemq:5.14.5-alpine
         ports:
           - 61613:61613
```

### Comparing `blueapi-0.2.3/.github/workflows/docs.yml` & `blueapi-0.2.3b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/workflows/docs_clean.yml` & `blueapi-0.2.3b1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/workflows/helm.yml` & `blueapi-0.2.3b1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.github/workflows/linkcheck.yml` & `blueapi-0.2.3b1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.gitignore` & `blueapi-0.2.3b1/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.pre-commit-config.yaml` & `blueapi-0.2.3b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.vscode/launch.json` & `blueapi-0.2.3b1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/.vscode/settings.json` & `blueapi-0.2.3b1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/LICENSE` & `blueapi-0.2.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/PKG-INFO` & `blueapi-0.2.3b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.3
+Version: 0.2.3b1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,19 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/DiamondLightSource/blueapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 blueapi
 ===========================
```

### Comparing `blueapi-0.2.3/README.rst` & `blueapi-0.2.3b1/README.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/conf.py` & `blueapi-0.2.3b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/explanations/architecture.rst` & `blueapi-0.2.3b1/docs/developer/explanations/architecture.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/explanations/decisions.rst` & `blueapi-0.2.3b1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/explanations/lifecycle.rst` & `blueapi-0.2.3b1/docs/developer/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/explanations/type_validators.rst` & `blueapi-0.2.3b1/docs/developer/explanations/type_validators.rst`

 * *Files 21% similar despite different names*

```diff
@@ -14,25 +14,25 @@
     # Internally becomes something like
 
     class MyPlanModel(BaseModel):
         a: int
         b: str = "b"
 
 
-That way, when the plan parameters are sent in JSON form, they can be parsed and validated by pydantic.
-However, it must also cover the case where a plan doesn't take a simple dictionary, list or primitive but
-instead a device, such as a detector.
+That way, when the plan parameters are send in JSON form, they can be parsed and validated by pydantic. 
+However, it must also cover the case where a plan doesn't take a simple dictionary, list or primitive but 
+instead a device, such as a detector. 
 
 .. code:: python
 
     def my_plan(a: int, b: Readable) -> Plan:
         ...
 
 
-An Ophyd object cannot be passed over the network as JSON because it has state.
+An Ophyd object cannot be passed over the network as JSON because it has state. 
 Instead, a string is passed, representing an ID of the object known to the ``BlueskyContext``.
 At the time a plan's parameters are validated, blueapi must take all the strings that are supposed
 to be devices and look them up against the context. For example with the request:
 
 .. code:: json
 
     {
@@ -48,49 +48,59 @@
     }
 
 ``andor`` and ``pilatus`` should be looked up and replaced with Ophyd objects.
 
 
 Solution
 --------
-When the context loads available plans, it iterates through the type signature
-and replaces any reference to a bluesky protocol (or instance of a protocol)
-with a new class that extends the original type. Defining a class validator on
-this new type allows it to check that the string being deserialised is the ID of
-a device of the correct type.
-
-These new intermediate types are used only in the deserialisation process. The
-object returned from validator method is not checked by pydantic so it can be
-the actual instance and the plan never sees the runtime generated reference
-type, only the type it was expecting.
-
-.. note:: This uses the fact that the new types generated at runtime have access to
-    the context that required them via their closure. This circumvents the usual
-    problem of pydantic validation not being able to access external state when
-    validating or deserialising.
 
-.. code:: python
+Before pydantic, blueapi used apischema_, which had an ideal feature for this called conversions_.
+Currently in the utils module of a blueapi is a similar feature called type validators.
+
+They enable the ``BlueskyContext`` to dynamically generate pydantic models, like above, that look 
+roughly like this:
 
+.. code:: python
+    
     def my_plan(a: int, b: Readable) -> Plan:
         ...
 
     # Becomes
 
     class MyPlanModel(BaseModel):
         a: int
-        b: Reference[Readable]
+        b: Readable
 
+        @validator("b")
+        def valdiate_b(self, val: str) -> Readable:
+            return ctx.find_device(val)
 
-This also allows ``Readable`` to be placed at various type levels. For example:
 
-.. code:: python
+It also handles the case of the ``Readable`` type being placed at various type levels? For example:
 
+.. code:: python
+    
     def my_weird_plan(
-        a: Readable,
-        b: List[Readable],
-        c: Dict[str, Readable],
-        d: List[List[Readable]],
+        a: Readable, 
+        b: List[Readable], 
+        c: Dict[str, Readable], 
+        d: List[List[Readable]], 
         e: List[Dict[str, Set[Readable]]]) -> Plan:
         ...
 
 
+Implementation Details
+----------------------
+
+Pydantic models have validators: functions that are applied to specific fields by name. This is
+insufficient for the requirements here, it would be helpful if validators could be applied by type, 
+rather than name.
+The type validation module is essentially a shim layer that works out the names of all fields of a
+particular type, then creates validators for all of those names. It also supports the type being in
+nested lists and/or dictionaries, as mentioned above.
+The field names are deteted by comparing the type annotation in the model to the type requested.
+The actual validator is a function supplied by the caller, but if a list or dictionary is passed,
+it will apply it to each item/value.
+
 .. _pydantic: https://docs.pydantic.dev/
+.. _apischema: https://wyfo.github.io/apischema/0.18/
+.. _conversions: https://wyfo.github.io/apischema/0.18/conversions/
```

### Comparing `blueapi-0.2.3/docs/developer/how-to/build-docs.rst` & `blueapi-0.2.3b1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/how-to/lint.rst` & `blueapi-0.2.3b1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/how-to/make-release.rst` & `blueapi-0.2.3b1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/how-to/run-tests.rst` & `blueapi-0.2.3b1/docs/developer/how-to/run-tests.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/how-to/update-tools.rst` & `blueapi-0.2.3b1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/index.rst` & `blueapi-0.2.3b1/docs/developer/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Developer Guide
 ===============
 
 Documentation is split into four categories, also accessible from links in the
 side-bar.
 
-.. note:: Assumes you have read the `../user/index`
-
 .. grid:: 2
     :gutter: 4
 
     .. grid-item-card:: :material-regular:`directions_run;3em`
 
         .. toctree::
             :caption: Tutorials
             :maxdepth: 1
 
             tutorials/dev-install
-            tutorials/dev-run
 
         +++
 
         Tutorials for getting up and running as a developer.
 
     .. grid-item-card:: :material-regular:`task;3em`
```

### Comparing `blueapi-0.2.3/docs/developer/reference/standards.rst` & `blueapi-0.2.3b1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/developer/tutorials/dev-install.rst` & `blueapi-0.2.3b1/docs/developer/tutorials/dev-install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     $ git clone git://github.com/DiamondLightSource/blueapi.git
 
 Install dependencies
 --------------------
 
 You can choose to either develop on the host machine using a `venv` (which
-requires python 3.9 or later) or to run in a container under `VSCode
+requires python 3.8 or later) or to run in a container under `VSCode
 <https://code.visualstudio.com/>`_
 
 .. tab-set::
 
     .. tab-item:: Local virtualenv
 
         .. code::
```

### Comparing `blueapi-0.2.3/docs/images/blueapi-architecture.png` & `blueapi-0.2.3b1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/images/dls-favicon.ico` & `blueapi-0.2.3b1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/images/dls-logo.svg` & `blueapi-0.2.3b1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/index.rst` & `blueapi-0.2.3b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/user/explanations/docs-structure.rst` & `blueapi-0.2.3b1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/docs/user/index.rst` & `blueapi-0.2.3b1/docs/user/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -46,13 +46,12 @@
     .. grid-item-card:: :material-regular:`menu_book;3em`
 
         .. toctree::
             :caption: Reference
             :maxdepth: 1
 
             reference/api
-            reference/asyncapi
             ../genindex
 
         +++
 
         Technical reference material including APIs and release notes.
```

### Comparing `blueapi-0.2.3/docs/user/tutorials/installation.rst` & `blueapi-0.2.3b1/docs/user/tutorials/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Check your version of python
 ----------------------------
 
-You will need python 3.9 or later. You can check your version of python by
+You will need python 3.8 or later. You can check your version of python by
 typing into a terminal::
 
     $ python3 --version
 
 
 Create a virtual environment
 ----------------------------
```

### Comparing `blueapi-0.2.3/helm/blueapi/Chart.yaml` & `blueapi-0.2.3b1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.2.3b1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/helm/blueapi/templates/deployment.yaml` & `blueapi-0.2.3b1/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.2.3b1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/helm/blueapi/values.yaml` & `blueapi-0.2.3b1/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/pyproject.toml` & `blueapi-0.2.3b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blueapi"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "One line description of your module"
 dependencies = [
     "bluesky",
@@ -22,15 +23,15 @@
     "scanspec",
     "PyYAML",
     "click",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -43,16 +44,15 @@
     "sphinx-design",
     "tox-direct",
     "types-mock",
     "types-PyYAML",
 ]
 
 [project.scripts]
-blueapi = "blueapi.cli:main"
-bluesky = "blueapi.cli._deprecated:main"
+bluesky = "blueapi.cli:main"
 
 [project.urls]
 GitHub = "https://github.com/DiamondLightSource/blueapi"
 
 [[project.authors]] # Further authors may be added by duplicating this section
 email = "callum.forrester@diamond.ac.uk"
 name = "Callum Forrester"
```

### Comparing `blueapi-0.2.3/src/blueapi/cli/amq.py` & `blueapi-0.2.3b1/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/cli/cli.py` & `blueapi-0.2.3b1/src/blueapi/cli/cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/cli/updates.py` & `blueapi-0.2.3b1/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/config.py` & `blueapi-0.2.3b1/src/blueapi/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/core/__init__.py` & `blueapi-0.2.3b1/src/blueapi/core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .bluesky_event_loop import configure_bluesky_event_loop
 from .bluesky_types import (
     BLUESKY_PROTOCOLS,
     DataEvent,
     Device,
     MsgGenerator,
     Plan,
     PlanGenerator,
@@ -24,9 +23,8 @@
     "EventPublisher",
     "EventStream",
     "DataEvent",
     "WatchableStatus",
     "is_bluesky_compatible_device",
     "is_bluesky_plan_generator",
     "is_bluesky_compatible_device_type",
-    "configure_bluesky_event_loop",
 ]
```

### Comparing `blueapi-0.2.3/src/blueapi/core/bluesky_types.py` & `blueapi-0.2.3b1/src/blueapi/core/bluesky_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import Any, Callable, Generator, Mapping, Type, Union, get_type_hints
+from typing import Any, Callable, Generator, Mapping, Type, Union
 
 from bluesky.protocols import (
     Checkable,
     Configurable,
     Flyable,
     HasHints,
     HasName,
@@ -71,19 +71,18 @@
 
 
 def _follows_bluesky_protocols(obj: Any) -> bool:
     return any(map(lambda protocol: isinstance(obj, protocol), BLUESKY_PROTOCOLS))
 
 
 def is_bluesky_plan_generator(func: PlanGenerator) -> bool:
-    try:
-        return get_type_hints(func).get("return") is MsgGenerator
-    except TypeError:
-        # get_type_hints fails on some objects (such as Union or Optinoal)
-        return False
+    return (
+        hasattr(func, "__annotations__")
+        and func.__annotations__.get("return") is MsgGenerator
+    )
 
 
 class Plan(BlueapiBaseModel):
     """
     A plan that can be run
     """
```

### Comparing `blueapi-0.2.3/src/blueapi/core/device_lookup.py` & `blueapi-0.2.3b1/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/core/event.py` & `blueapi-0.2.3b1/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/messaging/base.py` & `blueapi-0.2.3b1/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.2.3b1/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/messaging/utils.py` & `blueapi-0.2.3b1/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/plans/plans.py` & `blueapi-0.2.3b1/src/blueapi/plans/plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/plans/stubs.py` & `blueapi-0.2.3b1/src/blueapi/plans/stubs.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/service/app.py` & `blueapi-0.2.3b1/src/blueapi/service/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         self._template.subscribe("worker.run", self._on_run_request)
         self._template.subscribe("worker.plans", self._get_plans)
         self._template.subscribe("worker.devices", self._get_devices)
 
         self._template.connect()
 
-        self._worker.run()
+        self._worker.run_forever()
 
     def _publish_event_streams(
         self, streams_to_destinations: Mapping[EventStream, str]
     ) -> None:
         for stream, destination in streams_to_destinations.items():
             self._publish_event_stream(stream, destination)
```

### Comparing `blueapi-0.2.3/src/blueapi/service/model.py` & `blueapi-0.2.3b1/src/blueapi/service/model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/startup/adsim.py` & `blueapi-0.2.3b1/src/blueapi/startup/adsim.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/startup/bl45p.py` & `blueapi-0.2.3b1/src/blueapi/startup/bl45p.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/startup/example.py` & `blueapi-0.2.3b1/src/blueapi/startup/example.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/startup/simmotor.py` & `blueapi-0.2.3b1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/utils/base_model.py` & `blueapi-0.2.3b1/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/utils/config.py` & `blueapi-0.2.3b1/src/blueapi/utils/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/utils/modules.py` & `blueapi-0.2.3b1/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/utils/serialization.py` & `blueapi-0.2.3b1/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/utils/thread_exception.py` & `blueapi-0.2.3b1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/worker/event.py` & `blueapi-0.2.3b1/src/blueapi/worker/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/worker/multithread.py` & `blueapi-0.2.3b1/src/blueapi/worker/multithread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import Optional, TypeVar
 
-from blueapi.core import configure_bluesky_event_loop
 from blueapi.utils import handle_all_exceptions
 
 from .worker import Worker
 
 LOGGER = logging.getLogger(__name__)
 
 T = TypeVar("T")
@@ -40,11 +39,9 @@
     Helper function, run a worker forever, includes support for
     printing exceptions to stdout from a non-main thread.
 
     Args:
         worker (Worker[T]): The worker to run
     """
 
-    LOGGER.info("Setting up event loop")
-    configure_bluesky_event_loop()
     LOGGER.info("Worker starting")
-    worker.run()
+    worker.run_forever()
```

### Comparing `blueapi-0.2.3/src/blueapi/worker/task.py` & `blueapi-0.2.3b1/src/blueapi/worker/task.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/src/blueapi/worker/worker.py` & `blueapi-0.2.3b1/src/blueapi/worker/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,30 +21,17 @@
 
         Args:
             __name (str): A unique name to identify this task
             __task (T): The task to run
         """
 
     @abstractmethod
-    def start(self) -> None:
+    def run_forever(self) -> None:
         """
-        Start worker in a new thread. Does not block, configures the bluesky
-        event loop in the new thread.
-        """
-
-    @abstractmethod
-    def run(self) -> None:
-        """
-        Run all tasks that are submitted to the worker. Blocks thread.
-        """
-
-    @abstractmethod
-    def stop(self) -> None:
-        """
-        Command the worker to gracefully stop. Blocks until it has shut down.
+        Run all tasks as-submitted. Blocks thread.
         """
 
     @property
     @abstractmethod
     def worker_events(self) -> EventStream[WorkerEvent, int]:
         """
         Events representing changes/errors in worker state
```

### Comparing `blueapi-0.2.3/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.2.3b1/src/blueapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.3
+Version: 0.2.3b1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,19 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/DiamondLightSource/blueapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 blueapi
 ===========================
```

### Comparing `blueapi-0.2.3/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.2.3b1/src/blueapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,21 @@
 docs/developer/how-to/lint.rst
 docs/developer/how-to/make-release.rst
 docs/developer/how-to/run-tests.rst
 docs/developer/how-to/static-analysis.rst
 docs/developer/how-to/update-tools.rst
 docs/developer/reference/standards.rst
 docs/developer/tutorials/dev-install.rst
-docs/developer/tutorials/dev-run.rst
 docs/images/blueapi-architecture.png
-docs/images/debug-vscode.png
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
 docs/user/index.rst
 docs/user/explanations/docs-structure.rst
 docs/user/how-to/run-container.rst
 docs/user/reference/api.rst
-docs/user/reference/asyncapi.rst
-docs/user/reference/asyncapi.yaml
 docs/user/tutorials/installation.rst
 helm/blueapi/.helmignore
 helm/blueapi/Chart.yaml
 helm/blueapi/values.yaml
 helm/blueapi/templates/NOTES.txt
 helm/blueapi/templates/_helpers.tpl
 helm/blueapi/templates/configmap.yaml
@@ -69,20 +65,18 @@
 src/blueapi.egg-info/SOURCES.txt
 src/blueapi.egg-info/dependency_links.txt
 src/blueapi.egg-info/entry_points.txt
 src/blueapi.egg-info/requires.txt
 src/blueapi.egg-info/top_level.txt
 src/blueapi/cli/__init__.py
 src/blueapi/cli/__main__.py
-src/blueapi/cli/_deprecated.py
 src/blueapi/cli/amq.py
 src/blueapi/cli/cli.py
 src/blueapi/cli/updates.py
 src/blueapi/core/__init__.py
-src/blueapi/core/bluesky_event_loop.py
 src/blueapi/core/bluesky_types.py
 src/blueapi/core/context.py
 src/blueapi/core/device_lookup.py
 src/blueapi/core/event.py
 src/blueapi/messaging/__init__.py
 src/blueapi/messaging/base.py
 src/blueapi/messaging/context.py
@@ -101,21 +95,21 @@
 src/blueapi/startup/simmotor.py
 src/blueapi/utils/__init__.py
 src/blueapi/utils/base_model.py
 src/blueapi/utils/config.py
 src/blueapi/utils/modules.py
 src/blueapi/utils/serialization.py
 src/blueapi/utils/thread_exception.py
+src/blueapi/utils/type_validator.py
 src/blueapi/worker/__init__.py
 src/blueapi/worker/event.py
 src/blueapi/worker/multithread.py
 src/blueapi/worker/reworker.py
 src/blueapi/worker/task.py
 src/blueapi/worker/worker.py
-src/blueapi/worker/worker_busy_error.py
 tests/conftest.py
 tests/test_cli.py
 tests/core/__init__.py
 tests/core/test_context.py
 tests/core/test_event.py
 tests/messaging/__init__.py
 tests/messaging/test_stomptemplate.py
@@ -128,8 +122,8 @@
 tests/utils/lacksall.py
 tests/utils/nested_config.yaml
 tests/utils/override_config.yaml
 tests/utils/test_base_model.py
 tests/utils/test_config.py
 tests/utils/test_modules.py
 tests/utils/test_thread_exception.py
-tests/worker/test_reworker.py
+tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.2.3/tests/conftest.py` & `blueapi-0.2.3b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/core/test_event.py` & `blueapi-0.2.3b1/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/messaging/test_stomptemplate.py` & `blueapi-0.2.3b1/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/messaging/test_utils.py` & `blueapi-0.2.3b1/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/plans/test_scanspec_metadata.py` & `blueapi-0.2.3b1/tests/plans/test_scanspec_metadata.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/utils/test_config.py` & `blueapi-0.2.3b1/tests/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.3/tests/utils/test_thread_exception.py` & `blueapi-0.2.3b1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

