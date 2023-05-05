# Comparing `tmp/flox-0.6.9.tar.gz` & `tmp/flox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flox-0.6.9.tar", last modified: Wed Mar 22 15:48:49 2023, max compression
+gzip compressed data, was "flox-0.7.0.tar", last modified: Fri May  5 12:51:53 2023, max compression
```

## Comparing `flox-0.6.9.tar` & `flox-0.7.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.956099 flox-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-22 15:48:16.000000 flox-0.6.9/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-22 15:48:16.000000 flox-0.6.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-22 15:48:16.000000 flox-0.6.9/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-22 15:48:16.000000 flox-0.6.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-22 15:48:16.000000 flox-0.6.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-03-22 15:48:16.000000 flox-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-03-22 15:48:49.956099 flox-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-22 15:48:16.000000 flox-0.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/benchmarks/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-22 15:48:16.000000 flox-0.6.9/asv_bench/benchmarks/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-22 15:48:16.000000 flox-0.6.9/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-22 15:48:16.000000 flox-0.6.9/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-22 15:48:16.000000 flox-0.6.9/ci/minimal-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-22 15:48:16.000000 flox-0.6.9/ci/no-dask.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-22 15:48:16.000000 flox-0.6.9/ci/no-xarray.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-22 15:48:16.000000 flox-0.6.9/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-22 15:48:16.000000 flox-0.6.9/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.948099 flox-0.6.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-03-22 15:48:16.000000 flox-0.6.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.952099 flox-0.6.9/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/blockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/cohorts-month-chunk4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/cohorts-month-chunk5.png
--rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/map-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-blockwise-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-blockwise.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-cohorts-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-cohorts.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-map-reduce-reindex-False.svg
--rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-map-reduce-reindex-True.svg
--rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/new-split-apply-combine-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/split-apply-combine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-03-22 15:48:16.000000 flox-0.6.9/docs/diagrams/split-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-03-22 15:48:16.000000 flox-0.6.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-22 15:48:16.000000 flox-0.6.9/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.952099 flox-0.6.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.952099 flox-0.6.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/aggregations.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/arrays.md
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/engines.md
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/implementation.md
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.952099 flox-0.6.9/docs/source/user-stories/
--rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories/climatology-hourly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories/climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories/custom-aggregations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories/hourly-climatology.html
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories/overlaps.md
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/user-stories.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-22 15:48:16.000000 flox-0.6.9/docs/source/xarray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.956099 flox-0.6.9/flox/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-22 15:48:16.000000 flox-0.6.9/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 15:48:49.000000 flox-0.6.9/flox/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-03-22 15:48:16.000000 flox-0.6.9/flox/aggregate_flox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-22 15:48:16.000000 flox-0.6.9/flox/aggregate_npg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-03-22 15:48:16.000000 flox-0.6.9/flox/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-22 15:48:16.000000 flox-0.6.9/flox/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    71911 2023-03-22 15:48:16.000000 flox-0.6.9/flox/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:16.000000 flox-0.6.9/flox/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-22 15:48:16.000000 flox-0.6.9/flox/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23358 2023-03-22 15:48:16.000000 flox-0.6.9/flox/xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-03-22 15:48:16.000000 flox-0.6.9/flox/xrdtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-22 15:48:16.000000 flox-0.6.9/flox/xrutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.956099 flox-0.6.9/flox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-03-22 15:48:49.000000 flox-0.6.9/flox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-22 15:48:49.000000 flox-0.6.9/flox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:48:49.000000 flox-0.6.9/flox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-22 15:48:49.000000 flox-0.6.9/flox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-22 15:48:49.000000 flox-0.6.9/flox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-22 15:48:16.000000 flox-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-22 15:48:16.000000 flox-0.6.9/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 15:48:49.956099 flox-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 15:48:16.000000 flox-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:48:49.956099 flox-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-22 15:48:16.000000 flox-0.6.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 15:48:16.000000 flox-0.6.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    45705 2023-03-22 15:48:16.000000 flox-0.6.9/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20701 2023-03-22 15:48:16.000000 flox-0.6.9/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 12:51:21.000000 flox-0.7.0/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 12:51:21.000000 flox-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-05 12:51:21.000000 flox-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 12:51:21.000000 flox-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-05 12:51:21.000000 flox-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-05 12:51:53.769970 flox-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-05 12:51:21.000000 flox-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 12:51:21.000000 flox-0.7.0/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 12:51:21.000000 flox-0.7.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 12:51:21.000000 flox-0.7.0/ci/minimal-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 12:51:21.000000 flox-0.7.0/ci/no-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 12:51:21.000000 flox-0.7.0/ci/no-xarray.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 12:51:21.000000 flox-0.7.0/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 12:51:21.000000 flox-0.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-05 12:51:21.000000 flox-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/blockwise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/cohorts-month-chunk4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/cohorts-month-chunk5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/map-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-blockwise-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-blockwise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-cohorts-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-cohorts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-split-apply-combine-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/split-apply-combine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/split-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-05 12:51:21.000000 flox-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 12:51:21.000000 flox-0.7.0/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/aggregations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/arrays.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/engines.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/user-stories/
+-rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/climatology-hourly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/custom-aggregations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/hourly-climatology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/overlaps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/xarray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/flox/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 12:51:21.000000 flox-0.7.0/flox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:51:53.000000 flox-0.7.0/flox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregate_flox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregate_npg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 12:51:21.000000 flox-0.7.0/flox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72841 2023-05-05 12:51:21.000000 flox-0.7.0/flox/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:21.000000 flox-0.7.0/flox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-05 12:51:21.000000 flox-0.7.0/flox/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xrdtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xrutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/flox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-05 12:51:21.000000 flox-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 12:51:21.000000 flox-0.7.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:51:53.769970 flox-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 12:51:21.000000 flox-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-05 12:51:21.000000 flox-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 12:51:21.000000 flox-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46313 2023-05-05 12:51:21.000000 flox-0.7.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-05 12:51:21.000000 flox-0.7.0/tests/test_xarray.py
```

### Comparing `flox-0.6.9/.github/workflows/benchmarks.yml` & `flox-0.7.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/.github/workflows/ci-additional.yaml` & `flox-0.7.0/.github/workflows/ci-additional.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         run: |
           conda info -a
           conda list
       - name: Run doctests
         run: |
           python -m pytest --doctest-modules flox --ignore flox/tests --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -122,14 +122,14 @@
           python -m pip install mypy
 
       - name: Run mypy
         run: |
           python -m mypy --install-types --non-interactive --cobertura-xml-report mypy_report
 
       - name: Upload mypy coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: mypy_report/cobertura.xml
           flags: mypy
           env_vars: PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `flox-0.6.9/.github/workflows/ci.yaml` & `flox-0.7.0/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
       - name: Install flox
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -87,15 +87,15 @@
       - name: Install flox
         run: |
           python -m pip install --no-deps -e .
       - name: Run tests
         run: |
           python -m pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `flox-0.6.9/.github/workflows/pypi.yaml` & `flox-0.7.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/.github/workflows/testpypi-release.yaml` & `flox-0.7.0/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/.github/workflows/upstream-dev-ci.yaml` & `flox-0.7.0/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/.gitignore` & `flox-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/.pre-commit-config.yaml` & `flox-0.7.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 ci:
     autoupdate_schedule: quarterly
 
 repos:
     - repo: https://github.com/charliermarsh/ruff-pre-commit
       # Ruff version.
-      rev: 'v0.0.246'
+      rev: 'v0.0.260'
       hooks:
         - id: ruff
           args: ["--fix"]
 
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
         - id: check-yaml
         - id: trailing-whitespace
         - id: end-of-file-fixer
         - id: check-docstring-first
 
     - repo: https://github.com/psf/black
-      rev: 23.1.0
+      rev: 23.3.0
       hooks:
         - id: black
 
     - repo: https://github.com/executablebooks/mdformat
       rev: 0.7.16
       hooks:
       - id: mdformat
         additional_dependencies:
           - mdformat-black
           - mdformat-myst
 
     - repo: https://github.com/nbQA-dev/nbQA
-      rev: 1.6.1
+      rev: 1.7.0
       hooks:
           - id: nbqa-black
           - id: nbqa-ruff
             args: [--fix]
 
     - repo: https://github.com/kynan/nbstripout
       rev: 0.6.1
       hooks:
         - id: nbstripout
           args: [--extra-keys=metadata.kernelspec metadata.language_info.version]
 
     - repo: https://github.com/codespell-project/codespell
-      rev: v2.2.2
+      rev: v2.2.4
       hooks:
         - id: codespell
           additional_dependencies:
             - tomli
 
     - repo: https://github.com/abravalheri/validate-pyproject
-      rev: v0.12.1
+      rev: v0.12.2
       hooks:
         - id: validate-pyproject
```

### Comparing `flox-0.6.9/LICENSE` & `flox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/PKG-INFO` & `flox-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.6.9
+Version: 0.7.0
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.6.9/README.md` & `flox-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/asv.conf.json` & `flox-0.7.0/asv_bench/asv.conf.json`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/benchmarks/README_CI.md` & `flox-0.7.0/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/benchmarks/__init__.py` & `flox-0.7.0/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/benchmarks/cohorts.py` & `flox-0.7.0/asv_bench/benchmarks/cohorts.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/benchmarks/combine.py` & `flox-0.7.0/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/asv_bench/benchmarks/reduce.py` & `flox-0.7.0/asv_bench/benchmarks/reduce.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/Makefile` & `flox-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/blockwise.png` & `flox-0.7.0/docs/diagrams/blockwise.png`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/cohorts-month-chunk4.png` & `flox-0.7.0/docs/diagrams/cohorts-month-chunk4.png`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/cohorts-month-chunk5.png` & `flox-0.7.0/docs/diagrams/cohorts-month-chunk5.png`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/map-reduce.png` & `flox-0.7.0/docs/diagrams/map-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-blockwise-annotated.svg` & `flox-0.7.0/docs/diagrams/new-blockwise-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-blockwise.svg` & `flox-0.7.0/docs/diagrams/new-blockwise.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-cohorts-annotated.svg` & `flox-0.7.0/docs/diagrams/new-cohorts-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-cohorts.svg` & `flox-0.7.0/docs/diagrams/new-cohorts.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-map-reduce-reindex-False-annotated.svg` & `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-map-reduce-reindex-False.svg` & `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-map-reduce-reindex-True-annotated.svg` & `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-map-reduce-reindex-True.svg` & `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/new-split-apply-combine-annotated.svg` & `flox-0.7.0/docs/diagrams/new-split-apply-combine-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/split-apply-combine.svg` & `flox-0.7.0/docs/diagrams/split-apply-combine.svg`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/diagrams/split-reduce.png` & `flox-0.7.0/docs/diagrams/split-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/make.bat` & `flox-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/aggregations.md` & `flox-0.7.0/docs/source/aggregations.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/api.rst` & `flox-0.7.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/arrays.md` & `flox-0.7.0/docs/source/arrays.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/conf.py` & `flox-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/engines.md` & `flox-0.7.0/docs/source/engines.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/implementation.md` & `flox-0.7.0/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/index.md` & `flox-0.7.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/intro.md` & `flox-0.7.0/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/user-stories/climatology-hourly.ipynb` & `flox-0.7.0/docs/source/user-stories/climatology-hourly.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/user-stories/climatology.ipynb` & `flox-0.7.0/docs/source/user-stories/climatology.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/user-stories/custom-aggregations.ipynb` & `flox-0.7.0/docs/source/user-stories/custom-aggregations.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/user-stories/hourly-climatology.html` & `flox-0.7.0/docs/source/user-stories/hourly-climatology.html`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/user-stories/overlaps.md` & `flox-0.7.0/docs/source/user-stories/overlaps.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/docs/source/xarray.md` & `flox-0.7.0/docs/source/xarray.md`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox/aggregate_flox.py` & `flox-0.7.0/flox/aggregate_flox.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox/aggregate_npg.py` & `flox-0.7.0/flox/aggregate_npg.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox/aggregations.py` & `flox-0.7.0/flox/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,23 +553,28 @@
     else:
         agg.fill_value["numpy"] = (fv,)
 
     if finalize_kwargs is not None:
         assert isinstance(finalize_kwargs, dict)
         agg.finalize_kwargs = finalize_kwargs
 
+    if min_count is None:
+        min_count = 0
+
     # This is needed for the dask pathway.
     # Because we use intermediate fill_value since a group could be
     # absent in one block, but present in another block
     # We set it for numpy to get nansum, nanprod tests to pass
     # where the identity element is 0, 1
-    if min_count is not None:
+    if min_count > 0:
         agg.min_count = min_count
         agg.chunk += ("nanlen",)
         agg.numpy += ("nanlen",)
         agg.combine += ("sum",)
         agg.fill_value["intermediate"] += (0,)
         agg.fill_value["numpy"] += (0,)
         agg.dtype["intermediate"] += (np.intp,)
         agg.dtype["numpy"] += (np.intp,)
+    else:
+        agg.min_count = 0
 
     return agg
```

### Comparing `flox-0.6.9/flox/core.py` & `flox-0.7.0/flox/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
     else:
         return array.rechunk({axis: newchunks})
 
 
 def rechunk_for_blockwise(array: DaskArray, axis: T_Axis, labels: np.ndarray) -> DaskArray:
     """
     Rechunks array so that group boundaries line up with chunk boundaries, allowing
-    embarassingly parallel group reductions.
+    embarrassingly parallel group reductions.
 
     This only works when the groups are sequential
     (e.g. labels = ``[0,0,0,1,1,1,1,2,2]``).
     Such patterns occur when using ``.resample``.
 
     Parameters
     ----------
@@ -845,26 +845,26 @@
     1. Squeezing out dummy dimensions
     2. Calling agg.finalize with intermediate results
     3. Mask using counts and fill with user-provided fill_value.
     4. reindex to expected_groups
     """
     squeezed = _squeeze_results(results, axis)
 
-    if agg.min_count is not None:
+    if agg.min_count > 0:
         counts = squeezed["intermediates"][-1]
         squeezed["intermediates"] = squeezed["intermediates"][:-1]
 
     # finalize step
     finalized: FinalResultsDict = {}
     if agg.finalize is None:
         finalized[agg.name] = squeezed["intermediates"][0]
     else:
         finalized[agg.name] = agg.finalize(*squeezed["intermediates"], **agg.finalize_kwargs)
 
-    if agg.min_count is not None:
+    if agg.min_count > 0:
         count_mask = counts < agg.min_count
         if count_mask.any():
             # For one count_mask.any() prevents promoting bool to dtype(fill_value) unless
             # necessary
             if fill_value is None:
                 raise ValueError("Filling is required but fill_value is None.")
             # This allows us to match xarray's type promotion rules
@@ -1515,25 +1515,34 @@
     from dask.array.core import deepfirst
 
     # deepfirst should be not be needed here but sometimes we receive a list of dict?
     return deepfirst(result_dict)[key]
 
 
 def _validate_reindex(
-    reindex: bool | None, func, method: T_Method, expected_groups, any_by_dask: bool
+    reindex: bool | None,
+    func,
+    method: T_Method,
+    expected_groups,
+    any_by_dask: bool,
+    is_dask_array: bool,
 ) -> bool:
-    if reindex is True:
+    all_numpy = not is_dask_array and not any_by_dask
+    if reindex is True and not all_numpy:
         if _is_arg_reduction(func):
             raise NotImplementedError
         if method in ["blockwise", "cohorts"]:
             raise ValueError(
                 "reindex=True is not a valid choice for method='blockwise' or method='cohorts'."
             )
 
     if reindex is None:
+        if all_numpy:
+            return True
+
         if method == "blockwise" or _is_arg_reduction(func):
             reindex = False
 
         elif method == "cohorts":
             reindex = False
 
         elif method == "map-reduce":
@@ -1585,15 +1594,19 @@
 
 def _lazy_factorize_wrapper(*by: T_By, **kwargs) -> np.ndarray:
     group_idx, *rest = factorize_(by, **kwargs)
     return group_idx
 
 
 def _factorize_multiple(
-    by: T_Bys, expected_groups: T_ExpectIndexTuple, any_by_dask: bool, reindex: bool
+    by: T_Bys,
+    expected_groups: T_ExpectIndexTuple,
+    any_by_dask: bool,
+    reindex: bool,
+    sort: bool = True,
 ) -> tuple[tuple[np.ndarray], tuple[np.ndarray, ...], tuple[int, ...]]:
     if any_by_dask:
         import dask.array
 
         # unifying chunks will make sure all arrays in `by` are dask arrays
         # with compatible chunks, even if there was originally a numpy array
         inds = tuple(range(by[0].ndim))
@@ -1604,14 +1617,15 @@
             *by_,
             chunks=tuple(chunks.values()),
             meta=np.array((), dtype=np.int64),
             axes=(),  # always (), we offset later if necessary.
             expected_groups=expected_groups,
             fastpath=True,
             reindex=reindex,
+            sort=sort,
         )
 
         fg, gs = [], []
         for by_, expect in zip(by, expected_groups):
             if expect is None:
                 if is_duck_dask_array(by_):
                     raise ValueError(
@@ -1630,28 +1644,35 @@
     else:
         group_idx, found_groups, grp_shape, ngroups, size, props = factorize_(
             by,
             axes=(),  # always (), we offset later if necessary.
             expected_groups=expected_groups,
             fastpath=True,
             reindex=reindex,
+            sort=sort,
         )
 
     return (group_idx,), found_groups, grp_shape
 
 
 def _validate_expected_groups(nby: int, expected_groups: T_ExpectedGroupsOpt) -> T_ExpectTuple:
     if expected_groups is None:
         return (None,) * nby
 
     if nby == 1 and not isinstance(expected_groups, tuple):
-        if isinstance(expected_groups, pd.Index):
+        if isinstance(expected_groups, (pd.Index, np.ndarray)):
             return (expected_groups,)
         else:
-            return (np.asarray(expected_groups),)
+            array = np.asarray(expected_groups)
+            if np.issubdtype(array.dtype, np.integer):
+                # preserve default dtypes
+                # on pandas 1.5/2, on windows
+                # when a list is passed
+                array = array.astype(np.int64)
+            return (array,)
 
     if nby > 1 and not isinstance(expected_groups, tuple):  # TODO: test for list
         raise ValueError(
             "When grouping by multiple variables, expected_groups must be a tuple "
             "of either arrays or objects convertible to an array (like lists). "
             "For example `expected_groups=(np.array([1, 2, 3]), ['a', 'b', 'c'])`."
             f"Received a {type(expected_groups).__name__} instead. "
@@ -1792,15 +1813,17 @@
 
     if method in ["split-reduce", "cohorts"] and any_by_dask:
         raise ValueError(f"method={method!r} can only be used when grouping by numpy arrays.")
 
     if method == "split-reduce":
         method = "cohorts"
 
-    reindex = _validate_reindex(reindex, func, method, expected_groups, any_by_dask)
+    reindex = _validate_reindex(
+        reindex, func, method, expected_groups, any_by_dask, is_duck_dask_array(array)
+    )
 
     if not is_duck_array(array):
         array = np.asarray(array)
     is_bool_array = np.issubdtype(array.dtype, bool)
     array = array.astype(int) if is_bool_array else array
 
     if isinstance(isbin, Sequence):
@@ -1818,29 +1841,36 @@
                 f"`expected_groups` for array {idx} in `by` cannot be None since it is a dask.array."
             )
 
     # We convert to pd.Index since that lets us know if we are binning or not
     # (pd.IntervalIndex or not)
     expected_groups = _convert_expected_groups_to_index(expected_groups, isbins, sort)
 
-    is_binning = any([isinstance(e, pd.IntervalIndex) for e in expected_groups])
-
-    # TODO: could restrict this to dask-only
-    factorize_early = (nby > 1) or (
-        is_binning and method == "cohorts" and is_duck_dask_array(array)
+    # Don't factorize "early only when
+    # grouping by dask arrays, and not having expected_groups
+    factorize_early = not (
+        # can't do it if we are grouping by dask array but don't have expected_groups
+        any(is_dask and ex_ is None for is_dask, ex_ in zip(by_is_dask, expected_groups))
     )
     if factorize_early:
         bys, final_groups, grp_shape = _factorize_multiple(
-            bys, expected_groups, any_by_dask=any_by_dask, reindex=reindex
+            bys,
+            expected_groups,
+            any_by_dask=any_by_dask,
+            # This is the only way it makes sense I think.
+            # reindex controls what's actually allocated in chunk_reduce
+            # At this point, we care about an accurate conversion to codes.
+            reindex=True,
+            sort=sort,
         )
         expected_groups = (pd.RangeIndex(math.prod(grp_shape)),)
 
     assert len(bys) == 1
-    by_ = bys[0]
-    expected_groups = expected_groups[0]
+    (by_,) = bys
+    (expected_groups,) = expected_groups
 
     if axis is None:
         axis_ = tuple(array.ndim + np.arange(-by_.ndim, 0))
     else:
         # TODO: How come this function doesn't exist according to mypy?
         axis_ = np.core.numeric.normalize_axis_tuple(axis, array.ndim)  # type: ignore
     nax = len(axis_)
@@ -1883,15 +1913,20 @@
     #     The only way to do this consistently is mask out using min_count
     #     Consider np.sum([np.nan]) = np.nan, np.nansum([np.nan]) = 0
     if min_count is None:
         if nax < by_.ndim or fill_value is not None:
             min_count = 1
 
     # TODO: set in xarray?
-    if min_count is not None and func in ["nansum", "nanprod"] and fill_value is None:
+    if (
+        min_count is not None
+        and min_count > 0
+        and func in ["nansum", "nanprod"]
+        and fill_value is None
+    ):
         # nansum, nanprod have fill_value=0, 1
         # overwrite than when min_count is set
         fill_value = np.nan
 
     kwargs = dict(axis=axis_, fill_value=fill_value, engine=engine)
     agg = _initialize_aggregation(func, dtype, array.dtype, fill_value, min_count, finalize_kwargs)
```

### Comparing `flox-0.6.9/flox/visualize.py` & `flox-0.7.0/flox/visualize.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox/xarray.py` & `flox-0.7.0/flox/xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,16 +253,14 @@
         maybe_midx = ds._indexes.get(var, None)
         if isinstance(maybe_midx, PandasMultiIndex):
             idx_coord_names = set(maybe_midx.index.names + [maybe_midx.dim])
             idx_other_names = idx_coord_names - set(maybe_drop)
             more_drop.update(idx_other_names)
     maybe_drop.update(more_drop)
 
-    ds = ds.drop_vars([var for var in maybe_drop if var in ds.variables])
-
     if dim is Ellipsis:
         if nby > 1:
             raise NotImplementedError("Multiple by are not allowed when dim is Ellipsis.")
         name_ = by_da[0].name
         if name_ in ds.dims and not isbins[0]:
             dim_tuple = tuple(d for d in obj.dims if d != name_)
         else:
@@ -271,25 +269,31 @@
         dim_tuple = _atleast_1d(dim)
     else:
         dim_tuple = tuple(grouper_dims)
 
     # broadcast to make sure grouper dimensions are present in the array.
     exclude_dims = tuple(d for d in ds.dims if d not in grouper_dims and d not in dim_tuple)
 
+    if any(d not in grouper_dims and d not in obj.dims for d in dim_tuple):
+        raise ValueError(f"Cannot reduce over absent dimensions {dim}.")
+
     try:
         xr.align(ds, *by_da, join="exact", copy=False)
     except ValueError as e:
         raise ValueError(
             "Object being grouped must be exactly aligned with every array in `by`."
         ) from e
 
-    ds_broad = xr.broadcast(ds, *by_da, exclude=exclude_dims)[0]
-
-    if any(d not in grouper_dims and d not in obj.dims for d in dim_tuple):
-        raise ValueError(f"Cannot reduce over absent dimensions {dim}.")
+    needs_broadcast = any(
+        not set(grouper_dims).issubset(set(variable.dims)) for variable in ds.data_vars.values()
+    )
+    if needs_broadcast:
+        ds_broad = xr.broadcast(ds, *by_da, exclude=exclude_dims)[0]
+    else:
+        ds_broad = ds
 
     dims_not_in_groupers = tuple(d for d in dim_tuple if d not in grouper_dims)
     if dims_not_in_groupers == tuple(dim_tuple) and not any(isbins):
         # reducing along a dimension along which groups do not vary
         # This is really just a normal reduction.
         # This is not right when binning so we exclude.
         if isinstance(func, str):
@@ -301,14 +305,16 @@
         # TODO: skipna needs test
         result = getattr(ds_broad, dsfunc)(dim=dim_tuple, skipna=skipna)
         if isinstance(obj, xr.DataArray):
             return obj._from_temp_dataset(result)
         else:
             return result
 
+    ds = ds.drop_vars([var for var in maybe_drop if var in ds.variables])
+
     axis = tuple(range(-len(dim_tuple), 0))
 
     # Set expected_groups and convert to index since we need coords, sizes
     # for output xarray objects
     expected_groups = list(expected_groups)
     group_names: tuple[Any, ...] = ()
     group_sizes: dict[Any, int] = {}
@@ -428,15 +434,15 @@
             "dtype": dtype,
             "core_dims": input_core_dims,
         },
     )
 
     # restore non-dim coord variables without the core dimension
     # TODO: shouldn't apply_ufunc handle this?
-    for var in set(ds_broad.variables) - set(ds_broad._indexes) - set(ds_broad.dims):
+    for var in set(ds_broad._coord_names) - set(ds_broad._indexes) - set(ds_broad.dims):
         if all(d not in ds_broad[var].dims for d in dim_tuple):
             actual[var] = ds_broad[var]
 
     for name, expect, by_ in zip(group_names, expected_groups, by_da):
         # Can't remove this till xarray handles IntervalIndex
         if isinstance(expect, pd.IntervalIndex):
             expect = expect.to_numpy()
@@ -530,15 +536,15 @@
         debug=debug,
     )
 
 
 def rechunk_for_blockwise(obj: T_DataArray | T_Dataset, dim: str, labels: T_DataArray):
     """
     Rechunks array so that group boundaries line up with chunk boundaries, allowing
-    embarassingly parallel group reductions.
+    embarrassingly parallel group reductions.
 
     This only works when the groups are sequential
     (e.g. labels = ``[0,0,0,1,1,1,1,2,2]``).
     Such patterns occur when using ``.resample``.
 
     Parameters
     ----------
```

### Comparing `flox-0.6.9/flox/xrdtypes.py` & `flox-0.7.0/flox/xrdtypes.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox/xrutils.py` & `flox-0.7.0/flox/xrutils.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/flox.egg-info/PKG-INFO` & `flox-0.7.0/flox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.6.9
+Version: 0.7.0
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.6.9/flox.egg-info/SOURCES.txt` & `flox-0.7.0/flox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/pyproject.toml` & `flox-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/tests/__init__.py` & `flox-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.6.9/tests/test_core.py` & `flox-0.7.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 
     with pytest.raises(ValueError):
         groupby_reduce(da, labels, func="mean")
 
 
 @pytest.mark.parametrize("dtype", (float, int))
 @pytest.mark.parametrize("chunk", [False, True])
-@pytest.mark.parametrize("expected_groups", [None, [0, 1, 2], np.array([0, 1, 2])])
+# TODO: make this intp when python 3.8 is dropped
+@pytest.mark.parametrize("expected_groups", [None, [0, 1, 2], np.array([0, 1, 2], dtype=np.int64)])
 @pytest.mark.parametrize(
     "func, array, by, expected",
     [
         ("sum", np.ones((12,)), labels, [3, 4, 5]),  # form 1
         ("sum", np.ones((12,)), nan_labels, [1, 4, 2]),  # form 1
         ("sum", np.ones((2, 12)), labels, [[3, 4, 5], [3, 4, 5]]),  # form 3
         ("sum", np.ones((2, 12)), nan_labels, [[1, 4, 2], [1, 4, 2]]),  # form 3
@@ -144,15 +145,20 @@
         func=func,
         expected_groups=expected_groups,
         fill_value=123,
         engine=engine,
     )
     # we use pd.Index(expected_groups).to_numpy() which is always int64
     # for the values in this tests
-    g_dtype = by.dtype if expected_groups is None else np.int64
+    if expected_groups is None:
+        g_dtype = by.dtype
+    elif isinstance(expected_groups, np.ndarray):
+        g_dtype = expected_groups.dtype
+    else:
+        g_dtype = np.int64
 
     assert_equal(groups, np.array([0, 1, 2], g_dtype))
     assert_equal(expected_result, result)
 
 
 def gen_array_by(size, func):
     by = np.ones(size[-1])
@@ -649,15 +655,15 @@
 @pytest.mark.parametrize("method", ["cohorts", "map-reduce"])
 @pytest.mark.parametrize("chunk_labels", [False, True])
 @pytest.mark.parametrize("chunks", ((), (1,), (2,)))
 def test_groupby_bins(chunk_labels, kwargs, chunks, engine, method) -> None:
     array = [1, 1, 1, 1, 1, 1]
     labels = [0.2, 1.5, 1.9, 2, 3, 20]
 
-    if method in ["split-reduce", "cohorts"] and chunk_labels:
+    if method == "cohorts" and chunk_labels:
         pytest.xfail()
 
     if chunks:
         if not has_dask:
             pytest.skip()
         array = dask.array.from_array(array, chunks=chunks)
         if chunk_labels:
@@ -780,18 +786,16 @@
 
     array = dask.array.from_array(array, chunks=(4,))
     actual, _ = groupby_reduce(array, by, func=func, engine=engine)
     assert actual.dtype == expected
 
 
 @requires_dask
-@pytest.mark.parametrize("dtype", [np.int32, np.int64])
-@pytest.mark.parametrize(
-    "labels_dtype", [pytest.param(np.int32, marks=pytest.mark.xfail), np.int64]
-)
+@pytest.mark.parametrize("dtype", [np.float32, np.float64, np.int32, np.int64])
+@pytest.mark.parametrize("labels_dtype", [np.float32, np.float64, np.int32, np.int64])
 @pytest.mark.parametrize("method", ["map-reduce", "cohorts"])
 def test_cohorts_map_reduce_consistent_dtypes(method, dtype, labels_dtype):
     repeats = np.array([4, 4, 12, 2, 3, 4], dtype=np.int32)
     labels = np.repeat(np.arange(6, dtype=labels_dtype), repeats)
     array = dask.array.from_array(labels.astype(dtype), chunks=(4, 8, 4, 9, 4))
 
     actual, actual_groups = groupby_reduce(array, labels, func="count", method=method)
@@ -832,18 +836,15 @@
     kwargs = dict(func=func, engine=engine, method=method, axis=axis, fill_value=fill_value)
     actual, groups = groupby_reduce(array, by, **kwargs)
     expected, sorted_groups = groupby_reduce(array.compute(), by, **kwargs)
     assert_equal(groups, sorted_groups)
     assert_equal(actual, expected)
 
     actual, groups = groupby_reduce(array, by, sort=False, **kwargs)
-    if method == "map-reduce":
-        assert_equal(groups, np.array([1, 30, 2, 31, 3, 4, 40], dtype=np.int64))
-    else:
-        assert_equal(groups, np.array([1, 30, 2, 31, 3, 40, 4], dtype=np.int64))
+    assert_equal(groups, np.array([1, 30, 2, 31, 3, 4, 40], dtype=np.int64))
     reindexed = reindex_(actual, groups, pd.Index(sorted_groups))
     assert_equal(reindexed, expected)
 
 
 @pytest.mark.parametrize("func", ["sum", "count"])
 @pytest.mark.parametrize("fill_value, expected", ((0, np.integer), (np.nan, np.floating)))
 def test_dtype_promotion(func, fill_value, expected, engine):
@@ -1232,15 +1233,15 @@
     array = dask.array.from_array(np.arange(25).reshape((5, 5)), chunks=1)
     subset = subset_to_blocks(array, flatblocks)
     assert len(subset.dask.layers) == 2
     assert_equal(subset, array.compute()[expectidx])
 
 
 @pytest.mark.parametrize(
-    "expected, reindex, func, expected_groups, any_by_dask",
+    "dask_expected, reindex, func, expected_groups, any_by_dask",
     [
         # argmax only False
         [False, None, "argmax", None, False],
         # True when by is numpy but expected is None
         [True, None, "sum", None, False],
         # False when by is dask but expected is None
         [False, None, "sum", None, True],
@@ -1248,30 +1249,51 @@
         [True, None, "sum", [1, 2, 3], False],
         [True, None, "sum", ([1], [2]), False],
         [True, None, "sum", ([1], [2]), True],
         [True, None, "sum", ([1], None), False],
         [True, None, "sum", ([1], None), True],
     ],
 )
-def test_validate_reindex_map_reduce(expected, reindex, func, expected_groups, any_by_dask):
-    actual = _validate_reindex(reindex, func, "map-reduce", expected_groups, any_by_dask)
-    assert actual == expected
+def test_validate_reindex_map_reduce(
+    dask_expected, reindex, func, expected_groups, any_by_dask
+) -> None:
+    actual = _validate_reindex(
+        reindex, func, "map-reduce", expected_groups, any_by_dask, is_dask_array=True
+    )
+    assert actual is dask_expected
+
+    # always reindex with all numpy inputs
+    actual = _validate_reindex(
+        reindex, func, "map-reduce", expected_groups, any_by_dask=False, is_dask_array=False
+    )
+    assert actual
+
+    actual = _validate_reindex(
+        True, func, "map-reduce", expected_groups, any_by_dask=False, is_dask_array=False
+    )
+    assert actual
 
 
-def test_validate_reindex():
+def test_validate_reindex() -> None:
     for method in ["map-reduce", "cohorts"]:
         with pytest.raises(NotImplementedError):
-            _validate_reindex(True, "argmax", method, expected_groups=None, any_by_dask=False)
+            _validate_reindex(
+                True, "argmax", method, expected_groups=None, any_by_dask=False, is_dask_array=True
+            )
 
     for method in ["blockwise", "cohorts"]:
         with pytest.raises(ValueError):
-            _validate_reindex(True, "sum", method, expected_groups=None, any_by_dask=False)
+            _validate_reindex(
+                True, "sum", method, expected_groups=None, any_by_dask=False, is_dask_array=True
+            )
 
         for func in ["sum", "argmax"]:
-            actual = _validate_reindex(None, func, method, expected_groups=None, any_by_dask=False)
+            actual = _validate_reindex(
+                None, func, method, expected_groups=None, any_by_dask=False, is_dask_array=True
+            )
             assert actual is False
 
 
 @requires_dask
 def test_1d_blockwise_sort_optimization():
     # Make sure for resampling problems sorting isn't done.
     time = pd.Series(pd.date_range("2020-09-01", "2020-12-31 23:59", freq="3H"))
```

### Comparing `flox-0.6.9/tests/test_xarray.py` & `flox-0.7.0/tests/test_xarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,16 @@
     ds = xr.Dataset(
         {"foo": (("x", "y", "z"), np.ones((3, 4, 2)))},
         {"x": ["a", "b", "c"], "y": [1, 2, 3, 4]},
     )
     expected = ds.sum("z")
     stacked = ds.stack(space=["x", "y"])
     actual = xarray_reduce(stacked, "space", dim="z", func="sum", engine=engine)
+    expected_xarray = stacked.groupby("space").sum("z")
+    assert_equal(expected_xarray, actual)
     assert_equal(expected, actual.unstack("space"))
 
     actual = xarray_reduce(stacked.foo, "space", dim="z", func="sum", engine=engine)
     assert_equal(expected.foo, actual.unstack("space"))
 
     ds = xr.Dataset(
         dict(a=(("z",), np.ones(10))),
```

