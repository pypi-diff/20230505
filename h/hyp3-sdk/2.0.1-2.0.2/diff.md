# Comparing `tmp/hyp3_sdk-2.0.1.tar.gz` & `tmp/hyp3_sdk-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyp3_sdk-2.0.1.tar", last modified: Fri Mar 24 17:17:40 2023, max compression
+gzip compressed data, was "hyp3_sdk-2.0.2.tar", last modified: Fri May  5 19:13:18 2023, max compression
```

## Comparing `hyp3_sdk-2.0.1.tar` & `hyp3_sdk-2.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.483091 hyp3_sdk-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.475091 hyp3_sdk-2.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.475091 hyp3_sdk-2.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.479091 hyp3_sdk-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/distribute.yml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/labeled-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/notify-downstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/release-template-comment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/tag-version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.gitleaks.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/.trufflehog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-03-24 17:17:40.483091 hyp3_sdk-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.479091 hyp3_sdk-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/docs/sdk_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 17:17:40.483091 hyp3_sdk-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.475091 hyp3_sdk-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.479091 hyp3_sdk-2.0.1/src/hyp3_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/src/hyp3_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/src/hyp3_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/src/hyp3_sdk/hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/src/hyp3_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/src/hyp3_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.479091 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 17:17:40.000000 hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.483091 hyp3_sdk-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:17:40.483091 hyp3_sdk-2.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/data/product.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/test_hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-03-24 17:16:29.000000 hyp3_sdk-2.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.378377 hyp3_sdk-2.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.378377 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/distribute.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/labeled-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/notify-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/release-template-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/tag-version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.trufflehog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/docs/sdk_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.374376 hyp3_sdk-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/src/hyp3_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/data/product.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_util.py
```

### Comparing `hyp3_sdk-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/.github/workflows/distribute.yml` & `hyp3_sdk-2.0.2/.github/workflows/distribute.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
       - name: Build distribution
         id: build
         run: |
           python -m build
 
       - name: upload to PyPI.org
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.TOOLS_PYPI_PAK }}
 
   verify-distribution:
     runs-on: ubuntu-latest
     needs:
```

### Comparing `hyp3_sdk-2.0.1/.github/workflows/notify-downstream.yml` & `hyp3_sdk-2.0.2/.github/workflows/notify-downstream.yml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/.gitignore` & `hyp3_sdk-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/.gitleaks.toml` & `hyp3_sdk-2.0.2/.gitleaks.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/CHANGELOG.md` & `hyp3_sdk-2.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/) 
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [2.0.2]
+### Added
+* 20 m can now be provided to the `resolution` keyword argument of `hyp3.submit_rtc_job` and `hyp3.prepare_rtc_job`.
+
 ## [2.0.1]
 ### Fixed
 * Display the improved error messages regardless of whether the Earthdata credentials were provided by a `.netrc` file.
 
 ## [2.0.0]
 ### Changed
-* Improved error messages when Earthdata user must select Study Area or accept EULA.
+* Improved error messages when Earthdata user must select Study Area or accept EULA, thanks to @kevinxmorales in #170 
 ### Removed
 * The `hyp3_sdk.TESTING` constant has been removed in favor of mocking objects in unit tests.
 
 ## [1.7.5]
 ### Fixed
 * Path to `README.md` in `pyproject.toml` so that there is a package description on PyPI
```

### Comparing `hyp3_sdk-2.0.1/CODE_OF_CONDUCT.md` & `hyp3_sdk-2.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/LICENSE` & `hyp3_sdk-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/PKG-INFO` & `hyp3_sdk-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3_sdk
-Version: 2.0.1
+Version: 2.0.2
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.0.1/README.md` & `hyp3_sdk-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/docs/sdk_example.ipynb` & `hyp3_sdk-2.0.2/docs/sdk_example.ipynb`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/pyproject.toml` & `hyp3_sdk-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk/exceptions.py` & `hyp3_sdk-2.0.2/src/hyp3_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk/hyp3.py` & `hyp3_sdk-2.0.2/src/hyp3_sdk/hyp3.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                        name: Optional[str] = None,
                        dem_matching: bool = False,
                        include_dem: bool = False,
                        include_inc_map: bool = False,
                        include_rgb: bool = False,
                        include_scattering_area: bool = False,
                        radiometry: Literal['sigma0', 'gamma0'] = 'gamma0',
-                       resolution: Literal[10, 30] = 30,
+                       resolution: Literal[10, 20, 30] = 30,
                        scale: Literal['amplitude', 'decibel', 'power'] = 'power',
                        speckle_filter: bool = False,
                        dem_name: Literal['copernicus', 'legacy'] = 'copernicus') -> Batch:
         """Submit an RTC job
 
         Args:
             granule: The granule (scene) to use
@@ -272,15 +272,15 @@
                         name: Optional[str] = None,
                         dem_matching: bool = False,
                         include_dem: bool = False,
                         include_inc_map: bool = False,
                         include_rgb: bool = False,
                         include_scattering_area: bool = False,
                         radiometry: Literal['sigma0', 'gamma0'] = 'gamma0',
-                        resolution: Literal[10, 30] = 30,
+                        resolution: Literal[10, 20, 30] = 30,
                         scale: Literal['amplitude', 'decibel', 'power'] = 'power',
                         speckle_filter: bool = False,
                         dem_name: Literal['copernicus', 'legacy'] = 'copernicus') -> dict:
         """Submit an RTC job
 
         Args:
             granule: The granule (scene) to use
```

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk/jobs.py` & `hyp3_sdk-2.0.2/src/hyp3_sdk/jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk/util.py` & `hyp3_sdk-2.0.2/src/hyp3_sdk/util.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/PKG-INFO` & `hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3-sdk
-Version: 2.0.1
+Version: 2.0.2
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.0.1/src/hyp3_sdk.egg-info/SOURCES.txt` & `hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/conftest.py` & `hyp3_sdk-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/data/product.zip` & `hyp3_sdk-2.0.2/tests/data/product.zip`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/test_exceptions.py` & `hyp3_sdk-2.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/test_hyp3.py` & `hyp3_sdk-2.0.2/tests/test_hyp3.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/test_jobs.py` & `hyp3_sdk-2.0.2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.1/tests/test_util.py` & `hyp3_sdk-2.0.2/tests/test_util.py`

 * *Files identical despite different names*

