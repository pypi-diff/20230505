# Comparing `tmp/linopy-0.1.4.tar.gz` & `tmp/linopy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linopy-0.1.4.tar", last modified: Mon Mar 20 09:09:15 2023, max compression
+gzip compressed data, was "linopy-0.1.5.tar", last modified: Fri May  5 08:45:58 2023, max compression
```

## Comparing `linopy-0.1.4.tar` & `linopy-0.1.5.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.056864 linopy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (116)       67 2023-03-20 09:09:04.000000 linopy-0.1.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.036863 linopy-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.036863 linopy-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1702 2023-03-20 09:09:04.000000 linopy-0.1.4/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      836 2023-03-20 09:09:04.000000 linopy-0.1.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (116)      399 2023-03-20 09:09:04.000000 linopy-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2023-03-20 09:09:04.000000 linopy-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      119 2023-03-20 09:09:04.000000 linopy-0.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      137 2023-03-20 09:09:04.000000 linopy-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)    35141 2023-03-20 09:09:04.000000 linopy-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3377 2023-03-20 09:09:15.056864 linopy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2681 2023-03-20 09:09:04.000000 linopy-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.040864 linopy-0.1.4/benchmark/
--rw-r--r--   0 runner    (1001) docker     (116)     2857 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     7509 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (116)    21144 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (116)   188981 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark-absolute.png
--rw-r--r--   0 runner    (1001) docker     (116)    20512 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (116)   179946 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark-overhead.png
--rw-r--r--   0 runner    (1001) docker     (116)    18784 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark_resource-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (116)   149975 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark_resource-absolute.png
--rw-r--r--   0 runner    (1001) docker     (116)    18038 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark_resource-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (116)   132957 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/benchmark_resource-overhead.png
--rw-r--r--   0 runner    (1001) docker     (116)      339 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     7011 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/environment.fixed.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      249 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.040864 linopy-0.1.4/benchmark/notebooks/
--rw-r--r--   0 runner    (1001) docker     (116)     3362 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/notebooks/plot-benchmarks.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.044864 linopy-0.1.4/benchmark/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1450 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1537 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1541 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_jump.jl
--rwxr-xr-x   0 runner    (1001) docker     (116)     1458 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2007 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1796 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2043 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmark_pyomo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.044864 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/
--rw-r--r--   0 runner    (1001) docker     (116)      451 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (116)      503 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (116)      477 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (116)      708 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      469 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/common.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1050 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/concat-benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.044864 linopy-0.1.4/benchmark/scripts/leftovers/
--rw-r--r--   0 runner    (1001) docker     (116)      698 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmark-linopy.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.048864 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.048864 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (116)      742 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      777 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      764 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      380 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (116)    18477 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (116)      451 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (116)   103087 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (116)      503 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (116)    26681 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
--rw-r--r--   0 runner    (1001) docker     (116)    18332 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
--rw-r--r--   0 runner    (1001) docker     (116)      477 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (116)   381819 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (116)      247 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (116)      708 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1471 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/leftovers/common.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1392 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/merge-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (116)      613 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      291 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      291 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      399 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      290 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      287 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      399 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/run-pyomo.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1023 2023-03-20 09:09:04.000000 linopy-0.1.4/benchmark/scripts/write-lp-file.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.048864 linopy-0.1.4/doc/
--rw-r--r--   0 runner    (1001) docker     (116)      634 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.048864 linopy-0.1.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     1393 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (116)     3647 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)    57997 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/benchmark.png
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4054 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2964 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       51 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/create-a-model.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/creating-constraints.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       55 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/creating-variables.nblink
--rw-r--r--   0 runner    (1001) docker     (116)     3380 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)    80342 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (116)   132092 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/logo.py
--rw-r--r--   0 runner    (1001) docker     (116)      795 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       56 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/manipulating-models.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/migrating-from-pyomo.nblink
--rw-r--r--   0 runner    (1001) docker     (116)    14887 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (116)       52 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/solve-on-remote.nblink
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2415 2023-03-20 09:09:04.000000 linopy-0.1.4/doc/syntax.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.052864 linopy-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     9585 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/create-a-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    11695 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/creating-constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    10367 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/creating-variables.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)     7586 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/manipulating-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)      705 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/migrating-from-pyomo.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    27151 2023-03-20 09:09:04.000000 linopy-0.1.4/examples/solve-on-remote.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.052864 linopy-0.1.4/linopy/
--rw-r--r--   0 runner    (1001) docker     (116)      678 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5348 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     1324 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     5891 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)    28681 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (116)    35829 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/expressions.py
--rw-r--r--   0 runner    (1001) docker     (116)    15784 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     6313 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/matrices.py
--rw-r--r--   0 runner    (1001) docker     (116)    37679 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/model.py
--rw-r--r--   0 runner    (1001) docker     (116)      731 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/monkey_patch_xarray.py
--rw-r--r--   0 runner    (1001) docker     (116)     8171 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/remote.py
--rw-r--r--   0 runner    (1001) docker     (116)    19763 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/solvers.py
--rw-r--r--   0 runner    (1001) docker     (116)      172 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)    35691 2023-03-20 09:09:04.000000 linopy-0.1.4/linopy/variables.py
--rw-r--r--   0 runner    (1001) docker     (116)      160 2023-03-20 09:09:14.000000 linopy-0.1.4/linopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.052864 linopy-0.1.4/linopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3377 2023-03-20 09:09:14.000000 linopy-0.1.4/linopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4300 2023-03-20 09:09:15.000000 linopy-0.1.4/linopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-20 09:09:14.000000 linopy-0.1.4/linopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      286 2023-03-20 09:09:14.000000 linopy-0.1.4/linopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-03-20 09:09:14.000000 linopy-0.1.4/linopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      131 2023-03-20 09:09:04.000000 linopy-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-20 09:09:15.056864 linopy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2023-03-20 09:09:04.000000 linopy-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 09:09:15.056864 linopy-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (116)    10275 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     3421 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_inconsistency_checks.py
--rw-r--r--   0 runner    (1001) docker     (116)     2943 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    14142 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (116)     2839 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (116)    11259 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (116)     3808 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (116)      951 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_scalar_constraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     2086 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_scalar_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (116)     4374 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (116)     5494 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_variable_assignment.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2023-03-20 09:09:04.000000 linopy-0.1.4/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.168245 linopy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 08:45:45.000000 linopy-0.1.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.148246 linopy-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 08:45:45.000000 linopy-0.1.5/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 08:45:45.000000 linopy-0.1.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-05 08:45:45.000000 linopy-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 08:45:45.000000 linopy-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-05 08:45:45.000000 linopy-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-05 08:45:45.000000 linopy-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-05 08:45:58.168245 linopy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-05 08:45:45.000000 linopy-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/environment.fixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/benchmark/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/notebooks/plot-benchmarks.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_jump.jl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_pyomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/concat-benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/leftovers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmark-linopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/merge-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-pyomo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/write-lp-file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/benchmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/create-a-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/creating-constraints.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/creating-variables.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132092 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/manipulating-models.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/migrating-from-pyomo.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/solve-on-remote.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/syntax.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/create-a-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/creating-constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/creating-variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/manipulating-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/migrating-from-pyomo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/solve-on-remote.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/linopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30415 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38511 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/monkey_patch_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/linopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 08:45:45.000000 linopy-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:45:58.168245 linopy-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-05 08:45:45.000000 linopy-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_inconsistency_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_scalar_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_scalar_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variable_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variables.py
```

### Comparing `linopy-0.1.4/.github/workflows/CI.yaml` & `linopy-0.1.5/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/.pre-commit-config.yaml` & `linopy-0.1.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: check-merge-conflict
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black
     # Current docformatter version has a problem with urls (it's annoying)
 # -   repo: https://github.com/PyCQA/docformatter
 #     rev: v1.6.0.rc1
 #     hooks:
 #     -   id: docformatter
@@ -25,15 +25,15 @@
     -   id: absolufy-imports
 -   repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black", "--filter-files"]
 -   repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     -   id: codespell
         types_or: [python, rst, markdown]
         files: ^(linopy|doc)/
 -   repo: https://github.com/aflc/pre-commit-jupyter
     rev: v1.2.1
     hooks:
```

### Comparing `linopy-0.1.4/LICENSE.txt` & `linopy-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/PKG-INFO` & `linopy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `linopy-0.1.4/README.md` & `linopy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/README.md` & `linopy-0.1.5/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/Snakefile` & `linopy-0.1.5/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark-absolute.pdf` & `linopy-0.1.5/benchmark/benchmark-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark-absolute.png` & `linopy-0.1.5/benchmark/benchmark-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark-overhead.pdf` & `linopy-0.1.5/benchmark/benchmark-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark-overhead.png` & `linopy-0.1.5/benchmark/benchmark-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark_resource-absolute.pdf` & `linopy-0.1.5/benchmark/benchmark_resource-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark_resource-absolute.png` & `linopy-0.1.5/benchmark/benchmark_resource-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark_resource-overhead.pdf` & `linopy-0.1.5/benchmark/benchmark_resource-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/benchmark_resource-overhead.png` & `linopy-0.1.5/benchmark/benchmark_resource-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/environment.fixed.yaml` & `linopy-0.1.5/benchmark/environment.fixed.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/notebooks/plot-benchmarks.py.ipynb` & `linopy-0.1.5/benchmark/notebooks/plot-benchmarks.py.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_cvxpy.py` & `linopy-0.1.5/benchmark/scripts/benchmark_cvxpy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_gurobipy.py` & `linopy-0.1.5/benchmark/scripts/benchmark_gurobipy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_jump.jl` & `linopy-0.1.5/benchmark/scripts/benchmark_jump.jl`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_linopy.py` & `linopy-0.1.5/benchmark/scripts/benchmark_linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_ortools.py` & `linopy-0.1.5/benchmark/scripts/benchmark_ortools.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_pulp.py` & `linopy-0.1.5/benchmark/scripts/benchmark_pulp.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmark_pyomo.py` & `linopy-0.1.5/benchmark/scripts/benchmark_pyomo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/concat-benchmarks.py` & `linopy-0.1.5/benchmark/scripts/concat-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmark-linopy.py` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmark-linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/leftovers/common.py` & `linopy-0.1.5/benchmark/scripts/leftovers/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/merge-benchmarks.py` & `linopy-0.1.5/benchmark/scripts/merge-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/plot-benchmarks.py` & `linopy-0.1.5/benchmark/scripts/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/benchmark/scripts/write-lp-file.py` & `linopy-0.1.5/benchmark/scripts/write-lp-file.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/Makefile` & `linopy-0.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/_static/theme_overrides.css` & `linopy-0.1.5/doc/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/api.rst` & `linopy-0.1.5/doc/api.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/benchmark.png` & `linopy-0.1.5/doc/benchmark.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/benchmark.rst` & `linopy-0.1.5/doc/benchmark.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/conf.py` & `linopy-0.1.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/contributing.rst` & `linopy-0.1.5/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/index.rst` & `linopy-0.1.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/logo.pdf` & `linopy-0.1.5/doc/logo.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/logo.png` & `linopy-0.1.5/doc/logo.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/logo.py` & `linopy-0.1.5/doc/logo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/make.bat` & `linopy-0.1.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/release_notes.rst` & `linopy-0.1.5/doc/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Release Notes
 =============
 
 .. Upcoming Release
 .. ----------------
 
+Version 0.1.5
+-------------
+
+
+* Add `sel` functions to `Constraint` and `AnonymousConstraint` to allow for selection and inspection of constraints by coordinate.
+* The printout of `Variables` and `Constraints` was refactored to a more concise layout.
+* The solving termination condition "other" is now tagged as solving status "warning".
 
 Version 0.1.4
 -------------
 
 * Fix representation of empty variables and linear expressions.
 * The benchmark reported in [here](https://github.com/PyPSA/linopy/tree/master/benchmark) was updated to the latest version of linopy and adjusted to be fully reproducible.
```

### Comparing `linopy-0.1.4/doc/solvers.rst` & `linopy-0.1.5/doc/solvers.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/doc/syntax.rst` & `linopy-0.1.5/doc/syntax.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/create-a-model.ipynb` & `linopy-0.1.5/examples/create-a-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/creating-constraints.ipynb` & `linopy-0.1.5/examples/creating-constraints.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/creating-variables.ipynb` & `linopy-0.1.5/examples/creating-variables.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/manipulating-models.ipynb` & `linopy-0.1.5/examples/manipulating-models.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/migrating-from-pyomo.ipynb` & `linopy-0.1.5/examples/migrating-from-pyomo.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/examples/solve-on-remote.ipynb` & `linopy-0.1.5/examples/solve-on-remote.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/__init__.py` & `linopy-0.1.5/linopy/__init__.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/common.py` & `linopy-0.1.5/linopy/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/config.py` & `linopy-0.1.5/linopy/config.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/constants.py` & `linopy-0.1.5/linopy/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
 STATUS_TO_TERMINATION_CONDITION_MAP = {
     SolverStatus.ok: [
         TerminationCondition.optimal,
         TerminationCondition.iteration_limit,
         TerminationCondition.time_limit,
         TerminationCondition.terminated_by_limit,
-        TerminationCondition.other,
         TerminationCondition.suboptimal,
     ],
     SolverStatus.warning: [
         TerminationCondition.unbounded,
         TerminationCondition.infeasible,
         TerminationCondition.infeasible_or_unbounded,
         TerminationCondition.other,
```

### Comparing `linopy-0.1.4/linopy/constraints.py` & `linopy-0.1.5/linopy/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Linopy constraints module.
 
 This module contains implementations for the Constraint{s} class.
 """
 
+import functools
 import re
 from dataclasses import dataclass, field
 from itertools import product
 from typing import Any, Sequence, Union
 
 import dask
 import numpy as np
@@ -32,14 +33,36 @@
     print_single_expression,
     replace_by_map,
 )
 from linopy.config import options
 from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
 
 
+def conwrap(method, *default_args, **new_default_kwargs):
+    @functools.wraps(method)
+    def _conwrap(con, *args, **kwargs):
+        for k, v in new_default_kwargs.items():
+            kwargs.setdefault(k, v)
+        return con.__class__(
+            method(con.labels, *default_args, *args, **kwargs), con.model, con.name
+        )
+
+    _conwrap.__doc__ = f"Wrapper for the xarray {method} function for linopy.Constraint"
+    if new_default_kwargs:
+        _conwrap.__doc__ += f" with default arguments: {new_default_kwargs}"
+
+    return _conwrap
+
+
+def _con_unwrap(con):
+    if isinstance(con, Constraint):
+        return con.labels
+    return con
+
+
 @forward_as_properties(
     labels=[
         "attrs",
         "coords",
         "indexes",
         "name",
         "shape",
@@ -317,14 +340,18 @@
             )
         return self.model.dual[self.name]
 
     @property
     def shape(self):
         return self.labels.shape
 
+    sel = conwrap(DataArray.sel)
+
+    isel = conwrap(DataArray.isel)
+
 
 @dataclass(repr=False)
 class Constraints:
     """
     A constraint container used for storing multiple constraint arrays.
     """
 
@@ -348,26 +375,21 @@
     def __repr__(self):
         """
         Return a string representation of the linopy model.
         """
         r = "linopy.model.Constraints"
         line = "-" * len(r)
         r += f"\n{line}\n\n"
-        # matches string between "Data variables" and "Attributes"/end of string
+
+        labelprint = self.labels.__repr__()
         coordspattern = r"(?s)(?<=\<xarray\.Dataset\>\n).*?(?=Data variables:)"
-        datapattern = r"(?s)(?<=Data variables:).*?(?=($|\nAttributes))"
-        for k, K in zip(self.dataset_attrs, self.dataset_names):
-            orig = getattr(self, k).__repr__()
-            if k == "labels":
-                r += re.search(coordspattern, orig).group() + "\n"
-            data = re.search(datapattern, orig).group()
-            # drop first line which includes counter for long ds
-            data = data.split("\n", 1)[1]
-            line = "-" * (len(K) + 1)
-            r += f"{K}:\n{data}\n\n"
+        r += re.search(coordspattern, labelprint).group()
+        r += "Constraints:\n"
+        for name in self.labels:
+            r += f"  *  {name} ({', '.join(self.labels[name].coords)})\n"
         return r
 
     def __getitem__(
         self, names: Union[str, Sequence[str]]
     ) -> Union[Constraint, "Constraints"]:
         if isinstance(names, str):
             return Constraint(self.labels[names], self.model, names)
@@ -836,14 +858,49 @@
         lhs = expressions.LinearExpression._from_scalarexpression_list(
             exprs, coords, model
         )
         sign = DataArray(array([c.sign for c in cons]).reshape(shape), coords)
         rhs = DataArray(array([c.rhs for c in cons]).reshape(shape), coords)
         return cls(lhs, sign, rhs)
 
+    def sel(self, indexers=None, **indexer_kwargs):
+        """
+        Select a subset of the AnonymousConstraint array.
+
+        The function mirrors the behavior of the `xarray.Dataset.sel` function.
+        For further information please refer to its docstring.
+
+        Parameters
+        ----------
+        indexers : dict, optional
+            A dict with keys matching the dimensions and values given by scalars, slices or arrays. By default None.
+        **indexers_kwargs : {dim: indexer, ...}, optional
+            The keyword arguments form of ``indexers``.
+            One of indexers or indexers_kwargs must be provided.
+
+        Returns
+        -------
+        AnonymousConstraint
+            A new AnonymousConstraint including all values of the original
+            whose indexes lay within the realm of selection.
+        """
+
+        indexers = xr.core.utils.either_dict_or_kwargs(indexers, indexer_kwargs, "sel")
+
+        lhs_indexers = {k: v for k, v in indexers.items() if k in self.lhs.dims}
+        lhs = self.lhs.sel(lhs_indexers)
+
+        sign_indexers = {k: v for k, v in indexers.items() if k in self.sign.dims}
+        sign = self.sign.sel(sign_indexers)
+
+        rhs_indexers = {k: v for k, v in indexers.items() if k in self.rhs.dims}
+        rhs = self.rhs.sel(rhs_indexers)
+
+        return self.__class__(lhs, sign, rhs)
+
 
 class AnonymousScalarConstraint:
     """
     Container for anonymous scalar constraint.
 
     This contains a left-hand-side (lhs), a sign and a right-hand-side
     (rhs) for exactly one constraint.
```

### Comparing `linopy-0.1.4/linopy/expressions.py` & `linopy-0.1.5/linopy/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -882,14 +882,16 @@
 
     isel = exprwrap(Dataset.isel)
 
     shift = exprwrap(Dataset.shift)
 
     reindex = exprwrap(Dataset.reindex, fill_value=_fill_value)
 
+    reindex_like = exprwrap(Dataset.reindex_like, fill_value=_fill_value)
+
     rename = exprwrap(Dataset.rename)
 
     rename_dims = exprwrap(Dataset.rename_dims)
 
     roll = exprwrap(Dataset.roll)
```

### Comparing `linopy-0.1.4/linopy/io.py` & `linopy-0.1.5/linopy/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 
 def float_to_str(arr, ensure_sign=True):
     """
     Convert numpy array to str typed array.
     """
     if ensure_sign:
-        convert = np.frompyfunc(lambda f: "%+f" % f, 1, 1)
+        convert = np.frompyfunc(lambda f: "%+.12g" % f, 1, 1)
     else:
-        convert = np.frompyfunc(lambda f: "%f" % f, 1, 1)
+        convert = np.frompyfunc(lambda f: "%.12g" % f, 1, 1)
     return convert(arr)
 
 
 def fill_by(target_shape, where, fill, other=""):
     """
     Create array of `target_shape` with values from `fill` where `where` is
     True.
```

### Comparing `linopy-0.1.4/linopy/matrices.py` & `linopy-0.1.5/linopy/matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/model.py` & `linopy-0.1.5/linopy/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -468,15 +468,15 @@
             ), "Dimensions of mask not a subset of resulting labels dimensions."
 
         # It is important to end up with monotonically increasing labels in the
         # model's variables container as we use it for indirect indexing.
         labels_reindexed = labels.reindex_like(self.variables.labels, fill_value=-1)
         if not labels.equals(labels_reindexed):
             warnings.warn(
-                f"Reindexing variable {name} to match existing coordinates.",
+                f"Reindexing variable `{name}` to match existing coordinates.",
                 UserWarning,
             )
             labels = labels_reindexed
             lower = lower.reindex_like(labels)
             upper = upper.reindex_like(labels)
             if mask is None:
                 mask = labels != -1
@@ -589,25 +589,44 @@
         lhs = lhs.sanitize()
         sign = maybe_replace_signs(DataArray(sign))
         rhs = DataArray(rhs)
 
         if labels is None:
             labels = (lhs.vars.chunk() + rhs).sum("_term")
 
+        if mask is not None:
+            mask = DataArray(mask).astype(bool)
+            mask, _ = xr.align(mask, labels, join="right")
+            assert set(mask.dims).issubset(
+                labels.dims
+            ), "Dimensions of mask not a subset of resulting labels dimensions."
+
+        # It is important to end up with monotonically increasing labels in the
+        # model's constraints container as we use it for indirect indexing.
+        labels_reindexed = labels.reindex_like(self.constraints.labels, fill_value=-1)
+        if not labels.equals(labels_reindexed):
+            warnings.warn(
+                f"Reindexing constraint `{name}` to match existing coordinates.",
+                UserWarning,
+            )
+            labels = labels_reindexed
+            lhs = lhs.reindex_like(labels)
+            rhs = rhs.reindex_like(labels)
+            if mask is None:
+                mask = labels != -1
+            else:
+                mask = mask.reindex_like(labels_reindexed, fill_value=False)
+
         self.check_force_dim_names(labels)
 
         start = self._cCounter
         labels.data = np.arange(start, start + labels.size).reshape(labels.shape)
         self._cCounter += labels.size
 
         if mask is not None:
-            mask = DataArray(mask)
-            assert set(mask.dims).issubset(
-                labels.dims
-            ), "Dimensions of mask not a subset of resulting labels dimensions."
             labels = labels.where(mask, -1)
 
         lhs = lhs.data.rename({"_term": f"{name}_term"})
 
         if self.chunk:
             lhs = lhs.chunk(self.chunk)
             sign = sign.chunk(self.chunk)
```

### Comparing `linopy-0.1.4/linopy/monkey_patch_xarray.py` & `linopy-0.1.5/linopy/monkey_patch_xarray.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/remote.py` & `linopy-0.1.5/linopy/remote.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/solvers.py` & `linopy-0.1.5/linopy/solvers.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/linopy/variables.py` & `linopy-0.1.5/linopy/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -804,25 +804,21 @@
     def __repr__(self):
         """
         Return a string representation of the linopy model.
         """
         r = "linopy.model.Variables"
         line = "-" * len(r)
         r += f"\n{line}\n\n"
-        # matches string between "Data variables" and "Attributes"/end of string
+
+        labelprint = self.labels.__repr__()
         coordspattern = r"(?s)(?<=\<xarray\.Dataset\>\n).*?(?=Data variables:)"
-        datapattern = r"(?s)(?<=Data variables:).*?(?=($|\nAttributes))"
-        for k, K in zip(self.dataset_attrs, self.dataset_names):
-            orig = getattr(self, k).__repr__()
-            if k == "labels":
-                r += re.search(coordspattern, orig).group() + "\n"
-            data = re.search(datapattern, orig).group()
-            # drop first line which includes counter for long ds
-            data = data.split("\n", 1)[1]
-            r += f"{K}:\n{data}\n\n"
+        r += re.search(coordspattern, labelprint).group()
+        r += "Variables:\n"
+        for name in self.labels:
+            r += f"  *  {name} ({', '.join(self.labels[name].coords)})\n"
         return r
 
     def __iter__(self):
         return self.labels.__iter__()
 
     _merge_inplace = _merge_inplace
```

### Comparing `linopy-0.1.4/linopy.egg-info/PKG-INFO` & `linopy-0.1.5/linopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `linopy-0.1.4/linopy.egg-info/SOURCES.txt` & `linopy-0.1.5/linopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/setup.py` & `linopy-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_constraint.py` & `linopy-0.1.5/test/test_constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,20 @@
 
 def test_anonymous_scalar_constraint_from_linear_expression_fail(x, y):
     expr = 10 * x[0] + y[1]
     with pytest.raises(TypeError):
         expr == x[0]
 
 
+def test_anonymous_constraint_sel(x, y):
+    expr = 10 * x + y
+    con = expr <= 10
+    assert isinstance(con.sel(first=[1, 2]), AnonymousConstraint)
+
+
 def test_constraint_from_rule(m, x, y):
     def bound(m, i, j):
         if i % 2:
             return (i - 1) * x[i - 1] + y[j] >= 0
         else:
             return i * x[i] >= 0
 
@@ -235,14 +241,19 @@
 
 def test_constraint_labels_setter_invalid(c):
     # Test that assigning labels raises FrozenInstanceError
     with pytest.raises(AttributeError):
         c.labels = c.labels
 
 
+def test_constraint_sel(c):
+    assert isinstance(c.sel(first=[1, 2]), linopy.constraints.Constraint)
+    assert isinstance(c.isel(first=[1, 2]), linopy.constraints.Constraint)
+
+
 def test_constraint_assignment_with_anonymous_constraints(m, x, y):
     m.add_constraints(x + y == 0, name="c2")
     assert m.constraints["c2"].vars.notnull().all()
     assert m.constraints["c2"].coeffs.notnull().all()
 
 
 def test_constraint_assignment_sanitize_zeros(m, x, y):
```

### Comparing `linopy-0.1.4/test/test_constraints.py` & `linopy-0.1.5/test/test_constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 def test_constraint_assignment():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    x = m.add_variables(lower, upper)
-    y = m.add_variables()
+    x = m.add_variables(lower, upper, name="x")
+    y = m.add_variables(name="y")
 
     m.add_constraints(1 * x + 10 * y, EQUAL, 0)
 
     for attr in m.constraints.dataset_attrs:
         assert "con0" in getattr(m.constraints, attr)
 
     assert m.constraints.labels.con0.shape == (10, 10)
@@ -38,16 +38,16 @@
 
 
 def test_anonymous_constraint_assignment():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    x = m.add_variables(lower, upper)
-    y = m.add_variables()
+    x = m.add_variables(lower, upper, name="x")
+    y = m.add_variables(name="y")
     con = 1 * x + 10 * y == 0
     m.add_constraints(con)
 
     for attr in m.constraints.dataset_attrs:
         assert "con0" in getattr(m.constraints, attr)
 
     assert m.constraints.labels.con0.shape == (10, 10)
@@ -82,14 +82,34 @@
         10,
         10,
         1,
     )
     assert isinstance(m.constraints.coeffs.c.data, dask.array.core.Array)
 
 
+def test_constraint_assignment_with_reindex():
+    m = Model()
+
+    lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
+    upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
+    x = m.add_variables(lower, upper, name="x")
+    y = m.add_variables(name="y")
+
+    m.add_constraints(1 * x + 10 * y, EQUAL, 0)
+
+    shuffled_coords = pd.Index([2, 1, 3, 4, 6, 5, 7, 9, 8, 0], name="first")
+    con = m.variables["x"].loc[shuffled_coords] <= 10
+    with pytest.warns(UserWarning):
+        con_shuffled = m.add_constraints(con, name="con_shuffled")
+
+    assert con_shuffled.indexes["dim_0"].equals(m.constraints["con0"].indexes["dim_0"])
+    # check if labels are monotonically increasing
+    assert np.all(np.diff(np.ravel(con_shuffled.labels)) > 0)
+
+
 def test_wrong_constraint_assignment_repeated():
     # repeated variable assignment is forbidden
     m = Model()
     x = m.add_variables()
     m.add_constraints(x, LESS_EQUAL, 0, name="con")
     with pytest.raises(ValueError):
         m.add_constraints(x, LESS_EQUAL, 0, name="con")
```

### Comparing `linopy-0.1.4/test/test_inconsistency_checks.py` & `linopy-0.1.5/test/test_inconsistency_checks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_io.py` & `linopy-0.1.5/test/test_io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_linear_expression.py` & `linopy-0.1.5/test/test_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_matrices.py` & `linopy-0.1.5/test/test_matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_model.py` & `linopy-0.1.5/test/test_model.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_optimization.py` & `linopy-0.1.5/test/test_optimization.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_options.py` & `linopy-0.1.5/test/test_options.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_repr.py` & `linopy-0.1.5/test/test_repr.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_scalar_constraint.py` & `linopy-0.1.5/test/test_scalar_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_scalar_linear_expression.py` & `linopy-0.1.5/test/test_scalar_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_variable.py` & `linopy-0.1.5/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_variable_assignment.py` & `linopy-0.1.5/test/test_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.4/test/test_variables.py` & `linopy-0.1.5/test/test_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,23 @@
     upper = pd.Series(np.ones((12)))
     with pytest.warns(UserWarning):
         m.add_variables(upper)
 
     assert m.variables.labels.var0[-1].item() != -1
 
 
+def test_variables_assignment_with_reindex(m):
+    shuffled_coords = [pd.Index([2, 1, 3, 4, 6, 5, 7, 9, 8, 0], name="first")]
+    with pytest.warns(UserWarning):
+        a = m.add_variables(coords=shuffled_coords, name="a")
+    assert a.indexes["first"].equals(m["x"].indexes["first"])
+    # check if labels are monotonically increasing
+    assert np.all(np.diff(np.ravel(a.labels)) > 0)
+
+
 def test_scalar_variables_name_counter():
     m = Model()
     m.add_variables()
     m.add_variables()
     assert "var0" in m.variables
     assert "var1" in m.variables
```

