# Comparing `tmp/geocat.viz-2023.3.0.post0.tar.gz` & `tmp/geocat.viz-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.viz-2023.3.0.post0.tar", last modified: Tue Mar 28 15:22:57 2023, max compression
+gzip compressed data, was "geocat.viz-2023.5.0.tar", last modified: Fri May  5 15:41:39 2023, max compression
```

## Comparing `geocat.viz-2023.3.0.post0.tar` & `geocat.viz-2023.5.0.tar`

### file list

```diff
@@ -1,57 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.355460 geocat.viz-2023.3.0.post0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.github/workflows/upstream-examples-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-28 15:22:57.355460 geocat.viz-2023.3.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/ci/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/docs/user_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 15:22:57.355460 geocat.viz-2023.3.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.351460 geocat.viz-2023.3.0.post0/src/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/src/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.355460 geocat.viz-2023.3.0.post0/src/geocat/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/src/geocat/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27234 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/src/geocat/viz/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-03-28 15:22:43.000000 geocat.viz-2023.3.0.post0/src/geocat/viz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:22:57.355460 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 15:22:57.000000 geocat.viz-2023.3.0.post0/src/geocat.viz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/ISSUE_TEMPLATE/plot-type-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/upstream-examples-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/notpublic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/public.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   171533 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_long.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   291776 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_nsf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   180376 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_square.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/src/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/src/geocat/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30219 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51827 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/src/geocat.viz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/top_level.txt
```

### Comparing `geocat.viz-2023.3.0.post0/.github/workflows/pypi.yaml` & `geocat.viz-2023.5.0/.github/workflows/pypi.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 name: Upload geocat-viz to PyPI
 on:
-  release:
-    types:
-      - published
+  workflow_dispatch:
+
 jobs:
   test-build:
     if: github.repository == 'NCAR/geocat-viz'
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4.5.0
         with:
-          python-version: '3.x'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
         run: |
           python setup.py sdist bdist_wheel
           python -m pip wheel . -w dist --no-deps
       - name: Test the artifacts
         run: |
           python -m twine check dist/*
+
   publish:
     needs: test-build
     if: startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4.5.0
         with:
-          python-version: '3.x'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
         run: |
           python setup.py sdist bdist_wheel
           python -m pip wheel . -w dist --no-deps
       - name: Test the artifacts
         run: |
           python -m twine check dist/*
+
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.4.2
+        uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
           user: __token__
           password: ${{ secrets.PYPI_GEOCAT_VIZ }}
           skip_existing: true
           verbose: true
```

### Comparing `geocat.viz-2023.3.0.post0/.github/workflows/upstream-examples-ci.yml` & `geocat.viz-2023.5.0/.github/workflows/upstream-examples-ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 name: Upstream Examples CI
 on:
-  workflow_dispatch:
+  pull_request:
   push:
     branches:
       - main
-  pull_request:
+  schedule:
+    - cron: '0 0 * * *' # Daily “At 00:00”
+  workflow_dispatch:
+
 
 jobs:
   build-and-run:
     name: Build GeoCAT-examples (${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
 
     strategy:
       fail-fast: false
       matrix:
         os: [ "ubuntu-latest", "macos-latest" ]
-        python-version: [ "3.7", "3.9" ]
+        python-version: ["3.8", "3.9", "3.10" ]
 
     steps:
     - uses: actions/checkout@v2
     - name: Install GeoCAT-examples
       run: |
         git clone https://github.com/NCAR/GeoCAT-examples.git
 
     - name: Create geocat-examples environment
       uses: mamba-org/provision-with-micromamba@main
       with:
         micromamba-version: "latest"
-        environment-name: geocat-examples
-        environment-file: ./GeoCAT-examples/conda_environment.yml
+        environment-name: geocat_viz_upstream
+        environment-file: build_envs/upstream-dev-environment.yml
 
     - name: Install geocat-viz
       run: |
         python -m pip install --no-deps --ignore-installed -vv .
 
     - name: make html
       working-directory: ./GeoCAT-examples/docs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geocat.viz-2023.3.0.post0/.pre-commit-config.yaml` & `geocat.viz-2023.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/CONTRIBUTING.md` & `geocat.viz-2023.5.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,11 +36,21 @@
         - If so, please comment (or self-assign the issue if you have permissions to do so) indicating that
         you intend to work on it.
 
         - Otherwise, you may create and self-assign an issue under
         [GeoCAT-viz Issues](https://github.com/NCAR/GeoCAT-viz/issues)
         that describes need for the functionality you are planning to contribute.
 
-2. Create a new folder under `$GEOCAT_VIZ/src/geocat/viz/` and implement your plotting function inside, making
-use of the pre-defined parent classes if appropriate
+2. Determine which module is the best home for your new function.
 
-3. Add the function to the namespace by adding it to `$GEOCAT_VIZ/src/geocat/viz/__init__.py`
+    - If necessary, create a new `.py` module under `$GEOCAT_VIZ/src/geocat/viz/`.
+
+    - Implement your plotting function inside the chosen module, making
+    use of the pre-defined parent classes if appropriate
+
+3. Add new modules to the namespace by adding it to `$GEOCAT_VIZ/src/geocat/viz/__init__.py`
+
+# Adding functionality to the User API Documentation
+
+1. Add your new function to `GEOCAT_VIZ/docs/user_api/index.rst`.
+
+2. Ensure that the function docstring has examples linking to relevant GeoCAT-Examples scripts.
```

### Comparing `geocat.viz-2023.3.0.post0/LICENSE` & `geocat.viz-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/PKG-INFO` & `geocat.viz-2023.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: geocat.viz
-Version: 2023.3.0.post0
-Home-page: https://github.com/NCAR/geocat-viz
-Maintainer: GeoCAT
-Maintainer-email: geocat@ucar.edu
-Project-URL: Documentation, https://geocat-viz.readthedocs.io
-Project-URL: Source, https://github.com/NCAR/geocat-viz
-Project-URL: Tracker, https://github.com/NCAR/geocat-viz/issues
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # GeoCAT-viz
 
 The GeoCAT-viz repo contains tools to help plot data, including convenience and plotting functions that are used
 to facilitate plotting geosciences data with Matplotlib, Cartopy, and possibly other Python ecosystem
 plotting packages. GeoCAT-viz functionality is used by
 [GeoCAT-examples](https://github.com/NCAR/geocat-examples) and is of possible use for other GeoCAT components.
```

### Comparing `geocat.viz-2023.3.0.post0/docs/Makefile` & `geocat.viz-2023.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/docs/_static/images/nsf.png` & `geocat.viz-2023.5.0/docs/_static/images/logos/nsf.png`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/docs/_templates/autosummary/class.rst` & `geocat.viz-2023.5.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/docs/citation.rst` & `geocat.viz-2023.5.0/docs/citation.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Citation
-==========
+========
 
 How to cite GeoCAT-viz
 ----------------------
 
-If you use this software, please cite it as described below.
+If you use this software, we would appreciate a citation!
 
 Each GeoCAT-viz version is assigned a separate Digital Object Identifier (DOI) to allow
 users to access older releases. This ensures that users are not only able to cite the specific
 software version through DOIs but are also able to download & use the corresponding release for
 reproducibility purposes.
 
+Please find DOIs for all the GeoCAT-viz versions `here
+<https://zenodo.org/search?page=1&size=20&q=conceptrecid:%226678345%22&sort=-version&all_versions=True>`_.
+
+
 If you would like to cite GeoCAT-viz as a whole (without referring to a specific version), use
 the following text:
 
-**Visualization & Analysis Systems Technologies. (2020).
-Geoscience Community Analysis Toolkit: GeoCAT-viz [Software].
-Boulder, CO: UCAR/NCAR - Computational and Informational System Lab. doi:10.5281/zenodo.6678345.**
+    **Visualization & Analysis Systems Technologies. (2020).
+    Geoscience Community Analysis Toolkit: GeoCAT-viz [Software].
+    Boulder, CO: UCAR/NCAR - Computational and Informational System Lab. doi:10.5281/zenodo.6678345.**
 
 Instead, if you would like to cite a specific version of GeoCAT-viz, use the following text:
 
-**Visualization & Analysis Systems Technologies. (\<Year\>).
-Geoscience Community Analysis Toolkit: GeoCAT-viz (v\<version\>) [Software].
-Boulder, CO, USA: UCAR/NCAR - Computational and Informational System Lab. doi:\<DOI\>.**
+    **Visualization & Analysis Systems Technologies. (\<Year\>).
+    Geoscience Community Analysis Toolkit: GeoCAT-viz (v\<version\>) [Software].
+    Boulder, CO, USA: UCAR/NCAR - Computational and Informational System Lab. doi:\<DOI\>.**
 
 In the above citation text, update the year, GeoCAT-viz version, and DOI as appropriate. For
 example:
 
-**Visualization & Analysis Systems Technologies. (2022).
-Geoscience Community Analysis Toolkit: GeoCAT-viz (v2022.05.0) [Software].
-Boulder, CO, USA: UCAR/NCAR - Computational and Informational System Lab. doi:10.5281/zenodo.6678351.**
-
-Please find DOIs for all the GeoCAT-viz versions `here
-<https://zenodo.org/search?page=1&size=20&q=conceptrecid:%226678345%22&sort=-version&all_versions=True>`_.
+    **Visualization & Analysis Systems Technologies. (2022).
+    Geoscience Community Analysis Toolkit: GeoCAT-viz (v2022.05.0) [Software].
+    Boulder, CO, USA: UCAR/NCAR - Computational and Informational System Lab. doi:10.5281/zenodo.6678351.**
 
 Please note: The DOI minting service, Zenodo, might be suggesting their own citation text (as
 they are the publisher of such DOIs) in their website. We prefer the text we recommend here to be used;
 however, either way is acceptable.
 
 For further information, please refer to
 `GeoCAT homepage - Citation <https://geocat.ucar.edu/pages/citation.html>`_.
```

### Comparing `geocat.viz-2023.3.0.post0/docs/installation.rst` & `geocat.viz-2023.5.0/docs/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,114 +1,118 @@
+.. currentmodule:: geocat.viz
+
+.. _installation:
+
 Installation
 ============
 
 This installation guide includes only the GeoCAT-viz installation and build instructions.
-Please refer to `GeoCAT Contributor's Guide <https://geocat.ucar.edu/pages/contributing.html>`_ for installation of
+Please refer to `GeoCAT Contributor's Guide <https://geocat.ucar.edu/pages/contributing.html>`__ for installation of
 the whole GeoCAT project.
 
 Installing GeoCAT-viz via Conda in a New Environment
 -----------------------------------------------------
 
 The easiest way to install GeoCAT-viz is using
-`Conda <http://conda.pydata.org/docs/>`_::
+`Conda <http://conda.pydata.org/docs/>`__::
 
-    conda create -n geocat -c conda-forge -c ncar geocat-viz
+    conda create -n geocat -c conda-forge geocat-viz
 
-where :code:`geocat` is the name of a new conda environment, which can then be
+where ``geocat`` is the name of a new conda environment, which can then be
 activated using::
 
     conda activate geocat
 
 If you need to make use of other software packages, such as Jupyter
-with GeoCAT-viz, you may wish to install into your :code:`geocat`
-environment.  The following :code:`conda create` command can be used to create a new
-:code:`conda` environment that includes one of these additional commonly used Python
+with GeoCAT-viz, you may wish to install into your ``geocat``
+environment.  The following ``conda create`` command can be used to create a new
+``conda`` environment that includes one of these additional commonly used Python
 packages pre-installed::
 
-    conda create -n geocat -c conda-forge -c ncar geocat-viz jupyter
+    conda create -n geocat -c conda-forge geocat-viz jupyter
 
 Alternatively, if you already created a conda environment using the first
 command (without the extra packages), you can activate and install the packages
 in an existing environment with the following commands::
 
     conda activate geocat # or whatever your environment is called
     conda install -c conda-forge jupyter
 
 Also, note that the Conda package manager automatically installs all required dependencies,
 meaning it is not necessary to explicitly install NumPy, Matplotlib, Cartopy, Xarray, Scikit-learn,
 etc. when creating an environment.
 
 If you are interested in learning more about how Conda environments work, please
-visit the `managing environments <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_
+visit the `managing environments <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`__
 page of the Conda documentation.
 
 Installing GeoCAT-viz in a Pre-existing Conda Environment
 ----------------------------------------------------------
 
 If you started a project and later decided to use GeoCAT-viz, you will need to install it in your pre-existing environment.
 
 1. Make sure your conda is up to date by running this command from the terminal::
 
         conda update conda
 
-2. Activate the conda environment you want to add GeoCAT to. In this example, the environment is called :code:`geocat`::
+2. Activate the conda environment you want to add GeoCAT to. In this example, the environment is called ``geocat``::
 
         conda activate geocat
 
 3. Install geocat-viz::
 
         conda install -c ncar -c conda-forge geocat-viz
 
 Updating GeoCAT-viz via Conda
 -------------------------------
 
-It is important to keep your version of :code:`geocat-viz` up to date. This can be done as follows:
+It is important to keep your version of ``geocat-viz`` up to date. This can be done as follows:
 
 1. Make sure your Conda is up to date by running this command from the terminal::
 
         conda update conda
 
-2. Activate the conda environment you want to update. In this example, the environment is called :code:`geocat`::
+2. Activate the conda environment you want to update. In this example, the environment is called ``geocat``::
 
         conda activate geocat
 
-3. Update :code:`geocat-viz`::
+3. Update ``geocat-viz``::
 
         conda update geocat-viz
 
 
 Installing GeoCAT-viz via PyPi
 -------------------------------
 GeoCAT-viz is distributed also in PyPI; therefore, the above Conda installation instructions should, in theory,
-apply to PyPI installation through using :code:`pip install` commands instead of :code:`conda install` wherever they occur.
+apply to PyPI installation through using ``pip install`` commands instead of ``conda install`` wherever they occur.
 
 Building GeoCAT-viz from source
 --------------------------------
 
 Building GeoCAT-viz from source code is a fairly straightforward task, but
 doing so should not be necessary for most users. If you `are` interested in
 building GeoCAT-viz from source, you will need the following packages to be
 installed.
 
 Required dependencies for building and testing GeoCAT-viz
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     - Python 3.8+
-    - `numpy <https://numpy.org/doc/stable/>`_
-    - `xarray <http://xarray.pydata.org/en/stable/>`_
-    - `matplotlib <https://matplotlib.org/stable/index.html>`_
-    - `cartopy <https://scitools.org.uk/cartopy/docs/latest/>`_
+    - `numpy <https://numpy.org/doc/stable/>`__
+    - `xarray <http://xarray.pydata.org/en/stable/>`__
+    - `matplotlib <https://matplotlib.org/stable/index.html>`__
+    - `cartopy <https://scitools.org.uk/cartopy/docs/latest/>`__
 
 
 How to create a Conda environment for building GeoCAT-viz
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The GeoCAT-viz source code includes a conda environment definition file in
 the root directory that can be used to create a development environment containing
-all of the packages required to build GeoCAT-viz. The file :code:`conda_environment.yml`
+all of the packages required to build GeoCAT-viz. The file ``build_envs/environment.yml``
 is intended to be used on Linux systems and macOS.
 The following commands should work on both Linux and macOS::
 
     conda env create -f conda_environment.yml
     conda activate geocat_viz_build
```

### Comparing `geocat.viz-2023.3.0.post0/docs/make.bat` & `geocat.viz-2023.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.3.0.post0/src/geocat/viz/taylor.py` & `geocat.viz-2023.5.0/src/geocat/viz/taylor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Taylor Diagrams."""
 
+import typing
+
 import numpy as np
-import matplotlib.pyplot as plt
+
+import xarray as xr
+
 import matplotlib
-import typing
-import numpy
-import xarray
+import matplotlib.pyplot as plt
+from matplotlib.projections import PolarAxes
+import mpl_toolkits.axisartist.floating_axes as fa
+import mpl_toolkits.axisartist.grid_finder as gf
 
 
 class TaylorDiagram(object):
     """Taylor Diagram.
 
     Taylor diagrams provide a visual framework for comparing a suite of variables from one or more test data sets to
     one or more reference data sets. Commonly, the test data sets are model experiments while the reference data set
@@ -17,30 +22,30 @@
     derived from climatological monthly, seasonal or annual means. Because the different variables (eg:
     precipitation, temperature) may have widely varying numerical values, the results are normalized by the reference
     variables. The ratio of the normalized variances indicates the relative amplitude of the model and observed
     variations.
 
     Parameters
     ----------
-    refstd: :class:`float`
+    refstd : float
         Optional reference standard deviation
 
-    fig: :class:`matplotlib.figure.Figure`
+    fig : :class:`matplotlib.figure.Figure`
         Optional input figure. Default is None
 
-    rect: :class:`int`
+    rect : int
         Optional subplot definition
 
-    label: :class:`string`
+    label : str
         Optional reference label string indentifier
 
-    stdRange: :class:`tuple`
+    stdRange : tuple
         Optional stddev axis extent
 
-    stdLevel: :class:`list`
+    stdLevel : list
         Optional list of tick locations for stddev axis
 
     References
     ----------
     - https://validate-climate-model-validation.readthedocs.io/en/latest/_modules/validate/taylor.html
     - https://matplotlib.org/stable/gallery/axisartist/demo_floating_axes.html#sphx-glr-gallery-axisartist-demo-floating-axes-py
     - https://www.ncl.ucar.edu/Applications/taylor.shtml
@@ -53,37 +58,33 @@
                  label: str = 'REF',
                  std_range: tuple = (0, 1.65),
                  std_level: list = np.arange(0, 1.51, 0.25)):
         """Create base Taylor Diagram.
 
         Parameters
         ----------
-        refstd: :class:`float`
+        refstd : float
             Optional reference standard deviation
 
-        fig: :class:`matplotlib.figure.Figure`
+        fig : :class:`matplotlib.figure.Figure`
             Optional input figure. Default is None
 
-        rect: :class:`int`
+        rect : int
             Optional subplot definition
 
-        label: :class:`string`
+        label : str
             Optional reference label string indentifier
 
-        std_range: :class:tuple
+        std_range : tuple
             Optional stddev axis extent
 
-        std_level: :class:list
+        std_level : list
             Optional list of tick locations for stddev axis
         """
 
-        from matplotlib.projections import PolarAxes
-        import mpl_toolkits.axisartist.floating_axes as fa
-        import mpl_toolkits.axisartist.grid_finder as gf
-
         # Pull and set optional constructor variables
         # Set figure
         self.fig = fig
         if fig is None:
             self.fig = plt.figure(figsize=(8, 8))
 
         # Reference standard deviation
@@ -176,18 +177,18 @@
         # Collect sample points for latter use (e.g. legend)
         self.modelMarkerSet = []
 
         # Set number for models outside axes
         self.modelOutside = -1
 
     def add_model_set(self,
-                      stddev: typing.Union[xarray.DataArray, numpy.ndarray,
-                                           list, float],
-                      corrcoef: typing.Union[xarray.DataArray, numpy.ndarray,
-                                             list, float],
+                      stddev: typing.Union[xr.DataArray, np.ndarray, list,
+                                           float],
+                      corrcoef: typing.Union[xr.DataArray, np.ndarray, list,
+                                             float],
                       fontsize: float = 14,
                       xytext: tuple = (-5, 7),
                       annotate_on: bool = True,
                       model_outlier_on: bool = False,
                       percent_bias_on: bool = False,
                       bias_array: bool = None,
                       *args,
@@ -196,55 +197,61 @@
         style model markers and labels are achieved through Matplotlib markers
         and annotations. *xytext* argument can be used to adjust the
         positioning of the label relative to the markers if *annotate_on*
         argument is set to True.
 
         Parameters
         ----------
-        stddev: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, or :class:`float`
+        stddev : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, float
             An array of vertical coordinates of the data points that denote the standard deviation
 
-        corrcoef: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, or :class:`float`
+        corrcoef : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, float
             An array of horizontal coordinates of the data points that denote correlation
             Input should have the same size as *stddev*
 
-        fontsize: :class:`float`
+        fontsize : float
             Fonsize of marker labels. This argument is suplied to `matplotlib.axes.Axes.annotate` command. Optional. Default value 14.
 
-        xytext: :class:`tuple` (:class:`float`, :class:`float`)
+        xytext : tuple(float, float)
             The position (x, y) to place the marker label at. The coordinate system is set to pixels.
             This argument is supplied to `matplotlib.axes.Axes.annotate` command. Optional. Default set to (-5,7)
 
-        annotate_on: :class:`bool`
+        annotate_on : bool
             Determine whether model labels are added. Optional. Default to True.
 
-        model_outlier_on: :class:bool
+        model_outlier_on : bool
             If True, models with negative correlations and standard deviations > TaylorDiagram.smax(default to 1.65)
             are plotted as text at the bottom of the figure; if False, all models are plotted
             according to *stddev* and *corrcoef* Default to False. Optional.
 
-        percent_bias_on: :class:bool
+        percent_bias_on : bool
             If True, model marker and marker size is plotted based on *bias_array* Default to False. Optional.
 
-        bias_array: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, or :class:`float`
+        bias_array : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, float
             If this is given, it is used to determine individual marker size and marker style internally.
             Input should have the same size as *stddev* and *corrcoef* Default to None.
 
         Notes
         -----
         args and kwargs are directly propagated to the `matplotlib.axes.Axes.plot` command.
 
 
         Returns
         -------
-        modelTexts: array of :class:`matplotlib.text.Annotation`
+        modelTexts : array of :class:`matplotlib.text.Annotation`
             A list of text objects representing model labels
 
-        modelset: array of :class:`matplotlib.collections.PathCollection`
+        modelset : array of :class:`matplotlib.collections.PathCollection`
             A list of sets of markers representing sets of models
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_2.html?highlight=add_model_set>`_
         """
 
         # Convert to np arrays and make copies
         np_std = np.array(stddev)
         np_corr = np.array(corrcoef)
         std_plot = np_std
         corr_plot = np_corr
@@ -367,86 +374,97 @@
                                  r'$\frac{%.2f}{%.2f}$' % (std, corr),
                                  fontsize=17,
                                  transform=self.ax.transAxes)
 
         return modelTexts, modelset
 
     def add_xgrid(self,
-                  arr: typing.Union[xarray.DataArray, numpy.ndarray, list,
-                                    float],
+                  arr: typing.Union[xr.DataArray, np.ndarray, list, float],
                   color: str = 'lightgray',
                   linestyle=(0, (9, 5)),
                   linewidth: float = 0.5,
                   **kwargs):
         """Add gridlines to the X axis (correlation) specified by array *arr*
 
         Parameters
         ----------
-        arr: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, :class:`float`
+        arr : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, float
             An array of horizontal coordinates of the data points that denote correlation
 
-        color: :class:`str`
+        color : str
             Color of the gridline. Optional. Default to "lightgray"
 
         linestyle : {'-', '--', '-.', ':', '', (offset, on-off-seq), ...}
             See matplotlib Linestyle examples. Optional. Default to (0, (9,5))
 
-        linewidth: :class:`float`
+        linewidth : float
             Set the line width in points. Optional. Default to 0.5
 
         Notes
         -----
         kwargs are directly propagated to the `matplotlib.axes.Axes.vlines` command.
 
         Returns
         -------
         None
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_2.html?highlight=add_xgrid>`_
         """
 
         for value in arr:
             self.ax.vlines([np.arccos(value)],
                            ymin=self.smin,
                            ymax=self.smax,
                            color=color,
                            linestyle=linestyle,
                            linewidth=linewidth,
                            **kwargs)
 
     def add_ygrid(self,
-                  arr: typing.Union[xarray.DataArray, numpy.ndarray, list,
-                                    float],
+                  arr: typing.Union[xr.DataArray, np.ndarray, list, float],
                   color: str = 'lightgray',
                   linestyle=(0, (9, 5)),
                   linewidth: int = 1,
                   **kwargs):
         """Add gridlines (radii) to the Y axis (standard deviation) specified
         by array *arr*
 
         Parameters
         ----------
-        arr: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, :class:`float`
+        arr : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, float
             An array of vertical coordinates of the data points that denote standard deviation
 
-        color: :class:`str`
+        color : str
             Color of the gridline. Optional. Default to "lightgray"
 
-        linestyle: {'-', '--', '-.', ':', '', (offset, on-off-seq), ...}
+        linestyle : {'-', '--', '-.', ':', '', (offset, on-off-seq), ...}
             See matplotlib Linestyle examples. Optional. Default to (0, (9,5))
 
-        linewidth: :class:`float`
+        linewidth : float
             Set the line width in points. Optional. Default to 1
 
         Notes
         -----
         *kwargs* are directly propagated to the `matplotlib.axes.Axes.plot` command.
 
         Returns
         -------
         None
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+         - `NCL_taylor_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_2.html?highlight=add_ygrid>`_
         """
+
         t = np.linspace(0, np.pi / 2)
         for value in arr:
             r = np.zeros_like(t) + value
             h, = self.ax.plot(t,
                               r,
                               color=color,
                               linestyle=linestyle,
@@ -459,31 +477,38 @@
         Notes
         -----
         *args* and *kwargs* are propagated to `matplotlib.axes.Axes.grid`
         """
         self._ax.grid(*args, **kwargs)
 
     def add_contours(self,
-                     levels: typing.Union[xarray.DataArray, numpy.ndarray, list,
+                     levels: typing.Union[xr.DataArray, np.ndarray, list,
                                           int] = 5,
                      **kwargs):
         """Add constant centered RMS difference contours.
 
         Parameters
         ----------
-        levels: :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`, :class:`int`
+        levels : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list, int
             Determines the number and positions of the contour lines. Optional. Default to 5
 
         Notes
         -----
         *args* and *kwargs* are propagated to `matplotlib.axes.Axes.contour`
 
         Returns
         -------
-        :class:`matplotlib.contour.QuadContourSet`
+        contours : :class:`matplotlib.contour.QuadContourSet`
+            Matplotlib Contour Object
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+         - `NCL_taylor_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_2.html?highlight=add_contours>`_
         """
         # Return coordinate matrices from coordinate vectors
         rs, ts = np.meshgrid(np.linspace(self.smin, self.smax),
                              np.linspace(0, np.pi / 2))
 
         # Compute centered RMS difference
         rms = np.sqrt(self.refstd**2 + rs**2 -
@@ -491,64 +516,79 @@
 
         # Create contour lines
         contours = self.ax.contour(ts, rs, rms, levels, **kwargs)
 
         return contours
 
     def add_model_name(self,
-                       namearr: typing.Union[xarray.DataArray, numpy.ndarray,
-                                             list],
+                       namearr: typing.Union[xr.DataArray, np.ndarray, list],
                        x_loc: float = 0.1,
                        y_loc: float = 0.31,
                        verticalalignment: str = 'top',
                        fontsize: float = 13,
                        **kwargs):
         """Add texts of model names.
 
         The coordinate system of the Axes(transAxes) is used for more intuitive positioning of the texts.
         (x_loc=0, y_loc=0) is bottom left of the axes, and (x_loc=1, y_loc=1) is top right of the axes.
 
         Parameters
         ----------
-        namearr : :class:`xarray.DataArray`, :class:`numpy.ndarray`, :class:`list`
+        namearr : :class:`xarray.DataArray`, :class:`numpy.ndarray`, list
             List of model names
 
-        x_loc: :class:`float`
+        x_loc : float
             x component of text position. Optional. Default to 0.1
 
-        y_loc: :class:`float`
+        y_loc : float
             y component of text position. Optional. Default to 0.31
 
-        verticalalignment: :class:`str`
+        verticalalignment : str
             Vertical alignment. Options: {'center', 'top', 'bottom', 'baseline', 'center_baseline'}. Optional. Default to 'top'
 
-        fontsize: :class:`float`
+        fontsize : float
             Text fontsize. Optional. Default to 13
 
         Notes
         -----
         *kwargs* are directly propagated to the `matplotlib.axes.Axes.text` command
 
         Return
         ------
         None
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_3.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_3.html?highlight=add_model_name>`_
+
+        - `NCL_taylor_6.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_6.html?highlight=add_model_name>`_
         """
+
         text = [str(i + 1) + ' - ' + namearr[i] for i in range(len(namearr))]
         text = '\n'.join(text)
 
         self.ax.text(x_loc,
                      y_loc,
                      text,
                      verticalalignment=verticalalignment,
                      fontsize=fontsize,
                      transform=self.ax.transAxes,
                      **kwargs)
 
     def add_bias_legend(self):
-        """Add bias legend to the upper left hand corner."""
+        """Add bias legend to the upper left hand corner.
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_8.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_8.html?highlight=add_bias_legend>`_
+        """
         text = "-  /  +     Bias\n"
         percent = [">20%", "10-20%", "5-10%", "1-5%", "<1%"]
 
         self.ax.text(0.07,
                      0.92,
                      text,
                      fontsize=11,
@@ -596,35 +636,41 @@
         """Add a figure legend.
 
         The coordinate system is Axes(transAxes).
         (x_loc=0, y_loc=0) is bottom left of the axes, and (x_loc=1, y_loc=1) is top right of the axes.
 
         Parameters
         ----------
-        xloc: :class:`float`
+        xloc : float
             x location of legend position, supplied to bbox_to_anchor(). Optional. Default to 1.1
 
-        yloc: :class:`float`
+        yloc : float
             y location of legend position, upplied to bbox_to_anchor(). Optional. Default to 0.95
 
-        loc: :class:`str`
+        loc : str
             See Matplotlib legend documentations. Optional. Default to 'upper right'
 
-        fontsize: :class:`float`
+        fontsize : float
             Text fontsize. Optional. Default to 14
 
         Notes
         -----
         *kwargs* are directly propagated to the `matplotlib.axes.Axes.legend` command
         *kwargs* are directly propagated to the `matplotlib.pyplot.legend` command.
 
         Return
         ------
         legend : :class:`matplotlib.legend.Legend`
             Matplotlib legend object
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_3.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_3.html?highlight=add_legend>`_
         """
 
         if kwargs.get('handles') is None:
             handles = self.modelMarkerSet[::-1]
         if kwargs.get('labels') is None:
             labels = [p.get_label() for p in handles]
 
@@ -641,54 +687,66 @@
                   fontsize: float = 18,
                   y_loc: float = None,
                   **kwargs):
         """Add a main title.
 
         Parameters
         ----------
-        maintitle: :class:`str`
+        maintitle : str
             Title text
 
-        fontsize: :class:`float`
+        fontsize : float
             Text fontsize. Optional. Defaults to 18
 
-        y_loc: :class:`float`
+        y_loc : float
             Vertical Axes location. 1.0 is the top. Optional. Default to None
 
         Notes
         -----
         *kwargs* are directly propagated to the `matplotlib.axes.Axes.set_title` command.
 
         Return
         ------
         None
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_6.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_6.html?highlight=add_title>`_
         """
 
         self._ax.set_title(maintitle, fontsize=fontsize, y=y_loc, **kwargs)
 
     def set_fontsizes_and_pad(self,
                               ticklabel_fontsize: float = 14,
                               axislabel_fontsize: float = 16,
                               axislabel_pad: float = 8):
         """Reset ticklabel and axis label fontsizes, and axis label padding.
 
         Parameters
         ----------
-        ticklabel_fontsize: :class:`float`
+        ticklabel_fontsize : float
             Fontsize of all tick labels. Optional. Default to 14
 
-        axislabel_fontsize: :class:`float`
+        axislabel_fontsize : float
             Fontsize of axis labels. Optional. Default to 16
 
-        axislabel_pad: :class:`float`
+        axislabel_pad : float
             Padding between axis labels and axis. Optional. Default to 8
 
         Return
         ------
         None
+
+        Examples
+        --------
+        All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+        - `NCL_taylor_6.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_6.html?highlight=set_fontsize_and_pad>`_
         """
 
         self._ax.axis['top', 'right',
                       'left'].major_ticklabels.set_fontsize(ticklabel_fontsize)
         self._ax.axis['top', 'right'].label.set_fontsize(axislabel_fontsize)
         self._ax.axis['top', 'right'].label.set_pad(axislabel_pad)
```

### Comparing `geocat.viz-2023.3.0.post0/src/geocat/viz/util.py` & `geocat.viz-2023.5.0/src/geocat/viz/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,77 @@
-import cartopy.mpl.geoaxes
-from itertools import chain
+import warnings
+
+import numpy as np
+import typing
+
+import xarray as xr
+
+from pint import Quantity
+
+from sklearn.cluster import DBSCAN
+
+import matplotlib as mpl
 import matplotlib.axes
+import matplotlib.path as mpath
+import matplotlib.pyplot as plt
+import matplotlib.ticker as tic
+import matplotlib.cm as cm
+
+import cartopy.crs as ccrs
+import cartopy.util as cutil
+import cartopy.mpl.geoaxes
+from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
+
 import metpy.calc as mpcalc
-from pint import Quantity
 from metpy.units import units
-import numpy as np
-import typing
-import xarray
+
+from itertools import chain
 
 
 def set_tick_direction_spine_visibility(ax,
                                         tick_direction='out',
                                         top_spine_visible=True,
                                         bottom_spine_visible=True,
                                         left_spine_visible=True,
                                         right_spine_visible=True):
     """Utility function to turn off axes spines and set tickmark orientations.
 
     Note: This function should be called after calling add_major_minor_ticks()
 
-    Args:
+    Parameters
+    ----------
+    ax : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        Current axes to the current figure
 
-        ax (:class:`matplotlib.axes._subplots.AxesSubplot` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`):
-            Current axes to the current figure
+    tick_direction : str
+        Tick direction. Accepted alias:
 
-        tick_direction (:class:`str`):
-            Set 'in' to put ticks inside the axes,
-            'out' to put ticks outside the axes,
-            'inout' to put ticks both in and out of the axes.
+        - `in`: to put ticks inside the axes
+        - `out`: to put ticks outside the axes
+        - `inout`: to put ticks both in and out of the axes
 
-        top_spine_visible (:class:`bool`):
-            Set False to turn off top spine of the axes.
+    top_spine_visible : bool
+        Set False to turn off top spine of the axes.
 
-        bottom_spine_visible (:class:`bool`):
-            Set False to turn off bottom spine of the axes.
+    bottom_spine_visible : bool
+        Set False to turn off bottom spine of the axes.
 
-        left_spine_visible (:class:`bool`):
-            Set False to turn off left spine of the axes.
+    left_spine_visible : bool
+        Set False to turn off left spine of the axes.
 
-        right_spine_visible (:class:`bool`):
-            Set False to turn off right spine.
+    right_spine_visible : bool
+        Set False to turn off right spine.
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_box_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Boxplots/NCL_box_2.html?highlight=set_tick_direction_spine_visibility>`_
     """
+
     ax.tick_params(direction=tick_direction, axis='both', which='both')
     ax.spines['top'].set_visible(top_spine_visible)
     ax.spines['bottom'].set_visible(bottom_spine_visible)
     ax.spines['left'].set_visible(left_spine_visible)
     ax.spines['right'].set_visible(right_spine_visible)
 
     if top_spine_visible and bottom_spine_visible:
@@ -72,50 +99,58 @@
                           xlocator=np.arange(-180, 180, 15),
                           ylocator=np.arange(-90, 90, 15),
                           labelsize=12,
                           **kwargs):
     """Utility function that adds latitude and longtitude gridlines to the
     plot.
 
-    Args:
+    Parameters
+    ----------
+    ax : :class:`cartopy.mpl.geoaxes.GeoAxes`
+        Current axes to the current figure.
 
-        ax (:class:`cartopy.mpl.geoaxes.GeoAxes`):
-            Current axes to the current figure.
+    projection : :class:`cartopy.crs.CRS`
+        Defines a Cartopy Coordinate Reference System. If not given,
+        defaults to ccrs.PlateCarree()
 
-        projection (:class:`cartopy.crs.CRS`):
-            Defines a Cartopy Coordinate Reference System. If not given,
-            defaults to ccrs.PlateCarree()
+    draw_labels : bool
+        Toggle whether to draw labels, default to True.
 
-        draw_labels (:class:`bool`):
-            Toggle whether to draw labels, default to True.
+    xlocator, ylocator : :class:`numpy.ndarray`, list
+        Arrays of fixed locations of the gridlines in the x and y coordinate of the given CRS.
+        Default to np.arange(-180, 180, 15) and np.arange(-90, 90, 15).
 
-        xlocator, ylocator (:class:`numpy.ndarray` or list):
-            Arrays of fixed locations of the gridlines in the x and y coordinate of the given CRS.
-            Default to np.arange(-180, 180, 15) and np.arange(-90, 90, 15).
+    labelsize : float
+        Fontsizes of label fontsizes of x and y coordinates.
 
-        labelsize (:class:`float`):
-            Fontsizes of label fontsizes of x and y coordinates.
+    *kwargs* control line properties and are passed through to `matplotlib.collections.Collection`.
 
-        *kwargs* control line properties and are passed through to `matplotlib.collections.Collection`.
+    Returns
+    -------
+    gl : :class:`cartopy.mpl.gridliner.Gridliner`
+        A Cartopy GridLiner object.
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
-    Return:
+    - `NCL_native_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_native_1.html?highlight=add_lat_lon_gridlines>`_
 
-        gl (:class:`cartopy.mpl.gridliner.Gridliner`):
+    - `NCL_native_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_native_2.html?highlight=add_lat_lon_gridlines>`_
     """
-    import matplotlib.ticker as mticker
 
     # Draw gridlines
     gl = ax.gridlines(crs=projection,
                       draw_labels=draw_labels,
                       x_inline=False,
                       y_inline=False,
                       **kwargs)
 
-    gl.xlocator = mticker.FixedLocator(xlocator)
-    gl.ylocator = mticker.FixedLocator(ylocator)
+    gl.xlocator = tic.FixedLocator(xlocator)
+    gl.ylocator = tic.FixedLocator(ylocator)
     gl.xlabel_style = {"rotation": 0, "size": labelsize}
     gl.ylabel_style = {"rotation": 0, "size": labelsize}
 
     return gl
 
 
 def add_right_hand_axis(ax,
@@ -126,48 +161,51 @@
                         labelpad=10,
                         axislabelsize=16,
                         y_minor_per_major=None):
     """Utility function that adds a right hand axis to the plot.
 
     Parameters
     ----------
+    ax : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        Current axes to the current figure
 
-        ax (:class:`matplotlib.axes._subplots.AxesSubplot` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`):
-            Current axes to the current figure
-
-        label (:class:`str`):
-            Text to use for the right hand side label.
+    label : str
+        Text to use for the right hand side label.
 
-        ylim (:class:`tuple`):
-            Should be given as a tuple of numeric values (left, right), where left and right are the left and right
-            y-axis limits in data coordinates. Passing None for any of them leaves the limit unchanged. See Matplotlib
-            documentation for further information.
+    ylim : tuple
+        Should be given as a tuple of numeric values (left, right), where left and right are the left and right
+        y-axis limits in data coordinates. Passing None for any of them leaves the limit unchanged. See Matplotlib
+        documentation for further information.
 
-        yticks (:class:`list`):
-            List of y-axis tick locations. See Matplotlib documentation for further information.
+    yticks : list
+        List of y-axis tick locations. See Matplotlib documentation for further information.
 
-        ticklabelsize (:class:`int`):
-            Text font size of tick labels. A default value of 12 is used if nothing is set.
+    ticklabelsize : int
+        Text font size of tick labels. A default value of 12 is used if nothing is set.
 
-        labelpad (:class:`float`):
-            Spacing in points from the axes bounding box. A default value of 10 is used if nothing is set.
+    labelpad : float
+        Spacing in points from the axes bounding box. A default value of 10 is used if nothing is set.
 
-        axislabelsize (:class:`int`):
-            Text font size for y-axes. A default value of 16 is used if nothing is set.
+    axislabelsize : int
+        Text font size for y-axes. A default value of 16 is used if nothing is set.
 
-        y_minor_per_major (:class:`int`):
+    y_minor_per_major : int
             Number of minor ticks between adjacent major ticks on y-axis.
 
-        Returns
-        -------
+    Returns
+    -------
+    axRHS : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        The created right-hand axis
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
-        axRHS (:class:`matplotlib.axes._subplots.AxesSubplot` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`):
-            The created right-hand axis
+    - `NCL_coneff_8.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_coneff_8.html?highlight=add_right_hand_axis>`_
     """
-    import matplotlib.ticker as tic
 
     axRHS = ax.twinx()
     if label is not None:
         axRHS.set_ylabel(ylabel=label,
                          labelpad=labelpad,
                          fontsize=axislabelsize)
     set_axes_limits_and_ticks(axRHS, ylim=ylim, yticks=yticks)
@@ -175,43 +213,141 @@
     if y_minor_per_major is not None:
         axRHS.yaxis.set_minor_locator(tic.AutoMinorLocator(n=y_minor_per_major))
         axRHS.tick_params(length=4, width=0.4, which="minor")
 
     return axRHS
 
 
+def add_height_from_pressure_axis(ax,
+                                  heights=None,
+                                  pressure_units='hPa',
+                                  ticklabelsize=12,
+                                  label='Height (km)',
+                                  labelpad=10,
+                                  axislabelsize=16):
+    """Utility function that adds a right-hand Height axis to the plot, derived
+    from the left-hand Pressure axis. Replicates the height-axis functionality
+    in NCL's `gsn_csm_pres_hgt`method for drawing a pressure/height plot.
+
+    Parameters
+    ----------
+    ax : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        Current axes to the current figure
+
+    heights: :class:`numpy.ndarray`, list
+        Optional array of desired height values in km.
+
+    pressure_units :str
+        Optional Pint-compliant unit string associated with the Pressure values.
+        Assume to be `hPa`.
+
+    ticklabelsize : int
+        Optional text font size of tick labels. A default value of 12 is used if
+        nothing is set.
+
+    label : str
+        Optional text to use for the right hand side label.
+
+    labelpad : float
+        Optional spacing in points from the axes bounding box. A default value of
+        10 is used if nothing is set.
+
+    axislabelsize : int
+        Optional text font size for y-axes. A default value of 16 is used if
+        nothing is set.
+
+    Returns
+    -------
+    axRHS : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        The created right-hand axis
+
+    See ALso
+    --------
+    Related NCL Functions:
+        `gsn_csm_pres_hgt <https://www.ncl.ucar.edu/Document/Graphics/Interfaces/gsn_csm_pres_hgt.shtml>`_,
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_conOncon_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_1.html?highlight=add_height_from_pressure_axis>`_
+
+    - `NCL_h_lat_6.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_h_lat_6.html?highlight=add_height_from_pressure_axis>`_
+
+    - `NCL_h_lat_7.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_h_lat_7.html?highlight=add_height_from_pressure_axis>`_
+
+     - `NCL_h_vector_5.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Vectors/NCL_vector_5.html?highlight=add_height_from_pressure_axis>`_
+    """
+
+    # Create the right hand axis, inheriting from the left
+    axRHS = ax.twinx()
+
+    # If height array isn't given, infer it from pressure axis
+    if heights is None:
+        height_min, height_max = mpcalc.pressure_to_height_std(
+            ax.get_ylim() * units(pressure_units)).magnitude
+
+        # Range and step values mirror NCL's `set_pres_hgt_axes` logic
+        height_range = abs(height_max - height_min)
+        if (height_range < 35):
+            if (height_range < 70):
+                step = 7
+            else:
+                step = 4
+        else:
+            step = 10
+
+        # Select heights to display as tick labels
+        heights = np.arange(int(height_min), int(height_max) + 1, step)
+
+    # Send selected height values back to pressure to get tick locations
+    pressures = mpcalc.height_to_pressure_std(heights * units('km')).magnitude
+
+    # Display logrithmically to match right-hand pressure axis
+    axRHS.set_yscale('log')
+    axRHS.minorticks_off()  # Turn off minor ticks that are spaced by pressure
+
+    set_axes_limits_and_ticks(axRHS,
+                              ylim=ax.get_ylim(),
+                              yticks=pressures,
+                              yticklabels=heights)
+    axRHS.tick_params(labelsize=ticklabelsize)  # manually set tick label size
+    axRHS.set_ylabel(ylabel=label, labelpad=labelpad, fontsize=axislabelsize)
+
+    return axRHS
+
+
 def add_lat_lon_ticklabels(ax: typing.Union[matplotlib.axes.Axes,
                                             cartopy.mpl.geoaxes.GeoAxesSubplot],
                            zero_direction_label: bool = False,
                            dateline_direction_label: bool = False):
     """Utility function to make plots look like NCL plots by adding latitude,
     longitude tick labels.
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
-            Current axes to the current figure
+    ax : :class:`matplotlib.axes.Axes`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+        Current axes to the current figure
 
-    zero_direction_label: :class:`bool`
+    zero_direction_label : bool
         Set True to get 0 E / O W or False to get 0 only.
 
-    dateline_direction_label: :class:`bool`
+    dateline_direction_label : bool
         Set True to get 180 E / 180 W or False to get 180 only.
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
-    - `NCL_ce_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_1.html?highlight=add_lat_lon>`_
+    - `NCL_ce_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_1.html?highlight=add_lat_lon_ticklabels>`_
 
-    - `NCL_ce_3_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_3_2.html?highlight=add_lat_lon>`_
+    - `NCL_ce_3_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_3_2.html?highlight=add_lat_lon_ticklabels>`_
 
-    - `NCL_conOncon_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_2.html?highlight=add_lat_lon>`_
+    - `NCL_conOncon_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_2.html?highlight=add_lat_lon_ticklabels>`_
     """
-    from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
 
     lon_formatter = LongitudeFormatter(
         zero_direction_label=zero_direction_label,
         dateline_direction_label=dateline_direction_label)
     lat_formatter = LatitudeFormatter()
     ax.xaxis.set_major_formatter(lon_formatter)
     ax.yaxis.set_major_formatter(lat_formatter)
@@ -227,39 +363,39 @@
                           linthreshx: int = 2,
                           linthreshy: int = 2):
     """Utility function to make plots look like NCL plots by adding minor and
     major tick lines.
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+    ax : :class:`matplotlib.axes.Axes`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
         Current axes to the current figure
 
-    x_minor_per_major: :class:`int`
+    x_minor_per_major : int
         Number of minor ticks between adjacent major ticks on x-axis
 
-    y_minor_per_major: :class:`int`
+    y_minor_per_major : int
         Number of minor ticks between adjacent major ticks on y-axis
 
-    basex: :class:`int`
+    basex : int
         If the xaxis scale is logarithmic, this is the base for the logarithm. Default is base 10.
 
-    basey: :class:`int`
+    basey : int
         If the yaxis scale is logarithmic, this is the base for the logarithm. Default is base 10.
 
-    labelsize: :class:`str` or :class:`int`
+    labelsize : str, int
         Optional text size passed to tick_params. A default value of "small" is used if nothing is set.
 
-    linthreshx: :class:`int`
+    linthreshx : int
         An argument passed to SymmetricalLogLocator if the xaxis scale is
         `symlog`. Defines the range (-x, x), within which the plot is
         linear. This avoids having the plot go to infinity around zero.
         Defaults to 2.
 
-    linthreshy: :class:`int`
+    linthreshy : int
         An argument passed to SymmetricalLogLocator if the yaxis scale is
         `symlog`. Defines the range (-x, x), within which the plot is
         linear. This avoids having the plot go to infinity around zero.
         Defaults to 2.
 
     Examples
     --------
@@ -267,15 +403,14 @@
 
     - `NCL_bar_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Bar/NCL_bar_2.html?highlight=add_major_minor_ticks>`_
 
     - `NCL_box_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Boxplots/NCL_box_2.html?highlight=add_major_minor_ticks>`_
 
     - `NCL_scatter_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Scatter/NCL_scatter_1.html?highlight=add_major_minor_ticks>`_
     """
-    import matplotlib.ticker as tic
 
     ax.tick_params(labelsize=labelsize)
     ax.minorticks_on()
     if ax.xaxis.get_scale() == 'log':
         ax.xaxis.set_minor_locator(
             tic.LogLocator(base=basex,
                            subs=np.linspace(0, basex, x_minor_per_major + 1)))
@@ -339,44 +474,44 @@
     labels as they appear in NCL plots.
 
     The intent of this function is to help make the plot look like an NCL plot as well as to help developers use only
     this convenience function instead of multiple matplotlib.axes.Axes functions, when applicable.
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+    ax : :class:`matplotlib.axes.Axes`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
         Current axes to the current figure
 
-    maintitle: :class:`str`
+    maintitle : str
         Text to use for the maintitle.
 
-    maintitlefontsize: :class:`int`
+    maintitlefontsize : int
         Text font size for maintitle. A default value of 18 is used if nothing is set.
 
-    lefttitle: :class:`str`
+    lefttitle : str
         Text to use for an optional left-aligned title, if any. For most plots, only a maintitle is enough,
         but for some plot types, a lefttitle likely with a right-aligned title, righttitle, can be used together.
 
-    lefttitlefontsize: :class:`int`
+    lefttitlefontsize : int
         Text font size for lefttitle. A default value of 18 is used if nothing is set.
 
-    righttitle: :class:`str`
+    righttitle : str
         Text to use for an optional right-aligned title, if any. For most plots, only a maintitle is enough,
         but for some plot types, a righttitle likely with a left-aligned title, lefttitle, can be used together.
 
-    righttitlefontsize: :class:`int`
+    righttitlefontsize : int
         Text font size for righttitle. A default value of 18 is used if nothing is set.
 
-    xlabel: :class:`str`
+    xlabel : str
         Text for the x-axis label.
 
-    ylabel: :class:`str`
+    ylabel : str
         Text for the y-axis label.
 
-    labelfontsize: :class:`int`
+    labelfontsize : int
         Text font size for x- and y-axes. A default value of 16 is used if nothing is set.
 
     Notes
     -----
     If no lefttitle and righttitle is set, maintitle is placed just top to the axes as follows:
 
     >>>                  maintitle
@@ -441,37 +576,37 @@
     """Utility function to determine axis limits, tick values and labels.
 
     The intent of this function is to help developers use only this convenience function instead of multiple
     matplotlib.axes.Axes functions, when applicable.
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes` or :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
+    ax : :class:`matplotlib.axes.Axes`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
         Current axes to the current figure
 
-    xlim: :class:`tuple`
+    xlim : tuple
         Should be given as a tuple of numeric values (left, right), where left and right are the left and right
         x-axis limits in data coordinates. Passing None for any of them leaves the limit unchanged. See Matplotlib
         documentation for further information.
 
-    ylim: :class:`tuple`
+    ylim : tuple
         Should be given as a tuple of numeric values (left, right), where left and right are the left and right
         y-axis limits in data coordinates. Passing None for any of them leaves the limit unchanged. See Matplotlib
         documentation for further information.
 
-    xticks: :class:`list`
+    xticks : list
         List of x-axis tick locations. See Matplotlib documentation for further information.
 
-    yticks: :class:`list`
+    yticks : list
         List of y-axis tick locations. See Matplotlib documentation for further information.
 
-    xticklabels: :class:`list`
+    xticklabels : list
         List of string labels for x-axis ticks. See Matplotlib documentation for further information.
 
-    yticklabels: :class:`list`
+    yticklabels : list
         List of string labels for y-axis ticks. See Matplotlib documentation for further information.
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the
     `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
@@ -509,84 +644,79 @@
     """Utility function that truncates a colormap. Registers the new colormap
     by name in plt.cm, and also returns the updated map.
 
     `Copied from Stack Overflow <https://stackoverflow.com/questions/18926031/how-to-extract-a-subset-of-a-colormap-as-a-new-colormap-in-matplotlib>`_
 
     Parameters
     ----------
-    cmap: :class:`matplotlib.colors.Colormap`
+    cmap : :class:`matplotlib.colors.Colormap`
         Colormap to be truncated.
 
-    minval: :class:`int` or :class:`float`
+    minval : int, float
         Minimum value to be used for truncation of the color map.
 
-    maxval: :class:`int` or :class:`float`
+    maxval : int, float
         Maximum value to be used for truncation of the color map.
 
-    n: :class:`int`
+    n : int
         Number of color values in the new color map.
 
-    name: :class:`str`
+    name : str
         Optional name of the new color map. If not set, a new name is generated by using the name of the input
         colormap as well as min and max values.
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the
     `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_dev_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Panels/NCL_dev_2.html?highlight=truncate_colormap>`_
 
     - `NCL_vector_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Vectors/NCL_vector_1.html?highlight=truncate_colormap>`_
 
     - `NCL_mask_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Masking/NCL_mask_1.html?highlight=truncate_colormap>`_
     """
-    import matplotlib as mpl
-    from matplotlib import cm
 
     if not name:
         name = "trunc({n},{a:.2f},{b:.2f})".format(n=cmap.name,
                                                    a=minval,
                                                    b=maxval)
     new_cmap = mpl.colors.LinearSegmentedColormap.from_list(
         name=name,
         colors=cmap(np.linspace(minval, maxval, n)),
     )
     cm.register_cmap(name, new_cmap)
     return new_cmap
 
 
-def xr_add_cyclic_longitudes(da: xarray.DataArray, coord: str):
+def xr_add_cyclic_longitudes(da: xr.DataArray, coord: str):
     """Utility function to handle the no-shown-data artifact of 0 and
     360-degree longitudes.
 
     Parameters
     ----------
-    da: :class:`xarray.DataArray`
+    da : :class:`xarray.DataArray`
         Data array that contains one or more coordinates, strictly including the coordinate with the name
         given with the "coord" parameter.
 
-    coord: :class:`str`
+    coord : str
         Name of the longitude coordinate within "da" data array.
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the
     `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_lb_3.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_lb_3.html?highlight=xr_add_cyclic_longitudes>`_
 
     - `NCL_proj_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_proj_2.html?highlight=xr_add_cyclic_longitudes>`_
 
     - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=xr_add_cyclic_longitudes>`_
     """
 
-    import xarray as xr
-    import cartopy.util as cutil
-
     cyclic_data, cyclic_coord = cutil.add_cyclic_point(da.values,
                                                        coord=da[coord])
 
     coords = da.coords.to_dataset()
     coords[coord] = cyclic_coord
 
     new_da = xr.DataArray(cyclic_data,
@@ -611,47 +741,47 @@
     is drawn in the projection coordinates and therefore follows any curves
     created by the projection. As of now, this only works consistently for the
     Lambert Conformal Projection and North/South Polar Stereographic
     Projections.
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes`
+    ax : :class:`matplotlib.axes.Axes`
         The axes to which the boundary will be applied.
 
-    lon_range: :class:`tuple` or :class:`list`
+    lon_range : tuple, list
         The two-tuple containing the start and end of the desired range of
         longitudes. The first entry must be smaller than the second entry,
         except when the region crosses the antimeridian. Both entries must
         be between [-180 , 180]. If lon_range is from -180 to 180, then a
         full circle centered on the pole with a radius from the pole to the
         lowest latitude given by lat_range will be set as the boundary.
 
-    lat_range: :class:`tuple` or :class:`list`
+    lat_range : tuple, list
         The two-tuple containing the start and end of the desired range of
         latitudes. The first entry must be smaller than the second entry.
         Both entries must be between [-90 , 90].
 
-    north_pad: :class:`int`
+    north_pad : int
         A constant to be added to the second entry in lat_range. Use this
         if the northern edge of the plot is cut off. Defaults to 0.
 
-    south_pad: :class:`int`
+    south_pad : int
         A constant to be subtracted from the first entry in lat_range. Use
         this if the southern edge of the plot is cut off. Defaults to 0.
 
-    east_pad: :class:`int`
+    east_pad : int
         A constant to be added to the second entry in lon_range. Use this
         if the eastern edge of the plot is cut off. Defaults to 0.
 
-    west_pad: :class:`int`
+    west_pad : int
         A constant to be subtracted from the first entry in lon_range. Use
         this if the western edge of the plot is cut off. Defaults to 0.
 
-    res: :class:`int`
+    res : int
         The size of the incrementation for vertices in degrees. Default is
         a vertex every one degree of longitude. A higher number results in
         a lower resolution boundary.
 
     Notes
     -----
     Due to the behavior of Cartopy's set_extent() function, the curved
@@ -669,16 +799,14 @@
 
     - `NCL_conOncon_5.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_5.html?highlight=set_map_boundary>`_
 
     - `NCL_panel_9.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Panels/NCL_panel_9.html?highlight=set_map_boundary>`_
 
     - `NCL_polar_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_polar_1.html?highlight=set_map_boundary>`_
     """
-    import cartopy.crs as ccrs
-    import matplotlib.path as mpath
 
     if lon_range[0] >= lon_range[1]:
         if not (lon_range[0] > 0 > lon_range[1]):
             raise ValueError(
                 "The first longitude value must be strictly less than the second longitude value unless the region crosses over the antimeridian"
             )
 
@@ -724,65 +852,62 @@
     ax.set_extent([
         lon_range[0] - west_pad, lon_range[1] + east_pad,
         lat_range[0] - south_pad, lat_range[1] + north_pad
     ],
                   crs=ccrs.PlateCarree())
 
 
-def findLocalExtrema(da: xarray.DataArray,
+def findLocalExtrema(da: xr.DataArray,
                      highVal: int = 0,
                      lowVal: int = 1000,
                      eType: str = 'Low',
                      eps: float = 10) -> list:
     """Utility function to find local low/high field variable coordinates on a
     contour map. To classify as a local high, the data point must be greater
     than highval, and to classify as a local low, the data point must be less
     than lowVal.
 
     Parameters
     ----------
-    da: :class:`xarray.DataArray`
+    da : :class:`xarray.DataArray`
         Xarray data array containing the lat, lon, and field variable (ex. pressure) data values
 
-    highVal: :class:`int`
+    highVal : int
         Data value that the local high must be greater than to qualify as a "local high" location.
         Default highVal is 0.
 
-    lowVal: :class:`int`
+    lowVal : int
         Data value that the local low must be less than to qualify as a "local low" location.
         Default lowVal is 1000.
 
-    eType: :class:`str`
+    eType : str
         'Low' or 'High'
         Determines which extrema are being found- minimum or maximum, respectively.
         Default eType is 'Low'.
 
-    eps: :class:`float`
+    eps : float
             Parameter supplied to sklearn.cluster.DBSCAN determining the maximum distance between two samples
             for one to be considered as in the neighborhood of the other.
             Default eps is 10.
 
     Returns
     -------
-    clusterExtremas: :class:`list`
+    clusterExtremas : list
         List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
         that specify local low/high locations
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=findlocalextrema>`_
 
     - `NCL_sat_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_2.html?highlight=findlocalextrema>`_
     """
 
-    from sklearn.cluster import DBSCAN
-    import warnings
-
     # Create a 2D array of coordinates in the same shape as the field variable data
     # so each coordinate is easily mappable to a data value
     # ex:
     # (1, 1), (2, 1), (3, 1)
     # (1, 2)................
     # (1, 3)................
     lons, lats = np.meshgrid(np.array(da.lon), np.array(da.lat))
@@ -863,53 +988,52 @@
 
     This allows the user to specify the exact locations of the labels, rather than having matplotlib
     plot them automatically.
 
 
     Parameters
     ----------
-    ax: :class:`matplotlib.axes.Axes`
+    ax : :class:`matplotlib.axes.Axes`
         Axis containing the contour set.
 
-    contours: :class:`matplotlib.contour.QuadContourSet`
+    contours : :class:`matplotlib.contour.QuadContourSet`
         Contour set that is being labeled.
 
-    transform: :class:`cartopy.crs.CRS`
+    transform : :class:`cartopy.crs.CRS`
         Instance of CRS that represents the source coordinate system of coordinates.
         (ex. ccrs.Geodetic()).
 
-    proj: :class:`cartopy.crs.CRS`
+    proj : :class:`cartopy.crs.CRS`
         Projection 'ax' is defined by.
         This is the instance of CRS that the coordinates will be transformed to.
 
-    clabel_locations: :class:`list`
+    clabel_locations : list
         List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
         that specify where the contours with regular field variable values should be plotted.
 
-    fontsize: :class:`int`
+    fontsize : int
         Font size of contour labels.
 
-    whitebbox: :class:`bool`
+    whitebbox : bool
         Setting this to "True" will cause all labels to be plotted with white backgrounds
 
-    horizontal: :class:`bool`
+    horizontal : bool
         Setting this to "True" will cause the contour labels to be horizontal.
 
     Returns
     -------
-    cLabels: :class:`list`
+    cLabels : list
         List of text instances of all contour labels
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
-    - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=plotclabels>`_
+    - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=plotCLabels>`_
     """
-    import numpy as np
 
     # Initialize empty array that will be filled with contour label text objects and returned
     cLabels = []
 
     # Plot any regular contour levels
     if clabel_locations != []:
         clevelpoints = proj.transform_points(
@@ -932,15 +1056,15 @@
             txt.set_bbox(dict(facecolor='white', edgecolor='none', pad=2))
             for txt in cLabels
         ]
 
     return cLabels
 
 
-def plotELabels(da: xarray.DataArray,
+def plotELabels(da: xr.DataArray,
                 transform: cartopy.crs.CRS,
                 proj: cartopy.crs.CRS,
                 clabel_locations: list = [],
                 label: str = 'L',
                 fontsize: int = 22,
                 whitebbox: bool = False,
                 horizontal: bool = True) -> list:
@@ -948,58 +1072,56 @@
 
     High/Low contour labels will be plotted using text boxes for more accurate label values
     and placement.
     This function is exemplified in the python version of https://www.ncl.ucar.edu/Applications/Images/sat_1_lg.png
 
     Parameters
     ----------
-    da: :class:`xarray.DataArray`
+    da : :class:`xarray.DataArray`
         Xarray data array containing the lat, lon, and field variable data values.
 
-    transform: :class:`cartopy.crs.CRS`
+    transform : :class:`cartopy.crs.CRS`
         Instance of CRS that represents the source coordinate system of coordinates.
         (ex. ccrs.Geodetic()).
 
-    proj: :class:`cartopy.crs.CRS`
+    proj : :class:`cartopy.crs.CRS`
         Projection 'ax' is defined by.
         This is the instance of CRS that the coordinates will be transformed to.
 
-    clabel_locations: :class:`list`
+    clabel_locations : list
         List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
         that specify where the contour labels should be plotted.
 
-    label: :class:`str`
+    label : str
         ex. 'L' or 'H'
         The data value will be plotted as a subscript of this label.
 
-    fontsize: :class:`int`
+    fontsize : int
         Font size of regular contour labels.
 
-    horizontal: :class:`bool`
+    horizontal : bool
         Setting this to "True" will cause the contour labels to be horizontal.
 
-    whitebbox: :class:`bool`
+    whitebbox : bool
         Setting this to "True" will cause all labels to be plotted with white backgrounds
 
     Returns
     -------
-    extremaLabels: :class:`list`
+    extremaLabels : list
         List of text instances of all contour labels
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=plotELabels>`_
 
     - `NCL_sat_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_2.html?highlight=plotELabels>`_
     """
 
-    import matplotlib.pyplot as plt
-
     # Create array of coordinates in the same shape as field variable data
     # so each coordinate can be easily mapped to its data value.
     # ex:
     # (1, 1), (2, 1), (3, 1)
     # (1, 2)................
     # (1, 3)................
     lons, lats = np.meshgrid(np.array(da.lon), np.array(da.lat))
@@ -1045,29 +1167,29 @@
             txt.set_bbox(dict(facecolor='white', edgecolor='none', pad=2))
             for txt in extremaLabels
         ]
 
     return extremaLabels
 
 
-def set_vector_density(data: xarray.DataArray,
-                       minDistance: int = 0) -> xarray.DataArray:
+def set_vector_density(data: xr.DataArray,
+                       minDistance: int = 0) -> xr.DataArray:
     """Utility function to change density of vector plots.
 
     Parameters
     ----------
-    data: :class:`xarray.DataArray`
+    data : :class:`xarray.DataArray`
         Data array that contains the vector plot latitude/longitude data.
 
-    minDistance: :class:`int`
+    minDistance : int
         Value in degrees that determines the distance between the vectors.
 
     Returns
     -------
-    ds: :class:`xarray.DataArray`
+    ds : :class:`xarray.DataArray`
         Sliced version of the input data array.
 
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_vector_3.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Vectors/NCL_vector_3.html?highlight=set_vector_density>`_
@@ -1130,28 +1252,36 @@
         Pressure level input from dataset
     tc : :class:`pint.Quantity`
         Temperature for parcel from dataset
     tdc : :class:`pint.Quantity`
         Dew point temperature for parcel from dataset
     pro : :class:`pint.Quantity`
         Parcel profile temperature converted to degC
+
     Returns
     -------
-    joined : :class:`str`
+    joined : str
         A string element with the format "Plcl=<value> Tlcl[C]=<value> Shox=<value> Pwat[cm]=<value> Cape[J]=<value>" where:
         - Cape  -  Convective Available Potential Energy [J]
         - Pwat  -  Precipitable Water [cm]
         - Shox  -  Showalter Index (stability)
         - Plcl  -  Pressure of the lifting condensation level [hPa]
         - Tlcl  -  Temperature at the lifting condensation level [C]
+
     See Also
     --------
     Related NCL Functions:
-    `skewT_PlotData <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_PlotData.shtml>`_,
-    `skewt_BackGround <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_BackGround.shtml>`_
+        `skewT_PlotData <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_PlotData.shtml>`_,
+        `skewt_BackGround <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_BackGround.shtml>`_
+
+     Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_skewt_2_2 <https://geocat-examples.readthedocs.io/en/latest/gallery/Skew-T/NCL_skewt_2_2.html?highlight=get_skewt_vars>`_
     """
 
     # CAPE
     cape = mpcalc.cape_cin(p, tc, tdc, pro)
     cape = cape[0].magnitude
 
     # Precipitable Water
```

