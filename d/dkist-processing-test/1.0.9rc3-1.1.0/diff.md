# Comparing `tmp/dkist-processing-test-1.0.9rc3.tar.gz` & `tmp/dkist-processing-test-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-test-1.0.9rc3.tar", last modified: Mon Jan 30 22:30:23 2023, max compression
+gzip compressed data, was "dkist-processing-test-1.1.0.tar", last modified: Fri May  5 18:03:20 2023, max compression
```

## Comparing `dkist-processing-test-1.0.9rc3.tar` & `dkist-processing-test-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/parameters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fail.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fake_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/movie.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    13504 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4418 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/common_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/end_to_end.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/noop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.289480 dkist-processing-test-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-05-05 18:03:20.289480 dkist-processing-test-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.285480 dkist-processing-test-1.1.0/dkist_processing_test/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.285480 dkist-processing-test-1.1.0/dkist_processing_test/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/models/parameters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.285480 dkist-processing-test-1.1.0/dkist_processing_test/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/fake_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/movie.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.285480 dkist-processing-test-1.1.0/dkist_processing_test/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    13624 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.289480 dkist-processing-test-1.1.0/dkist_processing_test/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4418 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/common_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/end_to_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/dkist_processing_test/workflows/noop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:03:20.285480 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-05-05 18:03:20.000000 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-05 18:03:20.000000 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 18:03:20.000000 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-05 18:03:20.000000 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 18:03:20.000000 dkist-processing-test-1.1.0/dkist_processing_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-05 18:03:20.289480 dkist-processing-test-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-05 18:03:12.000000 dkist-processing-test-1.1.0/setup.py
```

### Comparing `dkist-processing-test-1.0.9rc3/.gitignore` & `dkist-processing-test-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/.pre-commit-config.yaml` & `dkist-processing-test-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/PKG-INFO` & `dkist-processing-test-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.0.9rc3
+Version: 1.1.0
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.0.9rc3/README.rst` & `dkist-processing-test-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/bitbucket-pipelines.yml` & `dkist-processing-test-1.1.0/bitbucket-pipelines.yml`

 * *Files 11% similar despite different names*

```diff
@@ -30,25 +30,23 @@
           - $SNYK_CLI_COMMAND
     - step: &test
         caches:
           - pip
         name: Test
         script:
           - pip install .[test]
-          - pip install -U dkist-processing-core
           - pytest -v -n auto -m "not development" --cov dkist_processing_test
         services:
           - redis
     - step: &push_workflow
         caches:
           - pip
         name: Push Workflow
         script:
           - pip install .
-          - pip install -U dkist-processing-core
           - export BUILD_VERSION="${BITBUCKET_TAG:1}"
           - export ARTIFACT_FOLDER="${BITBUCKET_REPO_SLUG}_${BUILD_VERSION}/"
           - python -c "from dkist_processing_core.build_utils import export; import dkist_processing_test.workflows as workflow_package; export(workflow_package, '${ARTIFACT_FOLDER}')"
           - export SOURCE_PATH="workflow_${BUILD_VERSION}.gz"
           - tar --exclude="bitbucket-pipelines.yml" -cvzf ${SOURCE_PATH} ${ARTIFACT_FOLDER}
           - export TARGET_PATH="generic-packages/dkist-processing-test/${BUILD_VERSION}/"
           - curl -fL https://getcli.jfrog.io | sh
```

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/models/parameters.py` & `dkist-processing-test-1.1.0/dkist_processing_test/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/exercise_numba.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tasks/exercise_numba.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fake_science.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tasks/fake_science.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/movie.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tasks/movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/parse.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/conftest.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_parameters.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_tasks.py` & `dkist-processing-test-1.1.0/dkist_processing_test/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     VARIANCE_CADENCE: float = 0.0
     STOKES_PARAMS: tuple[str] = (
         "I",
         "Q",
         "U",
         "V",
     )  # A tuple because lists aren't allowed on dataclasses
+    CONTRIBUTING_PROPOSAL_IDS: tuple[str] = ("abc", "def")
+    CONTRIBUTING_EXPERIMENT_IDS: tuple[str] = ("ghi", "jkl")
 
 
 @pytest.fixture()
 def noop_task():
     return NoOpTask(recipe_run_id=1, workflow_name="noop", workflow_version="VX.Y")
```

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/common_tasks.py` & `dkist-processing-test-1.1.0/dkist_processing_test/workflows/common_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/end_to_end.py` & `dkist-processing-test-1.1.0/dkist_processing_test/workflows/end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/noop.py` & `dkist-processing-test-1.1.0/dkist_processing_test/workflows/noop.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/PKG-INFO` & `dkist-processing-test-1.1.0/dkist_processing_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.0.9rc3
+Version: 1.1.0
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/SOURCES.txt` & `dkist-processing-test-1.1.0/dkist_processing_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc3/setup.cfg` & `dkist-processing-test-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.1.0rc2
-	dkist-header-validator == 3.0.3
-	dkist-fits-specifications == 3.0.0
+	dkist-processing-common == 2.6.0
+	dkist-header-validator == 3.0.5
+	dkist-fits-specifications == 3.6.0
 	numba == 0.56.0
 	astropy == 5.1.1
 	numpy == 1.22.4
+	dkist-spectral-lines == 1.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-xdist
 	pytest-cov
 	pytest-mock
```

