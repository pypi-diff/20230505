# Comparing `tmp/mqt.problemsolver-0.1.0.tar.gz` & `tmp/mqt.problemsolver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.problemsolver-0.1.0.tar", last modified: Wed Oct 26 07:22:19 2022, max compression
+gzip compressed data, was "mqt.problemsolver-0.2.0.tar", last modified: Fri May  5 08:39:13 2023, max compression
```

## Comparing `mqt.problemsolver-0.1.0.tar` & `mqt.problemsolver-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/img/
--rw-r--r--   0 runner    (1001) docker     (121)   437820 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/img/framework.png
--rw-r--r--   0 runner    (1001) docker     (121)    10822 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/img/kakuro.png
--rw-r--r--   0 runner    (1001) docker     (121)    63643 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/img/tsp.png
--rw-r--r--   0 runner    (1001) docker     (121)    64664 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/paper_figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.784705 mqt.problemsolver-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.784705 mqt.problemsolver-0.1.0/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/src/mqt/problemsolver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/src/mqt/problemsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11170 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/src/mqt/problemsolver/csp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/src/mqt/problemsolver/csp_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/src/mqt/problemsolver/tsp.py
--rw-r--r--   0 runner    (1001) docker     (121)    89198 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/src/mqt/problemsolver/tsp_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-10-26 07:22:19.000000 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-26 07:22:19.000000 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 07:22:19.000000 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-26 07:22:19.000000 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-26 07:22:19.000000 mqt.problemsolver-0.1.0/src/mqt.problemsolver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 07:22:19.788705 mqt.problemsolver-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/tests/test_csp.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-26 07:22:10.000000 mqt.problemsolver-0.1.0/tests/test_tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.764842 mqt.problemsolver-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.764842 mqt.problemsolver-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.764842 mqt.problemsolver-0.2.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   437820 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/framework.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/kakuro.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   149032 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/satellite_mission_planning_problem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63643 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/img/tsp.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.768842 mqt.problemsolver-0.2.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/csp_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.768842 mqt.problemsolver-0.2.0/notebooks/precompilation/
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/precompilation/evaluation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/precompilation/precompilation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/precompilation/precompilation_paper_figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/precompilation/res_qaoa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/precompilation/res_satellite.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/problemsolver_paper_figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.768842 mqt.problemsolver-0.2.0/notebooks/satellitesolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/satellitesolver/evaluation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/satellitesolver/res_satellite_solver.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/satellitesolver/res_satellite_solver_noisy.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/satellitesolver/satellitesolver_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/notebooks/tsp_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:39:13.776842 mqt.problemsolver-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.760842 mqt.problemsolver-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.760842 mqt.problemsolver-0.2.0/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/src/mqt/problemsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/csp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/src/mqt/problemsolver/partialcompiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/partialcompiler/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/partialcompiler/qaoa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/ImagingLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/satellitesolver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/src/mqt/problemsolver/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.768842 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-05 08:39:13.000000 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-05 08:39:13.000000 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:39:13.000000 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 08:39:13.000000 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 08:39:13.000000 mqt.problemsolver-0.2.0/src/mqt.problemsolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:39:13.772842 mqt.problemsolver-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/tests/test_csp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/tests/test_satellitesolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 08:39:00.000000 mqt.problemsolver-0.2.0/tests/test_tsp.py
```

### Comparing `mqt.problemsolver-0.1.0/.github/workflows/coverage.yml` & `mqt.problemsolver-0.2.0/.github/workflows/coverage.yml`

 * *Files 25% similar despite different names*

```diff
@@ -16,11 +16,12 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
       - name: Install MQT ProblemSolver
         run: pip install .[coverage]
       - name: Generate Report
         run: pytest -v --cov=./ --cov-report=xml
-#    - name: Upload coverage to Codecov
-#      uses: codecov/codecov-action@v3
-#      with:
-#        fail_ci_if_error: true
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: true
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `mqt.problemsolver-0.1.0/.github/workflows/deploy.yml` & `mqt.problemsolver-0.2.0/.github/workflows/deploy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -59,9 +59,9 @@
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
-          skip_existing: true
+          skip-existing: true
           verbose: true
```

### Comparing `mqt.problemsolver-0.1.0/.gitignore` & `mqt.problemsolver-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.problemsolver-0.1.0/.pre-commit-config.yaml` & `mqt.problemsolver-0.2.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 #
 #     pre-commit install
 #
 
 ci:
   autoupdate_commit_msg: "⬆️🪝 update pre-commit hooks"
   autofix_commit_msg: "🎨 pre-commit fixes"
+  skip: [mypy]
 
 repos:
   # Standard hooks
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.3.0"
+    rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-toml
@@ -27,83 +28,68 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   # Handling unwanted unicode characters
   - repo: https://github.com/sirosen/texthooks
-    rev: "0.4.0"
+    rev: "0.5.0"
     hooks:
       - id: fix-ligatures
       - id: fix-smartquotes
 
-  # Sort includes
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-        args: ["--profile", "black", "--filter-files"]
-
-  # Upgrade old Python syntax
-  - repo: https://github.com/asottile/pyupgrade
-    rev: "v2.37.3"
-    hooks:
-      - id: pyupgrade
-        args: ["--py37-plus"]
-
   # Run code formatting with Black
   - repo: https://github.com/psf/black
-    rev: "22.8.0" # Keep in sync with blacken-docs
+    rev: "23.3.0" # Keep in sync with blacken-docs
     hooks:
       - id: black
 
   # Also run Black on examples in the documentation
   - repo: https://github.com/asottile/blacken-docs
-    rev: "v1.12.1"
+    rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==22.8.0 # keep in sync with black hook
-
-  # Check for common mistakes
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: "v1.9.0"
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-log-warn
-      - id: python-no-eval
-      - id: python-use-type-annotations
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
-
-  # Run Flake8 checks
-  - repo: https://github.com/PyCQA/flake8
-    rev: "5.0.4"
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-bugbear
-          - flake8-comprehensions
-          - flake8-future-annotations
-          - flake8-new-union-types
-          - flake8-simplify
-          - flake8-2020
+          - black==23.3.0 # keep in sync with black hook
 
   # Check for spelling
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.1"
+    rev: "v2.2.4"
     hooks:
       - id: codespell
         args: ["-L", "wille,linz"]
         exclude: >
           (?x)^(
               .*\.ipynb
           )$
 
   # Format configuration files with prettier
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.0"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
+
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.263
+    hooks:
+      - id: ruff
+        args: ["--fix"]
+
+  # Clean jupyter notebooks
+  - repo: https://github.com/srstevenson/nb-clean
+    rev: "2.4.0"
+    hooks:
+      - id: nb-clean
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.2.0
+    hooks:
+      - id: mypy
+        files: ^(src|tests|setup.py)
+        args: []
+        additional_dependencies:
+          - types-setuptools
+          - python_tsp
+          - networkx
+          - mqt.ddsim
+          - pytest
```

### Comparing `mqt.problemsolver-0.1.0/img/framework.png` & `mqt.problemsolver-0.2.0/img/framework.png`

 * *Files identical despite different names*

### Comparing `mqt.problemsolver-0.1.0/img/kakuro.png` & `mqt.problemsolver-0.2.0/img/kakuro.png`

 * *Files identical despite different names*

### Comparing `mqt.problemsolver-0.1.0/img/tsp.png` & `mqt.problemsolver-0.2.0/img/tsp.png`

 * *Files identical despite different names*

### Comparing `mqt.problemsolver-0.1.0/src/mqt/problemsolver/csp.py` & `mqt.problemsolver-0.2.0/src/mqt/problemsolver/csp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING, TypedDict
+
 import numpy as np
+from mqt.ddsim import DDSIMProvider
 from qiskit import QuantumCircuit, QuantumRegister, execute
 
-from mqt import ddsim
+if TYPE_CHECKING:
+    from qiskit.circuit import Instruction
+
+
+class Constraint(TypedDict, total=False):
+    """
+    Class to store the properties of a single constraint.
+    """
+
+    constraint_type: str
+    operand_one: str
+    operand_two: str
+    to_be_satisfied_sum: int
 
 
 class CSP:
     def solve(
         self,
-        constraints: list[dict],
-        quantum_algorithm="Grover",
-    ):
+        constraints: list[Constraint],
+        quantum_algorithm: str = "Grover",
+    ) -> tuple[int, int, int, int] | bool:
         """Method to solve the problem.
 
         Keyword arguments:
         constraints -- List of to be satisfied constraints.
         quantum_algorithm -- Selected quantum algorithm to solve problem.
 
         Return values:
         solution -- Solution to the problem if it exists.
         """
         if quantum_algorithm == "Grover":
             qc, anc, anc_mct, flag, nqubits, nancilla, (a, b, c, d) = self.init_qc()
-            qc, mct_list = self.encode_constraints(
-                qc, a, b, c, d, anc, constraints=constraints
-            )
+            qc, mct_list = self.encode_constraints(qc, a, b, c, d, anc, constraints=constraints)
             oracle = self.create_oracle(qc, mct_list, flag, anc_mct)
             for m in (5, 6, 7, 8, 12):
-                qc = self.create_grover(
-                    oracle, nqubits, nancilla, ninputs=nqubits - 1, grover_iterations=m
-                )
+                qc = self.create_grover(oracle, nqubits, nancilla, ninputs=nqubits - 1, grover_iterations=m)
                 solution = self.simulate(qc)
                 if solution:
                     break
             if solution:
                 return solution
-            else:
-                return False
-
-        else:
-            print("ERROR: Selected quantum algorithm is not implemented.")
             return False
 
-    def print(
+        print("ERROR: Selected quantum algorithm is not implemented.")
+        return False
+
+    def print_problem(
         self,
         sum_s0: str | int = "s0",
         sum_s1: str | int = "s1",
         sum_s2: str | int = "s2",
         sum_s3: str | int = "s3",
         a: str | int = "a",
         b: str | int = "b",
         c: str | int = "c",
         d: str | int = "d",
-    ):
+    ) -> None:
         """Method to visualize the problem.
 
         Keyword arguments:
         sum_* -- Sums to be satisfied.
         a to d -- Variable values satisfying the respective sums.
         """
 
@@ -65,16 +74,20 @@
         print("------------------")
         print(" ", sum_s2, " | ", a, " | ", b, " |")
         print("------------------")
         print(" ", sum_s3, " | ", c, " | ", d, " |")
         print("------------------\n")
 
     def check_inequality(
-        self, qc: QuantumCircuit, x: tuple, y: tuple, res_anc: QuantumRegister
-    ):
+        self,
+        qc: QuantumCircuit,
+        x: tuple[QuantumRegister, QuantumRegister],
+        y: tuple[QuantumRegister, QuantumRegister],
+        res_anc: QuantumRegister,
+    ) -> None:
         x_low, x_high = x
         y_low, y_high = y
 
         qc.cx(x_high, y_high)
         qc.x(y_high)
         qc.cx(x_low, y_low)
         qc.x(y_low)
@@ -85,37 +98,41 @@
         # Uncompute
         qc.x(y_low)
         qc.cx(x_low, y_low)
         qc.x(y_high)
         qc.cx(x_high, y_high)
 
     def check_equality(
-        self, qc: QuantumCircuit, x: tuple, s: str, res_anc: QuantumRegister
-    ):
+        self,
+        qc: QuantumCircuit,
+        x: tuple[QuantumRegister, QuantumRegister, QuantumRegister],
+        s: str,
+        res_anc: QuantumRegister,
+    ) -> None:
         x_low, x_mid, x_high = x
 
         if s[-1] == "0":
             qc.x(x_low)
         if s[-2] == "0":
             qc.x(x_mid)
         if s[-3] == "0":
             qc.x(x_high)
 
         qc.rcccx(x_low, x_mid, x_high, res_anc)
 
     def add_two_numbers(
         self,
         qc: QuantumCircuit,
-        x: tuple,
-        y: tuple,
+        x: tuple[QuantumRegister, QuantumRegister],
+        y: tuple[QuantumRegister, QuantumRegister],
         ancs: QuantumRegister,
         res_anc_low: QuantumRegister,
         res_anc_high: QuantumRegister,
         anc_carry: QuantumRegister,
-    ):
+    ) -> tuple[QuantumRegister, QuantumRegister, QuantumRegister]:
         x_low, x_high = x
         y_low, y_high = y
 
         qc.rccx(x_low, y_low, res_anc_high)
         qc.cx(x_low, y_low)
         qc.cx(y_low, res_anc_low)
         qc.rccx(x_high, y_high, ancs[0])
@@ -138,95 +155,102 @@
         self,
         qc: QuantumCircuit,
         a: QuantumRegister,
         b: QuantumRegister,
         c: QuantumRegister,
         d: QuantumRegister,
         anc: QuantumRegister,
-        constraints: list[dict],
-    ):
+        constraints: list[Constraint],
+    ) -> tuple[QuantumCircuit, list[QuantumRegister]]:
         mct_list = []
 
         dict_variable_to_quantumregister = {
             "a": a,
             "b": b,
             "c": c,
             "d": d,
         }
         anc_needed_per_constraint = {
             "inequality": 1,
             "addition_equality": 6,
         }
         anc_index = 0
         for constraint in constraints:
-            if constraint.get("type") == "inequality":
-                first_qreg = dict_variable_to_quantumregister.get(
-                    constraint.get("operand_one")
-                )
-                second_qreg = dict_variable_to_quantumregister.get(
-                    constraint.get("operand_two")
-                )
+            if constraint.get("constraint_type") == "inequality":
+                first_qreg = dict_variable_to_quantumregister[constraint["operand_one"]]
+                second_qreg = dict_variable_to_quantumregister[constraint["operand_two"]]
 
                 self.check_inequality(qc, first_qreg, second_qreg, anc[anc_index])
                 mct_list.append(anc[anc_index])
                 qc.barrier()
-                anc_index += anc_needed_per_constraint.get(constraint.get("type"))
+                anc_index += anc_needed_per_constraint[constraint["constraint_type"]]
+
+            elif constraint.get("constraint_type") == "addition_equality":
+                first_qreg = dict_variable_to_quantumregister[constraint["operand_one"]]
+                second_qreg = dict_variable_to_quantumregister[constraint["operand_two"]]
 
-            elif constraint.get("type") == "addition_equality":
-                first_qreg = dict_variable_to_quantumregister.get(
-                    constraint.get("operand_one")
-                )
-                second_qreg = dict_variable_to_quantumregister.get(
-                    constraint.get("operand_two")
-                )
                 tmp_1 = self.add_two_numbers(
                     qc,
                     first_qreg,
                     second_qreg,
                     anc[anc_index : anc_index + 2],
                     anc[anc_index + 2],
                     anc[anc_index + 3],
                     anc[anc_index + 4],
                 )
                 qc.barrier()
                 self.check_equality(
                     qc,
                     tmp_1,
-                    bin(constraint.get("sum"))[2:].zfill(3),
+                    bin(constraint["to_be_satisfied_sum"])[2:].zfill(3),
                     anc[anc_index + 5],
                 )
                 mct_list.append(anc[anc_index + 5])
                 qc.barrier()
-                anc_index += anc_needed_per_constraint.get(constraint.get("type"))
+                anc_index += anc_needed_per_constraint[constraint["constraint_type"]]
             else:
-                print("Unexpected constraint type: ", constraint.get("type"))
+                print("Unexpected constraint type: ", constraint["constraint_type"])
 
         return (qc, mct_list)
 
     def create_oracle(
         self,
         qc: QuantumCircuit,
         mct_list: list[QuantumRegister],
         flag: QuantumRegister,
         anc_mct: QuantumRegister,
-    ):
+    ) -> Instruction:
         compute = qc.to_instruction()
 
         # mark solution
         qc.mct(mct_list, flag, ancilla_qubits=anc_mct, mode="v-chain")
 
         # uncompute
         uncompute = compute.inverse()
         uncompute.name = "uncompute"
         qc.append(uncompute, range(qc.num_qubits))
 
-        oracle = qc.to_instruction(label="oracle")
-        return oracle
+        return qc.to_instruction(label="oracle")
 
-    def init_qc(self):
+    def init_qc(
+        self,
+    ) -> tuple[
+        QuantumCircuit,
+        QuantumRegister,
+        QuantumRegister,
+        QuantumRegister,
+        int,
+        int,
+        tuple[
+            tuple[QuantumRegister, QuantumRegister],
+            tuple[QuantumRegister, QuantumRegister],
+            tuple[QuantumRegister, QuantumRegister],
+            tuple[QuantumRegister, QuantumRegister],
+        ],
+    ]:
         a_low = QuantumRegister(1, "a_low")
         a_high = QuantumRegister(1, "a_high")
         a = (a_low, a_high)
         b_low = QuantumRegister(1, "b_low")
         b_high = QuantumRegister(1, "b_high")
         b = (b_low, b_high)
         c_low = QuantumRegister(1, "c_low")
@@ -260,15 +284,15 @@
     def create_grover(
         self,
         oracle: QuantumCircuit,
         nqubits: int,
         nancilla: int,
         ninputs: int,
         grover_iterations: int,
-    ):
+    ) -> QuantumCircuit:
         import numpy as np
 
         qc = QuantumCircuit(nqubits + nancilla, ninputs)
         qc.h(range(ninputs))
         qc.x(nqubits + nancilla - 1)
         qc.h(nqubits + nancilla - 1)
 
@@ -279,100 +303,98 @@
             qc.mcp(np.pi, list(range(ninputs - 1)), ninputs - 1)
             qc.x(range(ninputs))
             qc.h(range(ninputs))
         qc.measure(range(ninputs), range(ninputs))
 
         return qc
 
-    def simulate(self, qc: QuantumCircuit):
-        backend = ddsim.DDSIMProvider().get_backend("qasm_simulator")
+    def simulate(self, qc: QuantumCircuit) -> tuple[int, int, int, int] | None:
+        backend = DDSIMProvider().get_backend("qasm_simulator")
         job = execute(qc, backend, shots=10000)
         counts = job.result().get_counts(qc)
 
         mean_counts = np.mean(list(counts.values()))
 
         found_sol = False
-        for entry in counts.keys():
-
+        for entry in counts:
             if counts.get(entry) > 5 * mean_counts:
                 found_sol = True
                 break
         if found_sol:
-            for entry in counts.keys():
+            for entry in counts:
                 d = int(entry[0:2], 2)
                 c = int(entry[2:4], 2)
                 b = int(entry[4:6], 2)
                 a = int(entry[6:8], 2)
                 if counts.get(entry) > 5 * mean_counts:
                     return (a, b, c, d)
-        else:
-            print("Simulation was unsuccessful.")
 
-    def get_available_quantum_algorithms(self):
+        print("Simulation was unsuccessful.")
+        return None
+
+    def get_available_quantum_algorithms(self) -> list[str]:
         """Method to get all available quantum algorithms in a list."""
         return ["Grover"]
 
-    def get_kakuro_constraints(
-        self, sum_s0: int, sum_s1: int, sum_s2: int, sum_s3: int
-    ):
+    def get_kakuro_constraints(self, sum_s0: int, sum_s1: int, sum_s2: int, sum_s3: int) -> list[Constraint]:
         """Method to get a list of constraints for the inserted sums."""
         list_of_constraints = []
-        constraint_1 = {
-            "type": "addition_equality",
+        constraint_1: Constraint = {
+            "constraint_type": "addition_equality",
             "operand_one": "a",
             "operand_two": "c",
-            "sum": sum_s0,
+            "to_be_satisfied_sum": sum_s0,
         }
         list_of_constraints.append(constraint_1)
 
-        constraint_2 = {
-            "type": "addition_equality",
+        constraint_2: Constraint = {
+            "constraint_type": "addition_equality",
             "operand_one": "b",
             "operand_two": "d",
-            "sum": sum_s1,
+            "to_be_satisfied_sum": sum_s1,
         }
         list_of_constraints.append(constraint_2)
 
-        constraint_3 = {
-            "type": "addition_equality",
+        constraint_3: Constraint = {
+            "constraint_type": "addition_equality",
             "operand_one": "a",
             "operand_two": "b",
-            "sum": sum_s2,
+            "to_be_satisfied_sum": sum_s2,
         }
         list_of_constraints.append(constraint_3)
 
-        constraint_4 = {
-            "type": "addition_equality",
+        constraint_4: Constraint = {
+            "constraint_type": "addition_equality",
             "operand_one": "c",
             "operand_two": "d",
-            "sum": sum_s3,
+            "to_be_satisfied_sum": sum_s3,
         }
         list_of_constraints.append(constraint_4)
 
-        constraint_5 = {
-            "type": "inequality",
+        constraint_5: Constraint = {
+            "constraint_type": "inequality",
             "operand_one": "a",
             "operand_two": "c",
         }
         list_of_constraints.append(constraint_5)
 
-        constraint_6 = {
-            "type": "inequality",
+        constraint_6: Constraint = {
+            "constraint_type": "inequality",
             "operand_one": "b",
             "operand_two": "d",
         }
         list_of_constraints.append(constraint_6)
 
-        constraint_7 = {
-            "type": "inequality",
+        constraint_7: Constraint = {
+            "constraint_type": "inequality",
             "operand_one": "a",
             "operand_two": "b",
         }
         list_of_constraints.append(constraint_7)
 
-        constraint_8 = {
-            "type": "inequality",
+        constraint_8: Constraint = {
+            "constraint_type": "inequality",
             "operand_one": "c",
             "operand_two": "d",
         }
         list_of_constraints.append(constraint_8)
         return list_of_constraints
```

### Comparing `mqt.problemsolver-0.1.0/src/mqt/problemsolver/tsp.py` & `mqt.problemsolver-0.2.0/src/mqt/problemsolver/tsp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Code is adapted from https://arxiv.org/abs/1805.10928 and https://qiskit.org/textbook/ch-paper-implementations/tsp.html
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, cast
+
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
+from mqt.ddsim import DDSIMProvider
 from python_tsp.exact import solve_tsp_dynamic_programming
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister, execute
 from qiskit.circuit.library import QFT
 
-from mqt import ddsim
+if TYPE_CHECKING:
+    from qiskit.circuit import Gate
 
 
 class TSP:
-    def print(self, solution: list[int] = None):
+    def print_problem(self, solution: list[int] | None = None) -> None:
         """Method to visualize the problem.
 
         Keyword arguments:
         solution -- If provided, the solution is visualized. Otherwise, the problem without solution is shown.
 
         """
         G = nx.DiGraph(directed=True)
@@ -35,43 +41,25 @@
         G.add_edge(3, 2)
         G.add_edge(3, 4)
 
         G.add_edge(4, 1)
         G.add_edge(4, 2)
         G.add_edge(4, 3)
 
-        if hasattr(self, "dist_1_2"):
-            dist_1_2 = self.dist_1_2
-        else:
-            dist_1_2 = "dist_1_2"
-
-        if hasattr(self, "dist_1_3"):
-            dist_1_3 = self.dist_1_3
-        else:
-            dist_1_3 = "dist_1_3"
-
-        if hasattr(self, "dist_1_4"):
-            dist_1_4 = self.dist_1_4
-        else:
-            dist_1_4 = "dist_1_4"
-
-        if hasattr(self, "dist_2_3"):
-            dist_2_3 = self.dist_2_3
-        else:
-            dist_2_3 = "dist_2_3"
-
-        if hasattr(self, "dist_2_4"):
-            dist_2_4 = self.dist_2_4
-        else:
-            dist_2_4 = "dist_2_4"
-
-        if hasattr(self, "dist_3_4"):
-            dist_3_4 = self.dist_3_4
-        else:
-            dist_3_4 = "dist_3_4"
+        dist_1_2 = self.dist_1_2 if hasattr(self, "dist_1_2") else "dist_1_2"
+
+        dist_1_3 = self.dist_1_3 if hasattr(self, "dist_1_3") else "dist_1_3"
+
+        dist_1_4 = self.dist_1_4 if hasattr(self, "dist_1_4") else "dist_1_4"
+
+        dist_2_3 = self.dist_2_3 if hasattr(self, "dist_2_3") else "dist_2_3"
+
+        dist_2_4 = self.dist_2_4 if hasattr(self, "dist_2_4") else "dist_2_4"
+
+        dist_3_4 = self.dist_3_4 if hasattr(self, "dist_3_4") else "dist_3_4"
 
         edge_labels = {
             (1, 2): dist_1_2,
             (1, 3): dist_1_3,
             (1, 4): dist_1_4,
             (2, 3): dist_2_3,
             (2, 4): dist_2_4,
@@ -90,48 +78,40 @@
             font_size=20,
         )
 
         if solution is not None:
             selected_graph_quantum = self.extract_selected_graph(solution)
 
             edges_quantum = selected_graph_quantum.edges()
-            colors_quantum = [
-                selected_graph_quantum[u][v]["color"] for u, v in edges_quantum
-            ]
-            weights_quantum = [
-                selected_graph_quantum[u][v]["weight"] for u, v in edges_quantum
-            ]
+            colors_quantum = [selected_graph_quantum[u][v]["color"] for u, v in edges_quantum]
+            weights_quantum = [selected_graph_quantum[u][v]["weight"] for u, v in edges_quantum]
             nx.draw(
                 selected_graph_quantum,
                 pos,
                 node_color="skyblue",
                 edge_color=colors_quantum,
                 width=weights_quantum,
                 node_size=2000,
                 font_size=20,
             )
 
-        nx.draw_networkx_edge_labels(
-            G, pos, edge_labels=edge_labels, label_pos=0.3, font_size=20
-        )
-
-        return
+        nx.draw_networkx_edge_labels(G, pos, edge_labels=edge_labels, label_pos=0.3, font_size=20)
 
     def solve(
         self,
         dist_1_2: int,
         dist_1_3: int,
         dist_1_4: int,
         dist_2_3: int,
         dist_2_4: int,
         dist_3_4: int,
-        objective_function="shortest_path",
-        quantum_algorithm="QPE",
-        num_qubits_qft=8,
-    ):
+        objective_function: str = "shortest_path",
+        quantum_algorithm: str = "QPE",
+        num_qubits_qft: int = 8,
+    ) -> list[int] | bool:
         """Method to solve the problem.
 
         Keyword arguments:
         dist_*_* -- Defining the adjacency matrix by the distances between the vertices.
         objective_function -- Optimization goal.
         quantum_algorithm -- Selected quantum algorithm to solve problem.
         num_qubits_qft -- Number of qubits used for QFT if "QPE" is selected as the algorithm.
@@ -143,66 +123,54 @@
             self.dist_1_2 = dist_1_2
             self.dist_1_3 = dist_1_3
             self.dist_1_4 = dist_1_4
             self.dist_2_3 = dist_2_3
             self.dist_2_4 = dist_2_4
             self.dist_3_4 = dist_3_4
 
-            self.distances_sum = sum(
-                [dist_1_2, dist_1_3, dist_1_4, dist_2_3, dist_2_4, dist_3_4]
-            )
+            self.distances_sum = sum([dist_1_2, dist_1_3, dist_1_4, dist_2_3, dist_2_4, dist_3_4])
 
             self.num_qubits_qft = num_qubits_qft
             sol_perm = self.solve_using_QPE()
             return sol_perm
 
-        else:
-            print(
-                "ERROR: Combination of objective function quantum algorithm is not implemented."
-            )
-            return False
-
-    def solve_using_QPE(self):
+        print("ERROR: Combination of objective function quantum algorithm is not implemented.")
+        return False
 
+    def solve_using_QPE(self) -> list[int]:
         eigen_values = ["11000110", "10001101", "10000111"]
         all_perms = []
         all_costs = []
         for eigenstate in eigen_values:
-
             qft_register = QuantumRegister(self.num_qubits_qft, "qft")
             eigenstate_register = QuantumRegister(8, "eigen")
-            qft_register_classical = ClassicalRegister(
-                self.num_qubits_qft, "qft_classical"
-            )
+            qft_register_classical = ClassicalRegister(self.num_qubits_qft, "qft_classical")
 
-            qc = self.create_TSP_qc(
-                qft_register, eigenstate_register, qft_register_classical, eigenstate
-            )
+            qc = self.create_TSP_qc(qft_register, eigenstate_register, qft_register_classical, eigenstate)
 
             most_frequent = self.simulate(qc)
 
             route = self.eigenvalue_to_route(eigenstate)
 
             most_frequent_decimal = int(most_frequent, 2)
             phase = most_frequent_decimal / (2**self.num_qubits_qft)
-            costs = self.phase_to_int(phase)
+            costs = self.phase_to_float(phase)
 
             all_perms.append(route)
             all_costs.append(costs)
 
-        solution = all_perms[np.argmin(all_costs)]
-        return solution
+        return all_perms[np.argmin(all_costs)]
 
     def create_TSP_qc(
         self,
         qft_register: QuantumRegister,
         eigenstate_register: QuantumRegister,
         qft_classical_register: ClassicalRegister,
         eigenstate: QuantumRegister,
-    ):
+    ) -> QuantumCircuit:
         qc = QuantumCircuit(qft_register, eigenstate_register, qft_classical_register)
 
         self.encode_eigenstate(qc, eigenstate_register, eigenstate)
 
         qc.h(qft_register[:])
         qc.barrier()
 
@@ -224,63 +192,60 @@
         qc.append(qft, qc.qubits[: len(qft_register)])
         qc.barrier()
 
         # Measure
         qc.measure(qft_register, qft_classical_register)
         return qc
 
-    def get_all_phases(self):
+    def get_all_phases(self) -> list[float]:
         a = self.int_to_phase(self.dist_1_2)
         d = a
         b = self.int_to_phase(self.dist_1_3)
         g = b
         c = self.int_to_phase(self.dist_1_4)
         j = c
         e = self.int_to_phase(self.dist_2_3)
         h = e
         f = self.int_to_phase(self.dist_2_4)
         k = f
         i = self.int_to_phase(self.dist_3_4)
         m = i
         return [a, b, c, d, e, f, g, h, i, j, k, m]
 
-    def simulate(self, qc: QuantumCircuit):
-
-        backend = ddsim.DDSIMProvider().get_backend("qasm_simulator")
+    def simulate(self, qc: QuantumCircuit) -> str:
+        backend = DDSIMProvider().get_backend("qasm_simulator")
         job = execute(qc, backend, shots=1000)
         count = job.result().get_counts()
 
-        return count.most_frequent()
+        return cast(str, count.most_frequent())
 
-    def get_classical_result(self):
+    def get_classical_result(self) -> list[int]:
         distance_matrix = np.array(
             [
                 [0, self.dist_1_2, self.dist_1_3, self.dist_1_4],
                 [self.dist_1_2, 0, self.dist_2_3, self.dist_2_4],
                 [self.dist_1_3, self.dist_2_3, 0, self.dist_3_4],
                 [self.dist_1_4, self.dist_1_3, self.dist_3_4, 0],
             ]
         )
         permutation, distance = solve_tsp_dynamic_programming(distance_matrix)
 
-        return (np.array(permutation) + 1).T
+        return cast(list[int], (np.array(permutation) + 1).T)
 
     def controlled_unitary(
-        self, qc: QuantumCircuit, qubits: list[QuantumRegister], phases: list[int]
-    ):  # x,y,z = Specific Qubit; a,b,c,d = Phases
+        self, qc: QuantumCircuit, qubits: list[QuantumRegister], phases: list[float]
+    ) -> None:  # x,y,z = Specific Qubit; a,b,c,d = Phases
         qc.cp(phases[2] - phases[0], qubits[0], qubits[1])  # controlled-U1(c-a)
         qc.p(phases[0], qubits[0])  # U1(a)
         qc.cp(phases[1] - phases[0], qubits[0], qubits[2])  # controlled-U1(b-a)
 
         # controlled controlled U1(d-c+a-b)
         qc.cp((phases[3] - phases[2] + phases[0] - phases[1]) / 2, qubits[1], qubits[2])
         qc.cx(qubits[0], qubits[1])
-        qc.cp(
-            -(phases[3] - phases[2] + phases[0] - phases[1]) / 2, qubits[1], qubits[2]
-        )
+        qc.cp(-(phases[3] - phases[2] + phases[0] - phases[1]) / 2, qubits[1], qubits[2])
         qc.cx(qubits[0], qubits[1])
         qc.cp((phases[3] - phases[2] + phases[0] - phases[1]) / 2, qubits[0], qubits[2])
 
         # Alternative formulation
         # from qiskit.extensions import UnitaryGate
         #
         # matrix = [
@@ -298,80 +263,76 @@
         # qc.append(gate, qubits)
 
     def U(
         self,
         qc: QuantumCircuit,
         control_qreg: QuantumRegister,
         eigenstate_register: QuantumRegister,
-    ):
-
+    ) -> None:
         phases = self.get_all_phases()
         # a,b,c = phases for U1; d,e,f = phases for U2; g,h,i = phases for U3; j,k,l = phases for U4;
-        self.controlled_unitary(
-            qc, [control_qreg[0]] + eigenstate_register[0:2], [0] + phases[0:3]
-        )
+
+        self.controlled_unitary(qc, [control_qreg[0]] + eigenstate_register[0:2], [0.0] + phases[0:3])
+
         self.controlled_unitary(
             qc,
             [control_qreg[0]] + eigenstate_register[2:4],
             [phases[3]] + [0] + phases[4:6],
         )
         self.controlled_unitary(
             qc,
             [control_qreg[0]] + eigenstate_register[4:6],
             phases[6:8] + [0] + [phases[8]],
         )
-        self.controlled_unitary(
-            qc, [control_qreg[0]] + eigenstate_register[6:8], phases[9:12] + [0]
-        )
+        self.controlled_unitary(qc, [control_qreg[0]] + eigenstate_register[6:8], phases[9:12] + [0])
 
-    def final_U(self, times: int, eigenstate_register: QuantumRegister):
+    def final_U(self, times: int, eigenstate_register: QuantumRegister) -> Gate:
         control_qreg = QuantumRegister(1, "control")
         qc = QuantumCircuit(control_qreg, eigenstate_register)
         for _ in range(2**times):
             self.U(qc, control_qreg, eigenstate_register)
-        return qc.to_gate(label="U" + "_" + (str(2**times)))
+        return qc.to_gate(label="U_" + (str(2**times)))
 
     def encode_eigenstate(
         self,
         qc: QuantumCircuit,
         eigen_register: QuantumRegister,
         eigenstate: QuantumRegister,
-    ):
+    ) -> QuantumCircuit:
         for i in range(0, len(eigen_register)):
             if eigenstate[i] == "1":
                 qc.x(eigen_register[i])
             if eigenstate[i] == "0":
                 pass
         qc.barrier()
         return qc
 
-    def int_to_phase(self, distance: int):
-        phase = distance / self.distances_sum * 2 * np.pi
-        return phase
+    def int_to_phase(self, distance: int) -> float:
+        return distance / self.distances_sum * 2 * np.pi
 
-    def phase_to_int(self, phase: float):
+    def phase_to_float(self, phase: float) -> float:
         return phase * self.distances_sum
 
-    def eigenvalue_to_route(self, eigenvalue: str):
+    def eigenvalue_to_route(self, eigenvalue: str) -> list[int]:
         a = int(eigenvalue[0:2], 2) + 1
         b = int(eigenvalue[2:4], 2) + 1
         c = int(eigenvalue[4:6], 2) + 1
         d = int(eigenvalue[6:8], 2) + 1
         return [a, b, c, d]
 
-    def extract_selected_graph(self, solution: list[int]):
+    def extract_selected_graph(self, solution: list[int]) -> nx.Graph:
         G = nx.Graph()
         for i in range(len(solution)):
             if i == len(solution) - 1:
                 G.add_edge(solution[i], solution[0], color="r", weight=2)
             else:
                 G.add_edge(solution[i], solution[i + 1], color="r", weight=2)
 
         return G
 
-    def get_available_quantum_algorithms(self):
+    def get_available_quantum_algorithms(self) -> list[str]:
         """Method to get all available quantum algorithms in a list."""
         return ["QPE"]
 
-    def show_classical_solution(self):
+    def show_classical_solution(self) -> None:
         """Method to visualize the solution of a classical solver."""
-        self.print(solution=self.get_classical_result())
+        self.print_problem(solution=self.get_classical_result())
```

### Comparing `mqt.problemsolver-0.1.0/tests/test_csp.py` & `mqt.problemsolver-0.2.0/tests/test_csp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from mqt.problemsolver.csp import CSP
 
 
-def test_csp():
+def test_csp() -> None:
     csp = CSP()
     sum_s0 = 1
     sum_s1 = 3
     sum_s2 = 3
     sum_s3 = 1
-    list_of_constraints = csp.get_kakuro_constraints(
-        sum_s0=sum_s0, sum_s1=sum_s1, sum_s2=sum_s2, sum_s3=sum_s3
-    )
+    list_of_constraints = csp.get_kakuro_constraints(sum_s0=sum_s0, sum_s1=sum_s1, sum_s2=sum_s2, sum_s3=sum_s3)
     res = csp.solve(constraints=list_of_constraints, quantum_algorithm="Grover")
     assert res == (0, 3, 1, 0)
 
     sum_s0 = 3
     sum_s1 = 5
     sum_s2 = 3
     sum_s3 = 5
-    list_of_constraints = csp.get_kakuro_constraints(
-        sum_s0=sum_s0, sum_s1=sum_s1, sum_s2=sum_s2, sum_s3=sum_s3
-    )
+    list_of_constraints = csp.get_kakuro_constraints(sum_s0=sum_s0, sum_s1=sum_s1, sum_s2=sum_s2, sum_s3=sum_s3)
     res = csp.solve(constraints=list_of_constraints, quantum_algorithm="Grover")
     assert res == (0, 3, 3, 2)
```

