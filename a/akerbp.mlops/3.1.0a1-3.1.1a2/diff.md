# Comparing `tmp/akerbp.mlops-3.1.0a1.tar.gz` & `tmp/akerbp.mlops-3.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-i_v3y1yw/akerbp.mlops-3.1.0a1.tar", last modified: Thu May  4 10:05:29 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-wj2c27py/akerbp.mlops-3.1.1a2.tar", last modified: Fri May  5 11:55:24 2023, max compression
```

## Comparing `akerbp.mlops-3.1.0a1.tar` & `akerbp.mlops-3.1.1a2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.013018 akerbp.mlops-3.1.0a1/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-04 10:05:29.013018 akerbp.mlops-3.1.0a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35941 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/install.sh
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.001018 akerbp.mlops-3.1.0a1/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/model_artifact/dummy.joblib
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.005018 akerbp.mlops-3.1.0a1/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-04 10:05:29.013018 akerbp.mlops-3.1.0a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:28.997018 akerbp.mlops-3.1.0a1/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:28.997018 akerbp.mlops-3.1.0a1/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.005018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.005018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38633 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.009018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16951 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.009018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21689 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.009018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22521 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.009018 akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7150 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3160 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.005018 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-04 10:05:28.000000 akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.013018 akerbp.mlops-3.1.0a1/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 10:05:29.013018 akerbp.mlops-3.1.0a1/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3549 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/test/test_version_increment.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-04 10:05:02.000000 akerbp.mlops-3.1.0a1/upload_dummy_artifacts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.527777 akerbp.mlops-3.1.1a2/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-05 11:55:24.527777 akerbp.mlops-3.1.1a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35941 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.507777 akerbp.mlops-3.1.1a2/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/model_artifact/dummy.joblib
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.507777 akerbp.mlops-3.1.1a2/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-05 11:55:24.527777 akerbp.mlops-3.1.1a2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.495777 akerbp.mlops-3.1.1a2/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.499777 akerbp.mlops-3.1.1a2/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.511777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.511777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38633 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.515777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16951 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.519777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6555 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21689 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.519777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22521 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.519777 akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8283 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3160 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.511777 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-05 11:55:24.000000 akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.523777 akerbp.mlops-3.1.1a2/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 11:55:24.523777 akerbp.mlops-3.1.1a2/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3549 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/test/test_version_increment.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-05 11:54:56.000000 akerbp.mlops-3.1.1a2/upload_dummy_artifacts.py
```

### Comparing `akerbp.mlops-3.1.0a1/.flake8` & `akerbp.mlops-3.1.1a2/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/.pre-commit-config.yaml` & `akerbp.mlops-3.1.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/LICENSE` & `akerbp.mlops-3.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/PKG-INFO` & `akerbp.mlops-3.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.0a1
+Version: 3.1.1a2
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.1.0a1/README.md` & `akerbp.mlops-3.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/bitbucket-pipelines.yml` & `akerbp.mlops-3.1.1a2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/build.sh` & `akerbp.mlops-3.1.1a2/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/increment_package_version.py` & `akerbp.mlops-3.1.1a2/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/mlops_settings.yaml` & `akerbp.mlops-3.1.1a2/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/model_artifact/dummy.joblib` & `akerbp.mlops-3.1.1a2/model_artifact/dummy.joblib`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/model_code/model.py` & `akerbp.mlops-3.1.1a2/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/model_code/test_model.py` & `akerbp.mlops-3.1.1a2/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/pyproject.toml` & `akerbp.mlops-3.1.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/prediction.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,52 +107,78 @@
                 public_key = data.get("public_key", None)
                 content = str(json.dumps(y))
                 data_encrypted = False
                 if public_key is None:
                     logger.warning(
                         "Public key is not provided. The predictions will not be encrypted. This is not recommended!"
                     )
+                    encrypted_content = None
+                    encrypted_key = None
                 else:
-                    from cryptography.hazmat.primitives import hashes
-                    from cryptography.hazmat.primitives.asymmetric import padding
+                    import os
+
+                    from cryptography.hazmat.primitives import hashes, padding
+                    from cryptography.hazmat.primitives.asymmetric import (
+                        padding as asym_padding,
+                    )
+                    from cryptography.hazmat.primitives.ciphers import (
+                        Cipher,
+                        algorithms,
+                        modes,
+                    )
                     from cryptography.hazmat.primitives.serialization import (
                         load_pem_public_key,
                     )
 
+                    # Encrypt content with AES
+                    key = os.urandom(32)
+                    iv = b"1234567890123456"
+                    algo = algorithms.AES(key)
+                    encryptor = Cipher(algo, modes.CBC(iv)).encryptor()
+                    padder = padding.PKCS7(algo.block_size).padder()
+                    padded_data = padder.update(content.encode()) + padder.finalize()
+                    encrypted_content = (
+                        encryptor.update(padded_data) + encryptor.finalize()
+                    )
+
+                    # Encrypt key with RSA public key
                     public_key = load_pem_public_key(
                         public_key.encode(),
                     )
-                    content = public_key.encrypt(
-                        str.encode(content),
-                        padding.OAEP(
-                            mgf=padding.MGF1(algorithm=hashes.SHA256()),
+                    encrypted_key = public_key.encrypt(
+                        key,
+                        asym_padding.OAEP(
+                            mgf=asym_padding.MGF1(algorithm=hashes.SHA256()),
                             algorithm=hashes.SHA256(),
                             label=None,
                         ),
                     )
                     data_encrypted = True
                 cdf_client = mlops_helpers.global_client["write"]
                 id = uuid.uuid4().hex
                 external_file_id = f"{c.model_name}_predictions_{id}.binary"
                 try:
                     cdf_client.files.delete(external_id=external_file_id)
                 except CogniteNotFoundError:
                     pass
                 cdf_client.files.upload_bytes(
-                    content=content,
+                    content=encrypted_content
+                    if encrypted_content is not None
+                    else content,
                     name=f"{c.model_name}_predictions_{id}",
                     external_id=external_file_id,
                 )
                 logger.info(f"Prediction file uploaded to {external_file_id}")
                 return dict(
                     status="ok",
                     prediction={},
                     prediction_file=external_file_id,
                     model_id=c.model_id,
                     data_encrypted=data_encrypted,
+                    encrypted_key=encrypted_key,
                 )
             elif platform == "gc":
                 raise NotImplementedError
             else:
                 raise ValueError(f"Platform {platform} is not supported")
         else:
             logger.info("Writing predictions to the response")
```

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.1.1a2/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.0a1
+Version: 3.1.1a2
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.1.0a1/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.1.1a2/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_data_validation.py` & `akerbp.mlops-3.1.1a2/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_install_requirements.py` & `akerbp.mlops-3.1.1a2/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_metadata_validation.py` & `akerbp.mlops-3.1.1a2/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.1.1a2/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.0a1/test/test_version_increment.py` & `akerbp.mlops-3.1.1a2/test/test_version_increment.py`

 * *Files identical despite different names*

