# Comparing `tmp/dataquality-0.8.9.tar.gz` & `tmp/dataquality-0.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.8.9.tar", last modified: Thu Dec 15 23:41:39 2022, max compression
+gzip compressed data, was "dataquality-0.9.1a1.tar", last modified: Thu May  4 22:17:34 2023, max compression
```

## Comparing `dataquality-0.8.9.tar` & `dataquality-0.9.1a1.tar`

### file list

```diff
@@ -1,176 +1,237 @@
--rw-r--r--   0        0        0       99 2022-10-11 23:00:09.655956 dataquality-0.8.9/.coveragerc
--rw-r--r--   0        0        0      131 2022-10-11 23:00:09.656126 dataquality-0.8.9/.editorconfig
--rw-r--r--   0        0        0      181 2022-10-11 23:00:09.656277 dataquality-0.8.9/.flake8
--rw-r--r--   0        0        0       75 2022-10-11 23:00:09.656495 dataquality-0.8.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      924 2022-10-11 23:00:09.656756 dataquality-0.8.9/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      590 2022-10-11 23:00:09.656922 dataquality-0.8.9/.github/ISSUE_TEMPLATE/doc.md
--rw-r--r--   0        0        0      700 2022-10-11 23:00:09.657078 dataquality-0.8.9/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      542 2022-10-11 23:00:09.657221 dataquality-0.8.9/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1169 2022-10-11 23:00:09.657374 dataquality-0.8.9/.github/pull_request_template.md
--rw-r--r--   0        0        0      525 2022-10-11 23:00:09.657583 dataquality-0.8.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      740 2022-10-11 23:00:09.657729 dataquality-0.8.9/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2292 2022-12-09 01:34:41.687656 dataquality-0.8.9/.gitignore
--rw-r--r--   0        0        0        6 2022-10-11 23:00:09.658013 dataquality-0.8.9/.python-version
--rw-r--r--   0        0        0     8078 2022-10-11 23:00:09.658217 dataquality-0.8.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2022-10-11 23:00:09.658384 dataquality-0.8.9/LICENSE
--rw-r--r--   0        0        0      548 2022-10-11 23:00:09.658550 dataquality-0.8.9/README.md
--rw-r--r--   0        0        0     4485 2022-12-15 23:41:37.187563 dataquality-0.8.9/dataquality/__init__.py
--rw-r--r--   0        0        0     8443 2022-12-15 23:31:05.910410 dataquality-0.8.9/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    31697 2022-12-15 23:31:05.927629 dataquality-0.8.9/dataquality/clients/api.py
--rw-r--r--   0        0        0     4125 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/core/__init__.py
--rw-r--r--   0        0        0     8371 2022-12-15 23:31:06.069608 dataquality-0.8.9/dataquality/core/_config.py
--rw-r--r--   0        0        0     3104 2022-12-15 23:31:06.045893 dataquality-0.8.9/dataquality/core/auth.py
--rw-r--r--   0        0        0     6108 2022-12-15 23:31:06.082327 dataquality-0.8.9/dataquality/core/finish.py
--rw-r--r--   0        0        0     9768 2022-12-15 23:31:06.062587 dataquality-0.8.9/dataquality/core/init.py
--rw-r--r--   0        0        0    15137 2022-12-15 23:31:06.053808 dataquality-0.8.9/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2022-12-15 23:31:06.076104 dataquality-0.8.9/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2022-11-28 17:23:58.644880 dataquality-0.8.9/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0     9405 2022-12-15 23:31:06.393084 dataquality-0.8.9/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     4098 2022-12-15 23:31:06.333955 dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7262 2022-12-15 23:31:06.379759 dataquality-0.8.9/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     3768 2022-12-15 23:31:06.310402 dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     3070 2022-12-15 23:31:06.384090 dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    11287 2022-12-15 23:31:06.373912 dataquality-0.8.9/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0      293 2022-10-31 17:31:56.991517 dataquality-0.8.9/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0    15422 2022-12-15 23:31:06.300508 dataquality-0.8.9/dataquality/integrations/experimental/keras.py
--rw-r--r--   0        0        0     9603 2022-12-15 23:31:06.289374 dataquality-0.8.9/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     4418 2022-12-15 23:31:06.250210 dataquality-0.8.9/dataquality/integrations/keras.py
--rw-r--r--   0        0        0    25573 2022-12-15 23:31:06.275830 dataquality-0.8.9/dataquality/integrations/spacy.py
--rw-r--r--   0        0        0     5701 2022-12-15 23:31:06.281061 dataquality-0.8.9/dataquality/integrations/torch.py
--rw-r--r--   0        0        0     8344 2022-12-15 23:31:06.259439 dataquality-0.8.9/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0       95 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    10577 2022-12-15 23:31:05.945221 dataquality-0.8.9/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      357 2022-12-15 23:31:05.989196 dataquality-0.8.9/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    21618 2022-12-15 23:31:06.020215 dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0     1935 2022-12-15 23:31:05.986971 dataquality-0.8.9/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0    19532 2022-12-15 23:31:05.994896 dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    14796 2022-12-15 23:31:06.000577 dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31289 2022-12-15 23:31:06.009806 dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     1702 2022-12-15 23:31:06.039210 dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      260 2022-12-09 01:34:41.691356 dataquality-0.8.9/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      958 2022-12-15 23:31:06.029388 dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1510 2022-12-15 23:31:06.032713 dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1608 2022-12-15 23:31:06.036035 dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      362 2022-12-15 23:31:05.953592 dataquality-0.8.9/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     8218 2022-12-15 23:31:05.979653 dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     1015 2022-12-15 23:31:05.950221 dataquality-0.8.9/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     7838 2022-12-15 23:31:05.958149 dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9058 2022-12-15 23:31:05.963261 dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    33524 2022-12-15 23:31:05.972893 dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    27895 2022-12-15 23:31:05.890944 dataquality-0.8.9/dataquality/metrics.py
--rw-r--r--   0        0        0      165 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8363 2022-12-15 23:31:06.224815 dataquality-0.8.9/dataquality/schemas/condition.py
--rw-r--r--   0        0        0      570 2022-12-15 23:31:06.204166 dataquality-0.8.9/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4382 2022-12-15 23:31:06.220218 dataquality-0.8.9/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2022-11-28 17:23:58.658371 dataquality-0.8.9/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2022-12-15 23:31:06.206491 dataquality-0.8.9/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5254 2022-12-15 23:31:06.201016 dataquality-0.8.9/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      992 2022-12-15 23:31:06.228257 dataquality-0.8.9/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      617 2022-12-15 23:31:06.239527 dataquality-0.8.9/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1397 2022-12-15 23:31:06.209696 dataquality-0.8.9/dataquality/schemas/route.py
--rw-r--r--   0        0        0      928 2022-12-15 23:31:06.231109 dataquality-0.8.9/dataquality/schemas/split.py
--rw-r--r--   0        0        0      770 2022-12-15 23:31:06.234039 dataquality-0.8.9/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      244 2022-12-15 23:31:06.236970 dataquality-0.8.9/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      674 2022-11-02 20:22:30.684530 dataquality-0.8.9/dataquality/utils/ampli.py
--rw-r--r--   0        0        0      401 2022-12-15 23:31:06.089109 dataquality-0.8.9/dataquality/utils/auth.py
--rw-r--r--   0        0        0     5784 2022-12-15 23:31:06.193967 dataquality-0.8.9/dataquality/utils/auto.py
--rw-r--r--   0        0        0      865 2022-12-15 21:23:01.762336 dataquality-0.8.9/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0      154 2022-12-15 23:31:06.103700 dataquality-0.8.9/dataquality/utils/cloud.py
--rw-r--r--   0        0        0      651 2022-12-09 01:34:41.693535 dataquality-0.8.9/dataquality/utils/cv.py
--rw-r--r--   0        0        0     3381 2022-12-15 23:31:06.154205 dataquality-0.8.9/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0      129 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/file.py
--rw-r--r--   0        0        0     1672 2022-12-15 23:31:06.129311 dataquality-0.8.9/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     3039 2022-12-15 23:31:06.189283 dataquality-0.8.9/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     9962 2022-12-15 23:31:06.095391 dataquality-0.8.9/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2022-11-28 17:23:58.665769 dataquality-0.8.9/dataquality/utils/imports.py
--rw-r--r--   0        0        0     7977 2022-12-15 23:31:06.111254 dataquality-0.8.9/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2022-12-15 23:31:06.142227 dataquality-0.8.9/dataquality/utils/ml.py
--rw-r--r--   0        0        0    23873 2022-11-02 20:22:30.685786 dataquality-0.8.9/dataquality/utils/name.py
--rw-r--r--   0        0        0     5923 2022-12-15 23:31:06.177280 dataquality-0.8.9/dataquality/utils/profiler.py
--rw-r--r--   0        0        0     4070 2022-12-15 23:31:06.125979 dataquality-0.8.9/dataquality/utils/spacy_integration.py
--rw-r--r--   0        0        0      260 2022-11-28 17:23:58.668908 dataquality-0.8.9/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1912 2022-12-15 23:31:06.114129 dataquality-0.8.9/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0     9488 2022-12-15 23:31:06.185769 dataquality-0.8.9/dataquality/utils/torch.py
--rw-r--r--   0        0        0     2739 2022-12-15 23:31:06.106465 dataquality-0.8.9/dataquality/utils/transformers.py
--rw-r--r--   0        0        0     9149 2022-12-15 23:31:06.136612 dataquality-0.8.9/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1440 2022-11-02 20:22:30.688040 dataquality-0.8.9/dataquality/utils/version.py
--rw-r--r--   0        0        0    18832 2022-10-11 23:00:09.671318 dataquality-0.8.9/docs/Dataquality-Client-Demo.ipynb
--rw-r--r--   0        0        0    10352 2022-12-06 23:24:23.704737 dataquality-0.8.9/docs/End to End runs per task type.ipynb
--rw-r--r--   0        0        0    12031 2022-10-11 23:00:09.671739 dataquality-0.8.9/docs/Inference-Demo.ipynb
--rw-r--r--   0        0        0     6893 2022-10-11 23:00:09.671910 dataquality-0.8.9/docs/NER Inference.ipynb
--rw-r--r--   0        0        0      172 2022-12-09 01:34:41.694895 dataquality-0.8.9/docs/cv/README.md
--rw-r--r--   0        0        0     4245 2022-12-09 01:34:41.695431 dataquality-0.8.9/docs/cv/cv-demo-hf.py
--rw-r--r--   0        0        0     1893 2022-12-09 01:34:41.695867 dataquality-0.8.9/docs/cv/cv-testing-benchmark.py
--rw-r--r--   0        0        0      154 2022-10-11 23:00:09.672060 dataquality-0.8.9/docs/index.md
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672196 dataquality-0.8.9/mkdocs.yml
--rw-r--r--   0        0        0       66 2022-10-11 23:00:09.672321 dataquality-0.8.9/mypy.ini
--rw-r--r--   0        0        0     1571 2022-12-15 21:23:01.763974 dataquality-0.8.9/pyproject.toml
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672594 dataquality-0.8.9/pytest.ini
--rwxr-xr-x   0        0        0      247 2022-10-11 23:00:09.672835 dataquality-0.8.9/scripts/bump-version.sh
--rwxr-xr-x   0        0        0      100 2022-10-11 23:00:09.672960 dataquality-0.8.9/scripts/clean.sh
--rwxr-xr-x   0        0        0       60 2022-10-11 23:00:09.673077 dataquality-0.8.9/scripts/docs-build.sh
--rwxr-xr-x   0        0        0       55 2022-10-11 23:00:09.673199 dataquality-0.8.9/scripts/docs-serve.sh
--rwxr-xr-x   0        0        0      320 2022-10-11 23:00:09.673322 dataquality-0.8.9/scripts/format.sh
--rwxr-xr-x   0        0        0      106 2022-10-11 23:00:09.673446 dataquality-0.8.9/scripts/install.sh
--rwxr-xr-x   0        0        0      126 2022-10-11 23:00:09.673573 dataquality-0.8.9/scripts/lint.sh
--rwxr-xr-x   0        0        0       29 2022-10-11 23:00:09.673690 dataquality-0.8.9/scripts/publish.sh
--rwxr-xr-x   0        0        0       66 2022-10-11 23:00:09.673820 dataquality-0.8.9/scripts/set-local-env.sh
--rwxr-xr-x   0        0        0       56 2022-10-11 23:00:09.673948 dataquality-0.8.9/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      216 2022-10-11 23:00:09.674078 dataquality-0.8.9/scripts/test.sh
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.674219 dataquality-0.8.9/tests/__init__.py
--rw-r--r--   0        0        0     3479 2022-12-15 23:31:06.527876 dataquality-0.8.9/tests/auto/test_ner_auto.py
--rw-r--r--   0        0        0    16171 2022-12-15 23:31:06.523820 dataquality-0.8.9/tests/auto/test_tc_auto.py
--rw-r--r--   0        0        0    10549 2022-12-15 23:31:06.444129 dataquality-0.8.9/tests/clients/test_api.py
--rw-r--r--   0        0        0     5852 2022-12-15 23:31:06.418269 dataquality-0.8.9/tests/conftest.py
--rw-r--r--   0        0        0     1409 2022-12-15 23:31:06.481108 dataquality-0.8.9/tests/core/test_auth.py
--rw-r--r--   0        0        0      418 2022-11-02 20:22:30.689801 dataquality-0.8.9/tests/core/test_cloud.py
--rw-r--r--   0        0        0     6719 2022-12-15 23:31:06.497841 dataquality-0.8.9/tests/core/test_config.py
--rw-r--r--   0        0        0     6122 2022-12-15 23:31:06.492412 dataquality-0.8.9/tests/core/test_finish.py
--rw-r--r--   0        0        0    15940 2022-12-15 23:31:06.511453 dataquality-0.8.9/tests/core/test_init.py
--rw-r--r--   0        0        0     6907 2022-12-15 23:31:06.487171 dataquality-0.8.9/tests/core/test_report.py
--rw-r--r--   0        0        0       40 2022-10-11 23:00:09.674520 dataquality-0.8.9/tests/exceptions.py
--rw-r--r--   0        0        0     4990 2022-12-15 23:31:06.709420 dataquality-0.8.9/tests/inference/test_inference.py
--rw-r--r--   0        0        0     3234 2022-11-02 20:22:30.691277 dataquality-0.8.9/tests/inference/test_text_classification_inf.py
--rw-r--r--   0        0        0     3792 2022-11-02 20:22:30.691419 dataquality-0.8.9/tests/inference/test_text_ner_inf.py
--rw-r--r--   0        0        0     3862 2022-10-11 23:00:09.675468 dataquality-0.8.9/tests/integration/mock_training_run.py
--rw-r--r--   0        0        0     3954 2022-12-15 23:31:06.679834 dataquality-0.8.9/tests/integrations/hf/test_cv_hf.py
--rw-r--r--   0        0        0    10897 2022-12-15 23:31:06.673447 dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py
--rw-r--r--   0        0        0    10123 2022-12-15 23:31:06.662649 dataquality-0.8.9/tests/integrations/hf/test_text_classification_hf.py
--rw-r--r--   0        0        0     9263 2022-12-15 23:31:06.640380 dataquality-0.8.9/tests/integrations/keras/test_experimental.py
--rw-r--r--   0        0        0      514 2022-12-15 21:23:01.768632 dataquality-0.8.9/tests/integrations/keras/test_utils.py
--rw-r--r--   0        0        0     1346 2022-12-15 23:31:06.689001 dataquality-0.8.9/tests/integrations/spacy/conftest.py
--rw-r--r--   0        0        0      760 2022-11-02 20:22:30.692338 dataquality-0.8.9/tests/integrations/spacy/test_spacy_integration.py
--rw-r--r--   0        0        0    16355 2022-12-15 23:31:06.699854 dataquality-0.8.9/tests/integrations/spacy/test_spacy_ner.py
--rw-r--r--   0        0        0      904 2022-12-15 23:31:06.645632 dataquality-0.8.9/tests/integrations/torch/test_pt_utils.py
--rw-r--r--   0        0        0     7367 2022-12-15 23:31:06.653430 dataquality-0.8.9/tests/integrations/torch/test_text_classification_pt.py
--rw-r--r--   0        0        0    11728 2022-12-15 23:31:06.453921 dataquality-0.8.9/tests/loggers/test_multi_label.py
--rw-r--r--   0        0        0    23385 2022-12-15 23:31:06.475658 dataquality-0.8.9/tests/loggers/test_ner.py
--rw-r--r--   0        0        0    13108 2022-12-15 23:31:06.460897 dataquality-0.8.9/tests/loggers/test_text_classification.py
--rw-r--r--   0        0        0     7226 2022-12-15 23:31:06.622782 dataquality-0.8.9/tests/schemas/test_conditions.py
--rw-r--r--   0        0        0      402 2022-11-02 20:22:30.695867 dataquality-0.8.9/tests/schemas/test_metrics.py
--rw-r--r--   0        0        0    29166 2022-12-15 23:31:06.434729 dataquality-0.8.9/tests/test_dataquality.py
--rw-r--r--   0        0        0     1783 2022-11-28 17:23:58.686840 dataquality-0.8.9/tests/test_telemetrics.py
--rw-r--r--   0        0        0        0 2022-11-02 20:22:30.697603 dataquality-0.8.9/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     5900 2022-12-15 23:31:06.565806 dataquality-0.8.9/tests/test_utils/data_utils.py
--rw-r--r--   0        0        0     3808 2022-12-15 23:31:06.536970 dataquality-0.8.9/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0        0        0    11378 2022-11-02 20:22:30.698317 dataquality-0.8.9/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0        0        0     8122 2022-11-28 17:23:58.687297 dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0        0        0     3695 2022-11-02 20:22:30.698590 dataquality-0.8.9/tests/test_utils/lightning_model.py
--rw-r--r--   0        0        0     4908 2022-12-15 23:31:06.548195 dataquality-0.8.9/tests/test_utils/mock_request.py
--rw-r--r--   0        0        0     2840 2022-11-02 20:22:30.699379 dataquality-0.8.9/tests/test_utils/ner_constants.py
--rw-r--r--   0        0        0     4239 2022-12-15 23:31:06.553629 dataquality-0.8.9/tests/test_utils/spacy_integration.py
--rw-r--r--   0        0        0    22487 2022-12-06 23:24:23.709042 dataquality-0.8.9/tests/test_utils/spacy_integration_constants.py
--rw-r--r--   0        0        0    23021 2022-12-06 23:24:23.709498 dataquality-0.8.9/tests/test_utils/spacy_integration_constants_inference.py
--rw-r--r--   0        0        0     4614 2022-12-15 23:31:06.607721 dataquality-0.8.9/tests/utils/test_auto.py
--rw-r--r--   0        0        0     1623 2022-11-02 20:22:30.700412 dataquality-0.8.9/tests/utils/test_dq_logger.py
--rw-r--r--   0        0        0      224 2022-12-15 23:31:06.612161 dataquality-0.8.9/tests/utils/test_name.py
--rw-r--r--   0        0        0      288 2022-11-28 17:23:58.689269 dataquality-0.8.9/tests/utils/test_tf_version.py
--rw-r--r--   0        0        0      601 2022-11-02 20:22:30.701010 dataquality-0.8.9/tests/utils/test_vaex_utils.py
--rw-r--r--   0        0        0     1316 2022-12-15 23:31:06.599087 dataquality-0.8.9/tests/utils/test_version.py
--rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 dataquality-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-02-16 18:20:37.484786 dataquality-0.9.1a1/.coveragerc
+-rw-r--r--   0        0        0      131 2023-02-16 18:20:37.484963 dataquality-0.9.1a1/.editorconfig
+-rw-r--r--   0        0        0      179 2023-03-06 18:27:08.322809 dataquality-0.9.1a1/.flake8
+-rw-r--r--   0        0        0       19 2023-04-28 02:34:07.405536 dataquality-0.9.1a1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      924 2023-02-16 18:20:37.485592 dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      590 2023-02-16 18:20:37.485749 dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/doc.md
+-rw-r--r--   0        0        0      700 2023-02-16 18:20:37.485896 dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      542 2023-02-16 18:20:37.486033 dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1169 2023-02-16 18:20:37.486183 dataquality-0.9.1a1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      950 2023-04-14 09:39:59.465229 dataquality-0.9.1a1/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      525 2023-04-14 09:39:59.466024 dataquality-0.9.1a1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      890 2023-04-14 09:39:59.467112 dataquality-0.9.1a1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2418 2023-05-03 22:49:30.076353 dataquality-0.9.1a1/.gitignore
+-rw-r--r--   0        0        0        6 2023-02-16 18:20:37.487014 dataquality-0.9.1a1/.python-version
+-rw-r--r--   0        0        0     8078 2023-02-16 18:20:37.487229 dataquality-0.9.1a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2023-02-16 18:20:37.487400 dataquality-0.9.1a1/LICENSE
+-rw-r--r--   0        0        0     4437 2023-02-16 18:20:37.487564 dataquality-0.9.1a1/README.md
+-rw-r--r--   0        0        0     6012 2023-05-04 22:17:29.379223 dataquality-0.9.1a1/dataquality/__init__.py
+-rw-r--r--   0        0        0     8461 2023-05-04 02:23:06.506407 dataquality-0.9.1a1/dataquality/analytics.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.639242 dataquality-0.9.1a1/dataquality/clients/__init__.py
+-rw-r--r--   0        0        0    33867 2023-05-04 02:23:06.529362 dataquality-0.9.1a1/dataquality/clients/api.py
+-rw-r--r--   0        0        0     8187 2023-05-04 02:23:06.516492 dataquality-0.9.1a1/dataquality/clients/objectstore.py
+-rw-r--r--   0        0        0     1848 2023-04-07 07:52:09.644595 dataquality-0.9.1a1/dataquality/core/__init__.py
+-rw-r--r--   0        0        0     8843 2023-05-04 02:23:06.793133 dataquality-0.9.1a1/dataquality/core/_config.py
+-rw-r--r--   0        0        0     3104 2023-05-04 02:23:06.759652 dataquality-0.9.1a1/dataquality/core/auth.py
+-rw-r--r--   0        0        0     6499 2023-05-04 22:17:22.621387 dataquality-0.9.1a1/dataquality/core/finish.py
+-rw-r--r--   0        0        0     7026 2023-05-04 02:23:06.783167 dataquality-0.9.1a1/dataquality/core/init.py
+-rw-r--r--   0        0        0    21161 2023-05-04 02:23:06.771183 dataquality-0.9.1a1/dataquality/core/log.py
+-rw-r--r--   0        0        0     7039 2023-05-04 02:23:06.799371 dataquality-0.9.1a1/dataquality/core/report.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.650876 dataquality-0.9.1a1/dataquality/dq_auto/__init__.py
+-rw-r--r--   0        0        0    10175 2023-05-04 22:17:22.621980 dataquality-0.9.1a1/dataquality/dq_auto/auto.py
+-rw-r--r--   0        0        0     4158 2023-05-04 02:23:07.126817 dataquality-0.9.1a1/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0        0        0     7710 2023-05-04 22:10:32.335211 dataquality-0.9.1a1/dataquality/dq_auto/ner.py
+-rw-r--r--   0        0        0     4265 2023-05-04 02:23:07.123093 dataquality-0.9.1a1/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0        0        0     1594 2023-05-04 02:23:07.142858 dataquality-0.9.1a1/dataquality/dq_auto/notebook.py
+-rw-r--r--   0        0        0     3559 2023-05-04 02:23:07.146263 dataquality-0.9.1a1/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0        0        0    11797 2023-05-04 22:10:43.269244 dataquality-0.9.1a1/dataquality/dq_auto/text_classification.py
+-rw-r--r--   0        0        0    13139 2023-05-04 02:23:06.545657 dataquality-0.9.1a1/dataquality/dq_start/__init__.py
+-rw-r--r--   0        0        0     4498 2023-05-04 02:23:06.465858 dataquality-0.9.1a1/dataquality/dqyolo.py
+-rw-r--r--   0        0        0      293 2023-04-07 07:52:09.656391 dataquality-0.9.1a1/dataquality/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.656535 dataquality-0.9.1a1/dataquality/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079624 dataquality-0.9.1a1/dataquality/integrations/cv/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079930 dataquality-0.9.1a1/dataquality/integrations/cv/torch/__init__.py
+-rw-r--r--   0        0        0    20077 2023-05-04 22:17:22.622375 dataquality-0.9.1a1/dataquality/integrations/cv/torch/semantic_segmentation.py
+-rw-r--r--   0        0        0    15575 2023-05-04 02:23:07.110977 dataquality-0.9.1a1/dataquality/integrations/experimental/keras.py
+-rw-r--r--   0        0        0    14914 2023-05-04 02:23:07.045645 dataquality-0.9.1a1/dataquality/integrations/fastai.py
+-rw-r--r--   0        0        0    10024 2023-05-04 02:23:07.102392 dataquality-0.9.1a1/dataquality/integrations/hf.py
+-rw-r--r--   0        0        0     4375 2023-05-04 02:23:07.050094 dataquality-0.9.1a1/dataquality/integrations/keras.py
+-rw-r--r--   0        0        0    26831 2023-05-04 02:23:07.079437 dataquality-0.9.1a1/dataquality/integrations/spacy.py
+-rw-r--r--   0        0        0    12787 2023-05-04 02:23:07.084631 dataquality-0.9.1a1/dataquality/integrations/torch.py
+-rw-r--r--   0        0        0    12375 2023-05-04 22:06:55.080834 dataquality-0.9.1a1/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0        0        0    16907 2023-05-04 02:23:07.095450 dataquality-0.9.1a1/dataquality/integrations/ultralytics.py
+-rw-r--r--   0        0        0       95 2023-04-07 07:52:09.664245 dataquality-0.9.1a1/dataquality/loggers/__init__.py
+-rw-r--r--   0        0        0    13292 2023-05-04 02:23:06.570857 dataquality-0.9.1a1/dataquality/loggers/base_logger.py
+-rw-r--r--   0        0        0      517 2023-05-04 02:23:06.665914 dataquality-0.9.1a1/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0        0        0    26263 2023-05-04 22:17:22.623202 dataquality-0.9.1a1/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0        0        0    10393 2023-05-04 02:23:06.662586 dataquality-0.9.1a1/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0        0        0     9368 2023-05-04 02:23:06.719013 dataquality-0.9.1a1/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0        0        0     2768 2023-05-04 22:17:22.623829 dataquality-0.9.1a1/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0     9864 2023-05-04 02:23:06.651100 dataquality-0.9.1a1/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0        0        0    20661 2023-05-04 02:23:06.678041 dataquality-0.9.1a1/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0        0        0    14941 2023-05-04 02:23:06.687072 dataquality-0.9.1a1/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0        0        0    31885 2023-05-04 02:23:06.699619 dataquality-0.9.1a1/dataquality/loggers/data_logger/text_ner.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.669046 dataquality-0.9.1a1/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0        0        0     1910 2023-05-04 22:17:22.624592 dataquality-0.9.1a1/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0        0        0      473 2023-04-07 07:52:09.669969 dataquality-0.9.1a1/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0        0        0      537 2023-04-14 09:39:59.476862 dataquality-0.9.1a1/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0        0        0      226 2023-05-03 22:49:30.083124 dataquality-0.9.1a1/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0        0        0      398 2023-05-03 22:49:30.083397 dataquality-0.9.1a1/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0        0        0      958 2023-05-04 02:23:06.738772 dataquality-0.9.1a1/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0        0        0     1510 2023-05-04 02:23:06.741859 dataquality-0.9.1a1/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0        0        0     1608 2023-05-04 02:23:06.745185 dataquality-0.9.1a1/dataquality/loggers/logger_config/text_ner.py
+-rw-r--r--   0        0        0      420 2023-05-04 02:23:06.588494 dataquality-0.9.1a1/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0        0        0     7510 2023-05-04 02:23:06.637489 dataquality-0.9.1a1/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0        0        0     3309 2023-05-04 02:23:06.583977 dataquality-0.9.1a1/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0        0        0     8975 2023-05-04 02:23:06.627055 dataquality-0.9.1a1/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0        0        0     6463 2023-05-04 22:17:22.624998 dataquality-0.9.1a1/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0      519 2023-05-03 22:49:30.084436 dataquality-0.9.1a1/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0        0        0     7555 2023-05-04 02:23:06.598643 dataquality-0.9.1a1/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0        0        0     9120 2023-05-04 02:23:06.605413 dataquality-0.9.1a1/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0        0        0    32052 2023-05-04 02:23:06.616819 dataquality-0.9.1a1/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0        0        0    28673 2023-05-04 02:23:06.482946 dataquality-0.9.1a1/dataquality/metrics.py
+-rw-r--r--   0        0        0      165 2023-04-07 07:52:09.676633 dataquality-0.9.1a1/dataquality/schemas/__init__.py
+-rw-r--r--   0        0        0     8361 2023-05-04 02:23:07.012740 dataquality-0.9.1a1/dataquality/schemas/condition.py
+-rw-r--r--   0        0        0      569 2023-05-04 02:23:06.968028 dataquality-0.9.1a1/dataquality/schemas/dataframe.py
+-rw-r--r--   0        0        0     4382 2023-05-04 02:23:07.004539 dataquality-0.9.1a1/dataquality/schemas/edit.py
+-rw-r--r--   0        0        0      662 2023-04-07 07:52:09.677611 dataquality-0.9.1a1/dataquality/schemas/hf.py
+-rw-r--r--   0        0        0      118 2023-05-04 02:23:06.970328 dataquality-0.9.1a1/dataquality/schemas/job.py
+-rw-r--r--   0        0        0     5241 2023-05-04 02:23:06.964247 dataquality-0.9.1a1/dataquality/schemas/metrics.py
+-rw-r--r--   0        0        0      165 2023-05-04 02:23:07.006560 dataquality-0.9.1a1/dataquality/schemas/model.py
+-rw-r--r--   0        0        0      992 2023-05-04 02:23:07.015866 dataquality-0.9.1a1/dataquality/schemas/ner.py
+-rw-r--r--   0        0        0      617 2023-05-04 02:23:07.027724 dataquality-0.9.1a1/dataquality/schemas/report.py
+-rw-r--r--   0        0        0      287 2023-04-07 07:52:09.678943 dataquality-0.9.1a1/dataquality/schemas/request_type.py
+-rw-r--r--   0        0        0     1491 2023-05-04 02:23:06.973737 dataquality-0.9.1a1/dataquality/schemas/route.py
+-rw-r--r--   0        0        0     2550 2023-05-04 22:17:22.626499 dataquality-0.9.1a1/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0        0        0      992 2023-05-04 02:23:07.018585 dataquality-0.9.1a1/dataquality/schemas/split.py
+-rw-r--r--   0        0        0     1055 2023-05-04 02:23:07.021496 dataquality-0.9.1a1/dataquality/schemas/task_type.py
+-rw-r--r--   0        0        0      740 2023-05-04 22:17:22.627338 dataquality-0.9.1a1/dataquality/schemas/torch.py
+-rw-r--r--   0        0        0      222 2023-04-07 07:52:09.680124 dataquality-0.9.1a1/dataquality/utils/__init__.py
+-rw-r--r--   0        0        0      674 2023-04-07 07:52:09.680377 dataquality-0.9.1a1/dataquality/utils/ampli.py
+-rw-r--r--   0        0        0      401 2023-05-04 02:23:06.815569 dataquality-0.9.1a1/dataquality/utils/auth.py
+-rw-r--r--   0        0        0     6824 2023-05-04 02:23:06.955706 dataquality-0.9.1a1/dataquality/utils/auto.py
+-rw-r--r--   0        0        0      928 2023-05-04 21:34:44.817254 dataquality-0.9.1a1/dataquality/utils/auto_trainer.py
+-rw-r--r--   0        0        0      154 2023-05-04 02:23:06.840003 dataquality-0.9.1a1/dataquality/utils/cloud.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:03:51.060491 dataquality-0.9.1a1/dataquality/utils/cuda.py
+-rw-r--r--   0        0        0     2082 2023-05-04 02:23:06.900954 dataquality-0.9.1a1/dataquality/utils/cv.py
+-rw-r--r--   0        0        0     3369 2023-05-04 02:23:06.908329 dataquality-0.9.1a1/dataquality/utils/dq_logger.py
+-rw-r--r--   0        0        0     3514 2023-05-04 02:23:06.813427 dataquality-0.9.1a1/dataquality/utils/dqyolo.py
+-rw-r--r--   0        0        0     4548 2023-05-04 02:23:06.896679 dataquality-0.9.1a1/dataquality/utils/emb.py
+-rw-r--r--   0        0        0     3591 2023-05-04 02:23:06.888460 dataquality-0.9.1a1/dataquality/utils/file.py
+-rw-r--r--   0        0        0     5685 2023-05-04 02:23:06.870438 dataquality-0.9.1a1/dataquality/utils/hdf5_store.py
+-rw-r--r--   0        0        0     3362 2023-05-04 02:23:06.951619 dataquality-0.9.1a1/dataquality/utils/helpers.py
+-rw-r--r--   0        0        0     2163 2023-05-04 02:23:06.828834 dataquality-0.9.1a1/dataquality/utils/hf_images.py
+-rw-r--r--   0        0        0    10182 2023-05-04 02:23:06.821861 dataquality-0.9.1a1/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0        0        0      429 2023-04-07 07:52:09.684739 dataquality-0.9.1a1/dataquality/utils/imports.py
+-rw-r--r--   0        0        0     8023 2023-05-04 02:23:06.846683 dataquality-0.9.1a1/dataquality/utils/keras.py
+-rw-r--r--   0        0        0     2408 2023-05-04 02:23:06.884881 dataquality-0.9.1a1/dataquality/utils/ml.py
+-rw-r--r--   0        0        0    24708 2023-04-07 07:52:09.685790 dataquality-0.9.1a1/dataquality/utils/name.py
+-rw-r--r--   0        0        0     1184 2023-04-14 09:39:59.480342 dataquality-0.9.1a1/dataquality/utils/od.py
+-rw-r--r--   0        0        0     5923 2023-05-04 02:23:06.929368 dataquality-0.9.1a1/dataquality/utils/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.085612 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0        0        0     4148 2023-05-04 22:17:22.627633 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0        0        0    14942 2023-05-04 22:17:22.627930 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0        0        0     5479 2023-05-04 22:17:22.628295 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0        0        0     5243 2023-05-04 22:17:22.628632 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0        0        0     1914 2023-05-04 22:17:22.628890 dataquality-0.9.1a1/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0        0        0     4070 2023-05-04 02:23:06.861802 dataquality-0.9.1a1/dataquality/utils/spacy_integration.py
+-rw-r--r--   0        0        0      260 2023-04-07 07:52:09.688175 dataquality-0.9.1a1/dataquality/utils/tf.py
+-rw-r--r--   0        0        0     1987 2023-05-04 02:23:06.850275 dataquality-0.9.1a1/dataquality/utils/thread_pool.py
+-rw-r--r--   0        0        0    18173 2023-05-04 02:23:06.939291 dataquality-0.9.1a1/dataquality/utils/torch.py
+-rw-r--r--   0        0        0     2739 2023-05-04 02:23:06.842731 dataquality-0.9.1a1/dataquality/utils/transformers.py
+-rw-r--r--   0        0        0    11924 2023-05-04 02:23:06.947607 dataquality-0.9.1a1/dataquality/utils/ultralytics.py
+-rw-r--r--   0        0        0     5207 2023-05-04 02:23:06.837592 dataquality-0.9.1a1/dataquality/utils/upload.py
+-rw-r--r--   0        0        0     8781 2023-05-04 02:23:06.878484 dataquality-0.9.1a1/dataquality/utils/vaex.py
+-rw-r--r--   0        0        0     1087 2023-04-07 07:52:09.690283 dataquality-0.9.1a1/dataquality/utils/version.py
+-rw-r--r--   0        0        0      634 2023-03-06 18:27:08.340955 dataquality-0.9.1a1/docs/autodocs/Makefile
+-rw-r--r--   0        0        0      120 2023-03-06 18:27:08.341186 dataquality-0.9.1a1/docs/autodocs/Readme.md
+-rw-r--r--   0        0        0   312552 2023-03-06 18:27:08.344287 dataquality-0.9.1a1/docs/autodocs/_build/doctrees/api/dataquality.doctree
+-rw-r--r--   0        0        0    49162 2023-03-06 18:27:08.345328 dataquality-0.9.1a1/docs/autodocs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     2703 2023-03-06 18:27:08.345810 dataquality-0.9.1a1/docs/autodocs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0    33107 2023-04-10 07:35:51.793733 dataquality-0.9.1a1/docs/autodocs/_build/markdown/api/dataquality.md
+-rw-r--r--   0        0        0     3191 2023-03-06 18:27:08.348392 dataquality-0.9.1a1/docs/autodocs/_build/markdown/index.md
+-rw-r--r--   0        0        0     1485 2023-03-06 18:27:08.349296 dataquality-0.9.1a1/docs/autodocs/api/dataquality.rst
+-rw-r--r--   0        0        0     2537 2023-03-06 18:27:08.349828 dataquality-0.9.1a1/docs/autodocs/conf.py
+-rw-r--r--   0        0        0       86 2023-03-06 18:27:08.350033 dataquality-0.9.1a1/docs/autodocs/index.rst
+-rw-r--r--   0        0        0      765 2023-03-06 18:27:08.350253 dataquality-0.9.1a1/docs/autodocs/make.bat
+-rw-r--r--   0        0        0      165 2023-03-06 18:27:08.350468 dataquality-0.9.1a1/docs/autodocs/requirements.txt
+-rw-r--r--   0        0        0      172 2023-02-16 18:20:37.512360 dataquality-0.9.1a1/docs/cv/README.md
+-rw-r--r--   0        0        0   122204 2023-05-04 22:17:22.629812 dataquality-0.9.1a1/docs/cv/coco_deeplab_hooks.ipynb
+-rw-r--r--   0        0        0     4245 2023-02-16 18:20:37.512548 dataquality-0.9.1a1/docs/cv/cv-demo-hf.py
+-rw-r--r--   0        0        0     1893 2023-02-16 18:20:37.512698 dataquality-0.9.1a1/docs/cv/cv-testing-benchmark.py
+-rw-r--r--   0        0        0    18832 2023-03-06 18:27:08.351257 dataquality-0.9.1a1/docs/notebooks/Dataquality-Client-Demo.ipynb
+-rw-r--r--   0        0        0    10352 2023-03-06 18:27:08.352178 dataquality-0.9.1a1/docs/notebooks/End to End runs per task type.ipynb
+-rw-r--r--   0        0        0    12031 2023-03-06 18:27:08.352622 dataquality-0.9.1a1/docs/notebooks/Inference-Demo.ipynb
+-rw-r--r--   0        0        0     6893 2023-03-06 18:27:08.353238 dataquality-0.9.1a1/docs/notebooks/NER Inference.ipynb
+-rw-r--r--   0        0        0     6378 2023-05-03 22:49:30.086339 dataquality-0.9.1a1/docs/notebooks/Tabular-Data.ipynb
+-rw-r--r--   0        0        0      121 2023-05-04 21:27:09.407392 dataquality-0.9.1a1/mypy.ini
+-rw-r--r--   0        0        0     2361 2023-05-04 21:27:05.391041 dataquality-0.9.1a1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-02-16 18:20:37.515251 dataquality-0.9.1a1/pytest.ini
+-rwxr-xr-x   0        0        0      247 2023-02-16 18:20:37.515473 dataquality-0.9.1a1/scripts/bump-version.sh
+-rwxr-xr-x   0        0        0      100 2023-02-16 18:20:37.515600 dataquality-0.9.1a1/scripts/clean.sh
+-rwxr-xr-x   0        0        0       53 2023-03-06 18:27:08.354433 dataquality-0.9.1a1/scripts/docs-build.sh
+-rwxr-xr-x   0        0        0      311 2023-02-16 18:20:37.515862 dataquality-0.9.1a1/scripts/format.sh
+-rwxr-xr-x   0        0        0      100 2023-04-14 09:39:59.483561 dataquality-0.9.1a1/scripts/install.sh
+-rwxr-xr-x   0        0        0      126 2023-02-16 18:20:37.516123 dataquality-0.9.1a1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       29 2023-02-16 18:20:37.516245 dataquality-0.9.1a1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       66 2023-02-16 18:20:37.516369 dataquality-0.9.1a1/scripts/set-local-env.sh
+-rwxr-xr-x   0        0        0       56 2023-02-16 18:20:37.516487 dataquality-0.9.1a1/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      216 2023-04-10 07:35:51.794690 dataquality-0.9.1a1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-02-16 18:20:37.516882 dataquality-0.9.1a1/tests/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-03 22:49:30.086944 dataquality-0.9.1a1/tests/assets/constants.py
+-rw-r--r--   0        0        0     6688 2023-03-08 21:36:54.587556 dataquality-0.9.1a1/tests/assets/images/Abyssinian_83.jpg
+-rw-r--r--   0        0        0     1977 2023-03-08 21:36:54.588075 dataquality-0.9.1a1/tests/assets/images/pug_198.jpg
+-rw-r--r--   0        0        0     3477 2023-05-04 02:23:07.287309 dataquality-0.9.1a1/tests/auto/test_ner_auto.py
+-rw-r--r--   0        0        0    16171 2023-05-04 02:23:07.284129 dataquality-0.9.1a1/tests/auto/test_tc_auto.py
+-rw-r--r--   0        0        0    11188 2023-05-04 02:23:07.200376 dataquality-0.9.1a1/tests/clients/test_api.py
+-rw-r--r--   0        0        0     6206 2023-05-04 02:23:07.176590 dataquality-0.9.1a1/tests/conftest.py
+-rw-r--r--   0        0        0     1409 2023-05-04 02:23:07.251253 dataquality-0.9.1a1/tests/core/test_auth.py
+-rw-r--r--   0        0        0      418 2023-02-16 18:20:37.518225 dataquality-0.9.1a1/tests/core/test_cloud.py
+-rw-r--r--   0        0        0     6719 2023-05-04 02:23:07.263635 dataquality-0.9.1a1/tests/core/test_config.py
+-rw-r--r--   0        0        0     6122 2023-05-04 02:23:07.259460 dataquality-0.9.1a1/tests/core/test_finish.py
+-rw-r--r--   0        0        0    24970 2023-05-04 02:23:07.275502 dataquality-0.9.1a1/tests/core/test_init.py
+-rw-r--r--   0        0        0     6907 2023-05-04 02:23:07.255690 dataquality-0.9.1a1/tests/core/test_report.py
+-rw-r--r--   0        0        0       40 2023-02-16 18:20:37.519164 dataquality-0.9.1a1/tests/exceptions.py
+-rw-r--r--   0        0        0     4991 2023-05-04 02:23:07.602654 dataquality-0.9.1a1/tests/inference/test_inference.py
+-rw-r--r--   0        0        0     3342 2023-04-10 07:35:51.795608 dataquality-0.9.1a1/tests/inference/test_text_classification_inf.py
+-rw-r--r--   0        0        0     3900 2023-04-10 07:35:51.795833 dataquality-0.9.1a1/tests/inference/test_text_ner_inf.py
+-rw-r--r--   0        0        0     3862 2023-02-16 18:20:37.519849 dataquality-0.9.1a1/tests/integration/mock_training_run.py
+-rw-r--r--   0        0        0     7624 2023-05-04 02:23:07.527584 dataquality-0.9.1a1/tests/integrations/fastai/test_cv_fai.py
+-rw-r--r--   0        0        0    10933 2023-05-04 02:23:07.547862 dataquality-0.9.1a1/tests/integrations/hf/test_hf_integration.py
+-rw-r--r--   0        0        0    13693 2023-05-04 22:09:08.118319 dataquality-0.9.1a1/tests/integrations/hf/test_text_classification_hf.py
+-rw-r--r--   0        0        0     9269 2023-05-04 02:23:07.487410 dataquality-0.9.1a1/tests/integrations/keras/test_experimental.py
+-rw-r--r--   0        0        0      514 2023-02-16 18:20:37.520738 dataquality-0.9.1a1/tests/integrations/keras/test_utils.py
+-rw-r--r--   0        0        0     1346 2023-05-04 02:23:07.555929 dataquality-0.9.1a1/tests/integrations/spacy/conftest.py
+-rw-r--r--   0        0        0      760 2023-04-07 02:45:30.770291 dataquality-0.9.1a1/tests/integrations/spacy/test_spacy_integration.py
+-rw-r--r--   0        0        0    17759 2023-05-04 02:23:07.564774 dataquality-0.9.1a1/tests/integrations/spacy/test_spacy_ner.py
+-rw-r--r--   0        0        0     5900 2023-05-04 02:23:07.499263 dataquality-0.9.1a1/tests/integrations/torch/test_dataloader_patching.py
+-rw-r--r--   0        0        0     9298 2023-05-04 02:23:07.505356 dataquality-0.9.1a1/tests/integrations/torch/test_pt_text_classification.py
+-rw-r--r--   0        0        0      904 2023-05-04 02:23:07.494930 dataquality-0.9.1a1/tests/integrations/torch/test_pt_utils.py
+-rw-r--r--   0        0        0     1490 2023-04-28 02:34:07.411121 dataquality-0.9.1a1/tests/integrations/ultralytics/coco128.yaml
+-rw-r--r--   0        0        0     4796 2023-05-04 02:23:07.595738 dataquality-0.9.1a1/tests/integrations/ultralytics/test_cv_yolo.py
+-rw-r--r--   0        0        0     2023 2023-05-04 02:23:07.213395 dataquality-0.9.1a1/tests/loggers/conftest.py
+-rw-r--r--   0        0        0    10010 2023-03-07 23:33:01.397781 dataquality-0.9.1a1/tests/loggers/test_image_classification.py
+-rw-r--r--   0        0        0    11728 2023-05-04 02:23:07.208952 dataquality-0.9.1a1/tests/loggers/test_multi_label.py
+-rw-r--r--   0        0        0    23505 2023-05-04 02:23:07.246089 dataquality-0.9.1a1/tests/loggers/test_ner.py
+-rw-r--r--   0        0        0    28799 2023-05-04 02:23:07.228543 dataquality-0.9.1a1/tests/loggers/test_tabular_classification.py
+-rw-r--r--   0        0        0    14066 2023-05-04 02:23:07.236161 dataquality-0.9.1a1/tests/loggers/test_text_classification.py
+-rw-r--r--   0        0        0     7226 2023-05-04 02:23:07.447407 dataquality-0.9.1a1/tests/schemas/test_conditions.py
+-rw-r--r--   0        0        0      402 2023-02-16 18:20:37.524191 dataquality-0.9.1a1/tests/schemas/test_metrics.py
+-rw-r--r--   0        0        0     2892 2023-05-04 02:23:07.385253 dataquality-0.9.1a1/tests/start/test_start_auto.py
+-rw-r--r--   0        0        0     4378 2023-05-04 02:23:07.380885 dataquality-0.9.1a1/tests/start/test_start_hf.py
+-rw-r--r--   0        0        0     4400 2023-05-04 02:23:07.389501 dataquality-0.9.1a1/tests/start/test_start_keras.py
+-rw-r--r--   0        0        0     8440 2023-05-04 02:23:07.398877 dataquality-0.9.1a1/tests/start/test_start_pt.py
+-rw-r--r--   0        0        0     2995 2023-03-08 21:36:54.589817 dataquality-0.9.1a1/tests/start/test_start_spacy.md
+-rw-r--r--   0        0        0    30343 2023-05-04 02:23:07.191886 dataquality-0.9.1a1/tests/test_dataquality.py
+-rw-r--r--   0        0        0     1783 2023-02-16 18:20:37.524712 dataquality-0.9.1a1/tests/test_telemetrics.py
+-rw-r--r--   0        0        0        0 2023-02-16 18:20:37.524869 dataquality-0.9.1a1/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     5910 2023-05-04 02:23:07.345615 dataquality-0.9.1a1/tests/test_utils/data_utils.py
+-rw-r--r--   0        0        0     1692 2023-05-04 02:23:07.294017 dataquality-0.9.1a1/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0        0        0    11616 2023-04-14 09:39:59.489879 dataquality-0.9.1a1/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0        0        0     8122 2023-02-16 18:20:37.525814 dataquality-0.9.1a1/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0        0        0     3695 2023-02-16 18:20:37.526020 dataquality-0.9.1a1/tests/test_utils/lightning_model.py
+-rw-r--r--   0        0        0     2057 2023-02-16 18:20:37.526167 dataquality-0.9.1a1/tests/test_utils/mock_data.py
+-rw-r--r--   0        0        0     5594 2023-05-04 02:23:07.311166 dataquality-0.9.1a1/tests/test_utils/mock_request.py
+-rw-r--r--   0        0        0     2840 2023-02-16 18:20:37.526602 dataquality-0.9.1a1/tests/test_utils/ner_constants.py
+-rw-r--r--   0        0        0      863 2023-02-16 18:20:37.526747 dataquality-0.9.1a1/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0        0        0     4299 2023-05-04 02:23:07.315210 dataquality-0.9.1a1/tests/test_utils/spacy_integration.py
+-rw-r--r--   0        0        0    22786 2023-04-14 09:39:59.490526 dataquality-0.9.1a1/tests/test_utils/spacy_integration_constants.py
+-rw-r--r--   0        0        0    23021 2023-02-16 18:20:37.527473 dataquality-0.9.1a1/tests/test_utils/spacy_integration_constants_inference.py
+-rw-r--r--   0        0        0     7910 2023-04-14 09:39:59.490924 dataquality-0.9.1a1/tests/test_utils/tc_constants.py
+-rw-r--r--   0        0        0     4614 2023-05-04 02:23:07.417591 dataquality-0.9.1a1/tests/utils/test_auto.py
+-rw-r--r--   0        0        0     1977 2023-04-10 07:35:51.802860 dataquality-0.9.1a1/tests/utils/test_dq_logger.py
+-rw-r--r--   0        0        0     1522 2023-05-04 02:23:07.427111 dataquality-0.9.1a1/tests/utils/test_name.py
+-rw-r--r--   0        0        0      288 2023-02-16 18:20:37.528250 dataquality-0.9.1a1/tests/utils/test_tf_version.py
+-rw-r--r--   0        0        0     1003 2023-05-04 02:23:07.408449 dataquality-0.9.1a1/tests/utils/test_vaex_utils.py
+-rw-r--r--   0        0        0     1098 2023-05-04 02:23:07.404632 dataquality-0.9.1a1/tests/utils/test_version.py
+-rw-r--r--   0        0        0     8002 1970-01-01 00:00:00.000000 dataquality-0.9.1a1/PKG-INFO
```

### Comparing `dataquality-0.8.9/.github/ISSUE_TEMPLATE/bug.md` & `dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/.github/ISSUE_TEMPLATE/doc.md` & `dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/doc.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/.github/ISSUE_TEMPLATE/feature.md` & `dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/.github/ISSUE_TEMPLATE/question.md` & `dataquality-0.9.1a1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/.github/pull_request_template.md` & `dataquality-0.9.1a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/.github/workflows/publish.yaml` & `dataquality-0.9.1a1/.github/workflows/publish.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
       - created
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
       - name: checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: set up python
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: "3.9"
 
       - name: install flit
         run: pip install flit
 
       - name: publish to pypi
```

### Comparing `dataquality-0.8.9/.github/workflows/test.yaml` & `dataquality-0.9.1a1/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,25 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.9, 3.8, 3.7]
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: set up python
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: install dependencies
-        run: scripts/install.sh
+        run: |
+          if [[ ${{ matrix.python-version }} == "3.7" ]]; then
+            scripts/install.sh --extras=py37
+          else
+            scripts/install.sh
+          fi
       - name: test
         run: scripts/test.sh
       - name: upload coverage
         uses: codecov/codecov-action@v1
         with:
           token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
```

### Comparing `dataquality-0.8.9/.gitignore` & `dataquality-0.9.1a1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-docs/_build/
+docs/_build/html
+docs/_build/doctrees
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
@@ -160,9 +161,21 @@
 *.csv
 *.jsonl
 *.ann
 tests/notebooks/dev/
 results/
 
 finetuned
+
+pytorch_sphinx_theme
 launch.json
 data/
+
+# OD
+yolov8n.pt
+runs
+VIA2COCO
+coco_dataset/
+coco.ipynb
+
+# SemSeg
+CV_datasets/
```

### Comparing `dataquality-0.8.9/CONTRIBUTING.md` & `dataquality-0.9.1a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/LICENSE` & `dataquality-0.9.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/analytics.py` & `dataquality-0.9.1a1/dataquality/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
 class Analytics(Borg):
     """Analytics is used to track errors and logs in the background"""
 
     _telemetrics_disabled: bool = True
 
     def __init__(self, ApiClient: Type[ApiClient], config: Config) -> None:
-        """To initialize the Analytics class you need to pass in an ApiClient and the dq config.
+        """To initialize the Analytics class you need
+        to pass in an ApiClient and the dq config.
         :param ApiClient: The ApiClient class
         :param config: The dq config
         """
         super().__init__()
 
         try:
             self._telemetrics_disabled = self._is_telemetrics_disabled(config)
@@ -123,15 +124,15 @@
 
     def ipython_exception_handler(
         self,
         shell: Any,
         etype: Type[BaseException],
         evalue: BaseException,
         tb: TracebackType,
-        tb_offset: Any = None,
+        tb_offset: Optional[Any] = None,
     ) -> None:
         """This function is used to handle exceptions in ipython."""
 
         # we hook into the traceback,
         # inbetween we log the exception
         # and then show the original traceback.
         # because recently the track_exception_ipython was failing
```

### Comparing `dataquality-0.8.9/dataquality/clients/api.py` & `dataquality-0.9.1a1/dataquality/clients/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,30 +63,40 @@
         except GalileoException:
             return False
 
     def make_request(
         self,
         request: RequestType,
         url: str,
-        body: Dict = None,
-        data: Dict = None,
-        params: Dict = None,
-        header: Dict = None,
+        body: Optional[Dict] = None,
+        data: Optional[Dict] = None,
+        params: Optional[Dict] = None,
+        header: Optional[Dict] = None,
         timeout: Union[int, None] = None,
+        files: Optional[Dict] = None,
+        return_response_without_validation: bool = False,
     ) -> Any:
         """Makes an HTTP request.
 
         This is the center point of all functions and the main entry/exit for the
         dataquality client to interact with the server.
         """
         self.__check_login()
         header = header or headers(config.token)
         res = RequestType.get_method(request.value)(
-            url, json=body, params=params, headers=header, data=data, timeout=timeout
+            url,
+            json=body,
+            params=params,
+            headers=header,
+            data=data,
+            timeout=timeout,
+            files=files,
         )
+        if return_response_without_validation:
+            return res
         self._validate_response(res)
         return res.json()
 
     def get_project(self, project_id: UUID4) -> Dict:
         return self.make_request(
             RequestType.GET,
             url=f"{config.api_url}/{Route.projects}/{project_id}",
@@ -255,15 +265,18 @@
             run = res["id"]
         else:
             project = config.current_project_id
             run = config.current_run_id
         return project, run
 
     def get_labels_for_run(
-        self, project_name: str = None, run_name: str = None, task: str = None
+        self,
+        project_name: Optional[str] = None,
+        run_name: Optional[str] = None,
+        task: Optional[str] = None,
     ) -> List[str]:
         """Gets the labels for a given run, else the currently initialized project/run
 
         If you do not provide a project and run name, the currently initialized
         project/run will be used. Otherwise you must provide both a project and run name
         If the run is a multi-label run, a task must be provided
         """
@@ -276,15 +289,15 @@
 
         url = f"{config.api_url}/{Route.content_path(project, run)}/{Route.labels}"
         params = {"task": task} if task else None
         res = self.make_request(RequestType.GET, url=url, params=params)
         return res["labels"]
 
     def get_tasks_for_run(
-        self, project_name: str = None, run_name: str = None
+        self, project_name: Optional[str] = None, run_name: Optional[str] = None
     ) -> List[str]:
         """Gets the task names for a given multi-label run,
 
         If you do not provide a project and run name, the currently initialized
         project/run will be used. Otherwise you must provide both a project and run name
 
         This function is only valid for multi-label runs.
@@ -316,17 +329,17 @@
         url = f"{config.api_url}/{path}/{Route.edits}"
         body = edit.dict()
         params = {"inference_name": edit.inference_name}
         return self.make_request(RequestType.POST, url=url, body=body, params=params)
 
     def reprocess_run(
         self,
-        project_name: str = None,
-        run_name: str = None,
-        labels: Union[List, List[List]] = None,
+        project_name: Optional[str] = None,
+        run_name: Optional[str] = None,
+        labels: Optional[Union[List, List[List]]] = None,
     ) -> Dict:
         """Reinitiate a project/run that has already been finished
 
         If a project and run name have been provided, that project/run will be
         reinitiated, otherwise we trigger the currently initialized project/run.
 
         This will clear out the current state in the server, and will recalculate
@@ -417,15 +430,15 @@
         :param project_name:
         :param run_name:
         :param split:
         """
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
         url = f"{config.api_url}/{Route.content_path(project, run, split)}/meta/columns"
-        return self.make_request(RequestType.GET, url)
+        return self.make_request(RequestType.POST, url, body={})
 
     def get_task_type(self, project_id: UUID4, run_id: UUID4) -> TaskType:
         return TaskType.get_mapping(
             self.get_project_run(project_id, run_id)["task_type"]
         )
 
     def export_run(
@@ -436,15 +449,15 @@
         file_name: str,
         inference_name: str = "",
         slice_name: Optional[str] = None,
         include_cols: Optional[List[str]] = None,
         col_mapping: Optional[Dict[str, str]] = None,
         hf_format: bool = False,
         tagging_schema: Optional[TaggingSchema] = None,
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> None:
         """Export a project/run to disk as a file
 
         :param project_name: The project name
         :param run_name: The run name
         :param split: The split to export on
         :param file_name: The file name. Must end in a supported FileType
@@ -526,15 +539,15 @@
         job_url = f"{config.api_url}/{Route.content_path(pid, rid)}/{Route.latest_job}"
         job = self.make_request(RequestType.GET, job_url)
         return job or {}
 
     def wait_for_run(
         self, project_name: Optional[str] = None, run_name: Optional[str] = None
     ) -> None:
-        print("Waiting for job...")
+        print("Waiting for job (you can safely close this window)...")
         last_progress_message = ""
         while True:
             job = self.get_run_status(project_name=project_name, run_name=run_name)
             if job.get("status") == "completed":
                 print(f"Done! Job finished with status {job.get('status')}")
                 return
             elif job.get("status") == "failed":
@@ -556,15 +569,19 @@
             else:
                 raise GalileoException(
                     f"It seems there was an issue with your job. Received "
                     f"an unexpected status {job.get('status')}"
                 )
 
     def get_presigned_url(
-        self, project_id: str, method: str, bucket_name: str, object_name: str
+        self,
+        method: str,
+        bucket_name: str,
+        object_name: str,
+        project_id: str,
     ) -> str:
         response = self.make_request(
             request=RequestType.GET,
             url=f"{config.api_url}/{Route.presigned_url}",
             params={
                 "api_url": config.api_url,
                 "bucket_name": bucket_name,
@@ -576,17 +593,17 @@
         return response["url"]
 
     def get_run_summary(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
-        filter_params: Dict = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict:
         """Gets overall run summary, or summary of a filtered subset.
 
         Use filter_params to apply arbitrary filters on the dataframe, based on the
         filter schema:
         https://api.dev.rungalileo.io/redoc#tag/insights
         """
@@ -605,18 +622,18 @@
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
     def get_run_metrics(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
         category: str = "gold",
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict[str, List]:
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         all_meta = self.get_metadata_columns(project_name, run_name, split)
         categorical_meta = [i["name"] for i in all_meta["meta"] if i["is_categorical"]]
         avl_cols = categorical_meta + ["gold", "pred"]
@@ -634,18 +651,18 @@
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
     def get_column_distribution(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
         column: str = "data_error_potential",
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict[str, List]:
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         all_meta = self.get_metadata_columns(project_name, run_name, split)
         continuous_meta = [i["name"] for i in all_meta["meta"] if i["is_continuous"]]
         avl_cols = continuous_meta + ["data_error_potential"]
@@ -660,25 +677,33 @@
         params = {"col": column}
         if inference_name:
             params["inference_name"] = inference_name
         body = {"task": task, "filter_params": filter_params or {}}
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
     def get_xray_cards(
-        self, project_name: str, run_name: str, split: str, inference_name: str = None
+        self,
+        project_name: str,
+        run_name: str,
+        split: str,
+        inference_name: Optional[str] = None,
     ) -> List[Dict[str, str]]:
         """Queries API for xray cards for a run/split"""
         project, run = self._get_project_run_id(project_name, run_name)
         path = Route.content_path(project, run, split)
         url = f"{config.api_url}/{path}/{Route.xray}"
         params = {"inference_name": inference_name} if inference_name else None
         return self.make_request(RequestType.GET, url, params=params)
 
     def get_edits(
-        self, project_name: str, run_name: str, split: str, inference_name: str = None
+        self,
+        project_name: str,
+        run_name: str,
+        split: str,
+        inference_name: Optional[str] = None,
     ) -> List:
         """Gets all edits for a run/split"""
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         url = (
             f"{config.api_url}/{Route.content_path(project, run, split)}/{Route.edits}"
@@ -688,15 +713,15 @@
 
     def export_edits(
         self,
         project_name: str,
         run_name: str,
         split: str,
         file_name: str,
-        inference_name: str = None,
+        inference_name: Optional[str] = None,
         include_cols: Optional[List[str]] = None,
         col_mapping: Optional[Dict[str, str]] = None,
         hf_format: bool = False,
         tagging_schema: Optional[TaggingSchema] = None,
     ) -> None:
         """Export the edits of a project/run/split to disk as a file
 
@@ -781,7 +806,54 @@
         return self.make_request(
             RequestType.GET,
             url=(
                 f"{config.api_url}/{Route.projects}/{project_id}/{Route.runs}/{run_id}/"
                 f"{Route.inference_names}"
             ),
         )
+
+    def set_metric_for_run(self, project_id: UUID4, run_id: UUID4, data: Dict) -> Dict:
+        return self.make_request(
+            RequestType.PUT,
+            url=(
+                f"{config.api_url}/{Route.projects}/{project_id}/{Route.runs}/{run_id}/"
+                f"{Route.metrics}"
+            ),
+            body=data,
+        )
+
+    def get_healthcheck_dq(self) -> Dict:
+        return self.make_request(
+            RequestType.GET, url=f"{config.api_url}/{Route.healthcheck_dq}"
+        )
+
+    def upload_file_for_project(
+        self,
+        project_id: str,
+        file_path: str,
+        export_format: str,
+        export_cols: List[str],
+    ) -> Any:
+        url = f"{config.api_url}/{Route.projects}/{project_id}/{Route.upload_file}"
+        res = self.make_request(
+            return_response_without_validation=True,
+            request=RequestType.POST,
+            url=url,
+            files={
+                "file": (
+                    os.path.basename(file_path),
+                    open(file_path, "rb"),
+                    "application/octet-stream",
+                ),
+                "upload_metadata": (
+                    None,
+                    json.dumps(
+                        {
+                            "export_format": export_format,
+                            "export_cols": export_cols,
+                        }
+                    ),
+                    "application/json",
+                ),
+            },
+        )
+        return res
```

### Comparing `dataquality-0.8.9/dataquality/core/_config.py` & `dataquality-0.9.1a1/dataquality/core/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.route import Route
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.helpers import galileo_disabled
 
 CLOUD_URL = "https://console.cloud.rungalileo.io"
 MINIMUM_API_VERSION = "0.4.0"
+GALILEO_DEFAULT_IMG_BUCKET_NAME = "galileo-images"
+GALILEO_DEFAULT_RUN_BUCKET_NAME = "galileo-project-runs"
+GALILEO_DEFAULT_RESULT_BUCKET_NAME = "galileo-project-runs-results"
+EXOSCALE_FQDN_SUFFIX = ".exo.io"
 
 
 class GalileoConfigVars(str, Enum):
     API_URL = "GALILEO_API_URL"
     CONSOLE_URL = "GALILEO_CONSOLE_URL"
 
     @staticmethod
@@ -51,14 +55,19 @@
 class Config(BaseModel):
     api_url: str
     token: Optional[str] = None
     current_user: Optional[str] = None
     current_project_id: Optional[UUID4] = None
     current_run_id: Optional[UUID4] = None
     task_type: Optional[TaskType] = None
+    root_bucket_name: str = GALILEO_DEFAULT_RUN_BUCKET_NAME
+    results_bucket_name: str = GALILEO_DEFAULT_RESULT_BUCKET_NAME
+    images_bucket_name: str = GALILEO_DEFAULT_IMG_BUCKET_NAME
+    minio_fqdn: Optional[str] = None
+    is_exoscale_cluster: bool = False
 
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
 
     def update_file_config(self) -> None:
@@ -110,15 +119,15 @@
         raise GalileoException(err_detail.format(err=str(e))) from None
 
 
 def _check_dq_version() -> None:
     """Check that user is running valid version of DQ client
     Pings backend to check minimum DQ version requirements.
     """
-    r = requests.get(f"{config.api_url}/{Route.healthcheck}/dq")
+    r = requests.get(f"{config.api_url}/{Route.healthcheck_dq}")
     if not r.ok:
         if r.status_code == 404:
             # We don't want to raise error if api doesn't have dq healthcheck yet
             return
         raise GalileoException(r.text) from None
 
     dq_version_parsed = version.parse(dq_version)
```

### Comparing `dataquality-0.8.9/dataquality/core/auth.py` & `dataquality-0.9.1a1/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/core/finish.py` & `dataquality-0.9.1a1/dataquality/core/finish.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,64 +8,70 @@
 from dataquality.clients.api import ApiClient
 from dataquality.core._config import config
 from dataquality.core.report import build_run_report
 from dataquality.schemas import RequestType, Route
 from dataquality.schemas.job import JobName
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.dq_logger import DQ_LOG_FILE_HOME, upload_dq_log_file
-from dataquality.utils.helpers import check_noop, open_console_url
+from dataquality.utils.helpers import check_noop, gpu_available, open_console_url
 from dataquality.utils.thread_pool import ThreadPoolManager
 from dataquality.utils.version import _version_check
 
 api_client = ApiClient()
 a = Analytics(ApiClient, config)  # type: ignore
 
 
 @check_noop
 def finish(
     last_epoch: Optional[int] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
+    create_data_embs: Optional[bool] = None,
 ) -> str:
     """
     Finishes the current run and invokes a job
 
     :param last_epoch: If set, only epochs up to this value will be uploaded/processed
         This is inclusive, so setting last_epoch to 5 would upload epochs 0,1,2,3,4,5
     :param wait: If true, after uploading the data, this will wait for the
         run to be processed by the Galileo server. If false, you can manually wait
         for the run by calling `dq.wait_for_run()` Default True
     :param create_data_embs: If True, an off-the-shelf transformer will run on the raw
         text input to generate data-level embeddings. These will be available in the
         `data view` tab of the Galileo console. You can also access these embeddings
-        via dq.metrics.get_data_embeddings()
+        via dq.metrics.get_data_embeddings(). Default True if a GPU is
+        available, else default False.
     """
     a.log_function("dq/finish")
+    if create_data_embs is None:
+        create_data_embs = gpu_available()
     ThreadPoolManager.wait_for_threads()
     assert config.current_project_id, "You must have an active project to call finish"
     assert config.current_run_id, "You must have an active run to call finish"
     assert config.task_type, "You must have a task type to call finish"
     data_logger = dataquality.get_data_logger()
     data_logger.validate_labels()
 
     _version_check()
 
     if data_logger.non_inference_logged():
         _reset_run(config.current_project_id, config.current_run_id, config.task_type)
 
+    # Certain tasks require extra finish logic
+    data_logger.logger_config.finish()
+
     data_logger.upload(last_epoch, create_data_embs=create_data_embs)
     upload_dq_log_file()
-
     body = dict(
         project_id=str(config.current_project_id),
         run_id=str(config.current_run_id),
         labels=data_logger.logger_config.labels,
         task_type=config.task_type.value,
         tasks=data_logger.logger_config.tasks,
         ner_labels=data_logger.logger_config.ner_labels,
+        feature_names=data_logger.logger_config.feature_names,
     )
     if data_logger.logger_config.inference_logged:
         body.update(
             job_name=JobName.inference,
             non_inference_logged=data_logger.non_inference_logged(),
         )
     res = api_client.make_request(
@@ -89,16 +95,20 @@
             run_id=config.current_run_id,
             link=res["link"],
         )
     elif wait:
         wait_for_run()
         open_console_url(res["link"])
 
-    # Reset the environment
+    # Reset the data logger
     data_logger._cleanup()
+
+    # Reset the model logger
+    dataquality.get_model_logger()._cleanup()
+
     return res.get("link") or ""
 
 
 @check_noop
 def wait_for_run(
     project_name: Optional[str] = None, run_name: Optional[str] = None
 ) -> None:
```

### Comparing `dataquality-0.8.9/dataquality/core/log.py` & `dataquality-0.9.1a1/tests/loggers/test_text_classification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,403 +1,389 @@
-from typing import Any, Dict, List, Optional, Type, Union
+import os
+import random
+from typing import Callable
+from unittest import mock
 
+import datasets
 import numpy as np
 import pandas as pd
-
-from dataquality.analytics import Analytics
-from dataquality.clients.api import ApiClient
-from dataquality.core._config import config
-from dataquality.exceptions import GalileoException
-from dataquality.loggers.data_logger import BaseGalileoDataLogger
-from dataquality.loggers.data_logger.base_data_logger import ITER_CHUNK_SIZE, DataSet
-from dataquality.loggers.data_logger.image_classification import (
-    ImageClassificationDataLogger,
-)
-from dataquality.loggers.logger_config.text_multi_label import (
-    text_multi_label_logger_config,
+import pytest
+import tensorflow as tf
+import vaex
+
+import dataquality
+import dataquality as dq
+from dataquality.exceptions import GalileoException, GalileoWarning
+from dataquality.loggers.data_logger.base_data_logger import DataSet
+from dataquality.loggers.data_logger.text_classification import (
+    TextClassificationDataLogger,
 )
-from dataquality.loggers.model_logger import BaseGalileoModelLogger
-from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
-from dataquality.schemas.task_type import TaskType
-from dataquality.utils.helpers import check_noop
-
-DEFAULT_RANDOM_EMB_DIM = 2
-a = Analytics(ApiClient, config)  # type: ignore
-
-
-@check_noop
-def log_data_samples(
-    *,
-    texts: List[str],
-    ids: List[int],
-    meta: Dict[str, List[Union[str, float, int]]] = None,
-    **kwargs: Any,
-) -> None:
-    """Logs a batch of input samples for model training/test/validation/inference.
-
-    Fields are expected as lists of their content. Field names are in the plural of
-    `log_input_sample` (text -> texts)
-    The expected arguments come from the task_type being used: See dq.docs() for details
-
-    ex (text classification):
-    .. code-block:: python
-
-        all_labels = ["A", "B", "C"]
-        dq.set_labels_for_run(labels = all_labels)
-
-        texts: List[str] = [
-            "Text sample 1",
-            "Text sample 2",
-            "Text sample 3",
-            "Text sample 4"
-        ]
+from dataquality.utils.vaex import GALILEO_DATA_EMBS_ENCODER
+from tests.conftest import LOCAL_MODEL_PATH, LOCATION, TEST_PATH
+from tests.test_utils.tc_constants import TC_LABELS, TEST_HF_DS, TRAIN_HF_DS
+
+
+def test_duplicate_rows(set_test_config, cleanup_after_use) -> None:
+    set_test_config(task_type="text_classification")
+    text_inputs = [
+        "what movies star bruce willis",
+        "show me films with drew barrymore from the 1980s",
+        "what movies starred both al pacino and robert deniro",
+        "find me all of the movies that starred harold ramis and bill murray",
+        "find me a movie with a quote about baseball in it",
+    ]
+    gold = ["A", "C", "B", "A", "C"]
+    ids = [0, 1, 2, 3, 4]
+
+    dq.set_labels_for_run(["A", "B", "C"])
+
+    dq.log_data_samples(texts=text_inputs, labels=gold, split="validation", ids=ids)
+    dq.log_data_samples(texts=text_inputs, labels=gold, split="training", ids=ids)
+
+    with pytest.raises(GalileoException):
+        dq.log_data_samples(texts=text_inputs, labels=gold, split="validation", ids=ids)
+
+    dq.log_data_samples(texts=text_inputs, labels=gold, split="test", ids=ids)
+
+    with pytest.raises(GalileoException):
+        dq.log_data_samples(texts=text_inputs, labels=gold, split="training", ids=ids)
+
+
+def test_duplicate_output_rows(set_test_config, cleanup_after_use) -> None:
+    set_test_config(task_type="text_classification")
+    text_inputs = [
+        "what movies star bruce willis",
+        "show me films with drew barrymore from the 1980s",
+        "what movies starred both al pacino and robert deniro",
+        "find me all of the movies that starred harold ramis and bill murray",
+        "find me a movie with a quote about baseball in it",
+    ]
+    gold = ["A", "C", "B", "A", "C"]
+    ids = list(range(5))
+    dq.set_labels_for_run(["A", "B", "C"])
+
+    dq.log_data_samples(texts=text_inputs, labels=gold, split="validation", ids=ids)
+    dq.log_data_samples(texts=text_inputs, labels=gold, split="training", ids=ids)
+
+    embs = np.random.rand(5, 100)
+    logits = np.random.rand(5, 100)
+    ids = list(range(5))
+    dq.log_model_outputs(embs=embs, logits=logits, ids=ids, split="training", epoch=0)
+    dq.log_model_outputs(embs=embs, logits=logits, ids=ids, split="training", epoch=0)
 
-        labels: List[str] = ["B", "C", "A", "A"]
-
-        meta = {
-            "sample_importance": ["high", "low", "low", "medium"]
-            "quality_ranking": [9.7, 2.4, 5.5, 1.2]
-        }
+    with pytest.raises(GalileoException) as e:
+        dq.get_data_logger().upload()
 
-        ids: List[int] = [0, 1, 2, 3]
-        split = "training"
+    assert str(e.value).startswith("It seems your logged output data has duplicate ids")
 
-        dq.log_data_samples(texts=texts, labels=labels, ids=ids, meta=meta split=split)
 
-    :param texts: List[str] the input samples to your model
-    :param ids: List[int | str] the ids per sample
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param meta: Dict[str, List[str | int | float]]. Log additional metadata fields to
-    each sample. The name of the field is the key of the dictionary, and the values are
-    a list that correspond in length and order to the text samples.
-    :param kwargs: See dq.docs() for details on other task specific parameters
-    """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    data_logger.log_data_samples(texts=texts, ids=ids, meta=meta, **kwargs)
-
-
-@check_noop
-def log_data_sample(*, text: str, id: int, **kwargs: Any) -> None:
-    """Log a single input example to disk
-
-    Fields are expected singular elements. Field names are in the singular of
-    `log_input_samples` (texts -> text)
-    The expected arguments come from the task_type being used: See dq.docs() for details
-
-    :param text: List[str] the input samples to your model
-    :param id: List[int | str] the ids per sample
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param kwargs: See dq.docs() for details on other task specific parameters
-    """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    # For logging a single sample, we don't want a progress bar because it will be
-    # nearly instant, and it's likely that the user will call this many times which
-    # would flood the output.
-    # We don't need to reset log_export_progress because this class instance is
-    # ephemeral
-    data_logger.log_export_progress = False
-    data_logger.log_data_sample(text=text, id=id, **kwargs)
-
-
-@check_noop
-def log_image_dataset(
-    dataset: DataSet,
-    imgs_dir: str,
-    *,
-    imgs_location_colname: Optional[str] = "relpath",
-    batch_size: int = ITER_CHUNK_SIZE,
-    id: Union[str, int] = "id",
-    label: Union[str, int] = "label",
-    split: Optional[Split] = None,
-    meta: Optional[List[Union[str, int]]] = None,
-    **kwargs: Any,
+def test_log_data_sample(
+    set_test_config: Callable, cleanup_after_use: Callable
 ) -> None:
-    assert isinstance(
-        dataset, pd.DataFrame
-    ), "dataset must be a pandas DataFrame"  # TODO: add support for other data types
-    a.log_function("dq/log_image_dataset")
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    assert isinstance(data_logger, ImageClassificationDataLogger), (
-        "This method is only supported for image tasks. "
-        "Please use dq.log_samples for text tasks."
-    )
-    data_logger.log_image_dataset(
-        dataset=dataset,
-        imgs_dir=imgs_dir,
-        imgs_location_colname=imgs_location_colname,
-        batch_size=batch_size,
-        id=id,
-        label=label,
-        split=split,
-        meta=meta,
-    )
-
-
-@check_noop
-def log_dataset(
-    dataset: DataSet,
-    *,
-    batch_size: int = ITER_CHUNK_SIZE,
-    text: Union[str, int] = "text",
-    id: Union[str, int] = "id",
-    split: Optional[Split] = None,
-    meta: Optional[List[Union[str, int]]] = None,
-    **kwargs: Any,
+    logger = TextClassificationDataLogger()
+    dq.set_labels_for_run(["A", "B", "C"])
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = logger
+        dq.log_data_sample(text="sample 1", label="A", id=1, split="training")
+
+        assert logger.texts == ["sample 1"]
+        assert logger.labels == ["A"]
+        assert logger.ids == [1]
+        assert logger.split == Split.training
+
+
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        pd.DataFrame(
+            {
+                "my_text": ["sample1", "sample2", "sample3"],
+                "my_labels": ["A", "A", "B"],
+                "my_id": [1, 2, 3],
+            }
+        ),
+        vaex.from_dict(
+            {
+                "my_text": ["sample1", "sample2", "sample3"],
+                "my_labels": ["A", "A", "B"],
+                "my_id": [1, 2, 3],
+            }
+        ),
+        [
+            {"my_text": "sample1", "my_labels": "A", "my_id": 1},
+            {"my_text": "sample2", "my_labels": "A", "my_id": 2},
+            {"my_text": "sample3", "my_labels": "B", "my_id": 3},
+        ],
+        tf.data.Dataset.from_tensor_slices(
+            {
+                "my_text": ["sample1", "sample2", "sample3"],
+                "my_labels": ["A", "A", "B"],
+                "my_id": [1, 2, 3],
+            }
+        ),
+        datasets.Dataset.from_dict(
+            dict(
+                my_text=["sample1", "sample2", "sample3"],
+                my_labels=["A", "A", "B"],
+                my_id=[1, 2, 3],
+            )
+        ),
+    ],
+)
+def test_log_dataset(
+    dataset: DataSet, set_test_config: Callable, cleanup_after_use: Callable
 ) -> None:
-    """Log an iterable or other dataset to disk. Useful for logging memory mapped files
+    dq.set_labels_for_run(["A", "B"])
+    logger = TextClassificationDataLogger()
 
-    Dataset provided must be an iterable that can be traversed row by row, and for each
-    row, the fields can be indexed into either via string keys or int indexes. Pandas
-    and Vaex dataframes are also allowed, as well as HuggingFace Datasets
-
-    valid examples:
-        d = [
-            {"my_text": "sample1", "my_labels": "A", "my_id": 1, "sample_quality": 5.3},
-            {"my_text": "sample2", "my_labels": "A", "my_id": 2, "sample_quality": 9.1},
-            {"my_text": "sample3", "my_labels": "B", "my_id": 3, "sample_quality": 2.7},
-        ]
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = logger
         dq.log_dataset(
-            d, text="my_text", id="my_id", label="my_labels", meta=["sample_quality"]
+            dataset, text="my_text", label="my_labels", id="my_id", split="train"
         )
 
-        Logging a pandas dataframe, df:
-              text label  id  sample_quality
-        0  sample1     A   1             5.3
-        1  sample2     A   2             9.1
-        2  sample3     B   3             2.7
-        # We don't need to set text id or label because it matches the default
-        dq.log_dataset(d, meta=["sample_quality"])
+        assert logger.texts == ["sample1", "sample2", "sample3"]
+        assert logger.labels == ["A", "A", "B"]
+        assert logger.ids == [1, 2, 3]
+        assert logger.split == Split.training
+
 
-        Logging and iterable of tuples:
-        d = [
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        [
             ("sample1", "A", "ID1"),
             ("sample2", "A", "ID2"),
             ("sample3", "B", "ID3"),
-        ]
-        dq.log_dataset(d, text=0, id=2, label=1)
-
-    Invalid example:
-        d = {
-            "my_text": ["sample1", "sample2", "sample3"],
-            "my_labels": ["A", "A", "B"],
-            "my_id": [1, 2, 3],
-            "sample_quality": [5.3, 9.1, 2.7]
-        }
-
-    In the invalid case, use `dq.log_data_samples`:
-        meta = {"sample_quality": d["sample_quality"]}
-        dq.log_data_samples(
-            texts=d["my_text"], labels=d["my_labels"], ids=d["my_ids"], meta=meta
-        )
-
-    Keyword arguments are specific to the task type. See dq.docs() for details
-
-    :param dataset: The iterable or dataframe to log
-    :batch_size: The number of data samples to log at a time. Useful when logging a
-    memory mapped dataset. A larger batch_size will result in faster logging at the
-    expense of more memory usage. Default 100,000
-    :param text: str | int The column, key, or int index for text data. Default "text"
-    :param id: str | int The column, key, or int index for id data. Default "id"
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param meta: List[str | int] Additional keys/columns to your input data to be
-        logged as metadata. Consider a pandas dataframe, this would be the list of
-        columns corresponding to each metadata field to log
-    :param kwargs: See help(dq.get_data_logger().log_dataset) for more details here
-    or dq.docs() for more general task details
-    """
-    a.log_function("dq/log_dataset")
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    data_logger.log_dataset(
-        dataset,
-        batch_size=batch_size,
-        text=text,
-        id=id,
-        split=split,
-        meta=meta,
-        **kwargs,
-    )
-
-
-@check_noop
-def log_model_outputs(
-    *,
-    embs: Optional[Union[List, np.ndarray]],
-    ids: Union[List, np.ndarray],
-    split: Optional[Split] = None,
-    epoch: Optional[int] = None,
-    logits: Union[List, np.ndarray] = None,
-    probs: Union[List, np.ndarray] = None,
-    inference_name: str = None,
-    exclude_embs: bool = False,
+        ],
+        tf.data.Dataset.from_tensor_slices(
+            [
+                ("sample1", "A", "ID1"),
+                ("sample2", "A", "ID2"),
+                ("sample3", "B", "ID3"),
+            ]
+        ),
+    ],
+)
+def test_log_dataset_tuple(
+    dataset: DataSet, set_test_config: Callable, cleanup_after_use: Callable
 ) -> None:
-    """Logs model outputs for model during training/test/validation.
-
-    :param embs: The embeddings per output sample
-    :param ids: The ids for each sample. Must match input ids of logged samples
-    :param split: The current split. Must be set either here or via dq.set_split
-    :param epoch: The current epoch. Must be set either here or via dq.set_epoch
-    :param logits: The logits for each sample
-    :param probs: Deprecated, use logits. If passed in, a softmax will NOT be applied
-    :param inference_name: Inference name indicator for this inference split.
-        If logging for an inference split, this is required.
-    :param exclude_embs: Optional flag to exclude embeddings from logging. If True and
-        embs is set to None, this will generate random embs for each sample.
+    logger = TextClassificationDataLogger()
+    dq.set_labels_for_run(["A", "B"])
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = logger
+        dq.log_dataset(dataset, text=0, label=1, id=2, split="train")
+
+        assert logger.texts == ["sample1", "sample2", "sample3"]
+        assert logger.labels == ["A", "A", "B"]
+        assert logger.ids == ["ID1", "ID2", "ID3"]
+        assert logger.split == Split.training
+
+
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        [
+            {"text": "sample1", "label": "A", "id": 1},
+            {"text": "sample2", "label": "A", "id": 2},
+            {"text": "sample3", "label": "B", "id": 3},
+        ],
+    ],
+)
+def test_log_dataset_default(
+    dataset: DataSet, set_test_config: Callable, cleanup_after_use: Callable
+) -> None:
+    """Tests that the default keys work as expected when not passed in"""
+    logger = TextClassificationDataLogger()
+    dq.set_labels_for_run(["A", "B"])
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = logger
+        dq.log_dataset(dataset, split="train")
+
+        assert logger.texts == ["sample1", "sample2", "sample3"]
+        assert logger.labels == ["A", "A", "B"]
+        assert logger.ids == [1, 2, 3]
+        assert logger.split == Split.training
+
+
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        [
+            {"text": "sample1", "label": "A", "id": 1},
+            {"text": "sample2", "label": "A", "id": 2},
+            {"text": "sample3", "label": "B", "id": 3},
+        ],
+    ],
+)
+def test_output_no_input_for_split(
+    dataset: DataSet, set_test_config: Callable, cleanup_after_use: Callable
+) -> None:
+    """Validates that no error is thrown and a warning is printed on finish
 
-    The expected argument shapes come from the task_type being used
-    See dq.docs() for more task specific details on parameter shape
+    When you try to upload data for a split that has no input data
     """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    assert (probs is not None) or (
-        logits is not None
-    ), "You must provide either logits or probs"
-    assert (embs is None and exclude_embs) or (
-        embs is not None and not exclude_embs
-    ), "embs can be omitted if and only if exclude_embs is True"
-    if embs is None and exclude_embs:
-        embs = np.random.rand(len(ids), DEFAULT_RANDOM_EMB_DIM)
-
-    model_logger = get_model_logger()(
-        embs=embs,
-        ids=ids,
-        split=Split[split].value if split else "",
-        epoch=epoch,
-        logits=logits,
-        probs=probs,
-        inference_name=inference_name,
+    dq.set_labels_for_run(["A", "B"])
+    dq.log_dataset(dataset, split="train")
+    dq.log_model_outputs(
+        embs=np.random.rand(3, 50),
+        logits=np.random.rand(3, 10),
+        ids=[1, 2, 3],
+        split="validation",
+        epoch=0,
     )
-    model_logger.log()
+    with pytest.warns(GalileoWarning, match=r"There was output data"):
+        dq.get_data_logger().upload()
 
 
-@check_noop
-def set_labels_for_run(labels: Union[List[List[str]], List[str]]) -> None:
-    """
-    Creates the mapping of the labels for the model to their respective indexes.
-
-    :param labels: An ordered list of labels (ie ['dog','cat','fish']
-    If this is a multi-label type, then labels are a list of lists where each inner
-    list indicates the label for the given task
-
-    This order MUST match the order of probabilities that the model outputs.
-
-    In the multi-label case, the outer order (order of the tasks) must match the
-    task-order of the task-probabilities logged as well.
-    """
-    a.log_function("dq/set_labels_for_run")
-
-    if isinstance(labels[0], (int, np.integer)):
-        get_data_logger().logger_config.int_labels = True
-    get_data_logger().logger_config.labels = labels
-
-
-@check_noop
-def set_tasks_for_run(tasks: List[str], binary: bool = True) -> None:
-    """Sets the task names for the run (multi-label case only).
-
-    This order MUST match the order of the labels list provided in log_input_data
-    and the order of the probability vectors provided in log_model_outputs.
-
-    This also must match the order of the labels logged in set_labels_for_run (meaning
-    that the first list of labels must be the labels of the first task passed in here)
-
-    :param tasks: The list of tasks for your run
-    :param binary: Whether this is a binary multi label run. If true, tasks will also
-    be set as your labels, and you should NOT call `dq.set_labels_for_run` it will be
-    handled for you. Default True
-    """
-    if config.task_type != TaskType.text_multi_label:
-        raise GalileoException("You can only set task names for multi-label use cases.")
-    get_data_logger().logger_config.tasks = tasks
-    text_multi_label_logger_config.binary = binary
-    if binary:
-        # The labels validator will handle adding the "NOT_" to each label
-        text_multi_label_logger_config.labels = [[task] for task in tasks]
-
-
-@check_noop
-def set_tagging_schema(tagging_schema: TaggingSchema) -> None:
-    """Sets the tagging schema for NER models
-
-    Only valid for text_ner task_types. Others will throw an exception
-    """
-    get_data_logger().set_tagging_schema(tagging_schema)
-
-
-def get_model_logger(task_type: TaskType = None) -> Type[BaseGalileoModelLogger]:
-    task_type = _get_task_type(task_type)
-    return BaseGalileoModelLogger.get_logger(task_type)
-
-
-def get_data_logger(task_type: TaskType = None) -> BaseGalileoDataLogger:
-    task_type = _get_task_type(task_type)
-    return BaseGalileoDataLogger.get_logger(task_type)()
-
-
-def _get_task_type(task_type: TaskType = None) -> TaskType:
-    task = task_type or config.task_type
-    if not task:
-        raise GalileoException(
-            "You must provide either a task_type or first call "
-            "dataqualtiy.init and provide one"
+@pytest.mark.parametrize("set_labels_first", [True, False])
+def test_logged_labels_dont_match_set_labels(
+    set_labels_first: bool, set_test_config: Callable, cleanup_after_use: Callable
+) -> None:
+    """An error should be thrown when the set labels dont match the logged labels"""
+    set_test_config(task_type="text_classification")
+    labels = ["A", "B", "C"]
+    # labels are the index, not the actual labels. No good
+    dataset = [
+        {"text": "sample1", "label": 1, "id": 1},
+        {"text": "sample2", "label": 1, "id": 2},
+        {"text": "sample3", "label": 2, "id": 3},
+    ]
+    if set_labels_first:
+        dataquality.set_labels_for_run(labels)
+        with pytest.raises(AssertionError) as e:
+            dataquality.log_dataset(dataset, split="train")
+        assert str(e.value).startswith("Labels set to")
+    else:
+        with pytest.raises(AssertionError) as e:
+            dataquality.log_dataset(dataset, split="train")
+        assert (
+            str(e.value) == "You must set labels before logging input data,"
+            " when label column is numeric"
         )
-    return task
-
 
-def docs() -> None:
-    """Print the documentation for your specific input and output logging format
-
-    Based on your task_type, this will print the appropriate documentation
-    """
-    get_data_logger().doc()
-    get_model_logger().doc()
 
+@pytest.mark.parametrize("set_labels_first", [True, False])
+@pytest.mark.parametrize("is_numeric", [True, False])
+def test_labels(
+    set_test_config: Callable, set_labels_first: bool, is_numeric: bool
+) -> None:
+    set_test_config(task_type="text_classification")
+    str_labels = ["A", "B", "C"]
+    if is_numeric:
+        labels = [0, 1, 2]
+    else:
+        labels = str_labels
+    df = pd.DataFrame(
+        {
+            "id": [0, 1, 2, 3, 4],
+            "text": ["hello", "world", "bye", "foo", "bar"],
+            "label": [random.choice(labels) for _ in range(5)],
+        }
+    )
 
-@check_noop
-def set_epoch(epoch: int) -> None:
-    """Set the current epoch.
+    if set_labels_first:
+        dq.set_labels_for_run(str_labels)
+        dataquality.log_dataset(df, split="train")
+    else:
+        if is_numeric:
+            with pytest.raises(AssertionError) as e:
+                dataquality.log_dataset(df, split="train")
+            assert (
+                str(e.value) == "You must set labels before logging input data,"
+                " when label column is numeric"
+            )
+
+
+def test_log_int_labels(set_test_config: Callable, cleanup_after_use: Callable) -> None:
+    """Tests that a user can log their labels as ints without issue"""
+    set_test_config(task_type="text_classification")
+    labels = [1, 2, 3]
+    # labels are the index, not the actual labels. No good
+    dataset = pd.DataFrame(
+        [
+            {"text": "sample1", "label": 1, "id": 1},
+            {"text": "sample2", "label": 1, "id": 2},
+            {"text": "sample3", "label": 2, "id": 3},
+        ]
+    )
+    dataquality.set_labels_for_run(labels)
+    dataquality.log_dataset(dataset, split="train")
+    dataquality.get_data_logger().logger_config.observed_num_labels = len(labels)
+
+    # Should not throw an error
+    dataquality.get_data_logger().validate_labels()
+    assert sorted(
+        dataquality.get_data_logger().logger_config.observed_labels
+    ) == sorted(["1", "2"])
+    assert sorted(dataquality.get_data_logger().logger_config.labels) == sorted(
+        ["1", "2", "3"]
+    )
 
-    When set, logging model outputs will use this if not logged explicitly
-    """
-    get_data_logger().logger_config.cur_epoch = epoch
 
+def test_log_int_labels_mapped(
+    set_test_config: Callable, cleanup_after_use: Callable
+) -> None:
+    """Tests that a user can log their labels as ints without issue"""
+    set_test_config(task_type="text_classification")
+    labels = ["apple", "banana", "strawberry"]
+    # labels are the index, not the actual labels. No good
+    dataset = pd.DataFrame(
+        [
+            {"text": "sample1", "label": 1, "id": 1},
+            {"text": "sample2", "label": 1, "id": 2},
+            {"text": "sample3", "label": 2, "id": 3},
+        ]
+    )
+    dataquality.set_labels_for_run(labels)
+    dataquality.log_dataset(dataset, split="train")
+    dataquality.get_data_logger().logger_config.observed_num_labels = len(labels)
+
+    # Should not throw an error
+    dataquality.get_data_logger().validate_labels()
+    assert sorted(
+        dataquality.get_data_logger().logger_config.observed_labels
+    ) == sorted(["banana", "strawberry"])
+    assert sorted(dataquality.get_data_logger().logger_config.labels) == sorted(labels)
+    df = vaex.open(f"{LOCATION}/input_data/training/data_0.arrow")
+    assert df["gold"].tolist() == ["banana", "banana", "strawberry"]
 
-@check_noop
-def set_split(split: Split, inference_name: Optional[str] = None) -> None:
-    """Set the current split.
 
-    When set, logging data inputs/model outputs will use this if not logged explicitly
-    When setting split to inference, inference_name must be included
-    """
-    get_data_logger().logger_config.cur_inference_name = inference_name
-    split = Split[split]
-    setattr(get_data_logger().logger_config, f"{split}_logged", True)
-    # Set cur_inference_name before split for pydantic validation
-    get_data_logger().logger_config.cur_split = split
+def test_create_and_upload_data_embs(
+    cleanup_after_use: Callable, set_test_config: Callable
+) -> None:
+    set_test_config(task_type="text_classification")
+    # Use the local mini bert model
+    os.environ[GALILEO_DATA_EMBS_ENCODER] = LOCAL_MODEL_PATH
+
+    df = vaex.from_arrays(id=list(range(10)))
+    df["text"] = "sentence number " + df["id"].astype(str)
+    logger = TextClassificationDataLogger()
+    logger.create_and_upload_data_embs(df, "training", 3)
+    data_embs_path = f"{TEST_PATH}/training/3/data_emb/data_emb.hdf5"
+    data_embs = vaex.open(data_embs_path)
+    assert len(data_embs) == 10
+    assert data_embs.get_column_names() == ["id", "emb"]
+    assert isinstance(data_embs.emb.values, np.ndarray)
+    assert data_embs.emb.values.ndim == 2
+    # mini BERT model spits out 32 dims
+    assert data_embs.emb.values.shape == (10, 32)
 
 
-@check_noop
-def set_epoch_and_split(
-    epoch: int, split: Split, inference_name: Optional[str] = None
+def test_log_dataset_hf_no_int2str(
+    set_test_config: Callable, cleanup_after_use: Callable
 ) -> None:
-    """Set the current epoch and set the current split.
-    When set, logging data inputs/model outputs will use this if not logged explicitly
-    When setting split to inference, inference_name must be included
-    """
-    set_epoch(epoch)
-    set_split(split, inference_name)
+    logger = TextClassificationDataLogger()
+    dataquality.set_labels_for_run(TC_LABELS)
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = logger
+        dq.log_dataset(TRAIN_HF_DS, split="train")
+        # We should grab the labels from the dataset and save them
+        assert logger.logger_config.labels == TC_LABELS
+
+    new_logger = TextClassificationDataLogger()
+    with mock.patch("dataquality.core.log.get_data_logger") as mock_method:
+        mock_method.return_value = new_logger
+        # Even thought the test ds doesn't have the label names, we should be able
+        # to grab them from the config.labels because we grabbed them from the train ds
+        dq.log_dataset(TEST_HF_DS, split="test")
```

### Comparing `dataquality-0.8.9/dataquality/core/report.py` & `dataquality-0.9.1a1/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/dq_auto/auto.py` & `dataquality-0.9.1a1/dataquality/dq_auto/auto.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from typing import Dict, List, Union
+import logging
+from typing import Dict, List, Optional, Union
 
 import pandas as pd
 from datasets import Dataset, DatasetDict
-
+from transformers import Trainer
 from dataquality.schemas.task_type import TaskType
-from dataquality.utils.auto import get_task_type_from_data
+from dataquality.utils.auto import get_task_type_from_data, set_global_logging_level
 
 AUTO_PROJECT_NAME = {
     TaskType.text_classification: "auto_tc",
     TaskType.text_ner: "auto_ner",
 }
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
     max_padding_length: int = 200,
     hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
-    project_name: str = None,
-    run_name: str = None,
+    num_train_epochs: int = 15,
+    labels: Optional[List[str]] = None,
+    project_name: Optional[str] = None,
+    run_name: Optional[str] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
-) -> None:
+    create_data_embs: Optional[bool] = None,
+) -> Trainer:
     """Automatically gets insights on a text classification or NER dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface transformer model, and
     provide Galileo insights via a link to the Galileo Console
 
     One of `hf_data`, `train_data` should be provided. If neither of those are, a
@@ -74,147 +76,168 @@
         * Huggingface dataset
         * Path to a local file
         * Huggingface dataset hub path
     :param max_padding_length: The max length for padding the input text
         during tokenization. Default 200
     :param hf_model: The pretrained AutoModel from huggingface that will be used to
         tokenize and train on the provided data. Default distilbert-base-uncased
+    :param num_train_epochs: The number of epochs to train for (early stopping will
+        always be active). Default 15
     :param labels: Optional list of labels for this dataset. If not provided, they
         will attempt to be extracted from the data
     :param project_name: Optional project name. If not set, a random name will
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
     :param create_data_embs: Whether to create data embeddings for this run. If True,
         Sentence-Transformers will be used to generate data embeddings for this dataset
         and uploaded with this run. You can access these embeddings via
         `dq.metrics.get_data_embeddings` in the `emb` column or
         `dq.metrics.get_dataframe(..., include_data_embs=True)` in the `data_emb` col
-        Only available for TC currently. NER coming soon. Default False.
+        Only available for TC currently. NER coming soon. Default True if a GPU is
+        available, else default False.
 
     For text classification datasets, the only required columns are `text` and `label`
 
     For NER, the required format is the huggingface standard format of `tokens` and
     `tags` (or `ner_tags`).
     See example: https://huggingface.co/datasets/rungalileo/mit_movies
 
         MIT Movies dataset in huggingface format
 
+    .. code-block:: python
+
         tokens	                                            ner_tags
         [what, is, a, good, action, movie, that, is, r...	[0, 0, 0, 0, 7, 0, ...
         [show, me, political, drama, movies, with, jef...	[0, 0, 7, 8, 0, 0, ...
         [what, are, some, good, 1980, s, g, rated, mys...	[0, 0, 0, 0, 5, 6, ...
         [list, a, crime, film, which, director, was, d...	[0, 0, 7, 0, 0, 0, ...
         [is, there, a, thriller, movie, starring, al, ...	[0, 0, 0, 7, 0, 0, ...
         ...                                               ...                      ...
 
 
     To see auto insights on a random, pre-selected dataset, simply run
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto()
-    ```
+
 
     An example using `auto` with a hosted huggingface text classification dataset
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto(hf_data="rungalileo/trec6")
-    ```
+
 
     Similarly, for NER
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto(hf_data="conll2003")
-    ```
+
 
     An example using `auto` with sklearn data as pandas dataframes
-    ```python
+
+    .. code-block:: python
+
+        import dataquality as dq
         import pandas as pd
         from sklearn.datasets import fetch_20newsgroups
-        from dataquality.auto.text_classification import auto
 
         # Load the newsgroups dataset from sklearn
         newsgroups_train = fetch_20newsgroups(subset='train')
         newsgroups_test = fetch_20newsgroups(subset='test')
         # Convert to pandas dataframes
         df_train = pd.DataFrame(
             {"text": newsgroups_train.data, "label": newsgroups_train.target}
         )
         df_test = pd.DataFrame(
             {"text": newsgroups_test.data, "label": newsgroups_test.target}
         )
 
-        auto(
+        dq.auto(
              train_data=df_train,
              test_data=df_test,
              labels=newsgroups_train.target_names,
              project_name="newsgroups_work",
              run_name="run_1_raw_data"
         )
-    ```
+
 
     An example of using `auto` with a local CSV file with `text` and `label` columns
-    ```python
-    from dataquality.auto.text_classification import auto
 
-    auto(
-         train_data="train.csv",
-         test_data="test.csv",
-         project_name="data_from_local",
-         run_name="run_1_raw_data"
-    )
-    ```
+    .. code-block:: python
+
+        import dataquality as dq
+
+        dq.auto(
+            train_data="train.csv",
+            test_data="test.csv",
+            project_name="data_from_local",
+            run_name="run_1_raw_data"
+        )
     """
+    # Remove all output from transformers and torch except the progress bar
+    set_global_logging_level(logging.ERROR, ["torch"])
+    set_global_logging_level(logging.ERROR, ["transformers"])
+
     # We need to import auto down here instead of at the top of the file like normal
     # because we simultaneously want analytic tracking on the files we import while
     # wanting dq.auto as a top level function. If we have these imports at the top,
     # and make dq.auto() available, then auto_tc and auto_ner will both always be
     # imported as soon as dataquality is imported. Also, transformers_trainer and
     # pytorch (which auto depends on) will be immediately imported. The only way to
     # avoid that is by having the imports only be made selectively when auto is called
     if hf_data is None and train_data is None:
         from dataquality.dq_auto.text_classification import auto as auto_tc
 
-        auto_tc()
+        return auto_tc(num_train_epochs=num_train_epochs)
+
     task_type = get_task_type_from_data(hf_data, train_data)
     # We cannot use a common list of *args or **kwargs here because mypy screams :(
     if task_type == TaskType.text_classification:
         from dataquality.dq_auto.text_classification import auto as auto_tc
 
-        auto_tc(
+        return auto_tc(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
             inference_data=inference_data,
             max_padding_length=max_padding_length,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             create_data_embs=create_data_embs,
+            num_train_epochs=num_train_epochs,
         )
     elif task_type == TaskType.text_ner:
         from dataquality.dq_auto.ner import auto as auto_ner
 
-        auto_ner(
+        return auto_ner(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
             inference_data=inference_data,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
+            num_train_epochs=num_train_epochs,
         )
     else:
         raise Exception("auto is only supported for text classification and NER!")
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.1a1/dataquality/dq_auto/base_data_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,20 @@
         raise GalileoException(
             "Dataset must be one of pandas DataFrame, "
             "huggingface Dataset, or string path"
         )
 
     def get_dataset_dict(
         self,
-        hf_data: Union[DatasetDict, str] = None,
-        hf_inference_names: List[str] = None,
-        train_data: Union[pd.DataFrame, Dataset, str] = None,
-        val_data: Union[pd.DataFrame, Dataset, str] = None,
-        test_data: Union[pd.DataFrame, Dataset, str] = None,
-        inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+        hf_data: Optional[Union[DatasetDict, str]] = None,
+        hf_inference_names: Optional[List[str]] = None,
+        train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
         labels: Optional[List[str]] = None,
     ) -> DatasetDict:
         """Creates and/or validates the DatasetDict provided by the user.
 
         If the user provides a DatasetDict, we simply validate it. Otherwise, we
         parse a combination of the parameters provided, generate a DatasetDict of their
         training data, and validate that.
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/ner.py` & `dataquality-0.9.1a1/dataquality/dq_auto/ner.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dataquality as dq
 from dataquality import Analytics, ApiClient
 from dataquality.dq_auto.base_data_manager import BaseDatasetManager
 from dataquality.dq_auto.ner_trainer import get_trainer
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.auto import add_val_data_if_missing, run_name_from_hf_dataset
 from dataquality.utils.auto_trainer import do_train
+from transformers import Trainer
 
 a = Analytics(ApiClient, dq.config)
 a.log_import("auto_ner")
 
 
 class NERDatasetManager(BaseDatasetManager):
     DEMO_DATASETS = ["conll2003", "rungalileo/mit_movies", "wnut_17"]
@@ -42,26 +43,28 @@
                 assert (
                     "tags" in ds.features or "ner_tags" in ds.features
                 ), "Dataset must have column `tags` or `ner_tags`"
         return add_val_data_if_missing(clean_dd)
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
+    num_train_epochs: int = 15,
     hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
+    labels: Optional[List[str]] = None,
     project_name: str = "auto_ner",
-    run_name: str = None,
+    run_name: Optional[str] = None,
     wait: bool = True,
-) -> None:
+    call_finish: bool = True,
+) -> Trainer:
     """Automatically gets insights on an NER or Token Classification dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface token classification model, and
     provide Galileo insights via a link to the Galileo Console
 
     One of `hf_data`, `train_data` should be provided. If neither of those are, a
@@ -113,14 +116,17 @@
         will attempt to be extracted from the data
     :param project_name: Optional project name. If not set, a random name will
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
+    :param call_finish: Whether to call `finish` on the Galileo client. Default True
+    :return: A Trainer object that can be used to train the model further or
+        to run predictions
 
     To see auto insights on a random, pre-selected dataset, simply run
     ```python
         from dataquality.auto.ner import auto
 
         auto()
     ```
@@ -156,18 +162,23 @@
          train_data="train.csv",
          test_data="test.csv",
          project_name="data_from_local",
          run_name="run_1_raw_data"
     )
     ```
     """
-    a.log_function("auto/ner")
     manager = NERDatasetManager()
     dd = manager.get_dataset_dict(
         hf_data, hf_inference_names, train_data, val_data, test_data, inference_data
     )
     dq.login()
+    a.log_function("auto/ner")
     if not run_name and isinstance(hf_data, str):
         run_name = run_name_from_hf_dataset(hf_data)
-    dq.init(TaskType.text_ner, project_name=project_name, run_name=run_name)
-    trainer, encoded_data = get_trainer(dd, hf_model, labels)
-    do_train(trainer, encoded_data, wait)
+    dq.init(
+        TaskType.text_ner,
+        project_name=project_name,
+        run_name=run_name,
+    )
+    trainer, encoded_data = get_trainer(dd, hf_model, num_train_epochs, labels)
+    do_train(trainer, encoded_data, wait, call_finish)
+    return trainer
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.1a1/dataquality/dq_auto/ner_trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
-import evaluate
 import numpy as np
 from datasets import DatasetDict
 from transformers import (
     AutoModelForTokenClassification,
     AutoTokenizer,
     DataCollatorForTokenClassification,
     EarlyStoppingCallback,
     EvalPrediction,
     IntervalStrategy,
     Trainer,
     TrainingArguments,
 )
 
 import dataquality as dq
+from dataquality.exceptions import GalileoException
 from dataquality.integrations.hf import tokenize_and_log_dataset
 from dataquality.schemas.hf import HFCol
 from dataquality.schemas.split import Split
+from dataquality.utils.helpers import mps_available
 
-# For NER training, there is only 1 evaluation tool
-# https://huggingface.co/course/chapter7/2#metrics
-metric = evaluate.load("seqeval")
+try:
+    # For NER training, there is only 1 evaluation tool
+    # https://huggingface.co/course/chapter7/2#metrics
+    import evaluate
+
+    metric = evaluate.load("seqeval")
+except ImportError:
+    raise GalileoException(
+        "⚠️ Huggingface evaluate library not installed "
+        "please run `pip install dataquality[evaluate]` "
+        "to enable metrics computation."
+    )
 
 
 def compute_metrics(eval_pred: EvalPrediction) -> Dict:
     """Metrics computation for token classification
 
     Taken directly from the docs https://huggingface.co/course/chapter7/2#metrics
     and updated for typing
@@ -51,55 +61,58 @@
         "accuracy": results["overall_accuracy"],
     }
 
 
 def get_trainer(
     dd: DatasetDict,
     model_checkpoint: str,
+    num_train_epochs: int,
     labels: Optional[List[str]] = None,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     default_cols = set(HFCol.get_fields())
     meta = [c for c in dd[Split.train].features if c not in default_cols]
     encoded_datasets = tokenize_and_log_dataset(
         dd, tokenizer, label_names=labels, meta=meta
     )
     # FIXME: Why do I need this? `tokenize_and_log_dataset` returns a DatasetDict
     #  not an Optional[DatasetDict]...?
     assert isinstance(encoded_datasets, DatasetDict)
 
-    model = AutoModelForTokenClassification.from_pretrained(
-        model_checkpoint, num_labels=len(dq.get_model_logger().logger_config.labels)
-    )
+    # Used to properly seed the model
+    def model_init() -> Any:
+        return AutoModelForTokenClassification.from_pretrained(
+            model_checkpoint, num_labels=len(dq.get_model_logger().logger_config.labels)
+        )
 
     batch_size = 64
     has_val = Split.validation in encoded_datasets
     eval_strat = IntervalStrategy.EPOCH if has_val else IntervalStrategy.NO
     load_best_model = has_val  # Can only load the best model if we have validation data
 
     args = TrainingArguments(
         "finetuned",
         evaluation_strategy=eval_strat,
-        learning_rate=2e-5,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size,
         load_best_model_at_end=load_best_model,
-        num_train_epochs=10,
+        num_train_epochs=num_train_epochs,
         weight_decay=0.01,
         save_strategy=IntervalStrategy.EPOCH,
         logging_strategy=IntervalStrategy.EPOCH,
         logging_dir="./logs",
         seed=42,
+        use_mps_device=mps_available(),
     )
 
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
-        model,
-        args,
+        model_init=model_init,
+        args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics,
         data_collator=DataCollatorForTokenClassification(tokenizer),
         callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.1a1/dataquality/dq_auto/tc_trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from functools import partial
-from typing import Dict, List, Tuple
+from typing import Any, Dict, List, Tuple
 
-import evaluate
 import numpy as np
 from datasets import Dataset, DatasetDict
-from evaluate import EvaluationModule
 from transformers import (
     AutoModelForSequenceClassification,
     AutoTokenizer,
     BatchEncoding,
     EarlyStoppingCallback,
     EvalPrediction,
     IntervalStrategy,
     PreTrainedTokenizerBase,
     Trainer,
     TrainingArguments,
 )
 
+from dataquality.exceptions import GalileoException
 from dataquality.schemas.split import Split
+from dataquality.utils.helpers import mps_available
 
 EVAL_METRIC = "f1"
 
+try:
+    import evaluate
+    from evaluate import EvaluationModule
+except ImportError:
+    raise GalileoException(
+        "⚠️ Huggingface evaluate library not installed "
+        "please run `pip install dataquality[evaluate]` "
+        "to enable metrics computation."
+    )
+
 
 # Taken from the docs of the trainer module:
 # https://github.com/huggingface/transformers/blob/main/examples/pytorch/
 # text-classification/run_glue.py#L434
 def preprocess_function(
     input_data: Dataset, tokenizer: PreTrainedTokenizerBase, max_length: int
 ) -> BatchEncoding:
@@ -42,52 +52,55 @@
 
 
 def get_trainer(
     dd: DatasetDict,
     labels: List[str],
     model_checkpoint: str,
     max_padding_length: int,
+    num_train_epochs: int,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     encoded_datasets = dd.map(
         lambda x: preprocess_function(x, tokenizer, max_padding_length), batched=True
     )
 
-    model = AutoModelForSequenceClassification.from_pretrained(
-        model_checkpoint, num_labels=len(labels)
-    )
+    # Used to properly seed the model
+    def model_init() -> Any:
+        return AutoModelForSequenceClassification.from_pretrained(
+            model_checkpoint, num_labels=len(labels)
+        )
 
     # Training arguments and training part
     metric = evaluate.load(EVAL_METRIC)
     # We use the users chosen evaluation metric by preloading it into the partial
     compute_metrics_partial = partial(compute_metrics, metric)
     batch_size = 64
     has_val = Split.validation in encoded_datasets
     eval_strat = IntervalStrategy.EPOCH if has_val else IntervalStrategy.NO
     load_best_model = has_val  # Can only load the best model if we have validation data
     args = TrainingArguments(
         "finetuned",
         evaluation_strategy=eval_strat,
         save_strategy=IntervalStrategy.EPOCH,
-        learning_rate=3e-4,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size,
-        num_train_epochs=10,
+        num_train_epochs=num_train_epochs,
         weight_decay=0.01,
         load_best_model_at_end=load_best_model,
         push_to_hub=False,
         report_to=["all"],
         seed=42,
+        use_mps_device=mps_available(),
     )
 
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
-        model,
-        args,
+        model_init=model_init,
+        args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics_partial,
         callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
     )
     return trainer, encoded_datasets
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.1a1/dataquality/dq_auto/text_classification.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from datasets import ClassLabel, Dataset, DatasetDict
-
+from transformers import Trainer
 import dataquality as dq
 from dataquality import Analytics, ApiClient
 from dataquality.dq_auto.base_data_manager import BaseDatasetManager
 from dataquality.dq_auto.tc_trainer import get_trainer
 from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.auto import add_val_data_if_missing, run_name_from_hf_dataset
@@ -35,15 +35,15 @@
         """
         for c in df.columns:
             if df[c].dtype == object:
                 df[c] = df[c].astype("str")
         return df
 
     def _add_class_label_to_dataset(
-        self, ds: Dataset, labels: List[str] = None
+        self, ds: Dataset, labels: Optional[List[str]] = None
     ) -> Dataset:
         """Map a not ClassLabel 'label' column to a ClassLabel, if possible"""
         if "label" not in ds.features or isinstance(ds.features["label"], ClassLabel):
             return ds
         labels = labels if labels is not None else sorted(set(ds["label"]))
         # For string columns, map the label2idx so we can cast to ClassLabel
         if ds.features["label"].dtype == "string":
@@ -52,15 +52,15 @@
 
         # https://github.com/python/mypy/issues/6239
         class_label = ClassLabel(num_classes=len(labels), names=labels)  # type: ignore
         ds = ds.cast_column("label", class_label)
         return ds
 
     def _convert_df_to_dataset(
-        self, df: pd.DataFrame, labels: List[str] = None
+        self, df: pd.DataFrame, labels: Optional[List[str]] = None
     ) -> Dataset:
         """Converts a pandas dataframe to a well-formed huggingface dataset
 
         The main thing happening here is that we are taking the pandas label column and
         mapping it to a Dataset ClassLabel if possible. If not, it will get parsed later
         or a validation error will be thrown if not possible in `_validate_dataset_dict`
         """
@@ -121,28 +121,30 @@
         if key in Split.get_valid_keys():
             dq.log_dataset(ds, meta=meta, split=key)
         else:
             dq.log_dataset(ds, meta=meta, split=Split.inference, inference_name=key)
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
     max_padding_length: int = 200,
+    num_train_epochs: int = 15,
     hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
+    labels: Optional[List[str]] = None,
     project_name: str = "auto_tc",
-    run_name: str = None,
+    run_name: Optional[str] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
-) -> None:
+    create_data_embs: Optional[bool] = None,
+    call_finish: bool = True,
+) -> Trainer:
     """Automatically gets insights on a text classification dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface transformer model, and
     provide Galileo insights via a link to the Galileo Console
 
     One of `hf_data`, `train_data` should be provided. If neither of those are, a
@@ -193,14 +195,18 @@
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
     :param create_data_embs: Whether to create data embeddings for this run. Default
         False
+    :param call_finish: Whether to call `finish` on the trainer after training
+        completes. Default True
+    :return: A Trainer object that can be used to train the model further or
+        to run predictions
 
     To see auto insights on a random, pre-selected dataset, simply run
     ```python
         from dataquality.auto.text_classification import auto
 
         auto()
     ```
@@ -246,27 +252,31 @@
          train_data="train.csv",
          test_data="test.csv",
          project_name="data_from_local",
          run_name="run_1_raw_data"
     )
     ```
     """
-    a.log_function("auto/tc")
     manager = TCDatasetManager()
     dd = manager.get_dataset_dict(
         hf_data,
         hf_inference_names,
         train_data,
         val_data,
         test_data,
         inference_data,
         labels,
     )
     labels = _get_labels(dd, labels)
     dq.login()
+    a.log_function("auto/tc")
     if not run_name and isinstance(hf_data, str):
         run_name = run_name_from_hf_dataset(hf_data)
     dq.init(TaskType.text_classification, project_name=project_name, run_name=run_name)
     dq.set_labels_for_run(labels)
     _log_dataset_dict(dd)
-    trainer, encoded_data = get_trainer(dd, labels, hf_model, max_padding_length)
-    do_train(trainer, encoded_data, wait, create_data_embs)
+    trainer, encoded_data = get_trainer(
+        dd, labels, hf_model, max_padding_length, num_train_epochs
+    )
+    do_train(trainer, encoded_data, wait, create_data_embs, call_finish)
+    trainer.save_model()
+    return trainer
```

### Comparing `dataquality-0.8.9/dataquality/integrations/experimental/keras.py` & `dataquality-0.9.1a1/dataquality/integrations/experimental/keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         super(DataQualityCallback, self).__init__()
         if not tf.executing_eagerly():
             raise GalileoException(
                 "Tensorflow must be running eagerly. "
                 "Set `model.compile(run_eagerly=True)` to fix this"
             )
 
-    def on_train_begin(self, logs: Any = None) -> None:
+    def on_train_begin(self, logs: Optional[Any] = None) -> None:
         """Initialize the training by extracting the model input arguments.
         and from it generate the indices of the batches."""
         assert self.model.run_eagerly, GalileoException(
             "Model must be run run eagerly."
             "Set `model.compile(run_eagerly=True)` to fix this"
         )
 
@@ -98,21 +98,21 @@
 
     def _clear_logger_config_helper_data(self) -> None:
         """Clear the helper data from the logger config for the current step."""
         self.store.pop("input", None)
         self.store.pop("output", None)
         self.store.pop("indices_ids", None)
 
-    def on_train_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the beginning of the batch we clear the
         helper data from the logger config."""
         self._clear_logger_config_helper_data()
         dq.set_split(Split.train)
 
-    def on_train_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the end of the batch we log the input
         of the classifier and the output.
         :param batch: The batch number.
         :param logs: The logs."""
         dq.set_split(Split.train)
         # We try to fetch the indices directly from the store
         ids = self.store.get("indices_ids")
@@ -130,15 +130,15 @@
 
         self.log_function(
             embs=self.store["input"],
             logits=self.store["output"],
             ids=ids,
         )
 
-    def on_test_begin(self, logs: Any = None) -> None:
+    def on_test_begin(self, logs: Optional[Any] = None) -> None:
         """At the beginning of the test we set the split to test.
         And generate the indices of the batches."""
         dq.set_split(Split.test)
         x_len = get_x_len(self.fit_kwargs.get("val_x"))
         if x_len is None:
             self.val_x_len_is_none = True
         else:
@@ -146,21 +146,21 @@
                 x=x_len,
                 batch_size=self.fit_kwargs.get(f"{Split.test}_batch_size")
                 or self.fit_kwargs["batch_size"],
                 steps_per_epoch=self.fit_kwargs.get(f"{Split.test}_steps"),
                 sample_weight=self.fit_kwargs.get("val_sample_weight"),
             )
 
-    def on_test_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the beginning of the batch we clear the helper
         data from the logger config."""
         self._clear_logger_config_helper_data()
         dq.set_split(Split.test)
 
-    def on_test_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the end of the test batch we log the input of the classifier
         and the output."""
         dq.set_split(Split.test)
         ids = self.store.get("indices_ids")
 
         if ids is None:
             step = batch
@@ -193,15 +193,15 @@
         else:
             self.store[f"{Split.validation}_indices"] = generate_indices(
                 x=x_len,
                 batch_size=predict_kwargs.get("batch_size"),
                 steps_per_epoch=predict_kwargs.get("steps"),
             )
 
-    def on_predict_batch_end(self, batch: int, logs: Any = None) -> None:
+    def on_predict_batch_end(self, batch: int, logs: Optional[Any] = None) -> None:
         """Log the validation batch"""
         dq.set_split(Split.validation)
         ids = self.store.get("indices_ids")
         if ids is None:
             step = batch
             ids = self.store.get(f"{Split.validation}_indices", {}).get(
                 f"epoch_0_{step}"
@@ -276,44 +276,47 @@
 
         return orig_func(*args, **kwargs)
 
     return train_step_wrapper
 
 
 def select_model_layer(
-    model: tf.keras.layers.Layer, layer: Optional[Union[tf.keras.layers.Layer, str]]
+    model: tf.keras.layers.Layer, layer: Union[tf.keras.layers.Layer, str, None] = None
 ) -> tf.keras.layers.Layer:
     """Selects the classifier layer from the model.
     :param model: The model.
-    :param layer: The layer to select. If the layer with the name
+    :param layer: The layer to select. If None, the layer with the name
     'classifier' is selected."""
-    chosen_layer = layer
-    if isinstance(chosen_layer, str) is None:
+    chosen_layer = None
+    if isinstance(layer, tf.keras.layers.Layer):
+        chosen_layer = layer
+    elif isinstance(layer, str):
         for model_layer in model.layers:
             if model_layer.name == layer:
                 chosen_layer = model_layer
                 break
     else:
+        layer = "classifier"
         for model_layer in model.layers:
-            if model_layer.name == "classifier":
+            if model_layer.name == layer:
                 chosen_layer = model_layer
                 break
-    assert chosen_layer is not None, GalileoException("Layer could not be found")
-    assert not isinstance(chosen_layer, str), GalileoException(
-        "Layer could not be found"
+
+    assert chosen_layer is not None, GalileoException(
+        f"Layer {layer} cannot be found, check that it exists in the model's summary."
     )
     return chosen_layer
 
 
 def _watch(
     logger_data: Dict[str, Any],
     logger_config: BaseLoggerConfig,
     log_function: Callable,
     model: tf.keras.layers.Layer,
-    layer: Any = None,
+    layer: Optional[Any] = None,
     seed: int = 42,
 ) -> None:
     """Internal watch function that is used to watch the model during training.
     :param logger_data: The store for temporary logger data
     :param logger_config: The configuration of the logger
     :param log_function: The function that is used to log the data
     :param model: The model that is watched
@@ -356,15 +359,17 @@
     patch_layer_call(
         chosen_layer,
         before_call=partial(save_input, logger_data),
         after_call=partial(save_output, logger_data),
     )
 
 
-def watch(model: tf.keras.layers.Layer, layer: Any = None, seed: int = 42) -> None:
+def watch(
+    model: tf.keras.layers.Layer, layer: Optional[Any] = None, seed: int = 42
+) -> None:
     """Watch a model and log the inputs and outputs of a layer.
     :param model: The model to watch
     :param layer: The layer to watch, if None the classifier layer is used
     :param seed: The seed to use for the model"""
     if not getattr(model, "_dq", False):
         model._dq = True
     else:
```

### Comparing `dataquality-0.8.9/dataquality/integrations/hf.py` & `dataquality-0.9.1a1/dataquality/integrations/hf.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     if HFCol.ner_tags in ds.features and hasattr(
         ds.features[HFCol.ner_tags].feature, "names"
     ):
         return ds.features[HFCol.ner_tags].feature.names
     # If there is an "ner_labels" column (like from the Galileo export), we can use that
     if HFCol.ner_labels in ds.features:
         return ds[HFCol.ner_labels][0]
-    # The user must provide them
+    # The user must provide label_names
     raise GalileoException(
         "Could not extract labels from Dataset. Provide `label_names` to the "
         "`tokenize_and_log_dataset` function as a list of strings"
     )
 
 
 @check_noop
@@ -187,19 +187,28 @@
         if ds_key not in Split.get_valid_keys():
             dq_split = Split.inference
             inference_name = ds_key
             kwargs = {"inference_name": inference_name}
             dataset = dataset.remove_columns([HFCol.gold_spans])
         else:
             dq_split = conform_split(ds_key)
-            # Filter out rows with no gold spans
-            dataset = dataset.filter(lambda row: len(row[HFCol.gold_spans]) != 0)
 
+        # Filter out rows with no tokens
+        dataset = dataset.filter(lambda row: len(row[HFCol.text_token_indices]) != 0)
         ids = list(range(len(dataset)))
         dataset = dataset.add_column(HFCol.id, ids)
+        ds_orig_len = len(dataset)
+        ds_len = len(dataset)
+        if ds_orig_len != ds_len:
+            warnings.warn(
+                f"We found {ds_orig_len-ds_len} empty samples in your dataset for "
+                f"split {ds_key}. These will not be logged to Galileo. If you are not "
+                "expecting these, you should inspect your original data",
+                GalileoWarning,
+            )
         tokenized_datasets[ds_key] = dataset
         split_meta = [c for c in meta if c in dataset.features]
         dq.log_dataset(
             dataset, split=dq_split, meta=split_meta, **kwargs  # type: ignore
         )
 
     return tokenized_datasets
```

### Comparing `dataquality-0.8.9/dataquality/integrations/keras.py` & `dataquality-0.9.1a1/dataquality/integrations/keras.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow import keras
 
 import dataquality as dq
 from dataquality.analytics import Analytics
@@ -94,28 +94,22 @@
 
     def on_epoch_begin(self, epoch: int, logs: Dict) -> None:
         dq.set_epoch(epoch)
 
     def _clear_logger_config_helper_data(self) -> None:
         dq.get_model_logger().logger_config.helper_data.clear()
 
-    def on_train_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         self._clear_logger_config_helper_data()
         dq.set_split(Split.train)
 
-    def on_train_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         dq.log_model_outputs(**dq.get_model_logger().logger_config.helper_data)
 
-    def on_test_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         # TODO: Somehow we should figure out whether this is in .fit
         #  (so really this should be val) or .evaluate (so this should be test)
         self._clear_logger_config_helper_data()
         dq.set_split(Split.test)
 
-    def on_test_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         dq.log_model_outputs(**dq.get_model_logger().logger_config.helper_data)
-
-
-# try:
-#     Analytics().log("import", "dataquality.keras")
-# except Exception:
-#     pass
```

### Comparing `dataquality-0.8.9/dataquality/integrations/spacy.py` & `dataquality-0.9.1a1/dataquality/integrations/spacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,21 @@
+from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Any, Callable, DefaultDict, Dict, Generator, List, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    DefaultDict,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+)
 
 import numpy as np
 import thinc
 from spacy.language import Language
 from spacy.ml.parser_model import ParserStepModel
 from spacy.ml.parser_model import precompute_hiddens as State2Vec
 from spacy.pipeline._parser_internals.stateclass import StateClass
@@ -11,22 +23,23 @@
 from spacy.tokens import Doc
 from spacy.training import Example
 from spacy.util import minibatch
 from thinc.api import set_dropout_rate
 from wrapt import CallableObjectProxy
 
 import dataquality
-from dataquality import check_noop, config
+from dataquality import config
 from dataquality.analytics import Analytics
 from dataquality.clients.api import ApiClient
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.logger_config.text_ner import text_ner_logger_config
 from dataquality.loggers.model_logger.text_ner import TextNERModelLogger
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split, conform_split
+from dataquality.utils.helpers import check_noop
 from dataquality.utils.spacy_integration import (
     convert_spacy_ents_for_doc_to_predictions,
     convert_spacy_ner_logits_to_valid_logits,
     validate_obj,
     validate_spacy_is_not_using_gpu,
     validate_spacy_version,
 )
@@ -35,15 +48,15 @@
 a.log_import("spacy")
 
 
 @check_noop
 def log_input_docs(
     docs: List[Doc],
     inference_name: str,
-    meta: Dict[str, List[Union[str, float, int]]] = None,
+    meta: Optional[Dict[str, List[Union[str, float, int]]]] = None,
 ) -> None:
     """Logs the input docs to the data logger.
 
     This function is used to log input docs to the data logger for an
     inference split.
 
     :param docs: List of spacy Doc objects to log.
@@ -80,15 +93,15 @@
     )
 
 
 @check_noop
 def log_input_examples(
     examples: List[Example],
     split: Union[Split, str],
-    meta: Dict[str, List[Union[str, float, int]]] = None,
+    meta: Optional[Dict[str, List[Union[str, float, int]]]] = None,
 ) -> None:
     """Logs a list of Spacy Examples using the dataquality client"""
     split = conform_split(split)
     if split == Split.inference:
         raise GalileoException(
             "`log_input_examples` cannot be used to log inference data. "
             "Try using `log_input_docs` instead."
@@ -137,15 +150,14 @@
     """Stores the nlp object before calling watch on the ner component within it
 
     We need access to the nlp object so that during training we can capture the
     model's predictions over the raw text by running nlp("user's text") and looking
     at the results
 
     :param nlp: The spacy nlp Language component.
-    :return: None
     """
     a.log_function("spacy/watch")
     validate_spacy_version()
     validate_spacy_is_not_using_gpu()
     if not (config.current_project_id and config.current_run_id):
         raise GalileoException(
             "You must initialize dataquality first! "
@@ -321,15 +333,15 @@
 
 
 @Language.factory("galileo_ner")
 def create_galileo_ner(nlp: Language, name: str) -> GalileoEntityRecognizer:
     return GalileoEntityRecognizer(nlp.get_pipe("ner"))
 
 
-class ThincModelWrapper(CallableObjectProxy):
+class ThincModelWrapper(CallableObjectProxy, ABC):
     """A Thinc Model obj wrapper using the wrapt library.
 
     wrapt primer: https://wrapt.readthedocs.io/en/latest/wrappers.html
     Wrapping an obj allows us to manipulate/watch its behavior. Compared to
     overwriting some of its functions, using an obj wrapper allows us to also
     maintain some state in between wrapped function calls. This also gives us a
     method of extending cython def classes to make them watchable. For example
@@ -351,14 +363,15 @@
         # https://github.com/python/mypy/issues/2427
         model._func = self._self_forward  # type: ignore
 
     def _self_get_unwrapt(self) -> thinc.model.Model:
         self.__wrapped__._func = self._self_orig_forward
         return self.__wrapped__
 
+    @abstractmethod
     def _self_forward(
         self, model: thinc.model.Model, X: Any, is_train: bool
     ) -> Tuple[Any, Any]:
         """Overwrite this to patch the Thinc model's forward fn"""
 
 
 class GalileoTransitionBasedParserModel(ThincModelWrapper):
@@ -509,19 +522,38 @@
                 )
                 docs_valid_logits[doc_id].append(valid_token_logits)
         return docs_valid_logits
 
     def _self_populate_model_logger(self, docs_valid_logits: DefaultDict) -> None:
         model_logger = self._self_model_logger
         helper_data = model_logger.log_helper_data
+
         model_logger.ids = list(model_logger.ids)  # for mypy's sake
+        # Set up the padded logits. We pad them to predict the O tag always, so
+        # they are never considered when we extract the spans from the tags
+        num_logits = len(next(iter(docs_valid_logits.values()))[0])
+        o_tag_idx = model_logger.logger_config.labels.index("O")
+        o_logits = np.array([1.0 if i == o_tag_idx else 0.0 for i in range(num_logits)])
+        max_doc_len = max(len(logits) for logits in docs_valid_logits.values())
         for doc_id, doc_valid_logits in docs_valid_logits.items():
-            model_logger.logits.append(np.array(doc_valid_logits))
             doc_embs = helper_data["embs"][doc_id]
-            model_logger.embs.append(np.array(doc_embs))
+            # Pad the input to the max logits/embs input
+            pad_size = max_doc_len - len(doc_valid_logits)
+            if pad_size:
+                # Pad just the end of the matrix with pad_size arrays
+                pad_config = ((0, pad_size), (0, 0))
+                doc_embs = np.pad(doc_embs, pad_config, constant_values=0)
+                # For logits, we use our special logits to ensure it's an O prediction
+                doc_valid_logits = np.resize(
+                    doc_valid_logits, (max_doc_len, num_logits)
+                )
+                doc_valid_logits[-pad_size:, :] = o_logits
+
+            cast(List, model_logger.logits).append(np.array(doc_valid_logits))
+            cast(List, model_logger.embs).append(np.array(doc_embs))
             model_logger.ids.append(doc_id)
 
     def _self_get_docs_copy(self) -> Dict[int, Doc]:
         spacy_states = self._self_model_logger.log_helper_data["spacy_states"]
         return {
             doc_id: states_for_doc[0].doc.copy()
             for doc_id, states_for_doc in spacy_states.items()
```

### Comparing `dataquality-0.8.9/dataquality/loggers/base_logger.py` & `dataquality-0.9.1a1/dataquality/loggers/base_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 import shutil
 from abc import abstractmethod
 from enum import Enum, unique
+from functools import lru_cache
 from glob import glob
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 
 from dataquality.core._config import ConfigData, config
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.logger_config.base_logger_config import (
     BaseLoggerConfig,
     base_logger_config,
 )
 from dataquality.schemas.split import Split, conform_split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.cloud import is_galileo_cloud
 from dataquality.utils.dq_logger import upload_dq_log_file
+from dataquality.utils.file import _shutil_rmtree_retry
 from dataquality.utils.imports import hf_available, tf_available, torch_available
 from dataquality.utils.tf import is_tf_2
 
 T = TypeVar("T", bound="BaseGalileoLogger")
 
 
 @unique
@@ -51,14 +53,15 @@
     pred_emb = "pred_emb"
     gold_emb = "gold_emb"
     pred_spans = "pred_spans"
     text_token_indices = "text_token_indices"
     text_token_indices_flat = "text_token_indices_flat"
     log_helper_data = "log_helper_data"
     inference_name = "inference_name"
+    image = "image"
 
     @staticmethod
     def get_valid() -> List[str]:
         return list(map(lambda x: x.value, BaseLoggerAttributes))
 
 
 class BaseGalileoLogger:
@@ -70,50 +73,104 @@
     LOG_FILE_DIR = f"{ConfigData.DEFAULT_GALILEO_CONFIG_DIR}/logs"
     logger_config: BaseLoggerConfig = base_logger_config
 
     def __init__(self) -> None:
         self.split: Optional[str] = None
         self.inference_name: Optional[str] = None
 
+    @property
+    def proj_run(self) -> str:
+        """Returns the project and run id
+
+        Example:
+            proj-id/run-id
+        """
+        return f"{config.current_project_id}/{config.current_run_id}"
+
+    @property
     def write_output_dir(self) -> str:
-        return (
-            f"{BaseGalileoLogger.LOG_FILE_DIR}/{config.current_project_id}/"
-            f"{config.current_run_id}"
-        )
+        """Returns the path to the output directory for the current run
 
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id
+        """
+        return f"{BaseGalileoLogger.LOG_FILE_DIR}/{self.proj_run}"
+
+    @property
     def split_name(self) -> str:
+        """Returns the name of the current split
+
+        If the split is inference, it will return the name of the inference
+        concatenated to the end of the split name
+
+        Example:
+            training
+            inference_inf-name1
+        """
         split = self.split
         if split == Split.inference:
             split = f"{split}_{self.inference_name}"
         return str(split)
 
+    @property
+    def split_name_path(self) -> str:
+        """Returns the path part of the current split
+
+        If the split is inference, it will return the name of the inference
+        run after the split name
+
+        Example:
+            training
+            inference/inf-name1
+        """
+        split = self.split
+        if split == Split.inference:
+            split = f"{split}/{self.inference_name}"
+        return str(split)
+
     @staticmethod
     def get_valid_attributes() -> List[str]:
         return BaseLoggerAttributes.get_valid()
 
     @abstractmethod
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """Validates params passed in during logging. Implemented by child"""
 
     def set_split_epoch(self) -> None:
+        """Sets the split for the current logger
+
+        If the split is not set, it will use the split set in the logger config
+        """
         if not self.split:
             if self.logger_config.cur_split:
                 self.split = self.logger_config.cur_split
             else:
                 raise GalileoException(
                     "You didn't log a split and did not set a split. Use "
                     "'dataquality.set_split' to set the split"
                 )
+
+        # Inference split must have inference name
+        if self.split == Split.inference and self.inference_name is None:
+            if self.logger_config.cur_inference_name is not None:
+                self.inference_name = self.logger_config.cur_inference_name
+            else:
+                raise GalileoException(
+                    "For inference split you must either log an inference name "
+                    "or set it before logging. Use `dataquality.set_split` to set "
+                    "inference_name"
+                )
+
         self.split = self.validate_split(self.split)
         # Set this config variable in validation, right before logging split data
         setattr(self.logger_config, f"{self.split}_logged", True)
 
     def is_valid(self) -> bool:
         try:
-            self.validate()
+            self.validate_and_format()
         except AssertionError:
             return False
         return True
 
     @classmethod
     def non_inference_logged(cls) -> bool:
         """Return true if training, test, or validation data is logged
@@ -202,38 +259,53 @@
             raise GalileoException(
                 f"Logged data should be of type int, string, pytorch tensor, "
                 f"or tf tensor, but got {type(v)}"
             )
         return v
 
     @staticmethod
-    def validate_task(task_type: Union[str, TaskType]) -> None:
-        if task_type not in TaskType.get_valid_tasks():
+    def validate_task(task_type: Union[str, TaskType]) -> TaskType:
+        """Raises error if task type is not a valid TaskType"""
+        try:
+            return TaskType[task_type]
+        except KeyError:
             raise GalileoException(
                 f"Task type {task_type} not valid. Choose one of "
                 f"{TaskType.get_valid_tasks()}"
             )
 
     @classmethod
     def _cleanup(cls) -> None:
-        """
-        Cleans up the current run data and metadata locally
+        """Cleans up the current run data and metadata locally
+
+        Does so by deleting the run directory and resetting the logger config
+
+        Example:
+            # Deletes all files in the run directory
+            /Users/username/.galileo/logs/proj-id/run-id
         """
         assert config.current_project_id
         assert config.current_run_id
         location = (
             f"{cls.LOG_FILE_DIR}/{config.current_project_id}"
             f"/{config.current_run_id}"
         )
         print("🧹 Cleaning up")
         for path in glob(f"{location}/*"):
             if os.path.isfile(path):
                 os.remove(path)
             else:
-                shutil.rmtree(path)
+                # Sometimes the directory is not deleted immediately
+                # This can happen if the client is using an nfs
+                # so we try again after a short delay
+                try:
+                    shutil.rmtree(path)
+                except OSError:
+                    _shutil_rmtree_retry(path)
+
         cls.logger_config.reset()
 
     def upload(self) -> None:
         ...
 
     @classmethod
     def get_all_subclasses(cls: Type[T]) -> List[Type[T]]:
@@ -253,14 +325,18 @@
 
     @classmethod
     def doc(cls) -> None:
         print(cls.__doc__)
 
     @classmethod
     def validate_split(cls, split: Union[str, Split]) -> str:
+        """Raises error if split is not a valid Split
+
+        Also raises if a cloud user tries to log inference data
+        """
         split = conform_split(split).value
         if is_galileo_cloud() and split == Split.inference:
             raise GalileoException(
                 "You cannot log inference data from a Galileo Cloud account, only "
                 "enterprise accounts can access this feature. Please email us at "
                 "team@rungalileo.io for more information."
             )
@@ -275,31 +351,36 @@
         # If a currently active thread crashed, check and raise a top level exception
         if cls.logger_config.exception:
             upload_dq_log_file()
             raise GalileoException(cls.logger_config.exception)
 
     @classmethod
     def is_hf_dataset(cls, df: Any) -> bool:
-        if hf_available:
+        if hf_available():
             import datasets
 
             return isinstance(df, datasets.Dataset)
         return False
 
+    @staticmethod
+    @lru_cache(1)
+    def _label_idx_map(labels: Tuple[str]) -> Dict[str, int]:
+        return {label: idx for idx, label in enumerate(labels)}
+
     @property
     def label_idx_map(self) -> Dict[str, int]:
         """Convert a list of labels to a dictionary of label to index
 
         Example:
         --------
         >>> labels = ["O", "B-PER", "I-PER", "B-LOC", "I-LOC"]
         >>> label_idx_map(labels)
         {"O": 0, "B-PER": 1, "I-PER": 2, "B-LOC": 3, "I-LOC": 4}
         """
-        return {label: idx for idx, label in enumerate(self.logger_config.labels or [])}
+        return self._label_idx_map(tuple(self.logger_config.labels or []))
 
     def labels_to_idx(self, gold_sequence: List[str]) -> np.ndarray:
         """Convert a list of labels to a np array of indices
 
         Example:
         --------
         # labels = ["O", "B-PER", "I-PER", "B-LOC", "I-LOC"]
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.1a1/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import gc
 import glob
 import os
-import shutil
 import sys
 import warnings
 from abc import abstractmethod
 from collections import Counter
-from typing import Any, Dict, Iterable, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
-import pyarrow as pa
 import vaex
 from vaex.dataframe import DataFrame
 
 from dataquality.clients.objectstore import ObjectStore
 from dataquality.core._config import config
 from dataquality.exceptions import GalileoException, GalileoWarning
 from dataquality.loggers.base_logger import BaseGalileoLogger, BaseLoggerAttributes
-from dataquality.schemas.dataframe import BaseLoggerInOutFrames, DFVar
+from dataquality.schemas.dataframe import BaseLoggerDataFrames, DFVar
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 from dataquality.utils import tqdm
 from dataquality.utils.cloud import is_galileo_cloud
-from dataquality.utils.hdf5_store import HDF5_STORE
+from dataquality.utils.cuda import cuml_available
+from dataquality.utils.emb import (
+    DATA_EMB_PATH,
+    apply_umap_to_embs,
+    upload_umap_data_embs,
+)
+from dataquality.utils.file import _shutil_rmtree_retry
 from dataquality.utils.helpers import galileo_verbose_logging
 from dataquality.utils.thread_pool import ThreadPoolManager
 from dataquality.utils.vaex import (
     _join_in_out_frames,
-    concat_hdf5_files,
-    create_data_embs,
+    create_data_embs_df,
     filter_df,
+    get_output_df,
     validate_unique_ids,
 )
 
 DATA_FOLDERS = ["emb", "prob", "data"]
 DataSet = TypeVar("DataSet", bound=Union[Iterable, pd.DataFrame, DataFrame])
 MetasType = TypeVar("MetasType", bound=Dict[str, List[Union[str, float, int]]])
 MetaType = TypeVar("MetaType", bound=Dict[str, Union[str, float, int]])
@@ -45,39 +49,62 @@
 try:
     vaex.progress.bar("vaex")
 except NameError:
     vaex.progress._progressbar_registry.registry["vaex"] = vaex.progress.simple
 
 
 class BaseGalileoDataLogger(BaseGalileoLogger):
+    """Base class for data loggers.
+
+    A document col is a large str > 1k chars < 10k chars
+    To avoid massive files, we limit the number of documents logged
+    """
+
     MAX_META_COLS = 25  # Limit the number of metadata attrs a user can log
-    MAX_STR_LEN = 1000  # Max characters in a string metadata attribute
+    MAX_STR_LEN = 1_000  # Max characters in a string metadata attribute
+    MAX_DOC_LEN = 10_000  # Max characters in document metadata attribute
+    LIMIT_NUM_DOCS = 3  # Limit the number of documents logged per split
     INPUT_DATA_BASE = "input_data"
     MAX_DATA_SIZE_CLOUD = 300_000
     # 2GB max size for arrow strings. We use 1.5GB for some buffer
     # https://issues.apache.org/jira/browse/ARROW-17828
     STRING_MAX_SIZE_B = 1.5e9
 
     DATA_FOLDER_EXTENSION = {data_folder: "hdf5" for data_folder in DATA_FOLDERS}
 
-    def __init__(self, meta: MetasType = None) -> None:
+    def __init__(self, meta: Optional[MetasType] = None) -> None:
         super().__init__()
         self.meta: Dict = meta or {}
         self.log_export_progress = True
 
+    @property
     def input_data_path(self) -> str:
-        return f"{self.write_output_dir()}/{BaseGalileoDataLogger.INPUT_DATA_BASE}"
+        """Return the path to the input data folder.
+
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id/input_data
+        """
+        return f"{self.write_output_dir}/{BaseGalileoDataLogger.INPUT_DATA_BASE}"
 
-    def input_data_file(self, input_num: int = None, split: str = None) -> str:
+    def input_data_file(
+        self, input_num: Optional[int] = None, split: Optional[str] = None
+    ) -> str:
+        """Return the path to the input data file.
+
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id/input_data/train/data_0.arrow
+        """
         if not split:
             assert self.split
             split = str(self.split)
         if input_num is None:
+            # input_data_logged is a dict of {split: input_num}
+            # where input_num is incremented in log()
             input_num = self.logger_config.input_data_logged[split]
-        return f"{self.input_data_path()}/{split}/data_{input_num}.arrow"
+        return f"{self.input_data_path}/{split}/data_{input_num}.arrow"
 
     @abstractmethod
     def log_data_sample(self, *, text: str, id: int, **kwargs: Any) -> None:
         """Log a single input sample. See child for details"""
 
     @abstractmethod
     def log_data_samples(
@@ -98,127 +125,184 @@
         **kwargs: Any,
     ) -> None:
         """Log a dataset/iterable of input samples.
 
         Provide the dataset and the keys to index into it. See child for details"""
 
     def validate_ids_for_split(self, ids: List[int]) -> None:
-        split = self.split_name()
+        """Validate ids for the current split
+
+        Validates:
+        - that the ids are unique for the current split
+        - that the ids are not already logged for the current split
+
+        On success:
+        - adds the ids to the logged_input_ids for the current split
+        """
+        split = self.split_name
         exc = (
             "If you've re-run a block of code or notebook cell that logs model "
             "outputs, that could be the cause. Try reinitializing with `dq.init` "
             "to clear your local environment, and then logging your data again. Call "
             "`dq.enable_galileo_verbose()` to see the duplicate IDs"
         )
         id_set = set(ids)
         if len(id_set) != len(ids):
             exc = "It seems you do not have unique ids in this logged data. " + exc
-            dups = {k: v for k, v in Counter(ids).items() if v > 1}
             if galileo_verbose_logging():
+                dups = {k: v for k, v in Counter(ids).items() if v > 1}
                 exc += f"split:{split}, dup ids and counts: {dups}"
             raise GalileoException(exc)
         # This means some logged ids were already logged!
         if len(id_set - self.logger_config.logged_input_ids[split]) != len(ids):
-            extra = self.logger_config.logged_input_ids[split].intersection(id_set)
             exc = "Some ids in this dataset were already logged for this split. " + exc
             if galileo_verbose_logging():
-                exc += f"split:{split}, overlapping ids: {extra}"
+                overlapping = self.logger_config.logged_input_ids[split].intersection(
+                    id_set
+                )
+                exc += f"split:{split}, overlapping ids: {overlapping}"
             raise GalileoException(exc)
+
         self.logger_config.logged_input_ids[split].update(ids)
 
     def add_ids_to_split(self, ids: List) -> None:
         if self.split:
             self.logger_config.idx_to_id_map[str(self.split)].extend(ids)
 
     def log(self) -> None:
         """Writes input data to disk in .galileo/logs
 
         If input data already exist, append new data to existing input file.
         If the dataset is very large this function will be called multiple
         times for a given split.
         """
-        self.validate()
-        write_input_dir = self.write_output_dir()
+        self.validate_and_format()
+        # E.g. /Users/username/.galileo/logs/proj-id/run-id
+        write_input_dir = self.write_output_dir
         os.makedirs(write_input_dir, exist_ok=True)
-        os.makedirs(f"{self.input_data_path()}/{self.split}", exist_ok=True)
+        # E.g. /Users/username/.galileo/logs/proj-id/run-id/training
+        os.makedirs(f"{self.input_data_path}/{self.split}", exist_ok=True)
 
         df = self._get_input_df()
+        # Validates cloud size limit
         self.validate_data_size(df)
+
         ids = df["id"].tolist()
         self.validate_ids_for_split(ids)
         self.add_ids_to_split(ids)
 
         file_path = self.input_data_file()
         if self.log_export_progress:
             with vaex.progress.tree("vaex", title=f"Logging {len(df)} samples"):
                 df.export(file_path)
         else:
             df.export(file_path)
 
         df.close()
         self.logger_config.input_data_logged[str(self.split)] += 1
 
+    @property
+    def support_data_embs(self) -> bool:
+        return True
+
     def upload(
         self, last_epoch: Optional[int] = None, create_data_embs: bool = False
     ) -> None:
         """
         Iterates through all of each splits children folders [data/emb/prob] for each
         inference name / epoch, concatenates all of the files with vaex, and uploads
         them to a single file in minio
 
         If create_data_embs is True, this will also run an off the shelf transformer
         and upload those text embeddings alongside the models finetuned embeddings
         """
+        # For linting
+        assert (
+            config.current_project_id and config.current_run_id
+        ), "You must call dq.init and train a model before calling finish"
         ThreadPoolManager.wait_for_threads()
         self.check_for_logging_failures()
         print("☁️ Uploading Data")
         object_store = ObjectStore()
         proj_run = f"{config.current_project_id}/{config.current_run_id}"
         location = f"{self.LOG_FILE_DIR}/{proj_run}"
 
+        if cuml_available():
+            apply_umap_to_embs(location, last_epoch)
+        else:
+            print(
+                "CuML libraries not found, running standard process. "
+                "For faster Galileo processing, consider installing\n"
+                "`pip install 'dataquality[cuda]' --extra-index-url="
+                "https://pypi.nvidia.com/`"
+            )
+
+        if cuml_available() and create_data_embs and self.support_data_embs:
+            print("Creating and uploading data embeddings")
+            upload_umap_data_embs(
+                config.current_project_id,
+                config.current_run_id,
+                self.input_data_path,
+                location,
+                last_epoch,
+            )
+            # We have already created them here, so don't try again later
+            create_data_embs = False
+
         for split in Split.get_valid_attributes():
-            split_loc = f"{location}/{split}"
-            input_logged = os.path.exists(f"{self.input_data_path()}/{split}")
-            output_logged = os.path.exists(split_loc)
-            if not output_logged:
-                continue
-            if not input_logged:
-                warnings.warn(
-                    f"There was output data logged for split {split} but no input data "
-                    "logged. Skipping upload for this split as there are no samples "
-                    "to join to.",
-                    GalileoWarning,
-                )
-                continue
-            in_frame_path = f"{self.input_data_path()}/{split}"
-            in_frame_split = vaex.open(f"{in_frame_path}/*.arrow")
-            in_frame_split = self.convert_large_string(in_frame_split)
             self.upload_split(
-                object_store,
-                in_frame_split,
-                split,
-                split_loc,
-                last_epoch,
-                create_data_embs,
+                location, split, object_store, last_epoch, create_data_embs
+            )
+
+    def upload_split(
+        self,
+        location: str,
+        split: str,
+        object_store: ObjectStore,
+        last_epoch: Optional[int],
+        create_data_embs: bool,
+    ) -> None:
+        split_loc = f"{location}/{split}"
+        in_frame_path = f"{self.input_data_path}/{split}"
+        input_logged = os.path.exists(in_frame_path)
+        output_logged = os.path.exists(split_loc)
+        if not output_logged:
+            return
+        if not input_logged:
+            warnings.warn(
+                f"There was output data logged for split {split} but no input data "
+                "logged. Skipping upload for this split as there are no samples "
+                "to join to.",
+                GalileoWarning,
             )
-            in_frame_split.close()
-            shutil.rmtree(in_frame_path)
-            gc.collect()
+            return
+        in_frame_split = vaex.open(f"{in_frame_path}/*.arrow")
+        in_frame_split = self.convert_large_string(in_frame_split)
+        self.upload_split_from_in_frame(
+            object_store,
+            in_frame_split,
+            split,
+            split_loc,
+            last_epoch,
+            create_data_embs,
+        )
+        in_frame_split.close()
+        _shutil_rmtree_retry(in_frame_path)
+        gc.collect()
 
     @classmethod
     def create_and_upload_data_embs(
         cls, df: DataFrame, split: str, epoch_or_inf: str
     ) -> None:
         """Uploads off the shelf data embeddings for a split"""
         object_store = ObjectStore()
         df_copy = df.copy()
-        # Create
-        data_embs = create_data_embs(df_copy)
+        data_embs = create_data_embs_df(df_copy)
         proj_run_split = f"{config.current_project_id}/{config.current_run_id}/{split}"
-        minio_file = f"{proj_run_split}/{epoch_or_inf}/data_emb/data_emb.hdf5"
+        minio_file = f"{proj_run_split}/{epoch_or_inf}/{DATA_EMB_PATH}"
         # And upload
         object_store.create_project_run_object_from_df(data_embs, minio_file)
 
     def convert_large_string(self, df: DataFrame) -> DataFrame:
         """Cast regular string to large_string for the text column
 
         Arrow strings have a max size of 2GB, so in order to export to hdf5 and
@@ -226,49 +310,49 @@
 
         We only do this for types that write to HDF5 files
         """
         df_copy = df.copy()
         # Characters are each 1 byte. If more bytes > max, it needs to be large_string
         text_bytes = df_copy["text"].str.len().sum()
         if text_bytes > self.STRING_MAX_SIZE_B:
-            df_copy["text"] = df_copy["text"].to_arrow().cast(pa.large_string())
+            df_copy["text"] = df_copy['astype(text, "large_string")']
         return df_copy
 
     @classmethod
-    def upload_split(
+    def upload_split_from_in_frame(
         cls,
         object_store: ObjectStore,
         in_frame: DataFrame,
         split: str,
         split_loc: str,
         last_epoch: Optional[int] = None,
         create_data_embs: bool = False,
     ) -> None:
-        # If set, last_epoch will only let you upload to and including the provided
-        # epoch value, nothing more.
-        # If None, then slicing a list [:None] will include all values
         epochs_or_infs = os.listdir(split_loc)
         epochs_or_infs = sorted(
             epochs_or_infs, key=lambda i: int(i) if split != Split.inference else i
         )
         # last_epoch is inclusive
         last_epoch = last_epoch + 1 if last_epoch else last_epoch
+        # If set, last_epoch will only let you upload to and including the provided
+        # epoch value, nothing more.
+        # If None, then slicing a list [:None] will include all values
         epochs_or_infs = epochs_or_infs[:last_epoch]
 
         largest_epoch = epochs_or_infs[-1]
 
         # For each inference name or epoch of the given split
         for epoch_or_inf in tqdm(
             epochs_or_infs,
             total=len(epochs_or_infs),
             desc=split,
             file=sys.stdout,
         ):
             input_batch = in_frame.copy()
-            prob_only = cls.prob_only(epochs_or_infs, split, epoch_or_inf)
+            prob_only = cls.prob_only(epochs_or_infs, split, epoch_or_inf, last_epoch)
             if split == Split.inference:
                 input_batch = filter_df(input_batch, "inference_name", epoch_or_inf)
                 if not len(input_batch):
                     warnings.warn(
                         "There was output data logged for inference_name "
                         f"{epoch_or_inf} but no input data logged. Skipping upload for "
                         "this inference run as there are no samples to join to.",
@@ -292,140 +376,144 @@
     def create_in_out_frames(
         cls,
         in_frame: DataFrame,
         dir_name: str,
         prob_only: bool,
         split: str,
         epoch_or_inf: Union[str, int],
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Formats the input data and model output data
 
         In this step, we concatenate the many hdf5 files created during model training
         and logging. We log those in threaded processes, and here we combine them
         into a single hdf5 file that vaex can read into a dataframe
 
         :param in_frame: the input dataframe
         :param dir_name: The directory of all of the output hdf5 files
         :param prob_only: If we are only uploading probability data. We only upload
             probability data for all epochs except the last one (we dont use cross-epoch
             embeddings currently, so we dont log them)
         :param split: The split we are logging for
         :param epoch_or_inf: The epoch or inference name we are logging for
         """
-        str_cols = concat_hdf5_files(dir_name, prob_only)
-        out_frame = vaex.open(f"{dir_name}/{HDF5_STORE}")
-
-        if split == Split.inference:
-            dtype: Union[str, None] = "str"
-            epoch_or_inf_name = "inference_name"
-        else:
-            dtype = None
-            epoch_or_inf_name = "epoch"
-
-        # Post concat, string columns come back as bytes and need conversion
-        for col in str_cols:
-            out_frame[col] = out_frame[col].to_arrow().cast(pa.large_string())
-        if prob_only:
-            out_frame["split"] = vaex.vconstant(
-                split, length=len(out_frame), dtype="str"
-            )
-            out_frame[epoch_or_inf_name] = vaex.vconstant(
-                epoch_or_inf, length=len(out_frame), dtype=dtype
-            )
-
+        out_frame = get_output_df(dir_name, prob_only, split, epoch_or_inf)
+        epoch_or_inf_name = "inference_name" if split == Split.inference else "epoch"
         return cls.process_in_out_frames(
             in_frame, out_frame, prob_only, epoch_or_inf_name, split
         )
 
     @classmethod
     def process_in_out_frames(
         cls,
         in_frame: DataFrame,
         out_frame: DataFrame,
         prob_only: bool,
         epoch_or_inf_name: str,
         split: str,
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Processes input and output dataframes from logging
 
         Validates uniqueness of IDs in the output dataframe
         Joins inputs and outputs
         Splits the dataframes into prob, emb, and data for uploading to minio
 
         :param in_frame: The input dataframe
         :param out_frame: The model output dataframe
         :param prob_only: If we are only uploading probabilities, or everything
         :param epoch_or_inf_name: The epoch or inference name we are uploading for
         """
         validate_unique_ids(out_frame, epoch_or_inf_name)
         in_out = _join_in_out_frames(in_frame, out_frame)
 
-        prob, emb, data_df = cls.split_dataframe(in_out, prob_only, split)
+        dataframes = cls.separate_dataframe(in_out, prob_only, split)
         # These df vars will be used in upload_in_out_frames
-        emb.set_variable("skip_upload", prob_only)
-        data_df.set_variable("skip_upload", prob_only)
+        dataframes.emb.set_variable("skip_upload", prob_only)
+        dataframes.data.set_variable("skip_upload", prob_only)
         epoch_inf_val = out_frame[[epoch_or_inf_name]][0][0]
-        prob.set_variable("progress_name", str(epoch_inf_val))
+        dataframes.prob.set_variable("progress_name", str(epoch_inf_val))
 
-        return BaseLoggerInOutFrames(prob=prob, emb=emb, data=data_df)
+        return dataframes
 
     @classmethod
     def upload_in_out_frames(
         cls,
         object_store: ObjectStore,
-        in_out_frames: BaseLoggerInOutFrames,
+        in_out_frames: BaseLoggerDataFrames,
         split: str,
         epoch_or_inf: Union[str, int],
     ) -> None:
         proj_run = f"{config.current_project_id}/{config.current_run_id}"
 
         prob = in_out_frames.prob
         emb = in_out_frames.emb
         data_df = in_out_frames.data
 
         epoch_inf = prob.variables.pop(DFVar.progress_name, "")
 
         name = "inf_name" if split == Split.inference else "epoch"
         desc = f"{split} ({name}={epoch_inf})"
+
         for data_folder, df_obj in tqdm(
             zip(DATA_FOLDERS, [emb, prob, data_df]),
             total=3,
             desc=desc,
             leave=False,
             file=sys.stdout,
         ):
             if df_obj.variables.get(DFVar.skip_upload):
                 continue
-
             ext = cls.DATA_FOLDER_EXTENSION[data_folder]
             minio_file = (
                 f"{proj_run}/{split}/{epoch_or_inf}/{data_folder}/{data_folder}.{ext}"
             )
+            cls._handle_numpy_types(df=df_obj)
             object_store.create_project_run_object_from_df(
                 df=df_obj, object_name=minio_file
             )
 
     @classmethod
+    def _handle_numpy_types(cls, df: DataFrame) -> None:
+        """Casts everything to float/int 32"""
+        for col, dt in zip(df.get_column_names(), df.dtypes):
+            if dt == "float" and dt != "float32":
+                df[col] = df[col].astype("float32")
+            elif dt == "int" and dt != "int32":
+                df[col] = df[col].astype("int32")
+
+    @classmethod
     def prob_only(
-        cls, epochs: List[str], split: str, epoch_or_inf_name: Union[int, str]
+        cls,
+        epochs: List[str],
+        split: str,
+        epoch_or_inf_name: Union[int, str],
+        last_epoch: Optional[int],
     ) -> bool:
         """Determines if we are only uploading probabilities
 
         For all epochs that aren't the last 2 (early stopping), we only want to
         upload the probabilities (for DEP calculation).
         """
         if split == Split.inference:  # Inference doesn't have DEP
             return False
 
         # If split is not inference, epoch_or_inf must be epoch
         epoch = int(epoch_or_inf_name)
         max_epoch_for_split = max([int(i) for i in epochs])
+        if last_epoch is not None:
+            max_epoch_for_split = min(max_epoch_for_split, last_epoch)
         return bool(epoch < max_epoch_for_split - 1)
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
+        """Validates the logger
+
+        Ensures that self.split is set, or sets it to the current split
+        from the logger_config.
+
+        Each child also defines an additional validate method that is called
+        """
         self.set_split_epoch()
 
     @classmethod
     @abstractmethod
     def validate_labels(cls) -> None:
         ...
 
@@ -436,16 +524,16 @@
                 f"The first {self.MAX_META_COLS} will be logged only.",
                 GalileoWarning,
             )
         # When logging metadata columns, if the user breaks a rule, don't fail
         # completely, just warn them and remove that metadata column
         # Cast to list for in-place dictionary mutation
         reserved_keys = BaseLoggerAttributes.get_valid()
-        valid_meta = {}
-        for key, values in list(self.meta.items())[: self.MAX_META_COLS]:
+        valid_meta_cols = []
+        for key, values in list(self.meta.items()):
             # Key must not override a default
             if key in reserved_keys:
                 warnings.warn(
                     f"Metadata column names must not override default values "
                     f"{reserved_keys}. Metadata field {key} "
                     f"will be removed.",
                     GalileoWarning,
@@ -466,30 +554,61 @@
                     f"Expected {batch_size} values for key {key} but got "
                     f"{len(values)}. Will not log this metadata column.",
                     GalileoWarning,
                 )
                 continue
             # Values must be a point, not an iterable
             valid_types = (str, int, float, np.floating, np.integer)
-            invalid_values = filter(
-                lambda t: not isinstance(t, valid_types)
-                or (isinstance(t, str) and len(t) > self.MAX_STR_LEN),
-                values,
-            )
+            invalid_values = filter(lambda t: not isinstance(t, valid_types), values)
             bad_val = next(invalid_values, None)
             if bad_val:
                 warnings.warn(
                     f"Metadata column {key} has one or more invalid values {bad_val} "
-                    f"of type {type(bad_val)}. Only strings of "
-                    f"len < {self.MAX_STR_LEN} and numbers can be logged.",
+                    f"of type {type(bad_val)}.",
                     GalileoWarning,
                 )
                 continue
-            valid_meta[key] = values
-        self.meta = valid_meta
+            valid_meta_cols.append(key)
+
+        def valid_str_col(df: DataFrame, key: str) -> bool:
+            """Valid str col checks length of longest str in metadata col"""
+            if df[key].dtype != "string":
+                return True
+
+            max_str_len = df[key].str.len().max()
+            if max_str_len > self.MAX_DOC_LEN:
+                warnings.warn(
+                    f"Metadata column {key} has one or more strings that are longer "
+                    f"than max document length of {self.MAX_DOC_LEN} characters. "
+                    "Will not log this metadata column.",
+                    GalileoWarning,
+                )
+                return False
+            if max_str_len > self.MAX_STR_LEN:
+                if len(self.logger_config.metadata_documents) >= self.LIMIT_NUM_DOCS:
+                    warnings.warn(
+                        "You have already logged limit of 3 document columns. A "
+                        "document column is a column that has max str length between"
+                        f"1,000 and 10,000 characters. Metadata column {key} has one "
+                        f"or more strings that are longer than {self.MAX_STR_LEN} "
+                        "characters. Will not log this metadata column.",
+                        GalileoWarning,
+                    )
+                    return False
+                else:
+                    self.logger_config.metadata_documents.add(key)
+
+            return True
+
+        df: DataFrame = vaex.from_dict(
+            {k: v for k, v in self.meta.items() if k in valid_meta_cols}
+        )
+        valid_meta_cols = [k for k in valid_meta_cols if valid_str_col(df, k)]
+        valid_meta_cols = valid_meta_cols[: self.MAX_META_COLS]  # Take first 25
+        self.meta = {k: v for k, v in self.meta.items() if k in valid_meta_cols}
 
     @staticmethod
     def get_data_logger_attr(cls: object) -> str:
         """
         Returns the attribute that corresponds to the logger in the class.
         This assumes only 1 logger object exists in the class
 
@@ -500,17 +619,17 @@
             member_class = getattr(cls, attr)
             if isinstance(member_class, BaseGalileoDataLogger):
                 return attr
         raise AttributeError("No data logger attribute found!")
 
     @classmethod
     @abstractmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = False, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
         ...
 
     def validate_kwargs(self, kwargs: Dict) -> None:
         """Raises if a function that shouldn't get kwargs gets any"""
         if kwargs.keys():
             raise GalileoException(f"Unexpected arguments: {tuple(kwargs.keys())}")
 
@@ -520,20 +639,24 @@
 
     @classmethod
     def set_tagging_schema(cls, tagging_schema: TaggingSchema) -> None:
         """Sets the tagging schema, if applicable. Must be implemented by child"""
         raise GalileoException(f"Cannot set tagging schema for {cls.__logger_name__}")
 
     def validate_data_size(self, df: DataFrame) -> None:
+        """Validates that the data size is within the limits of Galileo Cloud
+
+        If the data size is too large, a warning is raised.
+        """
         if not is_galileo_cloud():
             return
         samples_logged = len(df)
-        path_to_logged_data = f"{self.input_data_path()}/*/*arrow"
+        path_to_logged_data = f"{self.input_data_path}/*/*arrow"
         if glob.glob(path_to_logged_data):
-            samples_logged += len(vaex.open(f"{self.input_data_path()}/*/*arrow"))
+            samples_logged += len(vaex.open(f"{self.input_data_path}/*/*arrow"))
         nrows = BaseGalileoDataLogger.MAX_DATA_SIZE_CLOUD
         if samples_logged > nrows:
             warnings.warn(
                 f"⚠️ Hey there! You've logged over {nrows} rows in your input data. "
                 f"Galileo Cloud only supports up to {nrows} rows. "
                 "If you are using larger datasets, you may see degraded performance. "
                 "Please email us at team@rungalileo.io if you have any questions.",
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.1a1/dataquality/loggers/data_logger/text_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from collections import defaultdict
 from enum import Enum, unique
-from typing import Any, DefaultDict, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, DefaultDict, Dict, Iterable, List, Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 import vaex
 from vaex.dataframe import DataFrame
 
+import dataquality
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.data_logger.base_data_logger import (
     ITER_CHUNK_SIZE,
     BaseGalileoDataLogger,
     DataSet,
     MetasType,
     MetaType,
 )
 from dataquality.loggers.logger_config.text_classification import (
     text_classification_logger_config,
 )
 from dataquality.schemas import __data_schema_version__
+from dataquality.schemas.dataframe import BaseLoggerDataFrames
 from dataquality.schemas.split import Split
 from dataquality.utils.vaex import rename_df
 
 
 @unique
 class GalileoDataLoggerAttributes(str, Enum):
     texts = "texts"
@@ -71,20 +73,20 @@
     """
 
     __logger_name__ = "text_classification"
     logger_config = text_classification_logger_config
 
     def __init__(
         self,
-        texts: List[str] = None,
-        labels: List[str] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
-        inference_name: str = None,
+        texts: Optional[List[str]] = None,
+        labels: Optional[List[str]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Create data logger.
 
         :param texts: The raw text inputs for model training. List[str]
         :param labels: the ground truth labels aligned to each text field.
         List[str]
         :param ids: Optional unique indexes for each record. If not provided, will
@@ -251,34 +253,48 @@
     def _log_hf_dataset(
         self,
         dataset: Any,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
         meta: List[Union[str, int]],
-        label: Union[str, int] = None,
-        split: Split = None,
-        inference_name: str = None,
+        label: Optional[Union[str, int]] = None,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Helper function to log a huggingface dataset
 
         HuggingFace datasets can be sliced, returning a dict that is in the correct
         format to log directly.
         """
 
-        parse_label = lambda x: x  # noqa: E731
-        # If label is integer, convert to string #
-
-        if isinstance(dataset[0].get(label), int):
-            try:
-                parse_label = lambda x: dataset.features[label].int2str(x)  # noqa: E731
-            except Exception:
+        def parse_label(labels: Union[List[int], List[str]]) -> List[str]:
+            # If we have 1 str, they are all strings
+            if isinstance(labels[0], str):
+                return cast(List[str], labels)
+            # Otherwise they are all ints (typing)
+            else:
+                labels = cast(List[int], labels)
+            if hasattr(dataset.features[label], "int2str"):
+                return dataset.features[label].int2str(labels)
+            elif self.logger_config.labels:
+                return [self.logger_config.labels[gt] for gt in labels]
+            elif (
+                hasattr(dataset.features[label], "names")
+                and dataset.features[label].names
+            ):
+                classes = dataset.features[label].names
+                if not self.logger_config.labels:
+                    dataquality.set_labels_for_run(classes)
+                return [classes[gt] for gt in labels]
+            else:
                 # TODO: Simplify this logic with mapping the int label to string ticket
                 raise GalileoException(
-                    "Your dataset does not have label names. Please include them"
+                    "Your dataset does not have label names. Please include them or "
+                    "call dq.set_labels_for_run"
                 )
 
         assert dataset[0].get(id) is not None, GalileoException(
             f"id ({id}) field must be present in dataset"
         )
 
         for i in range(0, len(dataset), batch_size):
@@ -294,17 +310,17 @@
     def _log_iterator(
         self,
         dataset: Iterable,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
         meta: List[Union[str, int]],
-        label: Union[str, int] = None,
-        split: Split = None,
-        inference_name: str = None,
+        label: Optional[Union[str, int]] = None,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         batches = defaultdict(list)
         metas = defaultdict(list)
         for chunk in dataset:
             batches["text"].append(self._convert_tensor_to_py(chunk[text]))
             batches["id"].append(self._convert_tensor_to_py(chunk[id]))
             if label:
@@ -324,29 +340,33 @@
 
     def _process_label(self, batches: DefaultDict, label: Any) -> DefaultDict:
         """Process label for text-classification and multi-label accordingly"""
         batches["label"].append(self._convert_tensor_to_py(label))
         return batches
 
     def _log_dict(
-        self, d: Dict, meta: Dict, split: Split = None, inference_name: str = None
+        self,
+        d: Dict,
+        meta: Dict,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         self.log_data_samples(
             texts=d["text"],
             labels=d["label"],
             ids=d["id"],
             split=split,
             inference_name=inference_name,
             meta=meta,
         )
 
     def _log_df(
         self, df: Union[pd.DataFrame, DataFrame], meta: List[Union[str, int]]
     ) -> None:
-        """Helper to log a pandas or vex df"""
+        """Helper to log a pandas or vaex df"""
         self.texts = df["text"].tolist()
         self.ids = df["id"].tolist()
         # Inference case
         if "label" in df:
             self.labels = df["label"].tolist()
         for meta_col in meta:
             self.meta[str(meta_col)] = df[meta_col].tolist()
@@ -356,29 +376,28 @@
     def get_valid_attributes() -> List[str]:
         """
         Returns a list of valid attributes that this logger accepts
         :return: List[str]
         """
         return GalileoDataLoggerAttributes.get_valid()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * Text and Labels must both exist (unless split is 'inference' in which case
         labels must be None)
         * Text and Labels must be the same length
         * If ids exist, it must be the same length as text/labels
-        :return: None
 
         If the user logged labels as ints, convert them to the string labels.
         In the next optimization, we will support the API having int labels, but for
         now it expects string labels. When we make that change, we will do the opposite
         and always convert to the int index of the labels.
         """
-        super().validate()
+        super().validate_and_format()
         label_len = len(self.labels)
         text_len = len(self.texts)
         id_len = len(self.ids)
 
         set_labels_are_ints = self.logger_config.int_labels
 
         if self.split != Split.inference and str(self.labels[0]).isnumeric():
@@ -452,39 +471,40 @@
             **self.meta,
         )
         if self.inference_name:
             inp.update(inference_name=self.inference_name)
         return vaex.from_pandas(pd.DataFrame(inp))
 
     @classmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
-        """Splits the singular dataframe into its 3 components
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = True, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
+        """Separates the singular dataframe into its 3 components
 
         Gets the probability df, the embedding df, and the "data" df containing
         all other columns
         """
         df_copy = df.copy()
         # Separate out embeddings and probabilities into their own files
         prob_cols = cls._get_prob_cols()
         prob = df_copy[prob_cols]
 
         if prob_only:  # In this case, we don't care about the other columns
             emb_cols = ["id"]
             other_cols = ["id"]
         else:
-            emb_cols = ["id", "emb"]
-            ignore_cols = ["emb", "split_id"] + prob_cols
+            emb_cols = ["id", "emb", "x", "y", "emb_pca"]
+            emb_cols = [c for c in emb_cols if c in df_copy.get_column_names()]
+            ignore_cols = ["split_id"] + prob_cols + emb_cols
             other_cols = [i for i in df_copy.get_column_names() if i not in ignore_cols]
             other_cols += ["id"]
 
         emb = df_copy[emb_cols]
         data_df = df_copy[other_cols]
-        return prob, emb, data_df
+        return BaseLoggerDataFrames(prob=prob, emb=emb, data=data_df)
 
     @classmethod
     def _get_prob_cols(cls) -> List[str]:
         return ["id", "prob", "gold"]
 
     @classmethod
     def validate_labels(cls) -> None:
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.1a1/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,19 +67,19 @@
     __logger_name__ = "text_multi_label"
     logger_config: TextMultiLabelLoggerConfig = (
         text_multi_label_logger_config  # type: ignore
     )
 
     def __init__(
         self,
-        texts: List[str] = None,
-        labels: List[List[str]] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
+        texts: Optional[List[str]] = None,
+        labels: Optional[List[List[str]]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
     ) -> None:
         """Create data logger.
 
         :param text: The raw text inputs for model training. List[str]
         :param labels: the ground truth labels aligned to each text field.
         List[List[str]]
         :param ids: Optional unique indexes for each record. If not provided, will
@@ -134,16 +134,16 @@
     def log_data_samples(
         self,
         *,
         texts: List[str],
         ids: List[int],
         labels: Optional[List[str]] = None,
         split: Optional[Split] = None,
-        inference_name: str = None,
-        meta: MetasType = None,
+        inference_name: Optional[str] = None,
+        meta: Optional[MetasType] = None,
         task_labels: Optional[List[List[str]]] = None,
         **kwargs: Any,
     ) -> None:
         """Log input samples for text multi-label
 
         :param texts: List[str] text samples
         :param ids: List[int,str] IDs for each text sample
@@ -172,15 +172,19 @@
         # In binary multi-label, it will be a single string
         if self.logger_config.binary:
             return super()._process_label(batches, label)
         batches["label"].append(self._convert_tensor_ndarray(label).tolist())
         return batches
 
     def _log_dict(
-        self, d: Dict, meta: Dict, split: Split = None, inference_name: str = None
+        self,
+        d: Dict,
+        meta: Dict,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         self.log_data_samples(
             texts=d["text"],
             task_labels=d["label"],
             ids=d["id"],
             split=split,
             inference_name=inference_name,
@@ -215,24 +219,24 @@
                 if task in sample_label_set:
                     clean_sample_labels.append(task)
                 else:
                     clean_sample_labels.append(f"NOT_{task}")
             clean_task_labels.append(clean_sample_labels)
         self.labels = clean_task_labels
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Parent validation (text_classification) with additional validation on labels
 
         in multi_label modeling, each element in self.labels should itself be a list
         """
         if self.logger_config.binary:
             self._process_binary_labels()
         self.logger_config.observed_num_tasks = len(self.labels[0])
-        super().validate()
+        super().validate_and_format()
 
     def validate_logged_labels(self) -> None:
         for ind, input_labels in enumerate(self.labels):
             assert isinstance(
                 input_labels, (list, np.ndarray, pd.Series)
             ), "labels must be a list of lists in multi-label tasks"
             assert len(input_labels) == self.logger_config.observed_num_tasks, (
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.1a1/dataquality/loggers/data_logger/text_ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     BaseGalileoDataLogger,
     DataSet,
     MetasType,
     MetaType,
 )
 from dataquality.loggers.logger_config.text_ner import text_ner_logger_config
 from dataquality.schemas import __data_schema_version__
-from dataquality.schemas.dataframe import BaseLoggerInOutFrames, DFVar
+from dataquality.schemas.dataframe import BaseLoggerDataFrames, DFVar
 from dataquality.schemas.ner import NERColumns as NERCols
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 from dataquality.utils.vaex import rename_df
 
 
 @unique
@@ -110,21 +110,21 @@
     DATA_FOLDER_EXTENSION = {"emb": "hdf5", "prob": "hdf5", "data": "arrow"}
 
     __logger_name__ = "text_ner"
     logger_config = text_ner_logger_config
 
     def __init__(
         self,
-        texts: List[str] = None,
-        text_token_indices: List[List[Tuple[int, int]]] = None,
-        gold_spans: List[List[Dict]] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
-        inference_name: str = None,
+        texts: Optional[List[str]] = None,
+        text_token_indices: Optional[List[List[Tuple[int, int]]]] = None,
+        gold_spans: Optional[List[List[Dict]]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Create data logger.
 
         :param texts: The raw text inputs for model training. List[str]
         :param text_token_indices: Token boundaries of text. List[Tuple(int, int)].
         Used to convert the gold_spans into token level spans internally.
         t[0] indicates the start index of the span and t[1] is the end index (exclusive)
@@ -155,16 +155,16 @@
         return GalileoDataLoggerAttributes.get_valid()
 
     def log_data_samples(
         self,
         *,
         texts: List[str],
         ids: List[int],
-        text_token_indices: List[List[Tuple[int, int]]] = None,
-        gold_spans: List[List[Dict]] = None,
+        text_token_indices: Optional[List[List[Tuple[int, int]]]] = None,
+        gold_spans: Optional[List[List[Dict]]] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
         meta: Optional[MetasType] = None,
         **kwargs: Any,  # For typing
     ) -> None:
         """Log input samples for text NER
 
@@ -200,16 +200,16 @@
         self.log()
 
     def log_data_sample(
         self,
         *,
         text: str,
         id: int,
-        text_token_indices: List[Tuple[int, int]] = None,
-        gold_spans: List[Dict] = None,
+        text_token_indices: Optional[List[Tuple[int, int]]] = None,
+        gold_spans: Optional[List[Dict]] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
         meta: Optional[MetaType] = None,
         **kwargs: Any,
     ) -> None:
         """
         Log a single input sample for text classification
@@ -408,24 +408,23 @@
         self.ids = df["id"].tolist()
         self.text_token_indices = df["text_token_indices"].tolist()
         self.gold_spans = df["gold_spans"].tolist() if "gold_spans" in df else []
         for meta_col in meta:
             self.meta[str(meta_col)] = df[meta_col].tolist()
         self.log()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * Text and Labels must both exist (unless split is 'inference' in which case
         gold_spans must be None)
         * Text and Labels must be the same length
         * If ids exist, it must be the same length as text/labels
-        :return: None
         """
-        super().validate()
+        super().validate_and_format()
         assert self.logger_config.labels, (
             "You must set your labels before logging input data. "
             "See dataquality.set_labels_for_run"
         )
 
         assert self.logger_config.tagging_schema, (
             "You must set your tagging schema before logging input data. "
@@ -461,14 +460,16 @@
 
             assert text_len == text_tokenized_len == gold_span_len, (
                 f"gold spans, text, and tokenized text must be the same length for "
                 f"split {self.split}, but got (gold spans, text, text_token) "
                 f"({gold_span_len},{text_len},{text_tokenized_len})"
             )
 
+        self.text_token_indices_flat = []
+
         for sample_id, sample_spans, sample_indices, sample_text in zip(
             self.ids,
             self.gold_spans or [None] * id_len,  # type: ignore
             self.text_token_indices,
             self.texts,
         ):
             sample_key = self.logger_config.get_sample_key(Split(self.split), sample_id)
@@ -615,34 +616,36 @@
     def process_in_out_frames(
         cls,
         in_frame: DataFrame,
         out_frame: DataFrame,
         prob_only: bool,
         epoch_or_inf_name: str,
         split: str,
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Processes input and output dataframes from logging
 
         NER is a different case where the input data is logged at the sample level,
         but output data is logged at the span level, so we need to process it
         differently
 
         We don't have span IDs so we don't need to validate uniqueness
         We don't join the input and output frames
         We do need to split take only the rows from in_frame from this split
         Splits the dataframes into prob, emb, and input data for uploading to minio
         """
         cls._validate_duplicate_spans(out_frame, epoch_or_inf_name)
-        prob, emb, _ = cls.split_dataframe(out_frame, prob_only, split)
+        dataframes = cls.separate_dataframe(out_frame, prob_only, split)
+        # For NER data is the input data
+        dataframes.data = in_frame
         # These df vars will be used in upload_in_out_frames
-        emb.set_variable(DFVar.skip_upload, prob_only)
-        in_frame.set_variable(DFVar.skip_upload, prob_only)
+        dataframes.emb.set_variable(DFVar.skip_upload, prob_only)
+        dataframes.data.set_variable(DFVar.skip_upload, prob_only)
         epoch_inf_val = out_frame[[epoch_or_inf_name]][0][0]
-        prob.set_variable(DFVar.progress_name, str(epoch_inf_val))
-        return BaseLoggerInOutFrames(prob=prob, emb=emb, data=in_frame)
+        dataframes.prob.set_variable(DFVar.progress_name, str(epoch_inf_val))
+        return dataframes
 
     @classmethod
     def _validate_duplicate_spans(cls, df: DataFrame, epoch_or_inf_name: str) -> None:
         """Validates that duplicate spans aren't logged for an input sample
 
         Duplicate spans would be spans in a sample with identical start and end spans
         """
@@ -653,17 +656,17 @@
             raise GalileoException(
                 "It seems as though you have duplicate spans for samples in this "
                 f"split. (split:{split}, {epoch_or_inf_name}:{epoch_or_inf_value}),"
                 f"dups:\n {dup_counts[['sample_id', 'count']].to_records()}"
             )
 
     @classmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = True, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
         """Splits the dataframe into logical grouping for minio storage
 
         NER is a different case, where we store the text samples as "data" and
         all of the span level data is split into only "emb" and "prob". This function
         will only return 2 modified dataframes, where the third is expected to be the
         input data logged by the user
         """
@@ -692,16 +695,20 @@
                 NERCols.galileo_error_type.value,
             ]
 
         prob = df_copy[prob_cols]
         emb_cols = (
             [NERCols.id.value] if prob_only else [NERCols.id.value, NERCols.emb.value]
         )
+        # In the event that we did dimensionality reduction locally with nvidia
+        for col in ["x", "y", "emb_pca"]:
+            if col in df_copy.get_column_names():
+                emb_cols.append(col)
         emb = df_copy[emb_cols]
-        return prob, emb, df_copy
+        return BaseLoggerDataFrames(prob=prob, emb=emb, data=df_copy)
 
     @classmethod
     def validate_labels(cls) -> None:
         """Validates and cleans labels, see _clean_labels and saves ner_labels
 
         ner_labels are all of the labels that start with a tag (B-, I-, E- etc) as well
         as the O tag
@@ -775,14 +782,19 @@
             or label.startswith("U-")
         )
 
     @classmethod
     def set_tagging_schema(cls, tagging_schema: TaggingSchema) -> None:
         cls.logger_config.tagging_schema = tagging_schema
 
+    @property
+    def support_data_embs(self) -> bool:
+        """Not yet supported for NER. Coming soon!"""
+        return False
+
     @classmethod
     def create_and_upload_data_embs(
         cls, df: DataFrame, split: str, epoch_or_inf: str
     ) -> None:
         """Not yet supported for NER. Coming soon!"""
         warnings.warn(
             "Data embeddings are not yet supported for NER. Coming soon!",
```

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.1a1/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Any, DefaultDict, Dict, List, Optional, Set
+from typing import Any, Callable, DefaultDict, Dict, List, Optional, Set
 
 from pydantic import BaseModel, validator
 
 from dataquality.schemas.condition import Condition
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 
@@ -27,14 +27,17 @@
     input_data_logged: DefaultDict[str, int] = defaultdict(int)
     logged_input_ids: DefaultDict[str, Set] = defaultdict(set)
     idx_to_id_map: DefaultDict[str, List] = defaultdict(list)
     conditions: List[Condition] = []
     report_emails: List[str] = []
     ner_labels: List[str] = []
     int_labels: bool = False
+    feature_names: List[str] = []
+    metadata_documents: Set = set()  # A document is a large str > 1k chars < 10k chars
+    finish: Callable = lambda: None  # Overwritten in Semantic Segmentation
 
     class Config:
         validate_assignment = True
 
     def reset(self, factory: bool = False) -> None:
         """Reset all class vars"""
         self.__init__()  # type: ignore
```

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.1a1/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.1a1/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.1a1/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.1a1/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from dataquality.exceptions import GalileoException, GalileoWarning, LogBatchError
 from dataquality.loggers.base_logger import BaseGalileoLogger
 from dataquality.loggers.data_logger import BaseGalileoDataLogger
 from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.ampli import AmpliMetric
 from dataquality.utils.dq_logger import get_dq_logger
+from dataquality.utils.hdf5_store import _save_hdf5_file
 from dataquality.utils.thread_pool import ThreadPoolManager
-from dataquality.utils.vaex import _save_hdf5_file
 
 analytics = Analytics(ApiClient, config)  # type: ignore
 
 
 class BaseGalileoModelLogger(BaseGalileoLogger):
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List, np.ndarray] = None,
-        logits: Union[List, np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List, np.ndarray]] = None,
+        logits: Optional[Union[List, np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__()
         # Need to compare to None because they may be np arrays which cannot be
         # evaluated with bool directly
@@ -51,15 +51,15 @@
         (something is wrong)
 
         If validation fails with a LogBatchError, we simply warn and skip logging this
         batch, but do not halt model training
         (this batch is bad, but we can continue logging)
         """
         try:
-            self.validate()
+            self.validate_and_format()
         except AssertionError as e:
             get_dq_logger().error(
                 "Validation of data failed", split=self.split, epoch=self.epoch
             )
             raise GalileoException(
                 f"The provided logged data is invalid: {e}"
             ) from None
@@ -95,53 +95,36 @@
     def log(self) -> None:
         """The top level log function that try/excepts its child"""
         self.check_for_logging_failures()
         # We validate split and epoch before entering the thread because we reference
         # global variables (cur_split and cur_epoch) that are subject to change
         # between subsequent threads
         self.set_split_epoch()
-        get_dq_logger().debug(
-            "Starting logging process from thread", split=self.split, epoch=self.epoch
-        )
         ThreadPoolManager.add_thread(target=self._add_threaded_log)
 
     def write_model_output(self, data: Dict) -> None:
         """Creates an hdf5 file from the data dict"""
-        get_dq_logger().debug(
-            "Writing model output", split=self.split, epoch=self.epoch
-        )
         location = (
             f"{self.LOG_FILE_DIR}/{config.current_project_id}"
             f"/{config.current_run_id}"
         )
         split = data["split"][0]
 
         if split == Split.inference:
             inference_name = data["inference_name"][0]
             path = f"{location}/{split}/{inference_name}"
         else:
             epoch = data["epoch"][0]
             path = f"{location}/{split}/{epoch}"
 
         object_name = f"{str(uuid4()).replace('-', '')[:12]}.hdf5"
-        get_dq_logger().debug("Saving hdf5 file", split=self.split)
         _save_hdf5_file(path, object_name, data)
 
     def set_split_epoch(self) -> None:
         super().set_split_epoch()
-        # Inference split must have inference name
-        if self.split == Split.inference and self.inference_name is None:
-            if self.logger_config.cur_inference_name is not None:
-                self.inference_name = self.logger_config.cur_inference_name
-            else:
-                raise GalileoException(
-                    "For inference split you must either log an inference name "
-                    "or set it before logging. Use `dataquality.set_split` to set"
-                    "inference_name"
-                )
 
         # Non-inference split must have an epoch
         if self.split != Split.inference and self.epoch is None:
             if self.logger_config.cur_epoch is not None:
                 self.epoch = self.logger_config.cur_epoch
             else:
                 raise GalileoException(
@@ -188,13 +171,16 @@
         self, sample_logits: Union[List[np.ndarray], np.ndarray]
     ) -> np.ndarray:
         """Converts logits to probs via softmax"""
         # axis ensures that in a matrix of probs with dims num_samples x num_classes
         # we take the softmax for each sample
         if not isinstance(sample_logits, np.ndarray):
             sample_logits = self._convert_tensor_ndarray(sample_logits)
-        if len(sample_logits.shape) == 1 or sample_logits.shape[1] == 1:
+
+        # If shape is (num_samples, 1) or (num_samples,) then we have a binary case
+        if len(sample_logits.shape) == 1 or sample_logits.shape[-1] == 1:
             if len(sample_logits.shape) > 1:
                 # Remove final empty dimension if it's there
                 sample_logits = sample_logits.reshape(-1)
             return self.convert_logits_to_prob_binary(sample_logits)
+
         return softmax(np.array(sample_logits), axis=-1)
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.1a1/dataquality/loggers/model_logger/text_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from enum import Enum, unique
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 
 from dataquality.loggers.logger_config.text_classification import (
     text_classification_logger_config,
@@ -71,18 +70,18 @@
     """
 
     __logger_name__ = "text_classification"
     logger_config = text_classification_logger_config
 
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List, np.ndarray] = None,
-        logits: Union[List, np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List, np.ndarray]] = None,
+        logits: Optional[Union[List, np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
@@ -111,40 +110,36 @@
         """
         try:
             has_len = len(arr) != 0
         except TypeError:
             has_len = bool(arr.shape[0])
         return has_len
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        get_dq_logger().debug("Handling logits and probs", split=self.split)
         has_logits = self._has_len(self.logits)
         has_probs = self._has_len(self.probs)
         if has_logits:
             self.logits = self._convert_tensor_ndarray(self.logits, "Prob")
             self.probs = self.convert_logits_to_probs(self.logits)
             del self.logits
         elif has_probs:
-            warnings.warn("Usage of probs is deprecated, use logits instead")
             self.probs = self._convert_tensor_ndarray(self.probs, "Prob")
 
-        get_dq_logger().debug("Converting inputs to numpy arrays", split=self.split)
         self.embs = self._convert_tensor_ndarray(self.embs, "Embedding")
         self.ids = self._convert_tensor_ndarray(self.ids)
 
         embs_len = len(self.embs)
         probs_len = len(self.probs)
         ids_len = len(self.ids)
 
-        get_dq_logger().debug("Validating embedding shape", split=self.split)
         assert self.embs.ndim == 2, "Only one embedding vector is allowed per input."
 
         assert embs_len and probs_len and ids_len, (
             f"All of emb, probs, and ids for your logger must be set, but "
             f"got emb:{bool(embs_len)}, probs:{bool(probs_len)}, ids:{bool(ids_len)}"
         )
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.1a1/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,39 +58,39 @@
     __logger_name__ = "text_multi_label"
     logger_config: TextMultiLabelLoggerConfig = (
         text_multi_label_logger_config  # type: ignore
     )
 
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List[List[List]], List[np.ndarray]] = None,
-        logits: Union[List[List[List]], List[np.ndarray]] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List[List[List]], List[np.ndarray]]] = None,
+        logits: Optional[Union[List[List[List]], List[np.ndarray]]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
             logits=logits,
             ids=ids,
             split=split,
             epoch=epoch,
             inference_name=inference_name,
         )
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        super().validate()
+        super().validate_and_format()
         for ind, probs_per_task in enumerate(self.probs):
             assert len(probs_per_task) == self.logger_config.observed_num_tasks, (
                 f"Expected {self.logger_config.observed_num_tasks} probability vectors "
                 f"per input (based on input data logging) but found "
                 f"{len(probs_per_task)} for input {ind}."
             )
             for task_ind, task_probs in enumerate(probs_per_task):
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.1a1/dataquality/loggers/model_logger/text_ner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import warnings
 from collections import defaultdict
 from enum import Enum, unique
 from typing import Any, DefaultDict, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from numpy import ndarray
 
 from dataquality.exceptions import LogBatchError
 from dataquality.loggers.logger_config.text_ner import text_ner_logger_config
 from dataquality.loggers.model_logger.base_model_logger import BaseGalileoModelLogger
 from dataquality.schemas import __data_schema_version__
 from dataquality.schemas.ner import NERErrorType, NERProbMethod, TaggingSchema
 from dataquality.schemas.split import Split
-from dataquality.utils.dq_logger import get_dq_logger
 from dataquality.utils.ml import select_span_token_for_prob
 
 
 @unique
 class GalileoModelLoggerAttributes(str, Enum):
     gold_emb = "gold_emb"
     gold_spans = "gold_spans"
@@ -93,35 +91,31 @@
     """
 
     __logger_name__ = "text_ner"
     logger_config = text_ner_logger_config
 
     def __init__(
         self,
-        embs: List[np.ndarray] = None,
-        probs: List[np.ndarray] = None,
-        logits: List[np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[List[np.ndarray]] = None,
+        probs: Optional[List[np.ndarray]] = None,
+        logits: Optional[List[np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
             logits=logits,
             ids=ids,
             split=split,
             epoch=epoch,
             inference_name=inference_name,
         )
-        # Explicit cast to List from parent
-        self.embs: List[np.ndarray] = list(self.embs)
-        self.logits: List[np.ndarray] = list(self.logits)
-        self.probs: List[np.ndarray] = list(self.probs)
 
         # Calculated internally
         self.gold_emb: List[List[np.ndarray]] = []
         self.gold_spans: List[List[Dict]] = []
         self.gold_conf_prob: List[List[np.ndarray]] = []
         self.gold_loss_prob: List[List[np.ndarray]] = []
         self.gold_loss_prob_label: List[List[int]] = []
@@ -138,33 +132,31 @@
     def get_valid_attributes() -> List[str]:
         """
         Returns a list of valid attributes that GalileoModelConfig accepts
         :return: List[str]
         """
         return GalileoModelLoggerAttributes.get_valid()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        get_dq_logger().debug(
-            "Validating the output log.", split=self.split, epoch=self.epoch
-        )
         if len(self.logits):
-            self.probs = self.convert_logits_to_probs(self.logits).tolist()
+            self.probs = self.convert_logits_to_probs(self.logits)
         elif len(self.probs):
-            warnings.warn("Usage of probs is deprecated, use logits instead")
+            self.probs = self._convert_tensor_ndarray(self.probs)
 
         embs_len = len(self.embs)
         probs_len = len(self.probs)
         ids_len = len(self.ids)
 
         self.ids = self._convert_tensor_ndarray(self.ids)
+        self.embs = self._convert_tensor_ndarray(self.embs)
 
         assert all([embs_len, probs_len, ids_len]), (
             f"All of emb, probs, and ids for your logger must be set, but "
             f"got emb:{bool(embs_len)}, probs:{bool(probs_len)}, ids:{bool(ids_len)}"
         )
 
         assert embs_len == probs_len == ids_len, (
@@ -173,16 +165,14 @@
         )
 
         # We need to average the embeddings for the tokens within a span
         # so each span has only 1 embedding vector
         logged_sample_ids = []
         for sample_id, sample_emb, sample_prob in zip(self.ids, self.embs, self.probs):
             # This will return True if there was a prediction or gold span
-            sample_emb = self._convert_tensor_ndarray(sample_emb)
-            sample_prob = self._convert_tensor_ndarray(sample_prob)
             if self._process_sample(sample_id, sample_emb, sample_prob):
                 logged_sample_ids.append(sample_id)
 
         self.ids = logged_sample_ids
         if not self.ids:
             raise LogBatchError(
                 "No samples in this batch had any gold or prediction spans. "
@@ -195,17 +185,14 @@
         """Processes a sample. Returns whether or not the sample should be logged
 
         A sample should be logged only if there was at least 1 prediction span or 1
         gold span
 
         For inference mode, only prediction spans should be logged.
         """
-        get_dq_logger().debug(
-            "Processing a sample.", split=self.split, epoch=self.epoch
-        )
         # To extract metadata about the sample we are looking at
         sample_key = self.logger_config.get_sample_key(Split(self.split), sample_id)
 
         # Unpadded length of the sample. Used to extract true predicted spans
         # which are padded by the model
         sample_token_len = self.logger_config.sample_length[sample_key]
         # Remove padding from prob vector as well
@@ -242,22 +229,25 @@
             gold_sequence = self._construct_gold_sequence(
                 len(sample_prob), sample_gold_spans
             )
             gold_conf_prob, _ = self._extract_span_probs(
                 sample_gold_spans, sample_prob, NERProbMethod.confidence
             )
             gold_loss_prob, gold_loss_label = self._extract_span_probs(
-                sample_gold_spans, sample_prob, NERProbMethod.loss, gold_sequence
+                sample_gold_spans,
+                sample_prob,
+                NERProbMethod.loss,
+                gold_sequence_str=gold_sequence,
             )
-            argmax_indices: List[int] = sample_prob.argmax(axis=1).tolist()
-            pred_sequence: List[str] = [
-                self.logger_config.labels[x] for x in argmax_indices
-            ]
+            pred_sequence_idx = sample_prob.argmax(axis=1)
             pred_loss_prob, pred_gold_label = self._extract_span_probs(
-                sample_pred_spans, sample_prob, NERProbMethod.loss, pred_sequence
+                sample_pred_spans,
+                sample_prob,
+                NERProbMethod.loss,
+                gold_sequence_idx=pred_sequence_idx,
             )
 
             self.gold_spans.append(sample_gold_spans)
             self.gold_emb.append(gold_emb)
             self.gold_conf_prob.append(gold_conf_prob)
             self.gold_loss_prob.append(gold_loss_prob)
             self.pred_loss_prob.append(pred_loss_prob)
@@ -270,32 +260,30 @@
         self, spans: List[Dict], emb: np.ndarray
     ) -> List[np.ndarray]:
         """Get the embeddings for each span, on a per-sample basis
 
         We take the average of the token embeddings per span and use that as the span
         level embedding
         """
-        get_dq_logger().debug(
-            "Extracting span embeddings.", split=self.split, epoch=self.epoch
-        )
         embeddings = []
         for span in spans:
             start = span["start"]
             end = span["end"]
             span_embeddings = emb[start:end, :]
             avg_span_embedding = span_embeddings.mean(axis=0)
             embeddings.append(avg_span_embedding)
         return embeddings
 
     def _extract_span_probs(
         self,
         spans: List[Dict],
         prob: np.ndarray,
         method: NERProbMethod,
-        gold_sequence: Optional[List[str]] = None,
+        gold_sequence_str: Optional[List[str]] = None,
+        gold_sequence_idx: Optional[np.ndarray] = None,
     ) -> Tuple[List[np.ndarray], List[int]]:
         """Get the probs for each span, on a per-sample basis
 
         Parameters
         ----------
         spans
             The spans to extract probs for
@@ -308,28 +296,33 @@
         Returns
         -------
         List[np.ndarray]
             The probs for each span
         List[int]
             The gold label indices of token chosen for loss (needed for DEP calculation)
         """
-        get_dq_logger().debug(
-            "Extracting span probs.", split=self.split, epoch=self.epoch
-        )
         probs = []
         gold_labels = []
-        gold_sequence_str = gold_sequence or []
-        gold_sequence_idx = self.labels_to_idx(gold_sequence_str)
+        if gold_sequence_idx is None and gold_sequence_str is not None:
+            gold_sequence_idx = self.labels_to_idx(gold_sequence_str)
+
+        has_gold_sequence = (
+            gold_sequence_idx is not None and len(gold_sequence_idx) >= 0
+        )
 
         for span in spans:
             start = span["start"]
             end = span["end"]
             span_probs = prob[start:end, :]
+            # We ignore because if `has_gold_sequence` then has_gold_sequence must exist
+            # (see above), but mypy can't figure that out
             span_gold_seq = (
-                gold_sequence_idx[start:end] if gold_sequence_idx.size > 0 else None
+                gold_sequence_idx[start:end]  # type: ignore
+                if has_gold_sequence
+                else None
             )
             # We select a token prob to represent the span prob
             span_prob, gold_label = select_span_token_for_prob(
                 span_probs, method, span_gold_seq
             )
             probs.append(span_prob)
             # If method is 'loss' we return a list of gold labels
@@ -344,17 +337,14 @@
         """
         Extract prediction labels from probabilities, and generate pred spans
 
         If the schema is non-BIO, we just first convert them into BIO then extract spans
         """
         # use length of the tokens stored to strip the pads
         # Drop the spans post first PAD
-        get_dq_logger().debug(
-            "Extracting pred spans.", split=self.split, epoch=self.epoch
-        )
         argmax_indices: List[int] = pred_prob.argmax(axis=1)
         pred_sequence: List[str] = [
             self.logger_config.labels[x] for x in argmax_indices
         ]
 
         if self.logger_config.tagging_schema == TaggingSchema.BIO:
             pred_spans = self._extract_spans_bio(pred_sequence)
@@ -510,17 +500,14 @@
     ) -> List[str]:
         """
         Using gold spans and tagging schema, construct the underlying gold sequence
         e.g. gold_spans = [{start=5, end=8, label="nothing"}]
         gold_sequence = [O, O, O, O, O, B-nothing, I-nothing, I-nothing, O, O] for BIO
         gold_sequence = [O, O, O, O, O, B-nothing, I-nothing, L-nothing, O, O] for BILOU
         """
-        get_dq_logger().debug(
-            "Constructing a gold sequence", split=self.split, epoch=self.epoch
-        )
         gold_sequence = ["O"] * len_sequence
         for span in gold_spans:
             start = span["start"]
             end = span["end"]
             label = span["label"]
             if self.logger_config.tagging_schema == TaggingSchema.BIO:
                 gold_sequence[start:end] = [f"I-{label}"] * (end - start)
@@ -548,16 +535,14 @@
         will have repeating "sentence_id" values, which is OK. We will also loop
         through the data twice, once for prediction span information
         (one of pred_span, pred_emb, pred_prob per span) and once for gold span
         information (one of gold_span, gold_emb, gold_prob per span)
 
         NOTE: All spans are at the token level in this fn
         """
-        get_dq_logger().debug("Getting data dict.", split=self.split, epoch=self.epoch)
-
         if self.split == Split.inference:
             return self._get_data_dict_inference()
 
         data: defaultdict = defaultdict(list)
 
         # Loop through samples
         num_samples = len(self.ids)
@@ -805,17 +790,14 @@
         When indices don't match, the error is either span_shift or missed_label
         * span_shift: overlapping span start/end indices
         * missed_label: no overlap between span start/end indices
 
         In this function, we only look at spans that don't have pred/gold alignment,
         so the error can only be span_shift or missed_label.
         """
-        get_dq_logger().debug(
-            "Getting span error type.", split=self.split, epoch=self.epoch
-        )
         gold_start, gold_end = gold_span
         # We start by assuming missed_label (because it's the worst case)
         # and update if we see overlap
         error_type = NERErrorType.missed_label
         for pred_span in pred_spans:
             pred_start, pred_end = pred_span
             # We compare to the end of the spans non-inclusive because
@@ -834,22 +816,7 @@
     def __setattr__(self, key: Any, value: Any) -> None:
         if key not in self.get_valid_attributes():
             raise AttributeError(
                 f"{key} is not a valid attribute of {self.__logger_name__} logger. "
                 f"Only {self.get_valid_attributes()}"
             )
         super().__setattr__(key, value)
-
-    def convert_logits_to_probs(
-        self, sample_logits: Union[List[np.ndarray], np.ndarray]
-    ) -> np.ndarray:
-        """Converts logits to probs via softmax per sample"""
-        # axis ensures that in a matrix of probs with dims num_samples x num_classes
-        # we take the softmax for each sample
-        get_dq_logger().debug(
-            "Converting logits to probs.", split=self.split, epoch=self.epoch
-        )
-        token_probs = []
-        for token_logits in sample_logits:
-            token_probs.append(super().convert_logits_to_probs(token_logits))
-
-        return np.array(token_probs, dtype=object)
```

### Comparing `dataquality-0.8.9/dataquality/metrics.py` & `dataquality-0.9.1a1/dataquality/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 def get_run_summary(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> Dict:
     """Gets the summary for a run/split
 
     Calculates metrics (f1, recall, precision) overall (weighted) and per label.
     Also returns the top 50 rows of the dataframe (sorted by data_error_potential)
 
     :param project_name: The project name
@@ -121,15 +121,15 @@
 def get_metrics(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
     category: str = "gold",
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> Dict[str, List]:
     """Calculates available metrics for a run/split, grouped by a particular category
 
     The category/column provided (can be gold, pred, or any categorical metadata column)
     will result in metrics per "group" or unique value of that category/column
 
     :param project_name: The project name
@@ -163,15 +163,15 @@
 def display_distribution(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
     column: str = "data_error_potential",
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> None:
     """Displays the column distribution for a run. Plotly must be installed
 
     :param project_name: The project name
     :param run_name: The run name
     :param split: The split (training/test/validation/inference)
     :param task: (If multi-label only) the task name in question
@@ -264,15 +264,15 @@
     inference_name: str = "",
     file_type: FileType = FileType.arrow,
     include_embs: bool = False,
     include_probs: bool = False,
     include_token_indices: bool = False,
     hf_format: bool = False,
     tagging_schema: Optional[TaggingSchema] = None,
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
     as_pandas: bool = True,
     include_data_embs: bool = False,
 ) -> Union[pd.DataFrame, DataFrame]:
     """Gets the dataframe for a run/split
 
     Downloads an arrow (or specified type) file to your machine and returns a loaded
     Vaex dataframe.
@@ -432,14 +432,15 @@
     """Process dataframe after export of run or edits.
 
     See `get_dataframe` and `get_edited_dataframe` for details"""
     split = conform_split(split)
     # See docstring. In this case, we need span-level data
     # You can't attach embeddings/probs to the huggingface data, since the HF format is
     # sample level, and the embeddings are span level
+
     embs = include_embs or include_data_embs
     if (embs or include_probs) and task_type == TaskType.text_ner and not hf_format:
         # In NER, the `probabilities` contains the span level data
         span_df = get_probabilities(project_name, run_name, split, inference_name)
         keep_cols = [i for i in span_df.get_column_names() if "prob" not in i]
         span_df = span_df[keep_cols]
         # These are the token (not char) indices, lets make that clear
@@ -450,18 +451,16 @@
             if i != "sample_id":
                 data_df.rename(i, f"sample_{i}")
         data_df = data_df.join(span_df, on="sample_id", allow_duplication=True)
 
     tasks = []
     if task_type == TaskType.text_multi_label:
         tasks = api_client.get_tasks_for_run(project_name, run_name)
-        labels = [
-            api_client.get_labels_for_run(project_name, run_name, task)
-            for task in tasks
-        ]
+        # Don't provide a task, get all task-labels
+        labels = get_labels_for_run(project_name, run_name)
         data_df = _index_df(data_df, labels, tasks)
         data_df = _clean_mltc_df(data_df)
     if task_type == TaskType.text_classification:
         labels_per_task = api_client.get_labels_for_run(project_name, run_name)
         data_df = _index_df(data_df, labels_per_task)
 
     if include_embs:
@@ -533,15 +532,15 @@
 
 
 def get_embeddings(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the embeddings for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the embeddings from the final epoch. Note that only the
     n and n-1 epoch embeddings are available for download
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
@@ -589,15 +588,15 @@
 
 
 def get_probabilities(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the probabilities for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the probabilities from the final epoch.
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
 
@@ -614,15 +613,15 @@
 
 
 def get_raw_data(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the raw logged data for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the probabilities from the final epoch.
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
 
@@ -653,32 +652,48 @@
     """
     split = conform_split(split)
     return api_client.get_xray_cards(project_name, run_name, split, inference_name)
 
 
 def get_labels_for_run(
     project_name: str, run_name: str, task: Optional[str] = None
-) -> List[str]:
-    """Gets labels for a given run. If multi-label, a task must be provided"""
-    return api_client.get_labels_for_run(project_name, run_name, task)
+) -> List:
+    """Gets labels for a given run.
+
+    If multi-label, and a task is provided, this will get the labels for that task.
+    Otherwise, it will get all task-labels
+    """
+    try:
+        return api_client.get_labels_for_run(project_name, run_name, task)
+    except GalileoException as e:
+        if str(e) != "For multi-label runs, a task name must be provided":
+            raise e
+        # Multi-label case with no task provided. Get all tasks
+        pid, rid = api_client._get_project_run_id(project_name, run_name)
+        labels_object = f"{pid}/{rid}/labels/labels.json"
+        labels_path = object_store.download_file(
+            labels_object, "/tmp/labels.json", config.results_bucket_name
+        )
+        with open(labels_path) as f:
+            return json.loads(f.read())
 
 
 def get_tasks_for_run(project_name: str, run_name: str) -> List[str]:
     """Gets task names for a multi-label run"""
     return api_client.get_tasks_for_run(project_name, run_name)
 
 
 @cached(_get_cache(), key=_cache_key)
 def _get_hdf5_file_for_epoch(
     project_name: str,
     run_name: str,
     split: Split,
     object_name: str,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     split = conform_split(split)
     emb = "emb" in object_name
     if split == Split.inference and inference_name:
         split_path = inference_name
     else:
         split_path = str(_validate_epoch(project_name, run_name, split, epoch, emb=emb))
@@ -686,15 +701,19 @@
     object_name = f"{project_id}/{run_id}/{split}/{split_path}/{object_name}"
     file_name = f"/tmp/{uuid4()}-{os.path.split(object_name)[-1]}"
     object_store.download_file(object_name, file_name)
     return vaex.open(file_name)
 
 
 def _validate_epoch(
-    project_name: str, run_name: str, split: Split, epoch: int = None, emb: bool = False
+    project_name: str,
+    run_name: str,
+    split: Split,
+    epoch: Optional[int] = None,
+    emb: bool = False,
 ) -> int:
     split = conform_split(split)
     epochs = get_epochs(project_name, run_name, split)
     last_epoch = epochs[-1]
     if not epochs:
         raise GalileoException(f"No epochs found for {project_name}/{run_name}")
     if epoch is None:
@@ -715,38 +734,38 @@
 def _index_df(df: DataFrame, labels: List, tasks: Optional[List] = None) -> DataFrame:
     """Indexes gold and pred columns"""
     # We do this so if this is TC (no tasks), we can still iterate with the same logic
     tasks = tasks or [None]
     for ind, task in enumerate(tasks):
         # If multi label, must do it per task. If TC, then it's just 1 list of labels
         task_labels = labels[ind] if task else labels
-        for col in ["gold", "pred"]:
-            if col not in df.get_column_names():
+        for col in ["gold", "pred", "label"]:
+            if col not in df.get_column_names() or df[col].dtype == int:
                 continue
             df_col = f"{col}_{task}" if task else col
             df[f"{df_col}_idx"] = df[df_col]
             df = df.ordinal_encode(f"{df_col}_idx", values=task_labels, lazy=True)
     return df
 
 
 def _rename_prob_cols(df: DataFrame, tasks: List[str]) -> DataFrame:
     for ind, task in enumerate(tasks):
         df.rename(f"prob_{ind}", f"prob_{task}")
     return df
 
 
-def _validate_filter(filter: Union[FilterParams, Dict] = None) -> Dict:
+def _validate_filter(filter: Optional[Union[FilterParams, Dict]] = None) -> Dict:
     # Validate the fields provided with pydantic before making request
     return FilterParams(**dict(filter or {})).dict()
 
 
 def _conform_edit(edit: Union[Edit, Dict]) -> Edit:
     if isinstance(edit, Edit):
         return edit
     return Edit(**edit)
 
 
 def _clean_mltc_df(df: DataFrame) -> DataFrame:
     """In MLTC, don't return the non-task-indexes gold/pred/dep columns"""
-    drop_cols = ["gold", "pred", "data_error_potential", "prob"]
+    drop_cols = ["gold", "label", "pred", "data_error_potential", "prob"]
     keep_cols = [col for col in df.get_column_names() if col not in drop_cols]
     return df[keep_cols]
```

### Comparing `dataquality-0.8.9/dataquality/schemas/condition.py` & `dataquality-0.9.1a1/dataquality/schemas/condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 }
 
 
 class ConditionFilter(BaseModel):
     """Filter a dataframe based on the column value
 
     Note that the column used for filtering is the same as the metric used
-      in the condition.
+    in the condition.
 
     :param operator: The operator to use for filtering (e.g. "gt", "lt", "eq", "neq")
         See `Operator`
     :param value: The value to compare against
     """
 
     metric: str
```

### Comparing `dataquality-0.8.9/dataquality/schemas/dataframe.py` & `dataquality-0.9.1a1/dataquality/schemas/dataframe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
 from pydantic import BaseModel
 from vaex.dataframe import DataFrame
 
 
-class BaseLoggerInOutFrames(BaseModel):
+class BaseLoggerDataFrames(BaseModel):
     prob: DataFrame
     emb: DataFrame
     data: DataFrame
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `dataquality-0.8.9/dataquality/schemas/edit.py` & `dataquality-0.9.1a1/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/hf.py` & `dataquality-0.9.1a1/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/metrics.py` & `dataquality-0.9.1a1/dataquality/schemas/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,22 @@
         meta_filter: Optional[List[MetaFilter]] = None  see MetaFilter class
         inference_filter: Optional[InferenceFilter] = None  see InferenceFilter class
         span_sample_ids: Optional[List[int]] = None  (NER only) filter for full samples
         span_text: Optional[str] = None  (NER only) filter only on span text
         exclude_ids: List[int] = []  opposite of `ids`
         lasso: Optional[LassoSelection] = None  see LassoSelection class
         class_filter: Optional[List[StrictStr]] = None  filter GT OR prediction
-        likely_mislabeled: Optional[List[StrictStr]] = None  Filter for only
+        likely_mislabeled: Optional[bool] = None  Filter for only
             likely_mislabeled samples. False/None will return all samples
         likely_mislabeled_dep_percentile: Optional[int] A percentile threshold for l
             ikely mislabeled. This field (ranged 0-100) determines the precision of the
             likely_mislabeled filter. The threshold is applied against the DEP
             distribution of the likely_mislabeled samples. A threshold of 0 returns all,
             100 returns 1 sample, and 50 will return the top 50% DEP samples that are
-            likely_mislabeled. Higher = more precision, lower = more recall. Default 50.
+            likely_mislabeled. Higher = more precision, lower = more recall. Default 0.
     """
 
     ids: List[int] = []
     similar_to: Optional[List[int]] = None
     num_similar_to: Optional[int] = None
     text_pat: Optional[StrictStr] = None
     regex: Optional[bool] = None
@@ -107,8 +107,8 @@
     span_sample_ids: Optional[List[int]] = None
     span_text: Optional[str] = None
     span_regex: Optional[bool] = None
     exclude_ids: List[int] = []
     lasso: Optional[LassoSelection] = None
     class_filter: Optional[List[StrictStr]] = None
     likely_mislabeled: Optional[bool] = None
-    likely_mislabeled_dep_percentile: Optional[int] = Field(50, ge=0, le=100)
+    likely_mislabeled_dep_percentile: Optional[int] = Field(0, ge=0, le=100)
```

### Comparing `dataquality-0.8.9/dataquality/schemas/ner.py` & `dataquality-0.9.1a1/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/report.py` & `dataquality-0.9.1a1/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/route.py` & `dataquality-0.9.1a1/dataquality/schemas/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,37 @@
     projects = "projects"
     runs = "runs"
     users = "users"
     cleanup = "cleanup"
     login = "login"
     current_user = "current_user"
     healthcheck = "healthcheck"
+    healthcheck_dq = "healthcheck/dq"
     slices = "slices"
     split_path = "split"
     splits = "splits"
     inference_names = "inference_names"
     jobs = "jobs"
     latest_job = "jobs/latest"
     presigned_url = "presigned_url"
     tasks = "tasks"
     labels = "labels"
     epochs = "epochs"
     summary = "insights/summary"
     groupby = "insights/groupby"
+    metrics = "metrics"
     distribution = "insights/distribution"
     xray = "insights/xray"
     export = "export"
     edits = "edits"
     export_edits = "edits/export"
     ampli = "ampli"
     notify = "notify/email"
     token = "get-token"
+    upload_file = "upload_file"
 
     @staticmethod
     def content_path(
         project_id: Optional[Union[str, UUID4]] = None,
         run_id: Optional[Union[str, UUID4]] = None,
         split: Optional[Union[str, Split]] = None,
     ) -> str:
```

### Comparing `dataquality-0.8.9/dataquality/schemas/split.py` & `dataquality-0.9.1a1/dataquality/schemas/split.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from enum import Enum
 from typing import List, Union
 
 from dataquality.exceptions import GalileoException
 
 
 class Split(str, Enum):
-    training = "training"
     train = "training"
+    training = "training"
+    val = "validation"
+    valid = "validation"
     validation = "validation"
     test = "test"
     testing = "test"
     inference = "inference"
 
     @staticmethod
     def get_valid_attributes() -> List[str]:
         return list(map(lambda x: x.value, Split))
 
     @staticmethod
     def get_valid_keys() -> List[str]:
-        return ["train", "training", "test", "testing", "validation"]
+        return ["train", "training", "val", "valid", "validation", "test", "testing"]
 
 
 def conform_split(split: Union[str, Split]) -> Split:
     """Conforms split name to our naming conventions
 
     Raises GalileoException if split is invalid
     """
```

### Comparing `dataquality-0.8.9/dataquality/utils/ampli.py` & `dataquality-0.9.1a1/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/auto_trainer.py` & `dataquality-0.9.1a1/dataquality/utils/auto_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from typing import Optional
+
 from datasets import DatasetDict
 from transformers import Trainer
 
 import dataquality as dq
 from dataquality.integrations.transformers_trainer import watch
 from dataquality.schemas.split import Split
 
 
 def do_train(
     trainer: Trainer,
     encoded_data: DatasetDict,
     wait: bool,
-    create_data_embs: bool = False,
+    create_data_embs: Optional[bool] = None,
+    call_finish: bool = True,
 ) -> None:
     watch(trainer)
     trainer.train()
     if Split.test in encoded_data:
         # We pass in a huggingface dataset but typing wise they expect a torch dataset
-        trainer.predict(test_dataset=encoded_data[Split.test])  # type: ignore
+        trainer.predict(encoded_data[Split.test])
 
     inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
     for inf_name in inf_names:
         dq.set_split(Split.inference, inference_name=inf_name)
         trainer.predict(test_dataset=encoded_data[inf_name])
-    dq.finish(wait=wait, create_data_embs=create_data_embs)
+    if call_finish:
+        dq.finish(wait=wait, create_data_embs=create_data_embs)
```

### Comparing `dataquality-0.8.9/dataquality/utils/dq_logger.py` & `dataquality-0.9.1a1/dataquality/utils/dq_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def upload_dq_log_file() -> None:
     # For typing
     assert config.current_project_id and config.current_run_id
     obj_store = ObjectStore()
     obj_name = dq_log_object_name(config.current_project_id, config.current_run_id)
     file_path = dq_log_file_path()
     if os.path.isfile(file_path):
-        obj_store.create_project_run_object(
+        obj_store.create_object(
             object_name=obj_name,
             file_path=file_path,
             content_type="text/plain",
             progress=False,
         )
         remove_dq_log_file()
```

### Comparing `dataquality-0.8.9/dataquality/utils/helpers.py` & `dataquality-0.9.1a1/dataquality/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,14 +95,29 @@
     work in colab (because colab is running on a server, so there's no "browser" to
     interact with). This also prints out the link for users to click so even in those
     environments they still have something to interact with.
     """
     if not link:
         return
     try:
-
         webbrowser.open(link)
     # In some environments, webbrowser will raise. Other times it fails silently (colab)
     except Exception:
         pass
     finally:
         print(f"Click here to see your run! {link}")
+
+
+def gpu_available() -> bool:
+    import torch
+
+    return torch.cuda.is_available()
+
+
+def mps_available() -> bool:
+    """Checks for an MPS compatible GPU on Apple machines.
+
+    This will enabled Metal acceleration for model training when supported.
+    """
+    import torch
+
+    return torch.backends.mps.is_available()
```

### Comparing `dataquality-0.8.9/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.1a1/dataquality/utils/hf_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,19 @@
         self.gold_spans: List[Dict] = []
         self.current_gold_span_idx = -1
 
     def initialize_sample(self, k: int) -> None:
         self.previous_word_id = -1
         self.word_ids = self.tokenized_samples.word_ids(batch_index=k)
         # We check ds and ds.features to accomodate HF and arrow datasets
-        if HFCol.ner_tags in self.ds or HFCol.ner_tags in self.ds.features:
+        # Note we need to make sure that ds has an attr "features" to handle
+        # the weird case when type(ds) = datasets.formatting.formatting.LazyBatch
+        if HFCol.ner_tags in self.ds or (
+            hasattr(self.ds, "features") and HFCol.ner_tags in self.ds.features
+        ):
             existing_labels = [
                 self.idx_2_labels[label] for label in self.ds[HFCol.ner_tags][k]
             ]
             self.word_gold_spans = extract_gold_spans_at_word_level(
                 existing_labels, self.schema
             )
         # If ner_tags is not present, we know split must be 'inference'
@@ -139,15 +143,15 @@
         is_last_index = w_index_bpe == len(self.word_ids) - 1
         wid_is_last = wid != self.word_ids[w_index_bpe + 1] and wid == span_end_word
         return is_last_index or wid_is_last
 
     def _adjust_label_at_index(self, w_index_bpe: int, span_label_suffix: str) -> None:
         if self.schema == TaggingSchema.BILOU:
             self.adjusted_labels[w_index_bpe] = f"U-{span_label_suffix}"
-        if self.schema == TaggingSchema.BIOES:
+        elif self.schema == TaggingSchema.BIOES:
             self.adjusted_labels[w_index_bpe] = f"S-{span_label_suffix}"
         else:
             self.adjusted_labels[w_index_bpe] = f"B-{span_label_suffix}"
         self.adjusted_label_indices[w_index_bpe] = self.labels_2_idx[
             self.adjusted_labels[w_index_bpe]
         ]
         self.current_gold_span_idx += 1
@@ -170,15 +174,15 @@
                 SpanKey.label: span_label_suffix,
             }
         )
 
     def _adjust_last_bpe(self, w_index_bpe: int, span_label_suffix: str) -> None:
         if self.schema == TaggingSchema.BILOU:
             self.adjusted_labels[w_index_bpe] = f"L-{span_label_suffix}"
-        if self.schema == TaggingSchema.BIOES:
+        elif self.schema == TaggingSchema.BIOES:
             self.adjusted_labels[w_index_bpe] = f"E-{span_label_suffix}"
         else:
             self.adjusted_labels[w_index_bpe] = f"I-{span_label_suffix}"
         self.adjusted_label_indices[w_index_bpe] = self.labels_2_idx[
             self.adjusted_labels[w_index_bpe]
         ]
         # Update end indices
```

### Comparing `dataquality-0.8.9/dataquality/utils/keras.py` & `dataquality-0.9.1a1/dataquality/utils/keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,19 @@
     sample_weight = kwargs.get("sample_weight")
     x = tf.range(x_len)
     y = x
 
     if validation_split and validation_data is None:
         # Create the validation data using the training data. Only supported
         # for `Tensor` and `NumPy` input.
-        (x, y, sample_weight,), validation_data = data_adapter.train_validation_split(
+        (
+            x,
+            y,
+            sample_weight,
+        ), validation_data = data_adapter.train_validation_split(
             (x, y, sample_weight), validation_split=validation_split
         )
 
     if validation_data:
         (
             val_x,
             val_y,
```

### Comparing `dataquality-0.8.9/dataquality/utils/ml.py` & `dataquality-0.9.1a1/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/name.py` & `dataquality-0.9.1a1/dataquality/utils/name.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,38 @@
 import random
+import re
+from typing import Optional
+
+from dataquality.exceptions import GalileoException
+
+BAD_CHARS_REGEX = r"[^\w -]+"
+
+
+def validate_name(name: Optional[str], assign_random: bool = False) -> str:
+    """Validates project/run name ensuring only letters, numbers, space, - and _
+
+    If no name is provided, a random name is generated
+    """
+    if not name and assign_random:
+        name = random_name()
+
+    if not name:
+        raise GalileoException(
+            "Name is required. Set assign_random to True to generate a random name"
+        )
+
+    badchars = re.findall(BAD_CHARS_REGEX, name)
+    if badchars:
+        raise GalileoException(
+            "Only letters, numbers, whitespace, - and _ are allowed in a project "
+            f"or run name. Remove the following characters: {badchars}"
+        )
+
+    return name
+
 
 ADJECTIVES = [
     "able",
     "above",
     "absent",
     "absolute",
     "abstract",
```

### Comparing `dataquality-0.8.9/dataquality/utils/profiler.py` & `dataquality-0.9.1a1/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/spacy_integration.py` & `dataquality-0.9.1a1/dataquality/utils/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/thread_pool.py` & `dataquality-0.9.1a1/dataquality/utils/thread_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 import os
+import threading
 from threading import Thread
 from time import sleep
-from typing import Any, Callable, Iterable, List
+from typing import Any, Callable, Iterable, List, Optional
 
 from dataquality.exceptions import GalileoException
 
+lock = threading.Lock()
+
 
 class ThreadPoolManager:
     """
     A class for managing the threaded logging calls throughout dataquality
     """
 
     THREADS: List[Thread] = []
     MAX_THREADS = os.cpu_count() or 10
 
     @staticmethod
-    def add_thread(target: Callable, args: Iterable[Any] = None) -> None:
+    def add_thread(target: Callable, args: Optional[Iterable[Any]] = None) -> None:
         """
         Start a new function in a thread and store that in the global list of threads
 
         :param target: The callable
         :param args: The arguments to the function
-        :return: None
         """
         ThreadPoolManager.wait_for_thread()
         thread = Thread(target=target, args=args or [])
         try:
             thread.start()
             ThreadPoolManager.THREADS.append(thread)
         # Push up to the user
         except Exception as e:
             raise GalileoException(e)
 
     @staticmethod
     def wait_for_threads() -> None:
         """
         Joins all currently active threads and waits for all to be done
-
-        :return: None
         """
         ThreadPoolManager._cleanup()
         # Waits for each thread to finish
         for i in ThreadPoolManager.THREADS:
             i.join()
         ThreadPoolManager._cleanup()
 
     @staticmethod
     def wait_for_thread() -> None:
         """
         Waits for an open slot in the ThreadPool for another thread.
         """
         ThreadPoolManager._cleanup()
         while len(ThreadPoolManager.THREADS) >= ThreadPoolManager.MAX_THREADS:
+            # this sleep is necessary to prevent the thread from hogging compute
             sleep(0.05)
             ThreadPoolManager._cleanup()
 
     @staticmethod
     def _cleanup() -> None:
         """
         Cleans up the ThreadPoolManager, removing any dead ones
-
-        :return: None
         """
         ThreadPoolManager.THREADS = [
             i for i in ThreadPoolManager.THREADS if i.is_alive()
         ]
```

### Comparing `dataquality-0.8.9/dataquality/utils/transformers.py` & `dataquality-0.9.1a1/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/vaex.py` & `dataquality-0.9.1a1/dataquality/utils/vaex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,56 @@
 import os
-import sys
-import threading
-from typing import Dict, List
+from typing import Dict, List, Union
 
-import h5py
 import numpy as np
 import pyarrow as pa
 import vaex
-from vaex.arrow.convert import arrow_string_array_from_buffers as convert_bytes
+from sklearn.decomposition import IncrementalPCA
 from vaex.dataframe import DataFrame
 
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.base_logger import BaseLoggerAttributes
-from dataquality.utils import tqdm
-from dataquality.utils.hdf5_store import HDF5_STORE, HDF5Store
+from dataquality.schemas.split import Split
+from dataquality.utils.cuda import (
+    PCA_CHUNK_SIZE,
+    PCA_N_COMPONENTS,
+    cuml_available,
+    get_pca_embeddings,
+    get_umap_embeddings,
+)
+from dataquality.utils.hdf5_store import HDF5_STORE, concat_hdf5_files
 from dataquality.utils.helpers import galileo_verbose_logging
 
-lock = threading.Lock()
 # To decide between "all-MiniLM-L6-v2" or "all-mpnet-base-v2"
 # https://www.sbert.net/docs/pretrained_models.html#model-overview
 GALILEO_DATA_EMBS_ENCODER = "GALILEO_DATA_EMBS_ENCODER"
 DEFAULT_DATA_EMBS_MODEL = "all-MiniLM-L6-v2"
 
 
-def _save_hdf5_file(location: str, file_name: str, data: Dict) -> None:
-    """
-    Helper function to save a dictionary as an hdf5 file that can be read by vaex
-    """
-    if not os.path.isdir(location):
-        with lock:
-            os.makedirs(location, exist_ok=True)
-    file_path = f"{location}/{file_name}"
-    with h5py.File(file_path, "w") as f:
-        for col in data:
-            group = f.create_group(f"/table/columns/{col}")
-            col_data = np.array(data[col])
-            if None in col_data:
-                # h5py expects np.nan instead of None
-                col_data = col_data.astype(np.float_)
-
-            # String columns
-            ctype = col_data.dtype
-            if not np.issubdtype(ctype, np.number) and not np.issubdtype(
-                ctype, np.bool_
-            ):
-                dtype = h5py.string_dtype()
-                col_data = col_data.astype(dtype)
-            else:
-                dtype = col_data.dtype
-
-            shape = col_data.shape
-            group.create_dataset(
-                "data", data=col_data, dtype=dtype, shape=shape, chunks=shape
-            )
-
-
 def _join_in_out_frames(in_df: DataFrame, out_df: DataFrame) -> DataFrame:
     """Helper function to join our input and output frames"""
     in_frame = in_df.copy()
     # There is an odd vaex bug where sometimes we lose the continuity of this dataframe
     # it's hard to reproduce, only shows up on linux, and hasn't been pinpointed yet
     # but materializing the join-key column fixes the issue
     # https://github.com/vaexio/vaex/issues/1972
     in_frame["id"] = in_frame["id"].values
     out_frame = out_df.copy()
-    in_out = out_frame.join(
-        in_frame, on="id", how="inner", lsuffix="_L", rsuffix="_R"
-    ).copy()
+    in_out = out_frame.join(in_frame, on="id", how="inner", lsuffix="_L").copy()
     if len(in_out) != len(out_frame):
         num_missing = len(out_frame) - len(in_out)
         missing_ids = set(out_frame["id"].unique()) - set(in_out["id_L"].unique())
         split = out_frame["split"].unique()[0]
         raise GalileoException(
             "It seems there were logged outputs with no corresponding inputs logged "
             f"for split {split}. {num_missing} corresponding input IDs are missing:\n"
             f"{missing_ids}"
         )
     keep_cols = [c for c in in_out.get_column_names() if not c.endswith("_L")]
     in_out = in_out[keep_cols]
-    for c in in_out.get_column_names():
-        if c.endswith("_R"):
-            in_out.rename(c, c.rstrip("_R"))
     return in_out
 
 
 def validate_unique_ids(df: DataFrame, epoch_or_inf_name: str) -> None:
     """Helper function to validate the logged df has unique ids
 
     Fail gracefully otherwise
@@ -110,89 +76,14 @@
 def get_dup_ids(df: DataFrame) -> List:
     """Gets the list of duplicate IDs in a dataframe, if any"""
     df_copy = df.copy()
     dup_df = df_copy.groupby(by="id", agg="count")
     return dup_df[dup_df["count"] > 1].to_records()
 
 
-def _valid_prob_col(col: str) -> bool:
-    return (
-        col.endswith("id")
-        or "gold" in col
-        or "pred" in col
-        or "prob" in col  # encapsulates prob, conf_prob, and loss_prob
-        or col.startswith("span")
-        or col.startswith("galileo")
-    )
-
-
-def concat_hdf5_files(location: str, prob_only: bool) -> List[str]:
-    """Concatenates all hdf5 in a directory using an HDF5 store
-
-    Vaex stores a dataframe as an hdf5 file in a predictable format using groups
-
-    Each column gets its own group, following "/table/columns/{col}/data
-
-    We can exploit that by concatenating our datasets with that structure, so vaex
-    can open the final file as a single dataframe
-
-    :param location: The directory containing the files
-    :param prob_only: If True, only the id, prob, and gold columns will be concatted
-    """
-    str_cols = []
-    stores = {}
-    files = os.listdir(location)
-    df = vaex.open(f"{location}/{files[0]}")
-
-    # Construct a store per column
-    if prob_only:
-        cols = [c for c in df.get_column_names() if _valid_prob_col(c)]
-    else:
-        cols = df.get_column_names()
-    for col in cols:
-        group = f"/table/columns/{col}/data"
-        cval = df[col].to_numpy()
-        if cval.ndim == 2:
-            shape = cval[0].shape
-        else:
-            shape = ()
-        dtype = df[col].dtype.numpy
-        if not np.issubdtype(dtype, np.number) and not np.issubdtype(dtype, np.bool_):
-            dtype = h5py.string_dtype(encoding="utf-8")
-            str_cols.append(col)
-        stores[col] = HDF5Store(f"{location}/{HDF5_STORE}", group, shape, dtype=dtype)
-
-    for file in tqdm(
-        files,
-        leave=False,
-        desc="Processing data for upload",
-        file=sys.stdout,
-    ):
-        fname = f"{location}/{file}"
-        with h5py.File(fname, "r") as f:
-            dset = f["table"]["columns"]
-            keys = dset.keys()
-            keys = [key for key in keys if key in cols]
-            for key in keys:
-                col_data = dset[key]
-                # We have a string column, need to parse it
-                if "indices" in col_data.keys():
-                    assert key in str_cols, f"Unexpected string column ({key}) found"
-                    indcs = col_data["indices"][:]
-                    data = col_data["data"][:]
-                    d = convert_bytes(data, indcs, None).to_numpy(zero_copy_only=False)
-                else:
-                    d = col_data["data"][:]
-                if key in str_cols:
-                    d = d.astype(h5py.string_dtype(encoding="utf-8"))
-                stores[key].append(d)
-        os.remove(fname)
-    return str_cols
-
-
 def drop_empty_columns(df: DataFrame) -> DataFrame:
     """Drops any columns that have no values"""
     if len(df) == 0:
         return df
     df_copy = df.copy()
     cols = df.get_column_names()
     # Don't need to check the default columns, they've already been validated
@@ -220,25 +111,121 @@
     """Renames a vaex df using a mapping"""
     df_copy = df.copy()
     for old, new in columns.items():
         df_copy.rename(old, new)
     return df_copy
 
 
-def create_data_embs(df: DataFrame) -> DataFrame:
-    """Runs sentence transformer on raw text to get off the shelf data embeddings"""
+def add_umap_pca_to_df(df: DataFrame, data_embs: bool = False) -> DataFrame:
+    """Adds the PCA embeddings and UMAP xy embeddings if possible
+
+    If data_embs is True, the x and y values from umap will be named data_x and data_y
+    """
+    if not cuml_available():
+        return df
+    dfc = df.copy()
+    note = "[data embs]" if data_embs else "[embs]"
+    print(f"{note} Found cuda ML libraries")
+    print(f"{note} Applying dimensionality reduction step 1/2")
+    emb_pca = get_pca_embeddings(dfc["emb"].to_numpy())
+    print(f"{note} Applying dimensionality reduction step 2/2")
+    emb_xy = get_umap_embeddings(emb_pca)
+    x, y = ("data_x", "data_y") if data_embs else ("x", "y")
+    dfc["emb_pca"] = emb_pca
+    dfc[x] = emb_xy[:, 0]
+    dfc[y] = emb_xy[:, 1]
+    return dfc
+
+
+def create_data_embs_df(df: DataFrame, lazy: bool = True) -> DataFrame:
+    """Runs sentence transformer on raw text to get off the shelf data embeddings
+
+    :param df: The dataframe to get data embeddings for. Must have text col
+    :param lazy: If true, we lazily apply the model to encode the text
+    """
     # This import takes up to 25 seconds, so we don't want to eagerly import it
     import transformers
     from sentence_transformers import SentenceTransformer
 
     transformers.logging.disable_progress_bar()
     sentence_encoder = os.getenv(GALILEO_DATA_EMBS_ENCODER, DEFAULT_DATA_EMBS_MODEL)
     data_model = SentenceTransformer(sentence_encoder)
+    transformers.logging.enable_progress_bar()
     df_copy = df.copy()
 
     @vaex.register_function()
     def apply_sentence_transformer(text: pa.array) -> np.ndarray:
-        return data_model.encode(text.to_pylist(), show_progress_bar=False)
+        return data_model.encode(text.to_pylist(), show_progress_bar=False).astype(
+            np.float32
+        )
 
-    df_copy["emb"] = df_copy["text"].apply_sentence_transformer()
-    transformers.logging.enable_progress_bar()
-    return df_copy[["id", "emb"]]
+    if lazy:
+        df_copy["emb"] = df_copy["text"].apply_sentence_transformer()
+        df_copy = df_copy[["id", "emb"]]
+    else:
+        import torch
+
+        # Downcasts to float16 where possible, speeds up processing by 10 it/sec
+        with torch.autocast("cuda"):
+            df_copy["emb"] = data_model.encode(
+                df_copy["text"].tolist(), show_progress_bar=True
+            ).astype(np.float32)
+
+    return df_copy
+
+
+def get_output_df(
+    dir_name: str,
+    prob_only: bool,
+    split: str,
+    epoch_or_inf: Union[str, int],
+) -> DataFrame:
+    """Creates the single hdf5 file for the output data of a split/epoch
+
+    Applies the necessary conversions post-concatenation of files
+    (see `concat_hdf5_files`)
+    """
+    out_frame_path = f"{dir_name}/{HDF5_STORE}"
+    # It's possible the files were already concatenated and handled. In that case
+    # just open the processed file
+    if os.path.isfile(out_frame_path):
+        return vaex.open(out_frame_path)
+    str_cols = concat_hdf5_files(dir_name, prob_only)
+    out_frame = vaex.open(out_frame_path)
+
+    if split == Split.inference:
+        dtype: Union[str, None] = "str"
+        epoch_or_inf_name = "inference_name"
+    else:
+        dtype = None
+        epoch_or_inf_name = "epoch"
+
+    # Post concat, string columns come back as bytes and need conversion
+    for col in str_cols:
+        out_frame[col] = out_frame[col].as_arrow().astype("str")
+        out_frame[col] = out_frame[f'astype({col}, "large_string")']
+    if prob_only:
+        out_frame["split"] = vaex.vconstant(split, length=len(out_frame), dtype="str")
+        out_frame[epoch_or_inf_name] = vaex.vconstant(
+            epoch_or_inf, length=len(out_frame), dtype=dtype
+        )
+    return out_frame
+
+
+def add_pca_to_df(df: DataFrame, chunk_size: int = PCA_CHUNK_SIZE) -> DataFrame:
+    """Adds the 'emb_pca' to the dataframe"""
+    df_copy = df.copy()
+    # sklearn breaks if a the dataset has less samples than PCA_N_COMPONENTS
+    n_components = min(PCA_N_COMPONENTS, len(df_copy))
+    pca = IncrementalPCA(n_components=n_components)
+    for i1, i2, chunk in df_copy.evaluate_iterator("emb", chunk_size=chunk_size):
+        pca.partial_fit(chunk)
+
+    @vaex.register_function()
+    def apply_pca(emb: np.ndarray) -> np.ndarray:
+        return pca.transform(emb).astype(np.float32)
+
+    df_copy["emb_pca"] = df_copy["emb"].apply_pca()
+    # Fully apply the PCA model now, without ever bringing the full embeddings into
+    # memory, only the PCA embeddings (much smaller)
+    df_copy = df_copy.materialize("emb_pca")
+    return df_copy
```

### Comparing `dataquality-0.8.9/dataquality/utils/version.py` & `dataquality-0.9.1a1/dataquality/utils/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-from setuptools.version import pkg_resources  # type: ignore
 
 from dataquality import __version__ as dq_client_version
 from dataquality.core._config import config
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.route import Route
 
 
@@ -14,34 +13,27 @@
     matching major versions.
 
     https://semver.org/#summary.
 
     Returns:
         None
     """
-    client_semver = _parse_version(_get_client_version())
-    server_semver = _parse_version(_get_api_version())
+    client_semver = _get_client_version()
+    server_semver = _get_api_version()
     try:
         assert _major_version(client_semver) == _major_version(server_semver)
     except AssertionError:
         raise GalileoException(
             "Major mismatch between client, "
             f"{client_semver}, and server {server_semver}."
         )
 
 
-def _major_version(v: pkg_resources.extern.packaging.version.Version) -> str:
-    if hasattr(v, "major"):
-        return str(v.major)
-    else:
-        return str(v.base_version).split(".")[0]
-
-
-def _parse_version(version: str) -> pkg_resources.extern.packaging.version.Version:
-    return pkg_resources.parse_version(version)
+def _major_version(v: str) -> str:
+    return str(v).split(".")[0]
 
 
 def _get_client_version() -> str:
     return dq_client_version
 
 
 def _get_api_version() -> str:
```

### Comparing `dataquality-0.8.9/docs/Dataquality-Client-Demo.ipynb` & `dataquality-0.9.1a1/docs/notebooks/Dataquality-Client-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/docs/End to End runs per task type.ipynb` & `dataquality-0.9.1a1/docs/notebooks/End to End runs per task type.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/docs/Inference-Demo.ipynb` & `dataquality-0.9.1a1/docs/notebooks/Inference-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/docs/NER Inference.ipynb` & `dataquality-0.9.1a1/docs/notebooks/NER Inference.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/docs/cv/cv-demo-hf.py` & `dataquality-0.9.1a1/docs/cv/cv-demo-hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/docs/cv/cv-testing-benchmark.py` & `dataquality-0.9.1a1/docs/cv/cv-testing-benchmark.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/auto/test_ner_auto.py` & `dataquality-0.9.1a1/tests/auto/test_ner_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     mock_init: mock.MagicMock,
     mock_set_labels: mock.MagicMock,
     mock_log_dataset: mock.MagicMock,
     mock_get_trainer: mock.MagicMock,
     mock_watch: mock.MagicMock,
     mock_finish: mock.MagicMock,
 ) -> None:
-
     df_train = base_df.copy()
     trainer = mock.MagicMock()
     encoded_data = {}
     mock_get_trainer.return_value = trainer, encoded_data
     auto(train_data=df_train)
 
     mock_get_trainer.assert_called_once()
@@ -77,15 +76,14 @@
     mock_set_labels: mock.MagicMock,
     mock_log_dataset: mock.MagicMock,
     mock_get_trainer: mock.MagicMock,
     mock_watch: mock.MagicMock,
     mock_finish: mock.MagicMock,
     set_test_config: Callable,
 ) -> None:
-
     df_train = base_df.copy()
     df_inf = pd.DataFrame({"tokens": ["some", "new", "tokens", "heree"]})
     trainer = mock.MagicMock()
     encoded_data = {Split.training: df_train, "inf_1": df_inf}
     mock_get_trainer.return_value = trainer, encoded_data
     auto(train_data=df_train, inference_data={"inf_1": df_inf})
     trainer.predict.assert_called_once()
```

### Comparing `dataquality-0.8.9/tests/auto/test_tc_auto.py` & `dataquality-0.9.1a1/tests/auto/test_tc_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/clients/test_api.py` & `dataquality-0.9.1a1/tests/clients/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,7 +298,30 @@
         url="http://localhost:8088/notify/email",
         body={
             "data": {"foo": "bar"},
             "template": "template",
             "emails": ["foo@bar.com"],
         },
     )
+
+
+@mock.patch.object(ApiClient, "make_request")
+def test_set_metric_for_run(
+    mock_make_request: MagicMock, set_test_config: Callable
+) -> None:
+    proj_id, run_id = uuid4(), uuid4()
+    data = {
+        "key": "feature_importances",
+        "value": 0.0,
+        "epoch": 0,
+        "extra": {
+            "feature_0": 0.5,
+            "feature_1": 0.6,
+            "feature_2": 0.7,
+        },
+    }
+    api_client.set_metric_for_run(proj_id, run_id, data)
+    mock_make_request.assert_called_once_with(
+        RequestType.PUT,
+        url=f"http://localhost:8088/projects/{proj_id}/runs/{run_id}/metrics",
+        body=data,
+    )
```

### Comparing `dataquality-0.8.9/tests/conftest.py` & `dataquality-0.9.1a1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import shutil
-from typing import Any, Callable, Dict, Generator, List, Optional
+from typing import Any, Callable, Dict, Generator, List, Optional, Union
 from uuid import UUID
 
 import pytest
 import requests
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 from vaex.dataframe import DataFrame
 
@@ -45,29 +45,39 @@
 
 @pytest.fixture(autouse=True)
 def disable_network_calls(request, monkeypatch):
     # Tests that fetch datasets need network access
     if "noautofixt" in request.keywords:
         return
 
-    def stunted_get(url: str) -> MockResponse:
+    def stunted_get(url: str) -> Union[Dict, MockResponse]:
         """Unless it's a mocked call to healthcheck, disable network access"""
+        bucket_names = {
+            "images": "galileo-images",
+            "results": "galileo-project-runs-results",
+            "root": "galileo-project-runs",
+        }
         if "healthcheck" in url:
             return MockResponse(
-                json_data={"minimum_dq_version": "0.0.0"}, status_code=200
+                json_data={
+                    "minimum_dq_version": "0.0.0",
+                    "api_version": "100.0.0",
+                    "bucket_names": bucket_names,
+                },
+                status_code=200,
             )
         raise RuntimeError("Network access not allowed during testing!")
 
     monkeypatch.setattr(requests, "get", lambda url, *args, **kwargs: stunted_get(url))
 
 
 @pytest.fixture(scope="function")
 def cleanup_after_use() -> Generator:
     for task_type in list(TaskType):
-        dataquality.get_model_logger(task_type).logger_config.reset()
+        dataquality.get_data_logger(task_type).logger_config.reset()
     try:
         if os.path.isdir(BaseGalileoLogger.LOG_FILE_DIR):
             shutil.rmtree(BaseGalileoLogger.LOG_FILE_DIR)
         if not os.path.isdir(TEST_PATH):
             for split in SPLITS:
                 for subdir in SUBDIRS:
                     os.makedirs(f"{TEST_PATH}/{split}/{subdir}")
@@ -76,15 +86,15 @@
         yield
     finally:
         if os.path.exists(BaseGalileoLogger.LOG_FILE_DIR):
             shutil.rmtree(BaseGalileoLogger.LOG_FILE_DIR)
         if os.path.exists(DQ_LOG_FILE_LOCATION):
             shutil.rmtree(DQ_LOG_FILE_LOCATION)
         for task_type in list(TaskType):
-            dataquality.get_model_logger(task_type).logger_config.reset()
+            dataquality.get_data_logger(task_type).logger_config.reset()
 
 
 @pytest.fixture()
 def set_test_config(
     default_token: str = "sometoken",
     default_task_type: TaskType = TaskType.text_classification,
     default_api_url: str = DEFAULT_API_URL,
@@ -111,15 +121,15 @@
 
 
 @pytest.fixture()
 def input_data() -> Callable:
     def curry(
         split: str = "training",
         inference_name: str = "all-customers",
-        meta: Dict = None,
+        meta: Optional[Dict] = None,
     ) -> Dict:
         data = {
             "texts": ["sentence_1", "sentence_2"],
             "split": split,
             "ids": [1, 2],
         }
         if split == "inference":
```

### Comparing `dataquality-0.8.9/tests/core/test_auth.py` & `dataquality-0.9.1a1/tests/core/test_auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/core/test_config.py` & `dataquality-0.9.1a1/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/core/test_finish.py` & `dataquality-0.9.1a1/tests/core/test_finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/core/test_report.py` & `dataquality-0.9.1a1/tests/core/test_report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/inference/test_inference.py` & `dataquality-0.9.1a1/tests/inference/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         base_model_logger.split = Split.inference
         with pytest.raises(GalileoException) as e:
             base_model_logger.set_split_epoch()
 
         assert e.value.args[0] == (
             "For inference split you must either log an inference name or set "
-            "it before logging. Use `dataquality.set_split` to setinference_name"
+            "it before logging. Use `dataquality.set_split` to set inference_name"
         )
 
     @mock.patch(
         "dataquality.loggers.model_logger.base_model_logger._save_hdf5_file",
         return_value="1234-abcd-5678",
     )
     @mock.patch(
```

### Comparing `dataquality-0.8.9/tests/inference/test_text_classification_inf.py` & `dataquality-0.9.1a1/tests/inference/test_text_classification_inf.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datasets
 import pandas as pd
 import pytest
 import tensorflow as tf
 import vaex
 
 import dataquality
+from dataquality.exceptions import GalileoException
 from dataquality.loggers.data_logger.base_data_logger import DataSet
 from dataquality.loggers.data_logger.text_classification import (
     TextClassificationDataLogger,
 )
 from dataquality.schemas.split import Split
 
 
@@ -19,31 +20,32 @@
     def _setup(self, **kwargs) -> TextClassificationDataLogger:
         logger = TextClassificationDataLogger(split=Split.inference, **kwargs)
         logger.logger_config.reset()
         return logger
 
     def test_validate_inference(self):
         logger = self._setup(**{"inference_name": "animals"})
-        logger.validate()
+        logger.validate_and_format()
 
     def test_validate_inference_with_labels(self):
         logger = self._setup(**{"labels": ["dog", "cat"], "inference_name": "animals"})
         with pytest.raises(AssertionError) as e:
-            logger.validate()
+            logger.validate_and_format()
 
         assert e.value.args[0] == "You cannot have labels in your inference split!"
 
     def test_validate_inference_missing_inference_name(self):
         logger = self._setup()
-        with pytest.raises(AssertionError) as e:
-            logger.validate()
+        with pytest.raises(GalileoException) as e:
+            logger.validate_and_format()
 
-        assert e.value.args[0] == (
-            "Inference name must be set when logging an inference split. Use "
-            "set_split('inference', inference_name) to set inference name"
+        assert str(e.value) == (
+            "For inference split you must either log an inference name "
+            "or set it before logging. Use `dataquality.set_split` to set "
+            "inference_name"
         )
 
     @pytest.mark.parametrize(
         "dataset",
         [
             pd.DataFrame(
                 {
```

### Comparing `dataquality-0.8.9/tests/inference/test_text_ner_inf.py` & `dataquality-0.9.1a1/tests/inference/test_text_ner_inf.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import datasets
 import pandas as pd
 import pytest
 import vaex
 
 import dataquality
+from dataquality.exceptions import GalileoException
 from dataquality.loggers.data_logger.base_data_logger import DataSet
 from dataquality.loggers.data_logger.text_ner import TextNERDataLogger
 from dataquality.schemas.split import Split
 
 TEST_LABELS = ["[PAD]", "[CLS]", "[SEP]", "O", "B-ACTOR", "I-ACTOR"]
 
 
@@ -20,36 +21,37 @@
         logger.logger_config.reset()
         logger.logger_config.labels = TEST_LABELS
         logger.logger_config.tagging_schema = "BIO"
         return logger
 
     def test_validate_inference(self):
         logger = self._setup(**{"inference_name": "animals"})
-        logger.validate()
+        logger.validate_and_format()
 
     def test_validate_inference_with_labels(self):
         gold_spans = [
             {"start": 0, "end": 4, "label": "YEAR"},
             {"start": 17, "end": 29, "label": "ACTOR"},
         ]
         logger = self._setup(**{"gold_spans": gold_spans, "inference_name": "animals"})
 
         with pytest.raises(AssertionError) as e:
-            logger.validate()
+            logger.validate_and_format()
 
         assert e.value.args[0] == "You cannot have gold spans in your inference split!"
 
     def test_validate_inference_missing_inference_name(self):
         logger = self._setup()
-        with pytest.raises(AssertionError) as e:
-            logger.validate()
+        with pytest.raises(GalileoException) as e:
+            logger.validate_and_format()
 
-        assert e.value.args[0] == (
-            "Inference name must be set when logging an inference split. Use "
-            "set_split('inference', inference_name) to set inference name"
+        assert str(e.value) == (
+            "For inference split you must either log an inference name "
+            "or set it before logging. Use `dataquality.set_split` to set "
+            "inference_name"
         )
 
     @pytest.mark.parametrize(
         "dataset",
         [
             pd.DataFrame(
                 {
```

### Comparing `dataquality-0.8.9/tests/integration/mock_training_run.py` & `dataquality-0.9.1a1/tests/integration/mock_training_run.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py` & `dataquality-0.9.1a1/tests/integrations/hf/test_hf_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         ds_dict = datasets.DatasetDict(
             {
                 "train": mock_ds,
                 "test": mock_ds,
                 "validation": mock_ds,
             }
         )
+
         output = tokenize_and_log_dataset(ds_dict, mock_tokenizer)
 
     for split in ds_dict.keys():
         split_output = output[split]
         for k in ADJUSTED_TOKEN_DATA:
             token_data = ADJUSTED_TOKEN_DATA[k]
             if k == "text_token_indices":
@@ -265,15 +266,17 @@
     mock_ds_meta = mock_ds.add_column("test_meta_1", ["a", "b", "c", "d", "e"])
     with mock.patch("dataquality.integrations.hf.tokenize_adjust_labels") as mock_tok:
         mock_tok.return_value = tokenize_output
         # Only test and val have meta, make sure they both get logged with meta
         ds_dict = datasets.DatasetDict(
             {"train": mock_ds, "test": mock_ds_meta, "validation": mock_ds_meta}
         )
-        output = tokenize_and_log_dataset(ds_dict, mock_tokenizer, meta=["test_meta_1"])
+        output = tokenize_and_log_dataset(
+            ds_dict, mock_tokenizer, label_names, meta=["test_meta_1"]
+        )
     for split in ds_dict.keys():
         split_output = output[split]
         for k in ADJUSTED_TOKEN_DATA:
             token_data = ADJUSTED_TOKEN_DATA[k]
             if k == "text_token_indices":
                 # We abuse token data because outputs are returning tuples but we want
                 # to compare lists
```

### Comparing `dataquality-0.8.9/tests/integrations/hf/test_text_classification_hf.py` & `dataquality-0.9.1a1/tests/integrations/hf/test_text_classification_hf.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     Trainer,
     TrainingArguments,
 )
 
 import dataquality as dq
 from dataquality import config
 from dataquality.integrations.transformers_trainer import watch
+from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.thread_pool import ThreadPoolManager
 from tests.conftest import HF_TEST_BERT_PATH, LOCATION, model, tokenizer
-from tests.test_utils.hf_datasets_mock import mock_dataset, mock_dataset_repeat
+from tests.test_utils.hf_datasets_mock import mock_hf_dataset, mock_hf_dataset_repeat
 from tests.test_utils.mock_request import (
     mocked_create_project_run,
     mocked_get_project_run,
 )
+from tests.test_utils.pt_datasets_mock import CustomDatasetWithTokenizer
 
 metric = load_metric("accuracy")
 
 
 def preprocess_function(examples, tokenizer):
     return tokenizer(
         examples["text"], padding="max_length", max_length=201, truncation=True
@@ -38,16 +40,18 @@
 def compute_metrics(eval_pred):
     predictions, labels = eval_pred
     predictions = predictions.argmax(axis=1)
     return metric.compute(predictions=predictions, references=labels)
 
 
 # 🔭🌕 Galileo logging
-mock_dataset_with_ids = mock_dataset.map(lambda x, idx: {"id": idx}, with_indices=True)
-mock_dataset_with_ids_repeat = mock_dataset_repeat.map(
+mock_dataset_with_ids = mock_hf_dataset.map(
+    lambda x, idx: {"id": idx}, with_indices=True
+)
+mock_dataset_with_ids_repeat = mock_hf_dataset_repeat.map(
     lambda x, idx: {"id": idx}, with_indices=True
 )
 
 encoded_train_dataset = mock_dataset_with_ids.map(
     lambda x: preprocess_function(x, tokenizer), batched=True
 )
 encoded_test_dataset = mock_dataset_with_ids.map(
@@ -118,15 +122,15 @@
     mock_valid_user: MagicMock,
     set_test_config: Callable,
     cleanup_after_use: Generator,
 ) -> None:
     """Base case: Tests creating a new project and run"""
     set_test_config(task_type=TaskType.text_classification)
     # 🔭🌕 Galileo logging
-    dq.set_labels_for_run(mock_dataset.features["label"].names)
+    dq.set_labels_for_run(mock_hf_dataset.features["label"].names)
     train_dataset = mock_dataset_with_ids
     val_dataset = mock_dataset_with_ids
     test_dataset = mock_dataset_with_ids
     dq.log_dataset(train_dataset, split="train")
     dq.log_dataset(val_dataset, split="validation")
     dq.log_dataset(test_dataset, split="test")
 
@@ -158,18 +162,17 @@
     mock_valid_user: MagicMock,
     mock_requests_get: MagicMock,
     mock_requests_post: MagicMock,
     set_test_config: Callable,
 ) -> None:
     """Base case: Tests watch function to pass"""
     set_test_config(task_type=TaskType.text_classification)
-
     train_dataset = mock_dataset_with_ids
     test_dataset = mock_dataset_with_ids
-    dq.set_labels_for_run(mock_dataset.features["label"].names)
+    dq.set_labels_for_run(mock_hf_dataset.features["label"].names)
     dq.log_dataset(train_dataset, split="train")
     dq.log_dataset(test_dataset, split="test")
     assert config.current_run_id
     assert config.current_project_id
     t_args = TrainingArguments(
         output_dir="tmp",
         evaluation_strategy="epoch",
@@ -196,15 +199,14 @@
         tokenizer=tokenizer,
         compute_metrics=compute_metrics,
     )
 
     assert trainer._signature_columns is None, "Signature columns should be None"
     watch(trainer)
     assert trainer._signature_columns is None, "Signature columns should be None"
-
     trainer.train()
 
 
 @patch("requests.post", side_effect=mocked_create_project_run)
 @patch("requests.get", side_effect=mocked_get_project_run)
 @patch.object(dq.core.init.ApiClient, "valid_current_user", return_value=True)
 def test_training_run(
@@ -238,21 +240,20 @@
     assert tensor_sliced.shape == arr_sliced.shape, "sliced shape must match"
     assert np.array_equal(arr_sliced, tensor_sliced.numpy()), "shape must be same"
 
 
 historic_embeddings = None
 
 
-def _embedding_hook(model: Module, model_input: Any, model_output: Any) -> None:
+def _dq_embedding_hook(model: Module, model_input: Any, model_output: Any) -> None:
     """
     Hook to extract the embeddings from the model
     :param model: Model pytorch model
     :param model_input: Model input
     :param model_output: Model output
-    :return: None
     """
     global historic_embeddings
     if hasattr(model_output, "last_hidden_state"):
         output_detached = model_output.last_hidden_state.detach()
         if historic_embeddings is None:
             historic_embeddings = output_detached
 
@@ -284,14 +285,106 @@
     dataloader = DataLoader(
         train_sample,
         batch_size=4,
     )
     for batch in dataloader:
         batch.pop("id").detach().numpy()
         pred = model_base(**batch)
-        next(model_seq.children()).register_forward_hook(_embedding_hook)
+        next(model_seq.children()).register_forward_hook(_dq_embedding_hook)
         model_seq(**batch)
         embeddings = pred[0][:, 0].detach().numpy()[0]
         embeddings_cls = historic_embeddings[:, 0].detach().numpy()[0]
         break
 
     assert np.array_equal(embeddings, embeddings_cls), "Embeddings must be same"
+
+
+@patch.object(dq.core.init.ApiClient, "valid_current_user", return_value=True)
+@patch.object(dq.core.finish, "_version_check")
+@patch.object(dq.core.finish, "_reset_run")
+@patch.object(dq.core.finish, "upload_dq_log_file")
+@patch.object(dq.clients.api.ApiClient, "make_request")
+@patch.object(dq.core.finish, "wait_for_run")
+def test_hf_watch_with_pt_dataset_e2e(
+    mock_wait_for_run: MagicMock,
+    mock_make_request: MagicMock,
+    mock_upload_log_file: MagicMock,
+    mock_reset_run: MagicMock,
+    mock_version_check: MagicMock,
+    mock_valid_user: MagicMock,
+    set_test_config: Callable,
+    cleanup_after_use: Generator,
+) -> None:
+    """Base case: Tests creating a new project and run"""
+    set_test_config(task_type=TaskType.text_classification)
+    # 🔭🌕 Galileo logging
+    dq.set_labels_for_run(["pos", "neg"])
+    train_dataset = CustomDatasetWithTokenizer(tokenizer)
+    val_dataset = CustomDatasetWithTokenizer(tokenizer)
+    test_dataset = CustomDatasetWithTokenizer(tokenizer)
+    dq.log_dataset(mock_dataset_with_ids, split="train")
+    dq.log_dataset(mock_dataset_with_ids, split="validation")
+    dq.log_dataset(mock_dataset_with_ids, split="test")
+
+    trainer = Trainer(
+        model,
+        args_default,
+        train_dataset=train_dataset,
+        eval_dataset=test_dataset,
+        tokenizer=tokenizer,
+        compute_metrics=compute_metrics,
+    )
+    # 🔭🌕 Galileo logging
+    watch(trainer)
+    trainer.train()
+    trainer.predict(val_dataset)
+    ThreadPoolManager.wait_for_threads()
+    # All data for splits should be logged
+    assert len(vaex.open(f"{LOCATION}/training/0/*.hdf5")) == len(train_dataset)
+    assert len(vaex.open(f"{LOCATION}/validation/0/*.hdf5")) == len(val_dataset)
+    assert len(vaex.open(f"{LOCATION}/test/0/*.hdf5")) == len(test_dataset)
+
+    # Should upload without failing on data validation or otherwise
+    dq.finish()
+
+
+@patch.object(dq.core.init.ApiClient, "valid_current_user", return_value=True)
+@patch.object(dq.core.finish, "_version_check")
+@patch.object(dq.core.finish, "_reset_run")
+@patch.object(dq.core.finish, "upload_dq_log_file")
+@patch.object(dq.clients.api.ApiClient, "make_request")
+@patch.object(dq.core.finish, "wait_for_run")
+def test_hf_watch_no_train(
+    mock_wait_for_run: MagicMock,
+    mock_make_request: MagicMock,
+    mock_upload_log_file: MagicMock,
+    mock_reset_run: MagicMock,
+    mock_version_check: MagicMock,
+    mock_valid_user: MagicMock,
+    set_test_config: Callable,
+    cleanup_after_use: Generator,
+) -> None:
+    """Base case: Tests creating a new project and run"""
+    set_test_config(task_type=TaskType.text_classification)
+    # 🔭🌕 Galileo logging
+    dq.set_labels_for_run(mock_hf_dataset.features["label"].names)
+    test_dataset = mock_dataset_with_ids
+
+    dq.log_dataset(test_dataset, split="test")
+
+    trainer = Trainer(
+        model,
+        args_default,
+        train_dataset=encoded_train_dataset,
+        eval_dataset=encoded_test_dataset,
+        tokenizer=tokenizer,
+        compute_metrics=compute_metrics,
+    )
+    # 🔭🌕 Galileo logging
+    watch(trainer)
+    dq.set_epoch_and_split(0, Split.test)
+    trainer.predict(encoded_test_dataset)
+    ThreadPoolManager.wait_for_threads()
+    # All data for splits should be logged
+    assert len(vaex.open(f"{LOCATION}/test/0/*.hdf5")) == len(test_dataset)
+    # Should upload without failing on data validation or otherwise
+    dq.finish()
```

### Comparing `dataquality-0.8.9/tests/integrations/keras/test_experimental.py` & `dataquality-0.9.1a1/tests/integrations/keras/test_experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import dataquality as dq
 from dataquality.integrations.experimental.keras import unwatch, watch
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.thread_pool import ThreadPoolManager
 from tests.conftest import LOCATION
 
 # from tests.conftest import LOCATION
-from tests.test_utils.hf_datasets_mock import mock_dataset, mock_dataset_numbered
+from tests.test_utils.hf_datasets_mock import mock_dataset_numbered, mock_hf_dataset
 
 tmp_checkpoint = "tmp/tiny-distillbert"
 checkpoint = "hf-internal-testing/tiny-bert-for-token-classification"
 checkpoint = "distilbert-base-uncased"
 # Load models locally
 
 try:
@@ -46,15 +46,15 @@
         return_tensors="tf",
     )
 
 
 data_collator = DataCollatorWithPadding(tokenizer=tokenizer, return_tensors="tf")
 
 # 🔭🌕 Galileo logging
-mock_dataset_with_ids = mock_dataset.map(
+mock_dataset_with_ids = mock_hf_dataset.map(
     lambda x, idx: {"id": idx}, with_indices=True
 ).select(range(7))
 mock_dataset_with_ids_number = mock_dataset_numbered.map(
     lambda x, idx: {"id": idx}, with_indices=True
 ).select(range(7))
 
 encoded_train_dataset = mock_dataset_with_ids.map(
```

### Comparing `dataquality-0.8.9/tests/integrations/keras/test_utils.py` & `dataquality-0.9.1a1/tests/integrations/keras/test_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/integrations/spacy/conftest.py` & `dataquality-0.9.1a1/tests/integrations/spacy/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/integrations/spacy/test_spacy_integration.py` & `dataquality-0.9.1a1/tests/integrations/spacy/test_spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/integrations/spacy/test_spacy_ner.py` & `dataquality-0.9.1a1/tests/integrations/spacy/test_spacy_ner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pickle
-from typing import Dict, List, Tuple
+from typing import Callable, Dict, List, Tuple
 from unittest import mock
 from unittest.mock import MagicMock
 
 import numpy as np
+import pandas as pd
 import pytest
 import spacy
 import vaex
 from spacy.language import Language
 from spacy.pipeline.ner import EntityRecognizer
 from spacy.tokens import Doc
 from spacy.training import Example
@@ -38,15 +39,16 @@
 from tests.test_utils.spacy_integration_constants_inference import (
     NER_INFERENCE_DATA,
     NER_INFERENCE_PRED_TOKEN_SPANS,
     TestSpacyInfExpectedResults,
 )
 
 
-def test_log_input_examples_without_watch():
+def test_log_input_examples_without_watch(set_test_config: Callable):
+    set_test_config(task_type="text_ner")
     with pytest.raises(GalileoException) as e:
         log_input_examples(NER_TRAINING_DATA, split="training")
     assert (
         e.value.args[0]
         == "Galileo does not have any logged labels. Did you forget to call "
         "watch(nlp) before log_input_examples(...)?"
     )
@@ -183,21 +185,31 @@
 
     data, embs, probs = load_ner_data_from_local(
         "training", inf_name_or_epoch=num_epochs - 1
     )
 
     assert len(data) == 5
     assert all(data["id"] == range(len(data)))
-    assert data.equals(
-        TestSpacyExpectedResults.gt_data
-    ), f"Received the following data df {data}"
+    for col in data.columns:
+        if pd.api.types.is_numeric_dtype(data[col].dtype):
+            assert np.allclose(
+                data[col].to_numpy(), TestSpacyExpectedResults.gt_data[col].to_numpy()
+            )
+        else:
+            assert data[[col]].equals(TestSpacyExpectedResults.gt_data[[col]])
 
     assert embs["id"].tolist() == list(range(len(embs)))
-    embs = embs["emb"].to_numpy().astype(np.float16)
-    assert all([span_emb in TestSpacyExpectedResults.gt_embs for span_emb in embs])
+    embs = embs["emb"].to_numpy().astype(np.float32)
+    embs_expected = TestSpacyExpectedResults.gt_embs
+    is_close = np.isclose(embs[:, np.newaxis], embs_expected, atol=1e-2)
+    # For each element in array1, check if any element in array2 is close
+    any_close = np.any(is_close, axis=1)
+
+    # Check if all elements in array1 have a close value in array2
+    assert np.all(any_close)
 
     assert len(probs) == 8
     # arrange the probs array to account for misordering of logged samples
     probs = probs.sort(["sample_id", "span_start"])
     # Drop multi-dimensional columns
     probs = probs.drop(["id", "conf_prob", "loss_prob"]).to_pandas_df()
     probs.equals(TestSpacyExpectedResults.gt_probs)
@@ -401,33 +413,53 @@
 
     data, embs, probs = load_ner_data_from_local(
         "inference", inf_name_or_epoch="inf-name"
     )
 
     assert len(data) == 5
     assert all(data["id"] == range(len(data)))
-    assert data.equals(TestSpacyInfExpectedResults.gt_data)
+    for col in data.columns:
+        if pd.api.types.is_numeric_dtype(data[col].dtype):
+            assert np.allclose(
+                data[col].to_numpy(),
+                TestSpacyInfExpectedResults.gt_data[col].to_numpy(),
+            )
+        else:
+            assert data[[col]].equals(TestSpacyInfExpectedResults.gt_data[[col]])
 
     assert embs["id"].tolist() == list(range(7))
     embs = embs["emb"].to_numpy()
     # Since order might change due to multi-threading we verify each embedding
     # is in the expected list, but don't check the exact order
-    assert all([span_emb in TestSpacyInfExpectedResults.gt_embs for span_emb in embs])
+    embs_expected = TestSpacyInfExpectedResults.gt_embs
+    is_close = np.isclose(embs[:, np.newaxis], embs_expected, atol=1e-3)
+    # For each element in array1, check if any element in array2 is close
+    any_close = np.any(is_close, axis=1)
 
+    # Check if all elements in array1 have a close value in array2
+    assert np.all(any_close)
     # arrange the probs array to account for misordering of logged samples
     assert len(probs) == 7
     probs = probs.sort(["sample_id", "span_start"])
     conf_probs = probs["conf_prob"].to_numpy()
     assert np.isclose(conf_probs, TestSpacyInfExpectedResults.gt_conf_prob).all()
 
     # Drop conf_prob since pandas doesn't support multi-dimensional arrays
     pdf = probs.drop(["id", "conf_prob"]).to_pandas_df()
-    assert pdf.equals(TestSpacyInfExpectedResults.gt_probs)
+    for col in pdf.columns:
+        if pd.api.types.is_numeric_dtype(pdf[col].dtype):
+            assert np.allclose(
+                pdf[col].to_numpy(),
+                TestSpacyInfExpectedResults.gt_probs[col].to_numpy(),
+            )
+        else:
+            assert pdf[[col]].equals(TestSpacyInfExpectedResults.gt_probs[[col]])
 
 
+@pytest.mark.skip(reason="flaky, needs a fix")
 def test_spacy_training_then_inference(
     nlp: Language, training_examples: List[Example], inference_docs: List[Doc]
 ) -> None:
     """Test that we can log training data, then inference data
 
     We don't assert exact values here, just that the data is logged to the correct files
     and a few simple assertions about the DF lengths and split names.
```

### Comparing `dataquality-0.8.9/tests/integrations/torch/test_pt_utils.py` & `dataquality-0.9.1a1/tests/integrations/torch/test_pt_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/loggers/test_multi_label.py` & `dataquality-0.9.1a1/tests/loggers/test_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/loggers/test_ner.py` & `dataquality-0.9.1a1/tests/loggers/test_ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,18 @@
     good_new_spans = [
         {"start": 0, "end": 1, "label": "YEAR"},
         {"start": 3, "end": 7, "label": "ACTOR"},
     ]
     assert new_spans == good_new_spans
 
 
-def test_construct_gold_sequence() -> None:
+def test_construct_gold_sequence(
+    cleanup_after_use: Callable, set_test_config: Callable
+) -> None:
+    set_test_config(default_task_type=TaskType.text_ner)
     len_sequence = 15
     case_1_seq_bio = [
         "O",
         "O",
         "B-PER",
         "I-PER",
         "B-ORG",
@@ -712,15 +715,15 @@
         with pytest.raises(AssertionError) as e:
             TextNERDataLogger._clean_labels()
         assert e.value.args[0] == expected_err_message
     else:
         TextNERDataLogger._clean_labels()
 
 
-@mock.patch("dataquality.utils.vaex.create_data_embs")
+@mock.patch("dataquality.utils.vaex.create_data_embs_df")
 def test_create_and_upload_data_embs_skipped_ner(
     mock_create_embs: mock.MagicMock,
     cleanup_after_use: Callable,
     set_test_config: Callable,
 ) -> None:
     set_test_config(task_type="text_ner")
```

### Comparing `dataquality-0.8.9/tests/schemas/test_conditions.py` & `dataquality-0.9.1a1/tests/schemas/test_conditions.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_dataquality.py` & `dataquality-0.9.1a1/tests/test_dataquality.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     _log_text_classification_data,
     validate_cleanup_data,
     validate_uploaded_data,
 )
 
 MAX_META_COLS = BaseGalileoDataLogger.MAX_META_COLS
 MAX_STR_LEN = BaseGalileoDataLogger.MAX_STR_LEN
+MAX_DOC_LEN = BaseGalileoDataLogger.MAX_DOC_LEN
 
 
 def test_threaded_logging_and_upload(
     cleanup_after_use: Callable, set_test_config: Callable
 ) -> None:
     """
     Tests that threaded calls to upload still yield non-missing datasets
@@ -156,40 +157,42 @@
 ) -> None:
     """
     Tests our metadata logging validation
     """
     meta = {
         "test1": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],
         "meta2": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],
-        "bad_attr": [
+        "doc1": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "doc2": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "doc3": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "too_many_doc": [
             "te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)
+        ],  # 4th doc, ignored
+        "doc_too_long": [
+            "te" * MAX_DOC_LEN for _ in range(NUM_RECORDS * NUM_LOGS)
         ],  # String too long
         "another_bad_attr": ["test", "test", "test"],  # Wrong number of values
         # Right length, but can't contain a list
         "bad_attr_3": [[1]] + [random() for _ in range(NUM_RECORDS * NUM_LOGS - 1)],
         "gold": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],  # Reserved key
     }
 
     # Too many metadata columns
     for i in range(MAX_META_COLS):
         meta[f"attr_{i}"] = [random() for _ in range(NUM_RECORDS * NUM_LOGS)]
 
-    _log_text_classification_data(meta=meta)
-    valid_meta_cols = ["test1", "meta2"]
-    valid_meta_cols += [f"attr_{i}" for i in range(MAX_META_COLS - len(meta))]
-    try:
-        # Equivalent to the users `finish` call, but we don't want to clean up files yet
-        c = dataquality.get_data_logger("text_classification")
-        c.upload()
-        validate_uploaded_data(meta_cols=valid_meta_cols)
-        c._cleanup()
-        validate_cleanup_data()
-    finally:
-        # Mock finish() call without calling the API
-        ThreadPoolManager.wait_for_threads()
+    c = dataquality.get_data_logger("text_classification")
+    c.meta = meta
+    c.validate_metadata(NUM_RECORDS * NUM_LOGS)
+
+    removed_cols = ["too_many_doc", "doc_too_long", "another_bad_attr", "bad_attr_3"]
+    for col in removed_cols:
+        assert col not in c.meta
+
+    assert len(c.meta) == MAX_META_COLS
 
 
 def test_logging_duplicate_ids(
     cleanup_after_use: Callable, set_test_config: Callable
 ) -> None:
     """
     Tests that logging duplicate ids triggers a failure
@@ -214,15 +217,16 @@
 def test_logging_inference_run(
     cleanup_after_use: Callable, set_test_config: Callable, input_data: Callable
 ) -> None:
     """
     Tests that logging metadata columns only attach to the splits we log them for
     """
     inference_data = input_data(
-        split="inference", meta={"inference_meta_1": [3.14, 42]}
+        split="inference",
+        meta={"inference_meta_1": np.array([3.14, 42], dtype=np.float32)},
     )
     dataquality.log_data_samples(**inference_data)
     inference_data = input_data(split="inference", inference_name="last-week-customers")
     dataquality.log_data_samples(**inference_data)
 
     dataquality.set_split("inference", inference_name="all-customers")
     embs_1 = np.random.rand(2, 100)
@@ -249,41 +253,44 @@
     inference_data_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/data/data.hdf5")
     inference_data_2 = vaex.open(
         f"{TEST_PATH}/inference/last-week-customers/data/data.hdf5"
     )
 
     assert "inference_meta_1" in inference_data_1.get_column_names()
     assert "inference_meta_1" not in inference_data_2.get_column_names()
-    assert sorted(inference_data_1["inference_meta_1"].tolist()) == [3.14, 42]
+    # Compare each pair of float numbers within the tolerance level (1e-6)
+    actual = sorted(inference_data_1["inference_meta_1"].tolist())
+    expected = [3.14, 42]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
 
     inference_emb_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/emb/emb.hdf5")
     inference_emb_2 = vaex.open(
         f"{TEST_PATH}/inference/last-week-customers/emb/emb.hdf5"
     )
 
-    assert (inference_emb_1.emb.to_numpy() == embs_1).all()
-    assert (inference_emb_2.emb.to_numpy() == embs_2).all()
+    assert np.isclose(inference_emb_1.emb.to_numpy(), embs_1).all()
+    assert np.isclose(inference_emb_2.emb.to_numpy(), embs_2).all()
 
     inference_prob_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/prob/prob.hdf5")
     inference_prob_2 = vaex.open(
         f"{TEST_PATH}/inference/last-week-customers/prob/prob.hdf5"
     )
 
     assert "logits" not in inference_prob_1.get_column_names()
     assert "logits" not in inference_prob_2.get_column_names()
     assert "prob" in inference_prob_1.get_column_names()
     assert "prob" in inference_prob_2.get_column_names()
 
-    assert (
-        inference_prob_1.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(logits_1)
+    assert np.isclose(
+        inference_prob_1.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(logits_1),
     ).all()
-    assert (
-        inference_prob_2.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(logits_2)
+    assert np.isclose(
+        inference_prob_2.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(logits_2),
     ).all()
 
 
 def test_logging_train_test_inference(
     cleanup_after_use: Callable, set_test_config: Callable, input_data: Callable
 ) -> None:
     """
@@ -326,25 +333,31 @@
     dataquality.get_data_logger().upload()
 
     train_data = vaex.open(f"{TEST_PATH}/training/0/data/data.hdf5")
     test_data = vaex.open(f"{TEST_PATH}/test/0/data/data.hdf5")
     inference_data = vaex.open(f"{TEST_PATH}/inference/all-customers/data/data.hdf5")
 
     assert "training_meta" in train_data.get_column_names()
-    assert sorted(train_data["training_meta"].tolist()) == [1.414, 123]
+    # Compare each pair of float numbers within the tolerance level (1e-6)
+    actual = sorted(train_data["training_meta"].tolist())
+    expected = [1.414, 123]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
+
     assert "test_meta" in test_data.get_column_names()
-    assert sorted(test_data["test_meta"].tolist()) == [3.14, 42]
+    actual = sorted(test_data["test_meta"].tolist())
+    expected = [3.14, 42]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
 
     train_emb_data = vaex.open(f"{TEST_PATH}/training/0/emb/emb.hdf5")
     test_emb_data = vaex.open(f"{TEST_PATH}/test/0/emb/emb.hdf5")
     inference_emb_data = vaex.open(f"{TEST_PATH}/inference/all-customers/emb/emb.hdf5")
 
-    assert (train_emb_data.emb.to_numpy() == train_embs).all()
-    assert (test_emb_data.emb.to_numpy() == test_embs).all()
-    assert (inference_emb_data.emb.to_numpy() == inf_embs).all()
+    assert np.isclose(train_emb_data.emb.to_numpy(), train_embs).all()
+    assert np.isclose(test_emb_data.emb.to_numpy(), test_embs).all()
+    assert np.isclose(inference_emb_data.emb.to_numpy(), inf_embs).all()
 
     train_prob_data = vaex.open(f"{TEST_PATH}/training/0/prob/prob.hdf5")
     test_prob_data = vaex.open(f"{TEST_PATH}/test/0/prob/prob.hdf5")
     inference_prob_data = vaex.open(
         f"{TEST_PATH}/inference/all-customers/prob/prob.hdf5"
     )
 
@@ -356,41 +369,46 @@
     assert "test_meta" in test_data.get_column_names()
     assert "test_meta" not in inference_data.get_column_names()
 
     assert "logits" not in train_prob_data.get_column_names()
     assert "logits" not in test_prob_data.get_column_names()
     assert "logits" not in inference_prob_data.get_column_names()
 
-    assert (
-        train_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(train_logits)
+    assert np.isclose(
+        train_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(train_logits),
     ).all()
-    assert (
-        test_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(test_logits)
+    assert np.isclose(
+        test_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(test_logits),
     ).all()
-    assert (
-        inference_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(inf_logits)
+    assert np.isclose(
+        inference_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(inf_logits),
     ).all()
 
 
 def test_prob_only(set_test_config) -> None:
     """Tests that the last_epoch is determined at the split level"""
     logger = dataquality.get_data_logger()
     logger.logger_config.last_epoch = 5
     train_split_runs = ["0", "1", "5", "3", "4"]
     val_split_runs = ["0", "1", "3", "4"]
     test_split_runs = ["0"]
 
-    assert logger.prob_only(train_split_runs, "training", "0")
-    assert not logger.prob_only(train_split_runs, "training", "5")
-    assert logger.prob_only(val_split_runs, "validation", "0")
-    assert not logger.prob_only(val_split_runs, "validation", "5")
-    assert not logger.prob_only(test_split_runs, "test", "0")
+    assert logger.prob_only(train_split_runs, "training", "0", last_epoch=None)
+    assert not logger.prob_only(train_split_runs, "training", "5", last_epoch=None)
+    # Last epoch of 9 is invalid because the largest epoch is 5
+    assert not logger.prob_only(test_split_runs, "test", "5", last_epoch=9)
+    assert not logger.prob_only(train_split_runs, "training", "3", last_epoch=4)
+    assert logger.prob_only(val_split_runs, "validation", "0", last_epoch=None)
+    assert not logger.prob_only(val_split_runs, "validation", "5", last_epoch=None)
+    assert not logger.prob_only(test_split_runs, "test", "0", last_epoch=None)
+    # Last epoch of 2 is invalid because the largest epoch is 0
+    assert not logger.prob_only(test_split_runs, "test", "0", last_epoch=2)
 
 
 @mock.patch.object(dataquality.clients.api.ApiClient, "get_presigned_url")
 @mock.patch.object(
     dataquality.clients.objectstore.ObjectStore, "_upload_file_from_local"
 )
 def test_log_invalid_model_outputs(
@@ -647,15 +665,15 @@
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
     "_get_data_dict",
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
-    "validate",
+    "validate_and_format",
 )
 def test_log_batch_error_warns(
     mock_validate: mock.MagicMock,
     mock_get_data: mock.MagicMock,
     mock_write: mock.MagicMock,
     set_test_config: Callable,
 ) -> None:
@@ -675,15 +693,15 @@
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
     "_get_data_dict",
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
-    "validate",
+    "validate_and_format",
 )
 def test_log_assertion_error_raises(
     mock_validate: mock.MagicMock,
     mock_get_data: mock.MagicMock,
     mock_write: mock.MagicMock,
     set_test_config: Callable,
     cleanup_after_use: Callable,
```

### Comparing `dataquality-0.8.9/tests/test_telemetrics.py` & `dataquality-0.9.1a1/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/data_utils.py` & `dataquality-0.9.1a1/tests/test_utils/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 NUM_RECORDS = 50
 NUM_LOGS = 30
 MULTI_LABEL_NUM_TASKS = 4
 
 
 def validate_uploaded_data(
-    expected_num_records: int = None,
+    expected_num_records: Optional[int] = None,
     meta_cols: Optional[List] = None,
     multi_label=False,
 ) -> None:
     """
     Checks for testing
     """
     expected_num_records = expected_num_records or NUM_RECORDS * NUM_LOGS
```

### Comparing `dataquality-0.8.9/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.1a1/tests/test_utils/hf_integration_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,19 +455,28 @@
 mock_batch_encoding.word_ids = lambda batch_index: BATCH_WORD_IDS[batch_index]
 mock_batch_encoding._encodings = [BatchTokens(tokens) for tokens in BATCH_TOKENS]
 
 # We mock the tokenizer so we don't need to use the real tokenizer from hf
 mock_tokenizer = mock.Mock()
 mock_tokenizer.batch_encode_plus.return_value = mock_batch_encoding
 
-# We mock the hf dataset so we don't need to download a dataset from hf
-mock_ds = datasets.Dataset.from_dict(UNADJUSTED_TOKEN_DATA)
 tag_names = [
     "O",
     "B-PER",
     "I-PER",
     "B-ORG",
     "I-ORG",
     "B-LOC",
     "I-LOC",
 ]
-mock_ds.features["ner_tags"].feature.names = tag_names
+# We mock the hf dataset so we don't need to download a dataset from hf
+mock_ds = datasets.Dataset.from_dict(
+    UNADJUSTED_TOKEN_DATA,
+    # features=datasets.Features({"ner_tags": datasets.Features(names=tag_names)}),
+)
+new_features = mock_ds.features.copy()
+new_features["ner_tags"] = datasets.Sequence(
+    feature=datasets.ClassLabel(names=tag_names),
+    length=-1,
+    id=None,
+)
+mock_ds = mock_ds.cast(new_features)
```

### Comparing `dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.1a1/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/lightning_model.py` & `dataquality-0.9.1a1/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/mock_request.py` & `dataquality-0.9.1a1/tests/test_utils/mock_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 from uuid import uuid4
 
 import dataquality
 from dataquality import __version__
 
 config = dataquality.config
 
@@ -13,15 +13,15 @@
 
 
 class MockResponse:
     def __init__(
         self,
         json_data: Union[Dict, List],
         status_code: int,
-        headers: Dict = None,
+        headers: Optional[Dict] = None,
     ) -> None:
         self.headers = headers or {}
         self.json_data = json_data
         self.status_code = status_code
         if status_code in (200, 204):
             self.ok = True
         else:
@@ -51,14 +51,15 @@
 def mocked_login_requests(
     request_url: str,
     json: Dict = {},
     params: Dict = {},
     headers: Dict = {},
     data: Dict = {},
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("login"):
         return MockResponse(
             {
                 "access_token": "mock_token",
             },
             200,
@@ -71,59 +72,77 @@
 def mocked_failed_login_requests(
     request_url: str,
     json: Dict = {},
     params: Dict = {},
     headers: Dict = {},
     data: Dict = {},
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("login"):
         return MockResponse({"detail": "Incorrect login credentials."}, 404)
     return MockResponse({}, 404)
 
 
 def mocked_get_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     res = [
         {"id": uuid4(), "name": EXISTING_PROJECT, "project_id": uuid4()},
         {"id": uuid4(), "name": EXISTING_RUN, "project_id": uuid4()},
         {"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN, "project_id": uuid4()},
     ]
     return MockResponse(res, 200)
 
 
+def mocked_upload_image_dataset(
+    request_url: str,
+    json: Dict,
+    params: Dict,
+    headers: Dict,
+    data: Dict,
+    timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
+) -> MockResponse:
+    if request_url.endswith("task_type=image_classfication"):
+        return MockResponse({"response": "done"}, 200)
+    return MockResponse({}, 400)
+
+
 def mocked_create_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     global TMP_CREATE_NEW_PROJ_RUN
     TMP_CREATE_NEW_PROJ_RUN = json["name"]
     res = {"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN}
     return MockResponse(res, 200)
 
 
 def mocked_missing_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     # Run does not exist
     if "run_name" in request_url:
         return MockResponse([], 204)
     # Project does exist
@@ -148,40 +167,43 @@
 def mocked_missing_project_name(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse([], 200)
 
 
 def mocked_delete_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse([{"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN}], 200)
 
 
 def mocked_delete_project_not_found(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse({"detail": "project not found"}, 404)
 
 
 def mocked_login() -> None:
```

### Comparing `dataquality-0.8.9/tests/test_utils/ner_constants.py` & `dataquality-0.9.1a1/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/spacy_integration.py` & `dataquality-0.9.1a1/tests/test_utils/spacy_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from spacy.util import minibatch
 from thinc.model import Model
 from tqdm import tqdm
 from vaex.dataframe import DataFrameLocal
 
 import dataquality
 from dataquality.integrations.spacy import log_input_examples, watch
+from dataquality.schemas.split import Split
 from tests.conftest import SUBDIRS, TEST_PATH
 
 MINIBATCH_SZ = 3
 
 
 def train_model(
     nlp: Language,
@@ -30,28 +31,28 @@
         training_examples (List[Example]): The training examples.
         num_epochs (int, optional): The number of epochs to train for. Defaults to 5.
     """
     optimizer = nlp.initialize(lambda: training_examples)
 
     # Galileo code
     watch(nlp)
-    log_input_examples(training_examples, "training")
-    log_input_examples(training_examples, "test")
+    log_input_examples(training_examples, Split.training)
+    log_input_examples(training_examples, Split.test)
 
     training_losses = []
     for itn in range(num_epochs):
         dataquality.set_epoch(itn)
         batches = minibatch(training_examples, MINIBATCH_SZ)
 
-        dataquality.set_split("training")
+        dataquality.set_split(Split.training)
         for batch in tqdm(batches):
             training_loss = nlp.update(batch, drop=0.5, sgd=optimizer)
             training_losses.append(training_loss["ner"])
 
-        dataquality.set_split("test")
+        dataquality.set_split(Split.test)
         nlp.evaluate(training_examples, batch_size=MINIBATCH_SZ)
 
     # TODO: need to support the following line for inference
     # nlp('Thank you for your subscription renewal')
 
     # Evaluation Loop
     # TODO: Should change this with an actual evaluation loop
```

### Comparing `dataquality-0.8.9/tests/test_utils/spacy_integration_constants.py` & `dataquality-0.9.1a1/tests/test_utils/spacy_integration_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,21 @@
                         67,
                         68,
                         74,
                         75,
                         80,
                         81,
                         82,
-                    ]
+                    ],
+                    dtype=np.int32,
+                ),
+                np.array(
+                    [0, 5, 6, 9, 10, 13, 14, 18, 19, 31, 32, 39],
+                    dtype=np.int32,
                 ),
-                np.array([0, 5, 6, 9, 10, 13, 14, 18, 19, 31, 32, 39]),
                 np.array(
                     [
                         0,
                         3,
                         4,
                         7,
                         8,
@@ -153,18 +157,25 @@
                         86,
                         86,
                         92,
                         92,
                         93,
                         93,
                         98,
-                    ]
+                    ],
+                    dtype=np.int32,
+                ),
+                np.array(
+                    [0, 1, 2, 6, 7, 11, 12, 19, 20, 23, 24, 27, 28, 35],
+                    dtype=np.int32,
+                ),
+                np.array(
+                    [0, 4, 5, 8, 9, 11, 11, 12, 13, 17, 18, 25, 26, 28, 29, 36],
+                    dtype=np.int32,
                 ),
-                np.array([0, 1, 2, 6, 7, 11, 12, 19, 20, 23, 24, 27, 28, 35]),
-                np.array([0, 4, 5, 8, 9, 11, 11, 12, 13, 17, 18, 25, 26, 28, 29, 36]),
             ],
             "data_schema_version": [1] * 5,
         }
     )
     gt_embs = np.array(
         [
             [
@@ -692,15 +703,15 @@
                 2.2109e00,
                 1.5576e00,
                 -5.3760e-01,
                 2.5469e00,
                 -4.0625e-01,
             ],
         ],
-        dtype=np.float16,
+        dtype=np.float32,
     )
 
     gt_probs = pd.DataFrame(
         data={
             "sample_id": [0, 0, 1, 2, 2, 3, 4, 4],
             "split": ["training"] * _num_gold_spans,
             "epoch": [num_epochs - 1] * _num_gold_spans,
```

### Comparing `dataquality-0.8.9/tests/test_utils/spacy_integration_constants_inference.py` & `dataquality-0.9.1a1/tests/test_utils/spacy_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/utils/test_auto.py` & `dataquality-0.9.1a1/tests/utils/test_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/utils/test_dq_logger.py` & `dataquality-0.9.1a1/tests/utils/test_dq_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,32 @@
 from dataquality.utils.dq_logger import dq_log_file_path
 
 
 @mock.patch("dataquality.core.finish._reset_run")
 @mock.patch("dataquality.core.finish._version_check")
 @mock.patch.object(dq.clients.api.ApiClient, "make_request")
 @mock.patch.object(dq.clients.api.ApiClient, "get_presigned_url")
+@mock.patch.object(
+    dq.clients.api.ApiClient,
+    "get_healthcheck_dq",
+    return_value={
+        "bucket_names": {
+            "images": "galileo-images",
+            "results": "galileo-project-runs-results",
+            "root": "galileo-project-runs",
+        },
+        "minio_fqdn": "127.0.0.1:9000",
+    },
+)
 @mock.patch.object(dq.clients.objectstore.ObjectStore, "download_file")
 @mock.patch.object(dq.clients.objectstore.ObjectStore, "_upload_file_from_local")
 def test_std_log(
     mock_upload_from_local: MagicMock,
     mock_download: MagicMock,
+    mock_bucket_names: MagicMock,
     mock_presigned_url: MagicMock,
     mock_finish: MagicMock,
     mock_version_check: MagicMock,
     mock_reset_run: MagicMock,
     set_test_config: Callable,
     cleanup_after_use: Callable,
     input_data: Callable,
```

### Comparing `dataquality-0.8.9/tests/utils/test_version.py` & `dataquality-0.9.1a1/tests/utils/test_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,14 @@
 
 
 @mock.patch("requests.get", side_effect=mocked_healthcheck_request)
 def test_get_api_version(mock_get_api_version: MagicMock) -> None:
     assert version._get_api_version() == __version__
 
 
-def test_parse_version_alpha() -> None:
-    assert str(version._parse_version("v0.0.1-alpha")) == "0.0.1a0"
-
-
-def test_parse_version_beta() -> None:
-    assert str(version._parse_version("v0.0.2-beta")) == "0.0.2b0"
-
-
 @mock.patch("requests.get", side_effect=mocked_healthcheck_request_new_api_version)
 def test_version_check_fail(mock_get_healthcheck: MagicMock) -> None:
     with pytest.raises(GalileoException):
         version._version_check()
 
 
 @mock.patch("requests.get", side_effect=mocked_healthcheck_request)
```

