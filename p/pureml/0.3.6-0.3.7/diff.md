# Comparing `tmp/pureml-0.3.6.tar.gz` & `tmp/pureml-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.6.tar", max compression
+gzip compressed data, was "pureml-0.3.7.tar", max compression
```

## Comparing `pureml-0.3.6.tar` & `pureml-0.3.7.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0    11789 2023-04-27 08:41:10.100182 pureml-0.3.6/README.md
--rw-r--r--   0        0        0      735 2023-04-27 08:41:10.100182 pureml-0.3.6/pureml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:41:10.100182 pureml-0.3.6/pureml/cli/__init__.py
--rw-r--r--   0        0        0     9746 2023-04-27 08:41:10.116182 pureml-0.3.6/pureml/cli/auth.py
--rw-r--r--   0        0        0     2447 2023-04-27 08:41:10.128183 pureml-0.3.6/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3201 2023-04-27 08:41:10.128183 pureml-0.3.6/pureml/cli/main.py
--rw-r--r--   0        0        0     3365 2023-04-27 08:41:10.140183 pureml-0.3.6/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.6/pureml/cli/public.pem
--rw-r--r--   0        0        0     1697 2023-04-27 08:41:10.140183 pureml-0.3.6/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7182 2023-04-27 08:41:10.148183 pureml-0.3.6/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2861 2023-04-27 08:41:10.148183 pureml-0.3.6/pureml/components/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/auth.py
--rw-r--r--   0        0        0    15075 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/dataset.py
--rw-r--r--   0        0        0       88 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-27 08:41:10.168184 pureml-0.3.6/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6634 2023-04-27 08:41:10.180184 pureml-0.3.6/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6708 2023-04-27 08:41:10.188184 pureml-0.3.6/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9603 2023-04-27 08:41:10.196184 pureml-0.3.6/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6679 2023-04-27 08:41:10.200184 pureml-0.3.6/pureml/components/log/image.py
--rw-r--r--   0        0        0     2041 2023-04-27 08:41:10.200184 pureml-0.3.6/pureml/components/log/log.py
--rw-r--r--   0        0        0     5929 2023-04-27 08:41:10.212185 pureml-0.3.6/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     5925 2023-04-27 08:41:10.224185 pureml-0.3.6/pureml/components/log/params.py
--rw-r--r--   0        0        0     6166 2023-04-27 08:41:10.228185 pureml-0.3.6/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6181 2023-04-27 08:41:10.240185 pureml-0.3.6/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6049 2023-04-27 08:41:10.248185 pureml-0.3.6/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6776 2023-04-27 08:41:10.264186 pureml-0.3.6/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6168 2023-04-27 08:41:10.268186 pureml-0.3.6/pureml/components/log/video.py
--rw-r--r--   0        0        0    13206 2023-04-27 08:41:10.276186 pureml-0.3.6/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.6/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.6/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.6/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.6/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.6/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.6/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.6/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.6/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.6/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.6/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.6/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.6/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.6/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.6/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.6/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.6/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.6/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.6/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.6/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.6/pureml/package/__init__.py
--rw-r--r--   0        0        0     6446 2023-04-27 08:41:10.288186 pureml-0.3.6/pureml/package/docker.py
--rw-r--r--   0        0        0     6014 2023-04-27 08:41:10.300186 pureml-0.3.6/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.6/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.6/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.6/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.6/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      439 2023-04-27 08:41:10.308187 pureml-0.3.6/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2580 2023-04-27 08:41:10.308187 pureml-0.3.6/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.6/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.6/pureml/schema/dataset.py
--rw-r--r--   0        0        0      163 2023-04-27 08:41:10.312187 pureml-0.3.6/pureml/schema/env.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.6/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.6/pureml/schema/paths.py
--rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/schema/predict.py
--rw-r--r--   0        0        0      308 2023-04-27 08:41:10.316187 pureml-0.3.6/pureml/schema/request.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.6/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.6/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.6/pureml/utils/constants.py
--rw-r--r--   0        0        0     1230 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/env.py
--rw-r--r--   0        0        0     2942 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.6/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.6/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.6/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.6/pureml/utils/predict.py
--rw-r--r--   0        0        0      816 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.6/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.6/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.6/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1927 2023-04-27 08:41:10.324187 pureml-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-04-27 08:45:08.465073 pureml-0.3.7/README.md
+-rw-r--r--   0        0        0      735 2023-05-05 17:31:20.649406 pureml-0.3.7/pureml/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9746 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/auth.py
+-rw-r--r--   0        0        0     2447 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3201 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/main.py
+-rw-r--r--   0        0        0     3365 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.7/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1697 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7182 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2861 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/auth.py
+-rw-r--r--   0        0        0    15074 2023-04-27 20:01:59.833567 pureml-0.3.7/pureml/components/dataset.py
+-rw-r--r--   0        0        0       88 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6634 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6708 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9603 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6679 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2041 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/log.py
+-rw-r--r--   0        0        0     5929 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     5925 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6166 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6181 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6049 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6776 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6168 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13508 2023-04-27 20:02:03.894144 pureml-0.3.7/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.7/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.7/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.7/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.7/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.7/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.7/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.7/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.7/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.7/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.7/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.7/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.7/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.7/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.7/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.7/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.7/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.7/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.7/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.7/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.7/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6446 2023-04-30 20:33:34.175641 pureml-0.3.7/pureml/package/docker.py
+-rw-r--r--   0        0        0     6244 2023-05-05 17:28:39.229763 pureml-0.3.7/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.7/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.7/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.7/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.7/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      439 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2580 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.7/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.7/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      163 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/env.py
+-rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.7/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.7/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/schema/predict.py
+-rw-r--r--   0        0        0      308 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/schema/request.py
+-rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.7/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.7/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.7/pureml/utils/constants.py
+-rw-r--r--   0        0        0     1230 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/env.py
+-rw-r--r--   0        0        0     2942 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.7/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.7/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.7/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.7/pureml/utils/predict.py
+-rw-r--r--   0        0        0      816 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.7/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.7/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.7/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1927 2023-05-05 17:31:25.116351 pureml-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.7/PKG-INFO
```

### Comparing `pureml-0.3.6/README.md` & `pureml-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/__init__.py` & `pureml-0.3.7/pureml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

### Comparing `pureml-0.3.6/pureml/cli/auth.py` & `pureml-0.3.7/pureml/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/cli/helpers.py` & `pureml-0.3.7/pureml/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/cli/main.py` & `pureml-0.3.7/pureml/cli/main.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/cli/orgs.py` & `pureml-0.3.7/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/cli/puremlconfig.py` & `pureml-0.3.7/pureml/cli/puremlconfig.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/cli/secrets.py` & `pureml-0.3.7/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/__init__.py` & `pureml-0.3.7/pureml/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/auth.py` & `pureml-0.3.7/pureml/components/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/dataset.py` & `pureml-0.3.7/pureml/components/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,34 +340,35 @@
 
         response = requests.post(url, files=files, data=data, headers=headers)
         # print(response.request.headers)
         # print(response.request.body)
 
         if response.ok:
 
+            dataset_version = None
+
             # print(response.json())
             try:
                 dataset_version = response.json()["data"][0]["version"]
                 print("Version: ", dataset_version)
-                dataset_label = ":".join([label, dataset_label])
+                dataset_label = ":".join([label, dataset_version])
                 print("Dataset label: ", dataset_label)
 
                 if is_empty:
                     print(f"[bold green]Lineage has been registered!")
                 else:
                     print(f"[bold green]Dataset and lineage have been registered!")
 
                 # reset_config(key=config_keys.dataset.value)
 
             except Exception as e:
                 print(
                     "[bold red] Incorrect json response. Dataset has not been registered"
                 )
                 print(e)
-                dataset_version = None
 
             return True, dataset_hash, dataset_version
         else:
             print(f"[bold red]Dataset has not been registered!")
             print(response.text)
 
             return True, dataset_hash, None
```

### Comparing `pureml-0.3.6/pureml/components/log/arrays.py` & `pureml-0.3.7/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/artifacts.py` & `pureml-0.3.7/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/audio.py` & `pureml-0.3.7/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/figure.py` & `pureml-0.3.7/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/image.py` & `pureml-0.3.7/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/log.py` & `pureml-0.3.7/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/metrics.py` & `pureml-0.3.7/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/params.py` & `pureml-0.3.7/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/pip_requirement.py` & `pureml-0.3.7/pureml/components/log/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/predict.py` & `pureml-0.3.7/pureml/components/log/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/resources.py` & `pureml-0.3.7/pureml/components/log/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/tabular.py` & `pureml-0.3.7/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/log/video.py` & `pureml-0.3.7/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/components/model.py` & `pureml-0.3.7/pureml/components/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,22 +306,32 @@
             "storage": storage.STORAGE,
         }
 
         response = requests.post(url, files=files, data=data, headers=headers)
         # print(response.request.headers)
 
         if response.ok:
-            print(f"[bold green]Model has been registered!")
 
-            model_version = response.json()["data"][0]["version"]
-            print("Model Version: ", model_version)
-            model_label = ":".join([label, model_version])
-            print("Model label: ", model_label)
+            model_version = None
 
-            # reset_config(key=config_keys.model.value)
+            # print(response.json())
+            try:
+                print(f"[bold green]Model has been registered!")
+
+                model_version = response.json()["data"][0]["version"]
+                print("Model Version: ", model_version)
+                model_label = ":".join([label, model_version])
+                print("Model label: ", model_label)
+
+                # reset_config(key=config_keys.model.value)
+            except Exception as e:
+                print(
+                    "[bold red] Incorrect json response. Model has not been registered"
+                )
+                print(e)
 
             return True, model_hash, model_version
 
         else:
             print(f"[bold red]Model has not been registered!")
             print(response.text)
```

### Comparing `pureml-0.3.6/pureml/config/parser.py` & `pureml-0.3.7/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/dataset.py` & `pureml-0.3.7/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/load_data.py` & `pureml-0.3.7/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/model.py` & `pureml-0.3.7/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/pip_requirements.py` & `pureml-0.3.7/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/predict.py` & `pureml-0.3.7/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/decorators/transformer.py` & `pureml-0.3.7/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/classification.py` & `pureml-0.3.7/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/eval.py` & `pureml-0.3.7/pureml/evaluate/eval.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/grade.py` & `pureml-0.3.7/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.7/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.7/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/f1.py` & `pureml-0.3.7/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/mae.py` & `pureml-0.3.7/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/mse.py` & `pureml-0.3.7/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/precision.py` & `pureml-0.3.7/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/recall.py` & `pureml-0.3.7/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.7/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/evaluate/regression.py` & `pureml-0.3.7/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/lineage/data/create_lineage.py` & `pureml-0.3.7/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/package/docker.py` & `pureml-0.3.7/pureml/package/docker.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/package/fastapi.py` & `pureml-0.3.7/pureml/package/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import uvicorn
 from fastapi import FastAPI
 from pureml.schema import FastAPISchema, PredictSchema, PathSchema
 from pureml.utils.package import process_input, process_output
 from pureml.utils.version_utils import parse_version_label
 from pureml import predict, pip_requirement, resources
 from pureml.utils.resources import zip_content, unzip_content
+import sys
 
 
 prediction_schema = PredictSchema()
 fastapi_schema = FastAPISchema()
 path_schema = PathSchema()
 
 
@@ -192,16 +193,22 @@
 
 def run(label, predict_path=None, requirements_path=None):
 
     create_fastapi_file(
         label, predict_path=predict_path, requirements_path=requirements_path
     )
 
-    run_command = "python '{api_path}'".format(
-        api_path=fastapi_schema.PATH_FASTAPI_FILE
-    )
+    interpreter_path = str(sys.executable)
+
+    if os.path.exists(interpreter_path):
 
-    os.system(run_command)
+        run_command = "{interpreter_path} '{api_path}'".format(
+            interpreter_path=interpreter_path, api_path=fastapi_schema.PATH_FASTAPI_FILE
+        )
+
+        os.system(run_command)
+    else:
+        print("Interpreter not found at", interpreter_path)
 
     # app = FastAPI()
 
     # uvicorn.run(app, host=fastapi_schema.API_IP_HOST, port=fastapi_schema.PORT_FASTAPI)
```

### Comparing `pureml-0.3.6/pureml/packaging/__init__.py` & `pureml-0.3.7/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_framework.py` & `pureml-0.3.7/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.7/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.7/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.7/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.7/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.7/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.7/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.7/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.7/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.7/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/packaging.py` & `pureml-0.3.7/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/packaging/packaging_utils.py` & `pureml-0.3.7/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/predictor/predictor.py` & `pureml-0.3.7/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/schema/backend.py` & `pureml-0.3.7/pureml/schema/backend.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/schema/packaging.py` & `pureml-0.3.7/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/schema/paths.py` & `pureml-0.3.7/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/schema/predict.py` & `pureml-0.3.7/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/config.py` & `pureml-0.3.7/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/constants.py` & `pureml-0.3.7/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/env.py` & `pureml-0.3.7/pureml/utils/env.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/hash.py` & `pureml-0.3.7/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/log_utils.py` & `pureml-0.3.7/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/package.py` & `pureml-0.3.7/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/pipeline.py` & `pureml-0.3.7/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/predict.py` & `pureml-0.3.7/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/readme.py` & `pureml-0.3.7/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/resources.py` & `pureml-0.3.7/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pureml/utils/version_utils.py` & `pureml-0.3.7/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.6/pyproject.toml` & `pureml-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
```

### Comparing `pureml-0.3.6/PKG-INFO` & `pureml-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
```

