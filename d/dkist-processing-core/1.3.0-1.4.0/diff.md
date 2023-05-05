# Comparing `tmp/dkist-processing-core-1.3.0.tar.gz` & `tmp/dkist-processing-core-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-core-1.3.0.tar", last modified: Fri Feb 17 17:56:35 2023, max compression
+gzip compressed data, was "dkist-processing-core-1.4.0.tar", last modified: Fri May  5 16:05:51 2023, max compression
```

## Comparing `dkist-processing-core-1.3.0.tar` & `dkist-processing-core-1.4.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     3071 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6922 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.388428 dkist-processing-core-1.3.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      436 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.388428 dkist-processing-core-1.3.0/dkist_processing_core/
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     4093 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2992 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9936 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/task.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/dkist_processing_core/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/dkist_processing_core/tests/invalid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/invalid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/invalid_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/task_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_export.py
--rw-rw-rw-   0 root         (0) root         (0)     4041 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/test_workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/dkist_processing_core/tests/valid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/valid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/valid_workflow_package/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/dkist_processing_core/tests/zero_node_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     8722 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/dkist_processing_core/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.388428 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-02-17 17:56:35.000000 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-02-17 17:56:35.000000 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-17 17:56:35.000000 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-02-17 17:56:35.000000 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-02-17 17:56:35.000000 dkist-processing-core-1.3.0/dkist_processing_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    85295 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/auto-proc-concept-model.png
--rw-rw-rw-   0 root         (0) root         (0)    26060 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/auto_proc_brick.png
--rw-rw-rw-   0 root         (0) root         (0)   267222 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/automated-processing-deployed.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1294 2023-02-17 17:56:35.392428 dkist-processing-core-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-02-17 17:56:28.000000 dkist-processing-core-1.3.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7533 2023-05-05 16:05:51.926256 dkist-processing-core-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6922 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.918255 dkist-processing-core-1.4.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/changelog/17.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/changelog/18.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      436 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.918255 dkist-processing-core-1.4.0/dkist_processing_core/
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9936 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/task.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/dkist_processing_core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/dkist_processing_core/tests/invalid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/invalid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/invalid_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/task_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     4041 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/test_workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/dkist_processing_core/tests/valid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/valid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/valid_workflow_package/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/dkist_processing_core/tests/zero_node_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8722 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/dkist_processing_core/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.918255 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7533 2023-05-05 16:05:51.000000 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-05 16:05:51.000000 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 16:05:51.000000 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-05 16:05:51.000000 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 16:05:51.000000 dkist-processing-core-1.4.0/dkist_processing_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    85295 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/auto-proc-concept-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    26060 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/auto_proc_brick.png
+-rw-rw-rw-   0 root         (0) root         (0)   267222 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/automated-processing-deployed.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 16:05:51.922256 dkist-processing-core-1.4.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2023-05-05 16:05:51.926256 dkist-processing-core-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-05 16:05:45.000000 dkist-processing-core-1.4.0/setup.py
```

### Comparing `dkist-processing-core-1.3.0/.gitignore` & `dkist-processing-core-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/.pre-commit-config.yaml` & `dkist-processing-core-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/CHANGELOG.rst` & `dkist-processing-core-1.4.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v1.4.0 (2023-05-05)
+===================
+
+Misc
+----
+
+- Update pip before use (`#17 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/17>`__)
+- Move to airflow 2.6.0 (`#18 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/18>`__)
+
+
 v1.3.0 (2023-02-17)
 ===================
 
 Misc
 ----
 
 - Update Airflow to v2.5.1
```

### Comparing `dkist-processing-core-1.3.0/PKG-INFO` & `dkist-processing-core-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 1.3.0
+Version: 1.4.0
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-1.3.0/README.rst` & `dkist-processing-core-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/bitbucket-pipelines.yml` & `dkist-processing-core-1.4.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/_failure_callback.py` & `dkist-processing-core-1.4.0/dkist_processing_core/_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/_node.py` & `dkist-processing-core-1.4.0/dkist_processing_core/_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 echo NOMAD_GROUP_NAME
 echo $NOMAD_GROUP_NAME
 echo NOMAD_HOST_ADDR_worker
 echo $NOMAD_HOST_ADDR_worker
 echo NOMAD_ALLOC_NAME
 echo $NOMAD_ALLOC_NAME
 echo Host Python Environment i.e. system-site-packages
+python3 -m pip install --upgrade pip
 pip list
 echo Creating Virtual Environment
 python3 -m venv --system-site-packages .task_venv
 echo Activate Environment
 . .task_venv/bin/activate
 echo Python Interpreter Location
 which python
```

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/build_utils.py` & `dkist-processing-core-1.4.0/dkist_processing_core/build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/task.py` & `dkist-processing-core-1.4.0/dkist_processing_core/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/conftest.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/task_example.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/task_example.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_build_utils.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_export.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_failure_callback.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_node.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_task.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/test_workflow.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/tests/valid_workflow_package/workflow.py` & `dkist-processing-core-1.4.0/dkist_processing_core/tests/valid_workflow_package/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core/workflow.py` & `dkist-processing-core-1.4.0/dkist_processing_core/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core.egg-info/PKG-INFO` & `dkist-processing-core-1.4.0/dkist_processing_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 1.3.0
+Version: 1.4.0
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-1.3.0/dkist_processing_core.egg-info/SOURCES.txt` & `dkist-processing-core-1.4.0/dkist_processing_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/17.misc.rst
+changelog/18.misc.rst
 dkist_processing_core/__init__.py
 dkist_processing_core/_failure_callback.py
 dkist_processing_core/_node.py
 dkist_processing_core/build_utils.py
 dkist_processing_core/task.py
 dkist_processing_core/workflow.py
 dkist_processing_core.egg-info/PKG-INFO
```

### Comparing `dkist-processing-core-1.3.0/docs/Makefile` & `dkist-processing-core-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/docs/auto-proc-concept-model.png` & `dkist-processing-core-1.4.0/docs/auto-proc-concept-model.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/docs/auto_proc_brick.png` & `dkist-processing-core-1.4.0/docs/auto_proc_brick.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/docs/automated-processing-deployed.png` & `dkist-processing-core-1.4.0/docs/automated-processing-deployed.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/docs/conf.py` & `dkist-processing-core-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/docs/make.bat` & `dkist-processing-core-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/licenses/LICENSE.rst` & `dkist-processing-core-1.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/pyproject.toml` & `dkist-processing-core-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-1.3.0/setup.cfg` & `dkist-processing-core-1.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	apache-airflow[postgres, celery] == 2.5.1
+	apache-airflow[postgres, celery] == 2.6.0
 	elastic-apm < 7.0.0
 	requests >= 2.23
 	talus >= 0.2.0
 
 [options.extras_require]
 test = 
 	pytest
```

