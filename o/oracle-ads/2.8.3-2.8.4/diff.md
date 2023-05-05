# Comparing `tmp/oracle_ads-2.8.3.tar.gz` & `tmp/oracle_ads-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracle_ads-2.8.3.tar", last modified: Wed Mar 22 22:35:15 2023, max compression
+gzip compressed data, was "oracle_ads-2.8.4.tar", last modified: Fri May  5 18:10:05 2023, max compression
```

## Comparing `oracle_ads-2.8.3.tar` & `oracle_ads-2.8.4.tar`

### file list

```diff
@@ -1,552 +1,535 @@
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.579111 oracle_ads-2.8.3/
--rwxrwxrwx   0 datascience  (1000) users      (100)     1845 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/LICENSE.txt
--rwxrwxrwx   0 datascience  (1000) users      (100)      822 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/MANIFEST.in
--rw-r--r--   0 datascience  (1000) users      (100)     8872 2023-03-22 22:35:15.579111 oracle_ads-2.8.3/PKG-INFO
--rwxrwxrwx   0 datascience  (1000) users      (100)     7466 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/README.md
--rwxrwxrwx   0 datascience  (1000) users      (100)    48614 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/THIRD_PARTY_LICENSES.txt
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.461111 oracle_ads-2.8.3/ads/
--rwxrwxrwx   0 datascience  (1000) users      (100)     3835 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)       66 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/ads
--rwxrwxrwx   0 datascience  (1000) users      (100)       25 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/ads_version.json
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.462111 oracle_ads-2.8.3/ads/automl/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/automl/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    13159 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/automl/driver.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    35984 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/automl/provider.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.463111 oracle_ads-2.8.3/ads/bds/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/bds/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3846 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/bds/auth.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7714 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/bds/big_data_service.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.464111 oracle_ads-2.8.3/ads/catalog/
--rwxrwxrwx   0 datascience  (1000) users      (100)      459 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/catalog/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    59997 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/catalog/model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16462 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/catalog/notebook.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16091 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/catalog/project.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5791 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/catalog/summary.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      938 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/cli.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.470111 oracle_ads-2.8.3/ads/common/
--rwxrwxrwx   0 datascience  (1000) users      (100)      293 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1893 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/analyzer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.471111 oracle_ads-2.8.3/ads/common/artifact/
--rwxrwxrwx   0 datascience  (1000) users      (100)      879 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/artifact/.model-ignore
--rwxrwxrwx   0 datascience  (1000) users      (100)      265 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/artifact/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    33843 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/auth.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7852 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/base_properties.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2458 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/card_identifier.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    20253 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/config.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6939 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/data.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3548 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/data_serializer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.472111 oracle_ads-2.8.3/ads/common/decorator/
--rwxrwxrwx   0 datascience  (1000) users      (100)      207 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/decorator/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2834 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/decorator/argument_to_case.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2042 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/decorator/deprecate.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6121 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/decorator/runtime_dependency.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1253 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/decorator/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      493 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/error.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      849 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/extended_enum.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.473111 oracle_ads-2.8.3/ads/common/function/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/function/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4937 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/function/fn_util.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      645 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/function/func_conf.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)     2859 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/ipython.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    27269 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    72273 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_artifact.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2557 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_artifact_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)    26571 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_export_util.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9351 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_introspect.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      641 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_metadata.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16529 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/model_metadata_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3977 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/object_storage_details.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4623 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/oci_client.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1325 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/oci_datascience.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    42155 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/oci_logging.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    34334 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/oci_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4463 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/oci_resource.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15688 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/serializer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    44314 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    22306 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/common/word_lists.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5945 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/config.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.474111 oracle_ads-2.8.3/ads/data_labeling/
--rwxrwxrwx   0 datascience  (1000) users      (100)      678 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     8530 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/boundingbox.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1131 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/constants.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9558 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/data_labeling_service.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.475111 oracle_ads-2.8.3/ads/data_labeling/interface/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/interface/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      395 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/interface/loader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      386 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/interface/parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      652 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/interface/reader.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.476111 oracle_ads-2.8.3/ads/data_labeling/loader/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/loader/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7769 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/loader/file_loader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3446 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/metadata.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.476111 oracle_ads-2.8.3/ads/data_labeling/mixin/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/mixin/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9452 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/mixin/data_labeling.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3489 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/ner.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.477111 oracle_ads-2.8.3/ads/data_labeling/parser/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/parser/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    13651 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/parser/dls_record_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3378 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/parser/export_metadata_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17416 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/parser/export_record_parser.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.479111 oracle_ads-2.8.3/ads/data_labeling/reader/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    22145 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/dataset_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4082 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/dls_record_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2303 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/export_record_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2756 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/jsonl_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6885 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/metadata_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10548 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/reader/record_reader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1396 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/record.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.480111 oracle_ads-2.8.3/ads/data_labeling/visualizer/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/visualizer/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15880 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/visualizer/image_visualizer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10774 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/data_labeling/visualizer/text_visualizer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.480111 oracle_ads-2.8.3/ads/database/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/database/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11015 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/database/connection.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.481111 oracle_ads-2.8.3/ads/dataflow/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataflow/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    65401 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataflow/dataflow.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2829 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataflow/dataflowsummary.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.488111 oracle_ads-2.8.3/ads/dataset/
--rwxrwxrwx   0 datascience  (1000) users      (100)      265 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11654 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/classification_dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     8025 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/correlation.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17306 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/correlation_plot.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5427 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/dask_series.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3592 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/dataframe_transformer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    69799 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11935 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/dataset_browser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    32506 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/dataset_with_target.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      602 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/exception.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    37220 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/factory.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1140 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/feature_engineering_transformer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4144 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/feature_selection.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      941 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/forecasting_dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    27776 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/helper.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1989 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/label_encoder.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1642 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/pipeline.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    26056 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/plot.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2293 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/progress.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    12909 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/recommendation.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    22004 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/recommendation_transformer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      523 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/regression_dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    39503 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/sampled_dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3646 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/target.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      522 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dataset/timeseries.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.488111 oracle_ads-2.8.3/ads/dbmixin/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dbmixin/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5803 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/dbmixin/db_pandas_accessor.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.489111 oracle_ads-2.8.3/ads/environment/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/environment/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2171 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/environment/ml_runtime.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.490111 oracle_ads-2.8.3/ads/evaluations/
--rwxrwxrwx   0 datascience  (1000) users      (100)     4387 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/evaluations/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    39617 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/evaluations/evaluation_plot.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    53173 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/evaluations/evaluator.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    20748 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/evaluations/statistical_metrics.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.490111 oracle_ads-2.8.3/ads/experiments/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/experiments/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.492111 oracle_ads-2.8.3/ads/explanations/
--rwxrwxrwx   0 datascience  (1000) users      (100)      429 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4109 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/base_explainer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7448 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/explainer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    41704 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/mlx_global_explainer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15006 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/mlx_interface.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    12273 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/mlx_local_explainer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     8509 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/explanations/mlx_whatif_explainer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.494111 oracle_ads-2.8.3/ads/feature_engineering/
--rwxrwxrwx   0 datascience  (1000) users      (100)      860 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.494111 oracle_ads-2.8.3/ads/feature_engineering/accessor/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    18295 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/dataframe_accessor.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.496111 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5787 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/correlation.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10212 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/eda_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3184 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     8527 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1972 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15334 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/accessor/series_accessor.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.497111 oracle_ads-2.8.3/ads/feature_engineering/adsimage/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsimage/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6726 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsimage/image.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5416 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsimage/image_reader.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.497111 oracle_ads-2.8.3/ads/feature_engineering/adsimage/interface/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsimage/interface/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      488 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsimage/interface/reader.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.498111 oracle_ads-2.8.3/ads/feature_engineering/adsstring/
--rwxrwxrwx   0 datascience  (1000) users      (100)      308 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9676 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/common_regex_mixin.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.498111 oracle_ads-2.8.3/ads/feature_engineering/adsstring/oci_language/
--rwxrwxrwx   0 datascience  (1000) users      (100)      392 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/oci_language/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3219 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/oci_language.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.499111 oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      956 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2906 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/nltk_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6724 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/spacy_parser.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.500111 oracle_ads-2.8.3/ads/feature_engineering/adsstring/string/
--rwxrwxrwx   0 datascience  (1000) users      (100)      384 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/string/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6925 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/adsstring/string.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      974 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/data_schema.json
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.500111 oracle_ads-2.8.3/ads/feature_engineering/dataset/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/dataset/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)  1600358 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/dataset/zip_code_data.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1174 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/exceptions.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.510111 oracle_ads-2.8.3/ads/feature_engineering/feature_type/
--rwxrwxrwx   0 datascience  (1000) users      (100)     5185 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5558 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/address.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.511111 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9676 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3513 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/oci_language.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.512111 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/parsers/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      956 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/parsers/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2919 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6737 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7203 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/string.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1642 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5214 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/boolean.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4455 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/category.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3779 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/constant.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4771 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/continuous.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9299 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/creditcard.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5771 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/datetime.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3825 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/discrete.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1005 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/document.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7233 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/gis.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.513111 oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17237 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/feature_validator.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11659 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/feature_warning.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3769 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/warnings.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4240 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/integer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4230 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3866 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address_v4.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3945 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address_v6.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7822 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/lat_long.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      980 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/object.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3919 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/ordinal.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3780 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/phone_number.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5048 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/string.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2611 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/text.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      999 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/unknown.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4545 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type/zip_code.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15686 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/feature_type_manager.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    23829 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/schema.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6605 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/feature_engineering/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.515111 oracle_ads-2.8.3/ads/hpo/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3379 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/_imports.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15276 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/ads_search_space.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10630 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/distributions.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9706 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/objective.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    57385 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/search_cv.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1725 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/stopping_criterion.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16525 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/tuner_artifact.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2752 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5207 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/validation.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.517111 oracle_ads-2.8.3/ads/hpo/visualization/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      716 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_contour.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      596 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_edf.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      638 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_intermediate_values.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      694 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_optimization_history.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5850 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_parallel_coordinate.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      821 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/hpo/visualization/_param_importances.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.519111 oracle_ads-2.8.3/ads/jobs/
--rwxrwxrwx   0 datascience  (1000) users      (100)     1399 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    18578 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/ads_job.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.519111 oracle_ads-2.8.3/ads/jobs/builders/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4133 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/base.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.521111 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/
--rwxrwxrwx   0 datascience  (1000) users      (100)      246 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4178 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    34769 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dataflow.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    52780 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dsc_job.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    40361 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dsc_job_runtime.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1623 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/infrastructure/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.522111 oracle_ads-2.8.3/ads/jobs/builders/runtimes/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/runtimes/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    12640 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/runtimes/artifact.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7069 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/runtimes/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3866 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/runtimes/container_runtime.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    31887 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/builders/runtimes/python_runtime.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3168 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4643 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/env_var_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5288 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/extension.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.523111 oracle_ads-2.8.3/ads/jobs/schema/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/schema/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2202 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/schema/infrastructure_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)      649 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/schema/job_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)     3460 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/schema/runtime_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)     4244 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/schema/validator.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7902 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/serializer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.525111 oracle_ads-2.8.3/ads/jobs/templates/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      258 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/container.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6248 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/driver_notebook.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17947 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/driver_oci.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1803 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/driver_python.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17935 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/templates/driver_utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3324 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/jobs/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.529111 oracle_ads-2.8.3/ads/model/
--rwxrwxrwx   0 datascience  (1000) users      (100)     1900 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17205 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/artifact.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6897 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/artifact_downloader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7251 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/artifact_uploader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7885 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/base_properties.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.529111 oracle_ads-2.8.3/ads/model/common/
--rwxrwxrwx   0 datascience  (1000) users      (100)      898 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/common/.model-ignore
--rwxrwxrwx   0 datascience  (1000) users      (100)      207 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/common/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4068 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/common/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    37743 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/datascience_model.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.531111 oracle_ads-2.8.3/ads/model/deployment/
--rwxrwxrwx   0 datascience  (1000) users      (100)      665 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.532111 oracle_ads-2.8.3/ads/model/deployment/common/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/common/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4397 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/common/progress_bar.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10088 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/common/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17227 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/model_deployer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    58620 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/model_deployment.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15962 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/model_deployment_infrastructure.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17700 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/model_deployment_properties.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16357 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/deployment/model_deployment_runtime.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.535111 oracle_ads-2.8.3/ads/model/extractor/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2352 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/automl_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2244 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/huggingface_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2081 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/keras_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2442 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/lightgbm_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2927 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/model_info_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3729 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/model_info_extractor_factory.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2156 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/pytorch_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/sklearn_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2263 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/spark_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2148 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/tensorflow_extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2472 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/extractor/xgboost_extractor.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.537111 oracle_ads-2.8.3/ads/model/framework/
--rwxrwxrwx   0 datascience  (1000) users      (100)      201 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7561 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/automl_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17008 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/huggingface_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10414 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/lightgbm_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11379 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/pytorch_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9888 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/sklearn_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11926 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/spark_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9817 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/tensorflow_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    10337 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/framework/xgboost_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)   126348 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/generic_model.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.538111 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.538111 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/artifact_introspection_test/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17101 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1802 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/score.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9348 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_introspect.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    54098 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_metadata.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16621 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_metadata_mixin.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2088 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_properties.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    22821 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/model_version_set.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.540111 oracle_ads-2.8.3/ads/model/runtime/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9350 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/env_info.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1100 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/model_deployment_details.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1740 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/model_provenance_details.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2379 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/runtime_info.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.541111 oracle_ads-2.8.3/ads/model/runtime/schemas/
--rwxrwxrwx   0 datascience  (1000) users      (100)      286 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/schemas/inference_env_info_schema.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)      603 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/schemas/model_provenance_schema.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)      278 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/schemas/training_env_info_schema.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)     6689 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/runtime/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.542111 oracle_ads-2.8.3/ads/model/serde/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/serde/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1124 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/serde/common.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    18577 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/serde/model_input.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    43205 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/serde/model_serializer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.543111 oracle_ads-2.8.3/ads/model/service/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/service/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    21155 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/service/oci_datascience_model.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    22054 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/service/oci_datascience_model_deployment.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5648 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/service/oci_datascience_model_version_set.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.543111 oracle_ads-2.8.3/ads/model/transformer/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/transformer/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    11252 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model/transformer/onnx_transformer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.544111 oracle_ads-2.8.3/ads/model_artifact_boilerplate/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model_artifact_boilerplate/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.544111 oracle_ads-2.8.3/ads/model_artifact_boilerplate/artifact_introspection_test/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model_artifact_boilerplate/artifact_introspection_test/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    17053 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1802 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/model_artifact_boilerplate/score.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.545111 oracle_ads-2.8.3/ads/mysqldb/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/mysqldb/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7828 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/mysqldb/mysql_db.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.546111 oracle_ads-2.8.3/ads/opctl/
--rwxrwxrwx   0 datascience  (1000) users      (100)      396 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.548111 oracle_ads-2.8.3/ads/opctl/backend/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4872 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/ads_dataflow.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    19863 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/ads_ml_job.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3314 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/ads_ml_pipeline.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7407 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/ads_model_deployment.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1908 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    25282 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/backend/local.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    13506 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    24780 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/cmds.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.550111 oracle_ads-2.8.3/ads/opctl/conda/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4802 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    21785 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/cmds.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1026 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/config.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)      194 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/manifest_template.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)     6180 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/multipart_uploader.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2196 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/conda/pack.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.551111 oracle_ads-2.8.3/ads/opctl/config/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1472 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/base.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.552111 oracle_ads-2.8.3/ads/opctl/config/diagnostics/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/diagnostics/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.552111 oracle_ads-2.8.3/ads/opctl/config/diagnostics/distributed/
--rwxrwxrwx   0 datascience  (1000) users      (100)     2822 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
--rwxrwxrwx   0 datascience  (1000) users      (100)     8354 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/merger.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    12603 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/resolver.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2263 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/utils.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      630 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/validator.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1928 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/versioner.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.552111 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/
--rwxrwxrwx   0 datascience  (1000) users      (100)      342 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2152 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/base.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.553111 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/distributed/
--rwxrwxrwx   0 datascience  (1000) users      (100)      293 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/distributed/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     7756 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1299 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/constants.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.554111 oracle_ads-2.8.3/ads/opctl/diagnostics/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/diagnostics/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      862 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/diagnostics/__main__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9103 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/diagnostics/check_distributed_job_requirements.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5215 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/diagnostics/check_requirements.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      254 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/diagnostics/requirement_exception.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.555111 oracle_ads-2.8.3/ads/opctl/distributed/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1187 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/certificates.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5520 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    18772 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/cmds.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.557111 oracle_ads-2.8.3/ads/opctl/distributed/common/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    16060 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/abstract_cluster_provider.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3454 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/abstract_framework_spec_builder.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4477 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_config_helper.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      603 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_provider_factory.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2145 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_runner.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      890 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/distributed/common/framework_factory.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.559111 oracle_ads-2.8.3/ads/opctl/docker/
--rwxrwxrwx   0 datascience  (1000) users      (100)     1154 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/Dockerfile
--rwxrwxrwx   0 datascience  (1000) users      (100)     3509 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.gpu
--rwxrwxrwx   0 datascience  (1000) users      (100)     3746 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.job
--rwxrwxrwx   0 datascience  (1000) users      (100)     5965 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.job.gpu
--rwxrwxrwx   0 datascience  (1000) users      (100)      165 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/cuda.repo
--rwxrwxrwx   0 datascience  (1000) users      (100)     1579 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/docker/merge_dependencies.py
--rwxrwxrwx   0 datascience  (1000) users      (100)       68 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/index.yaml
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.559111 oracle_ads-2.8.3/ads/opctl/spark/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spark/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1198 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spark/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5055 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spark/cmds.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.560111 oracle_ads-2.8.3/ads/opctl/spec/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spec/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6050 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spec/abstract_operator_spec.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1509 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spec/operator_spec_factory.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/spec/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.560111 oracle_ads-2.8.3/ads/opctl/templates/
--rwxrwxrwx   0 datascience  (1000) users      (100)     3341 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/templates/diagnostic_report_template.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)    10887 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/opctl/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.561111 oracle_ads-2.8.3/ads/oracledb/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/oracledb/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    12889 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/oracledb/oracle_db.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.563111 oracle_ads-2.8.3/ads/pipeline/
--rwxrwxrwx   0 datascience  (1000) users      (100)     1268 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    82750 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/ads_pipeline.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    27985 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/ads_pipeline_run.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    19688 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/ads_pipeline_step.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.563111 oracle_ads-2.8.3/ads/pipeline/builders/
--rwxrwxrwx   0 datascience  (1000) users      (100)      205 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/builders/__init__.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.563111 oracle_ads-2.8.3/ads/pipeline/builders/infrastructure/
--rwxrwxrwx   0 datascience  (1000) users      (100)      205 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/builders/infrastructure/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1103 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/builders/infrastructure/custom_script.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3480 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/cli.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9067 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/extension.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.564111 oracle_ads-2.8.3/ads/pipeline/schema/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/schema/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      589 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/schema/cs_step_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)      507 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/schema/ml_step_schema.json
--rwxrwxrwx   0 datascience  (1000) users      (100)     1369 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/schema/pipeline_schema.json
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.565111 oracle_ads-2.8.3/ads/pipeline/visualizer/
--rwxrwxrwx   0 datascience  (1000) users      (100)      204 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/visualizer/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15542 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/visualizer/base.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     9208 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/visualizer/graph_renderer.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2625 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/pipeline/visualizer/text_renderer.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.567111 oracle_ads-2.8.3/ads/secrets/
--rwxrwxrwx   0 datascience  (1000) users      (100)      381 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15817 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/adb.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3705 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/auth_token.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    13926 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/big_data_service.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5668 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/mysqldb.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6146 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/oracledb.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15230 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/secrets/secrets.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.567111 oracle_ads-2.8.3/ads/telemetry/
--rwxrwxrwx   0 datascience  (1000) users      (100)      230 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/telemetry/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1695 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/telemetry/telemetry.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.572111 oracle_ads-2.8.3/ads/templates/
--rwxrwxrwx   0 datascience  (1000) users      (100)      254 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/dataflow_pyspark.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)      466 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/dataflow_sparksql.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)      441 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/func.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5304 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score-pkl.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)    10498 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     4956 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_generic.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5455 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_huggingface_pipeline.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5695 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_lightgbm.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)    13892 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_onnx.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)    15835 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_onnx_new.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5621 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_oracle_automl.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5035 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_pyspark.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     6503 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_pytorch.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5743 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_scikit-learn.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     4953 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_spark.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5626 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_tensorflow.jinja2
--rwxrwxrwx   0 datascience  (1000) users      (100)     5516 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/templates/score_xgboost.jinja2
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.574111 oracle_ads-2.8.3/ads/text_dataset/
--rwxrwxrwx   0 datascience  (1000) users      (100)      210 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6563 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/backends.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    15378 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/dataset.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     6102 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/extractor.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1507 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/options.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      600 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/udfs.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1551 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/text_dataset/utils.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.577111 oracle_ads-2.8.3/ads/type_discovery/
--rwxrwxrwx   0 datascience  (1000) users      (100)      264 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)      583 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/abstract_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1416 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/constant_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1746 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/continuous_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     4457 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/credit_card_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3134 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/datetime_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3987 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/discrete_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     5900 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/document_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     3519 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/ip_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2831 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/latlon_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1952 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/phone_number_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     2710 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/type_discovery_driver.py
--rwxrwxrwx   0 datascience  (1000) users      (100)    20105 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/typed_feature.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1341 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/unknown_detector.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     1421 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/type_discovery/zipcode_detector.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.578111 oracle_ads-2.8.3/ads/vault/
--rwxrwxrwx   0 datascience  (1000) users      (100)      245 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/vault/__init__.py
--rwxrwxrwx   0 datascience  (1000) users      (100)     8624 2023-03-22 22:30:50.000000 oracle_ads-2.8.3/ads/vault/vault.py
-drwxr-xr-x   0 datascience  (1000) users      (100)        0 2023-03-22 22:35:15.579111 oracle_ads-2.8.3/oracle_ads.egg-info/
--rw-r--r--   0 datascience  (1000) users      (100)     8872 2023-03-22 22:35:14.000000 oracle_ads-2.8.3/oracle_ads.egg-info/PKG-INFO
--rw-r--r--   0 datascience  (1000) users      (100)    16761 2023-03-22 22:35:15.000000 oracle_ads-2.8.3/oracle_ads.egg-info/SOURCES.txt
--rw-r--r--   0 datascience  (1000) users      (100)        1 2023-03-22 22:35:14.000000 oracle_ads-2.8.3/oracle_ads.egg-info/dependency_links.txt
--rw-r--r--   0 datascience  (1000) users      (100)     3286 2023-03-22 22:35:15.000000 oracle_ads-2.8.3/oracle_ads.egg-info/requires.txt
--rw-r--r--   0 datascience  (1000) users      (100)        4 2023-03-22 22:35:15.000000 oracle_ads-2.8.3/oracle_ads.egg-info/top_level.txt
--rwxrwxrwx   0 datascience  (1000) users      (100)      103 2023-03-22 22:35:15.580111 oracle_ads-2.8.3/setup.cfg
--rwxrwxrwx   0 datascience  (1000) users      (100)     5058 2023-03-22 22:30:51.000000 oracle_ads-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/THIRD_PARTY_LICENSES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/ads
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/ads_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/automl/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/bds/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/bds/big_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.662151 oracle_ads-2.8.4/ads/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/catalog/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/artifact/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/card_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/argument_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/runtime_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/decorator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/dsc_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/extended_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/common/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/fn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/function/func_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_artifact_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_export_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/object_storage_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_datascience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/oci_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45941 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/common/word_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/data_labeling_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/loader/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/mixin/data_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.666151 oracle_ads-2.8.4/ads/data_labeling/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/dls_record_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/export_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/parser/export_record_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/data_labeling/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/dls_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/export_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/jsonl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/reader/record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/data_labeling/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/data_labeling/visualizer/text_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/database/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65402 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataflow/dataflowsummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dask_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataframe_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70924 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/dataset_with_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/feature_engineering_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/forecasting_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/recommendation_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/regression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dataset/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.670151 oracle_ads-2.8.4/ads/dbmixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dbmixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/dbmixin/db_pandas_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/environment/ml_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/evaluations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/evaluation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/evaluations/statistical_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/base_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_global_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_local_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/explanations/mlx_whatif_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/dataframe_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/accessor/series_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsimage/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/image_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsimage/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/oci_language/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/oci_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.674152 oracle_ads-2.8.4/ads/feature_engineering/adsstring/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/adsstring/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/data_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.678151 oracle_ads-2.8.4/ads/feature_engineering/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/dataset/zip_code_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/oci_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/creditcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type/zip_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/feature_type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/feature_engineering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/ads_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/tuner_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.682152 oracle_ads-2.8.4/ads/hpo/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/hpo/visualization/_param_importances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/ads_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59213 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/infrastructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/builders/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/container_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/builders/runtimes/python_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/env_var_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/infrastructure_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/job_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/runtime_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/schema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.686152 oracle_ads-2.8.4/ads/jobs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/templates/driver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/jobs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/artifact_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/base_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/datascience_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/deployment/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60706 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/deployment/model_deployment_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.690152 oracle_ads-2.8.4/ads/model/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/automl_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/huggingface_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/keras_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/lightgbm_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/model_info_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/model_info_extractor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/pytorch_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/sklearn_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/spark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/tensorflow_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/extractor/xgboost_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/automl_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/lightgbm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/tensorflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/framework/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131287 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/generic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_metadata_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/env_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/model_deployment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/model_provenance_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/runtime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/runtime/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/inference_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/model_provenance_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/schemas/training_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/serde/model_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21239 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/service/oci_datascience_model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/model/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/model/transformer/onnx_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/mysqldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/mysqldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/mysqldb/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.694152 oracle_ads-2.8.4/ads/opctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_ml_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/ads_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/manifest_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/multipart_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/conda/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/diagnostics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/check_distributed_job_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/diagnostics/requirement_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.698152 oracle_ads-2.8.4/ads/opctl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/distributed/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_cluster_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_framework_spec_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/distributed/common/framework_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/cuda.repo
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/docker/merge_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/model/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spark/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/abstract_operator_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/operator_spec_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/opctl/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/templates/diagnostic_report_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/opctl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/oracledb/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/oracledb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/oracledb/oracle_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/ads_pipeline_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.702152 oracle_ads-2.8.4/ads/pipeline/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/pipeline/visualizer/text_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/big_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/oracledb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/secrets/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/telemetry/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/dataflow_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/dataflow_sparksql.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/func.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score-pkl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_generic.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_huggingface_pipeline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_lightgbm.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_onnx.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_onnx_new.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_oracle_automl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_pytorch.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_scikit-learn.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_tensorflow.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/templates/score_xgboost.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.706152 oracle_ads-2.8.4/ads/text_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/text_dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/ads/type_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/abstract_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/constant_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/continuous_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/credit_card_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/datetime_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/discrete_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/document_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/ip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/latlon_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/phone_number_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/type_discovery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/typed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/unknown_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/type_discovery/zipcode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/ads/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/ads/vault/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/oracle_ads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 18:10:05.000000 oracle_ads-2.8.4/oracle_ads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 18:10:05.710152 oracle_ads-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-05 18:10:01.000000 oracle_ads-2.8.4/setup.py
```

### Comparing `oracle_ads-2.8.3/LICENSE.txt` & `oracle_ads-2.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/MANIFEST.in` & `oracle_ads-2.8.4/MANIFEST.in`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 include ads/model/runtime/schemas/*.yaml
 include ads/jobs/schema/**
 include ads/opctl/index.yaml
 include ads/opctl/operators/**/*.py
 include ads/opctl/docker/**
 include ads/opctl/conda/manifest_template.yaml
 include ads/opctl/conda/config.yaml
-include ads/pipeline/schema/*.json
 include ads/opctl/config/diagnostics/**/*.yaml
 include ads/opctl/templates/*.jinja2
 global-exclude tests/**
 global-exclude notebooks/**
 exclude tests/**
 exclude notebooks/**
 exclude build/lib/tests/**
 exclude build/lib/notebooks/**
 exclude benchmark/**
 include ads/ads
-include ads/model/common/*.*
+include ads/model/common/*.*
```

### Comparing `oracle_ads-2.8.3/PKG-INFO` & `oracle_ads-2.8.4/oracle_ads.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: oracle_ads
-Version: 2.8.3
+Name: oracle-ads
+Version: 2.8.4
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,141 +19,141 @@
 Description-Content-Type: text/markdown
 Provides-Extra: boosted
 Provides-Extra: notebook
 Provides-Extra: text
 Provides-Extra: viz
 Provides-Extra: data
 Provides-Extra: opctl
-Provides-Extra: mysql
 Provides-Extra: bds
 Provides-Extra: spark
 Provides-Extra: huggingface
 Provides-Extra: torch
 Provides-Extra: tensorflow
 Provides-Extra: geo
 Provides-Extra: onnx
 Provides-Extra: optuna
 Provides-Extra: complete
 Provides-Extra: all-optional
 Provides-Extra: all-public
 
-# Oracle Accelerated Data Science SDK (ADS)
+# Oracle Accelerated Data Science (ADS)
 
-[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=plastic)](https://pypi.org/project/oracle-ads/)
+[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://github.com/ambv/black)
 
-The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
+
+The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, ML Pipelines, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
 
 With ADS you can:
 
- - Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
- - Use feature types to characterize your data, create meaning summary statistics and plot. Use the warning and validation system to test the quality of your data.
- - Tune models using hyperparameter optimization with the `ADSTuner` tool.
- - Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
- - Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
- - Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
- - Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
- - Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
- - Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
+- Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
+- Tune models using hyperparameter optimization with the `ADSTuner` tool.
+- Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
+- Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
+- Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
+- Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
+- Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
+- Define and run an end-to-end machine learning orchestration covering all the steps of machine learning lifecycle in a repeatable, continuous [ML Pipelines](https://accelerated-data-science.readthedocs.io/en/latest/user_guide/pipeline/overview.html#).
+- Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
 
 ## Installation
 
 You have various options when installing ADS.
 
 ### Installing the oracle-ads base package
 
 ```bash
-  $ python3 -m pip install oracle-ads
+  python3 -m pip install oracle-ads
 ```
 
 ### Installing extras libraries
 
-The `all-optional` module will install all optional dependencies.
+The `all-optional` module will install all optional dependencies. Note the single quotes around installation of extra libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[all-optional]
+  python3 -m pip install 'oracle-ads[all-optional]'
 ```
 
 To work with gradient boosting models, install the `boosted` module. This module includes XGBoost and LightGBM model classes.
 
 ```bash
-  $ python3 -m pip install oracle-ads[boosted]
+  python3 -m pip install 'oracle-ads[boosted]'
 ```
 
 For big data use cases using Oracle Big Data Service (BDS), install the `bds` module. It includes the following libraries, `ibis-framework[impala]`, `hdfs[kerberos]` and `sqlalchemy`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[bds]
+  python3 -m pip install 'oracle-ads[bds]'
 ```
 
 To work with a broad set of data formats (for example, Excel, Avro, etc.) install the `data` module. It includes the `fastavro`, `openpyxl`, `pandavro`, `asteval`, `datefinder`, `htmllistparse`, and `sqlalchemy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[data]
+  python3 -m pip install 'oracle-ads[data]'
 ```
 
 To work with geospatial data install the `geo` module. It includes the `geopandas` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[geo]
+  python3 -m pip install 'oracle-ads[geo]'
 ```
 
 Install the `notebook` module to use ADS within a OCI Data Science service [notebook session](https://docs.oracle.com/en-us/iaas/data-science/using/manage-notebook-sessions.htm). This module installs `ipywidgets` and `ipython` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[notebook]
+  python3 -m pip install 'oracle-ads[notebook]'
 ```
 
 To work with ONNX-compatible run times and libraries designed to maximize performance and model portability, install the `onnx` module. It includes the following libraries, `onnx`, `onnxruntime`, `onnxmltools`, `skl2onnx`, `xgboost`, `lightgbm` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[onnx]
+  python3 -m pip install 'oracle-ads[onnx]'
 ```
 
 For infrastructure tasks, install the `opctl` module. It includes the following libraries, `oci-cli`, `docker`, `conda-pack`, `nbconvert`, `nbformat`, and `inflection`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[opctl]
+  python3 -m pip install 'oracle-ads[opctl]'
 ```
 
 For hyperparameter optimization tasks install the `optuna` module. It includes the `optuna` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[optuna]
+  python3 -m pip install 'oracle-ads[optuna]'
 ```
 
 Install the `tensorflow` module to include `tensorflow` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[tensorflow]
+  python3 -m pip install 'oracle-ads[tensorflow]'
 ```
 
 For text related tasks, install the `text` module. This will include the `wordcloud`, `spacy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[text]
+  python3 -m pip install 'oracle-ads[text]'
 ```
 
 Install the `torch` module to include `pytorch` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[torch]
+  python3 -m pip install 'oracle-ads[torch]'
 ```
 
 Install the `viz` module to include libraries for visualization tasks. Some of the key packages are `bokeh`, `folium`, `seaborn` and related packages.
 
 ```bash
-  $ python3 -m pip install oracle-ads[viz]
+  python3 -m pip install 'oracle-ads[viz]'
 ```
 
 **Note**
 
 Multiple extra dependencies can be installed together. For example:
 
 ```bash
-  $ python3 -m pip install  oracle-ads[notebook,viz,text]
+  python3 -m pip install  'oracle-ads[notebook,viz,text]'
 ```
 
 ## Documentation
 
   - [Oracle Accelerated Data Science SDK (ADS) Documentation](https://accelerated-data-science.readthedocs.io/en/latest/index.html)
   - [OCI Data Science and AI services Examples](https://github.com/oracle/oci-data-science-ai-samples)
   - [Oracle AI & Data Science Blog](https://blogs.oracle.com/ai-and-datascience/)
@@ -201,20 +200,18 @@
       bind_variables={ max_rows : 100 },
       connection_parameters=connection_parameters,
   )
 ```
 
 ## Contributing
 
-This project welcomes contributions from the community. Before submitting a pull request, please review our contribution guide [CONTRIBUTING.md](https://github.com/oracle/accelerated-data-science/blob/main/CONTRIBUTING.md).
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
 Find Getting Started instructions for developers in [README-development.md](https://github.com/oracle/accelerated-data-science/blob/main/README-development.md)
 
 ## Security
 
 Consult the security guide [SECURITY.md](https://github.com/oracle/accelerated-data-science/blob/main/SECURITY.md) for our responsible security vulnerability disclosure process.
 
 ## License
 
 Copyright (c) 2020, 2022 Oracle and/or its affiliates. Licensed under the [Universal Permissive License v1.0](https://oss.oracle.com/licenses/upl/)
-
-
```

### Comparing `oracle_ads-2.8.3/README.md` & `oracle_ads-2.8.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,122 @@
-# Oracle Accelerated Data Science SDK (ADS)
+# Oracle Accelerated Data Science (ADS)
 
-[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=plastic)](https://pypi.org/project/oracle-ads/)
+[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://github.com/ambv/black)
 
-The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
+
+The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, ML Pipelines, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
 
 With ADS you can:
 
- - Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
- - Use feature types to characterize your data, create meaning summary statistics and plot. Use the warning and validation system to test the quality of your data.
- - Tune models using hyperparameter optimization with the `ADSTuner` tool.
- - Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
- - Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
- - Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
- - Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
- - Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
- - Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
+- Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
+- Tune models using hyperparameter optimization with the `ADSTuner` tool.
+- Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
+- Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
+- Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
+- Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
+- Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
+- Define and run an end-to-end machine learning orchestration covering all the steps of machine learning lifecycle in a repeatable, continuous [ML Pipelines](https://accelerated-data-science.readthedocs.io/en/latest/user_guide/pipeline/overview.html#).
+- Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
 
 ## Installation
 
 You have various options when installing ADS.
 
 ### Installing the oracle-ads base package
 
 ```bash
-  $ python3 -m pip install oracle-ads
+  python3 -m pip install oracle-ads
 ```
 
 ### Installing extras libraries
 
-The `all-optional` module will install all optional dependencies.
+The `all-optional` module will install all optional dependencies. Note the single quotes around installation of extra libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[all-optional]
+  python3 -m pip install 'oracle-ads[all-optional]'
 ```
 
 To work with gradient boosting models, install the `boosted` module. This module includes XGBoost and LightGBM model classes.
 
 ```bash
-  $ python3 -m pip install oracle-ads[boosted]
+  python3 -m pip install 'oracle-ads[boosted]'
 ```
 
 For big data use cases using Oracle Big Data Service (BDS), install the `bds` module. It includes the following libraries, `ibis-framework[impala]`, `hdfs[kerberos]` and `sqlalchemy`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[bds]
+  python3 -m pip install 'oracle-ads[bds]'
 ```
 
 To work with a broad set of data formats (for example, Excel, Avro, etc.) install the `data` module. It includes the `fastavro`, `openpyxl`, `pandavro`, `asteval`, `datefinder`, `htmllistparse`, and `sqlalchemy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[data]
+  python3 -m pip install 'oracle-ads[data]'
 ```
 
 To work with geospatial data install the `geo` module. It includes the `geopandas` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[geo]
+  python3 -m pip install 'oracle-ads[geo]'
 ```
 
 Install the `notebook` module to use ADS within a OCI Data Science service [notebook session](https://docs.oracle.com/en-us/iaas/data-science/using/manage-notebook-sessions.htm). This module installs `ipywidgets` and `ipython` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[notebook]
+  python3 -m pip install 'oracle-ads[notebook]'
 ```
 
 To work with ONNX-compatible run times and libraries designed to maximize performance and model portability, install the `onnx` module. It includes the following libraries, `onnx`, `onnxruntime`, `onnxmltools`, `skl2onnx`, `xgboost`, `lightgbm` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[onnx]
+  python3 -m pip install 'oracle-ads[onnx]'
 ```
 
 For infrastructure tasks, install the `opctl` module. It includes the following libraries, `oci-cli`, `docker`, `conda-pack`, `nbconvert`, `nbformat`, and `inflection`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[opctl]
+  python3 -m pip install 'oracle-ads[opctl]'
 ```
 
 For hyperparameter optimization tasks install the `optuna` module. It includes the `optuna` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[optuna]
+  python3 -m pip install 'oracle-ads[optuna]'
 ```
 
 Install the `tensorflow` module to include `tensorflow` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[tensorflow]
+  python3 -m pip install 'oracle-ads[tensorflow]'
 ```
 
 For text related tasks, install the `text` module. This will include the `wordcloud`, `spacy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[text]
+  python3 -m pip install 'oracle-ads[text]'
 ```
 
 Install the `torch` module to include `pytorch` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[torch]
+  python3 -m pip install 'oracle-ads[torch]'
 ```
 
 Install the `viz` module to include libraries for visualization tasks. Some of the key packages are `bokeh`, `folium`, `seaborn` and related packages.
 
 ```bash
-  $ python3 -m pip install oracle-ads[viz]
+  python3 -m pip install 'oracle-ads[viz]'
 ```
 
 **Note**
 
 Multiple extra dependencies can be installed together. For example:
 
 ```bash
-  $ python3 -m pip install  oracle-ads[notebook,viz,text]
+  python3 -m pip install  'oracle-ads[notebook,viz,text]'
 ```
 
 ## Documentation
 
   - [Oracle Accelerated Data Science SDK (ADS) Documentation](https://accelerated-data-science.readthedocs.io/en/latest/index.html)
   - [OCI Data Science and AI services Examples](https://github.com/oracle/oci-data-science-ai-samples)
   - [Oracle AI & Data Science Blog](https://blogs.oracle.com/ai-and-datascience/)
@@ -162,15 +163,15 @@
       bind_variables={ max_rows : 100 },
       connection_parameters=connection_parameters,
   )
 ```
 
 ## Contributing
 
-This project welcomes contributions from the community. Before submitting a pull request, please review our contribution guide [CONTRIBUTING.md](https://github.com/oracle/accelerated-data-science/blob/main/CONTRIBUTING.md).
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
 Find Getting Started instructions for developers in [README-development.md](https://github.com/oracle/accelerated-data-science/blob/main/README-development.md)
 
 ## Security
 
 Consult the security guide [SECURITY.md](https://github.com/oracle/accelerated-data-science/blob/main/SECURITY.md) for our responsible security vulnerability disclosure process.
```

### Comparing `oracle_ads-2.8.3/THIRD_PARTY_LICENSES.txt` & `oracle_ads-2.8.4/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/__init__.py` & `oracle_ads-2.8.4/ads/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,32 +118,27 @@
 
     """
     global test_mode
     test_mode = mode
 
 
 def hello():
-    """
-    Imports Pandas, sets the documentation mode, and prints a fancy "Hello".
-    """
-    import pandas
-
-    global documentation_mode
-    global debug_mode
+    import oci
+    import ocifs
 
     print(
         f"""
 
   O  o-o   o-o
  / \\ |  \\ |
 o---o|   O o-o
 |   ||  /     |
 o   oo-o  o--o
 
-ADS SDK version: {__version__}
-Pandas version: {pandas.__version__}
-Debug mode: {debug_mode}
-"""
-    )
+ads v{__version__}
+oci v{oci.__version__}
+ocifs v{ocifs.__version__}
+
+""")
 
 
 configure_plotting()
```

### Comparing `oracle_ads-2.8.3/ads/automl/driver.py` & `oracle_ads-2.8.4/ads/automl/driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/automl/provider.py` & `oracle_ads-2.8.4/ads/automl/provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/bds/auth.py` & `oracle_ads-2.8.4/ads/bds/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from contextlib import contextmanager
 
 
 DEFAULT_KRB5_CONFIG_PATH = "~/.bds_config/krb5.conf"
 KRB5_CONFIG = "KRB5_CONFIG"
 
 
-class KRB5KinitError(Exception):
+class KRB5KinitError(Exception):   # pragma: no cover
     """KRB5KinitError class when kinit -kt command failed to generate cached ticket with the keytab file and the krb5 config file."""
 
     pass
 
 
 def has_kerberos_ticket():
     """Whether kerberos cache ticket exists."""
```

### Comparing `oracle_ads-2.8.3/ads/bds/big_data_service.py` & `oracle_ads-2.8.4/ads/bds/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/catalog/model.py` & `oracle_ads-2.8.4/ads/catalog/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,19 @@
 ]
 _MODEL_PROVENANCE_ATTRIBUTES = ModelProvenance().swagger_types.keys()
 _ETAG_KEY = "ETag"
 _MAX_ARTIFACT_SIZE_IN_BYTES = 2147483648  # 2GB
 _WORK_REQUEST_INTERVAL_IN_SEC = 3
 
 
-class ModelWithActiveDeploymentError(Exception):
+class ModelWithActiveDeploymentError(Exception):   # pragma: no cover
     pass
 
 
-class ModelArtifactSizeError(Exception):
+class ModelArtifactSizeError(Exception):   # pragma: no cover
     def __init__(self, max_artifact_size: str):
         super().__init__(
             f"The model artifacts size is greater than `{max_artifact_size}`. "
             "The `bucket_uri` needs to be specified to "
             "copy artifacts to the object storage bucket. "
             "Example: `bucket_uri=oci://<bucket_name>@<namespace>/prefix/`"
         )
```

### Comparing `oracle_ads-2.8.3/ads/catalog/notebook.py` & `oracle_ads-2.8.4/ads/catalog/notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/catalog/project.py` & `oracle_ads-2.8.4/ads/catalog/project.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/catalog/summary.py` & `oracle_ads-2.8.4/ads/catalog/summary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/cli.py` & `oracle_ads-2.8.4/ads/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
 # Copyright (c) 2021, 2022 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
+from ads.common import logger
+import traceback
+
 try:
     import click
     import ads.opctl.cli
     import ads.jobs.cli
     import ads.pipeline.cli
     import os
     import json
-except:
+except Exception as ex:
     print(
-        "Please run `pip install oracle-ads[opctl]` to install the required dependencies for ADS CLI"
+        "Please run `pip install oracle-ads[opctl]` to install "
+        "the required dependencies for ADS CLI."
     )
+    logger.debug(ex)
+    logger.debug(traceback.format_exc())
     exit()
 
 
 with open(
     os.path.join(os.path.dirname(os.path.abspath(__file__)), "ads_version.json")
 ) as version_file:
     ADS_VERSION = json.load(version_file)["version"]
```

### Comparing `oracle_ads-2.8.3/ads/common/analyzer.py` & `oracle_ads-2.8.4/ads/common/analyzer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/artifact/.model-ignore` & `oracle_ads-2.8.4/ads/common/artifact/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/auth.py` & `oracle_ads-2.8.4/ads/common/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/base_properties.py` & `oracle_ads-2.8.4/ads/model/base_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import dataclasses
 import json
 import os
 from typing import Any, Dict, Optional, Union
 
@@ -187,26 +187,26 @@
             The URI of the config file.
             Can be local path or OCI object storage URI.
         profile: str
             The config profile name.
         force_overwrite: (bool, optional). Defaults to False.
             Whether to overwrite existing files or not.
         auth: (Dict, optional). Defaults to None.
-            The default authetication is set using `ads.set_auth` API. If you need to override the
+            The default authentication is set using `ads.set_auth` API. If you need to override the
             default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
             authentication signer and kwargs required to instantiate IdentityClient object.
 
         Returns
         -------
         None
             Nothing
         """
         config = Config(uri=uri, auth=auth)
         config.section_set(key=profile, info=self.to_dict(), replace=force_overwrite)
-        config.save()
+        config.save(force_overwrite=force_overwrite)
 
     @classmethod
     def from_config(
         cls,
         uri: str,
         profile: str,
         auth: Optional[Dict] = None,
@@ -217,15 +217,15 @@
         ----------
         uri: str
             The URI of the config file.
             Can be local path or OCI object storage URI.
         profile: str
             The config profile name.
         auth: (Dict, optional). Defaults to None.
-            The default authetication is set using `ads.set_auth` API. If you need to override the
+            The default authentication is set using `ads.set_auth` API. If you need to override the
             default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
             authentication signer and kwargs required to instantiate IdentityClient object.
 
         Returns
         -------
         BaseProperties
             Instance of the BaseProperties.
```

### Comparing `oracle_ads-2.8.3/ads/common/card_identifier.py` & `oracle_ads-2.8.4/ads/common/card_identifier.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/config.py` & `oracle_ads-2.8.4/ads/common/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/data.py` & `oracle_ads-2.8.4/ads/common/data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/decorator/argument_to_case.py` & `oracle_ads-2.8.4/ads/common/decorator/argument_to_case.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/decorator/deprecate.py` & `oracle_ads-2.8.4/ads/common/decorator/deprecate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import warnings
 from enum import Enum
 from functools import wraps
 
 
-class NotSupportedError(Exception):
+class NotSupportedError(Exception):   # pragma: no cover
     pass
 
 
 class TARGET_TYPE(Enum):
     CLASS = "Class"
     METHOD = "Method"
     ATTRIBUTE = "Attribute"
```

### Comparing `oracle_ads-2.8.3/ads/common/decorator/runtime_dependency.py` & `oracle_ads-2.8.4/ads/common/decorator/runtime_dependency.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/decorator/utils.py` & `oracle_ads-2.8.4/ads/common/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/function/fn_util.py` & `oracle_ads-2.8.4/ads/common/function/fn_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/function/func_conf.yaml` & `oracle_ads-2.8.4/ads/common/function/func_conf.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/ipython.py` & `oracle_ads-2.8.4/ads/common/ipython.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/model.py` & `oracle_ads-2.8.4/ads/common/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/model_artifact.py` & `oracle_ads-2.8.4/ads/common/model_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 INPUT_SCHEMA_FILE_NAME = "input_schema.json"
 OUTPUT_SCHEMA_FILE_NAME = "output_schema.json"
 
 _TRAINING_RESOURCE_OCID = JOB_RUN_OCID or NB_SESSION_OCID
 _COMPARTMENT_OCID = NB_SESSION_COMPARTMENT_OCID or JOB_RUN_COMPARTMENT_OCID
 
 
-class InvalidDataType(Exception):
+class InvalidDataType(Exception):   # pragma: no cover
     """Invalid Data Type."""
 
     pass
 
 
 SAMPLE_RUNTIME_YAML = f"""
 MODEL_ARTIFACT_VERSION: '{MODEL_ARTIFACT_VERSION}'
```

### Comparing `oracle_ads-2.8.3/ads/common/model_artifact_schema.json` & `oracle_ads-2.8.4/ads/common/model_artifact_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/model_export_util.py` & `oracle_ads-2.8.4/ads/common/model_export_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/model_introspect.py` & `oracle_ads-2.8.4/ads/model/model_introspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,29 @@
 import os
 from abc import ABC
 from copy import copy
 from dataclasses import dataclass
 from typing import List
 
 import pandas as pd
-from ads.common.model_metadata import MetadataTaxonomyKeys
+from ads.model.model_metadata import MetadataTaxonomyKeys
+from ads.common.object_storage_details import ObjectStorageDetails
 
 
 class IntrospectionNotPassed(ValueError):
     pass
 
 
 class TEST_STATUS(str):
     PASSED = "Passed"
     NOT_PASSED = "Failed"
     NOT_TESTED = "Skipped"
 
 
-_PATH_TO_MODEL_ARTIFACT_VALIDATOR = (
-    "ads.model_artifact_boilerplate.artifact_introspection_test.model_artifact_validate"
-)
+_PATH_TO_MODEL_ARTIFACT_VALIDATOR = "ads.model.model_artifact_boilerplate.artifact_introspection_test.model_artifact_validate"
 _INTROSPECT_METHOD_NAME = "validate_artifact"
 _INTROSPECT_RESULT_FILE_NAME = "test_json_output.json"
 
 
 class _PRINT_COLUMNS(Enum):
     KEY = "Test key"
     CASE = "Test name"
@@ -174,20 +173,25 @@
         None
             Nothing.
 
         Raises
         ------
             FileNotFoundError: If path to model artifacts does not exist.
         """
-        if not os.path.isdir(self._artifact.artifact_dir):
+        artifact_dir = (
+            self._artifact.artifact_dir
+            if not ObjectStorageDetails.is_oci_path(self._artifact.artifact_dir)
+            else self._artifact.local_copy_dir
+        )
+        if not os.path.isdir(artifact_dir):
             raise FileNotFoundError(
-                errno.ENOENT, os.strerror(errno.ENOENT), self._artifact.artifact_dir
+                errno.ENOENT, os.strerror(errno.ENOENT), artifact_dir
             )
 
-        output_file = f"{self._artifact.artifact_dir}/{_INTROSPECT_RESULT_FILE_NAME}"
+        output_file = f"{artifact_dir}/{_INTROSPECT_RESULT_FILE_NAME}"
         with open(output_file, "w") as f:
             json.dump(self._result, f, indent=4)
 
     def _save_result_to_metadata(self) -> None:
         """Saves the result of introspection to the model metadata."""
         self._artifact.metadata_taxonomy[
             MetadataTaxonomyKeys.ARTIFACT_TEST_RESULT
@@ -204,25 +208,29 @@
         None
             Nothing.
 
         Raises
         ------
         FileNotFoundError: If path to model artifacts does not exist.
         """
-
-        if not os.path.isdir(self._artifact.artifact_dir):
+        artifact_dir = (
+            self._artifact.artifact_dir
+            if not ObjectStorageDetails.is_oci_path(self._artifact.artifact_dir)
+            else self._artifact.local_copy_dir
+        )
+        if not os.path.isdir(artifact_dir):
             raise FileNotFoundError(
                 errno.ENOENT,
                 os.strerror(errno.ENOENT),
             )
 
         module = importlib.import_module(_PATH_TO_MODEL_ARTIFACT_VALIDATOR)
         importlib.reload(module)
         method = getattr(module, _INTROSPECT_METHOD_NAME)
-        params = {"artifact": self._artifact.artifact_dir}
+        params = {"artifact": artifact_dir}
         test_result, _ = method(**params)
 
         self._status = _TEST_STATUS_MAP.get(test_result)
         self._result = copy(module.TESTS)
         self._prepared_result = self._prepare_result()
 
     @property
```

### Comparing `oracle_ads-2.8.3/ads/common/model_metadata.py` & `oracle_ads-2.8.4/ads/common/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/model_metadata_mixin.py` & `oracle_ads-2.8.4/ads/model/model_metadata_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 
 import logging
 import os
 import sys
 import textwrap
 from typing import List, Tuple, Union
 
 import git
 import numpy as np
 import pandas as pd
 from ads.common import logger, utils
 from ads.common.data import ADSData
-from ads.common.model_metadata import (
+from ads.model.model_metadata import (
     MetadataCustomCategory,
     MetadataCustomKeys,
     MetadataTaxonomyKeys,
     ModelCustomMetadataItem,
     ModelProvenanceMetadata,
     UseCaseType,
 )
@@ -42,15 +42,15 @@
 
 class MetadataMixin:
     """MetadataMixin class which populates the custom metadata, taxonomy metadata,
     input/output schema and provenance metadata.
     """
 
     def _populate_metadata_taxonomy(
-        self, model: callable = None, use_case_type: str = None
+        self, model: callable = None, use_case_type: str = None, **kwargs
     ):
         """Populates the taxonomy metadata.
 
         Parameters
         ----------
         model: (callable, optional). Defaults to None.
             Any model.
@@ -207,14 +207,15 @@
         )
         self.metadata_custom._add_many(model_metadata_items, replace=True)
 
     def _prepare_data_for_schema(
         self,
         X_sample: Union[List, Tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         y_sample: Union[List, Tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
+        **kwargs,
     ):
         """
         Any Framework-specific work before generic schema generation.
         """
         return X_sample, y_sample
 
     def _populate_provenance_metadata(
@@ -266,14 +267,16 @@
         data_sample: ADSData = None,
         X_sample: Union[list, tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         y_sample: Union[list, tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         training_script_path: str = None,
         training_id: str = None,
         ignore_pending_changes: bool = True,
         max_col_num: int = DATA_SCHEMA_MAX_COL_NUM,
+        ignore_conda_error: bool = False,
+        **kwargs,
     ):
         """Populates input schema and output schema.
         If the schema exceeds the limit of 32kb, save as json files to the artifact directory.
 
         Parameters
         ----------
         use_case_type: (str, optional). Defaults to None.
@@ -299,49 +302,54 @@
             Nothing.
         """
         if (
             self.estimator is None
             and self.metadata_taxonomy[MetadataTaxonomyKeys.ALGORITHM].value is None
         ):
             logger.info(
-                "To auto-extract taxonomy metadata the model must be provided. Supported models: automl, keras, lightgbm, pytorch, sklearn, tensorflow, pyspark, and xgboost."
+                "To auto-extract taxonomy metadata the model must be provided. Supported models: keras, lightgbm, pytorch, sklearn, tensorflow, pyspark, and xgboost."
             )
         if use_case_type is None:
             use_case_type = self.metadata_taxonomy[
                 MetadataTaxonomyKeys.USE_CASE_TYPE
             ].value
+
         self._populate_metadata_taxonomy(
-            model=self.estimator, use_case_type=use_case_type
+            model=self.estimator, use_case_type=use_case_type, **kwargs
         )
-        self._populate_metadata_custom()
+        if not ignore_conda_error:
+            self._populate_metadata_custom()
         self.populate_schema(
             data_sample=data_sample,
             X_sample=X_sample,
             y_sample=y_sample,
             max_col_num=max_col_num,
+            **kwargs,
         )
         self._populate_provenance_metadata(
             training_script_path=training_script_path,
             ignore_pending_changes=ignore_pending_changes,
             training_id=training_id,
         )
         self._summary_status.update_action(
-            detail="Populated metadata(Custom, Taxonomy and Provenance)", action=""
+            detail="Populated metadata(Custom, Taxonomy and Provenance)",
+            action="",
         )
         self._summary_status.update_status(
             detail="Populated metadata(Custom, Taxonomy and Provenance)",
             status="Done",
         )
 
     def populate_schema(
         self,
         data_sample: ADSData = None,
         X_sample: Union[List, Tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         y_sample: Union[List, Tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         max_col_num: int = DATA_SCHEMA_MAX_COL_NUM,
+        **kwargs,
     ):
         """Populate input and output schemas.
         If the schema exceeds the limit of 32kb, save as json files to the artifact dir.
 
         Parameters
         ----------
         data_sample: ADSData
@@ -357,31 +365,34 @@
             assert isinstance(
                 data_sample, ADSData
             ), "`data_sample` expects data of ADSData type. \
             Pass in to `X_sample` and `y_sample` for other data types."
             X_sample = data_sample.X
             y_sample = data_sample.y
 
-        X_sample, y_sample = self._prepare_data_for_schema(X_sample, y_sample)
+        X_sample, y_sample = self._prepare_data_for_schema(X_sample, y_sample, **kwargs)
         self.schema_input = self._populate_schema(
             X_sample,
             schema_file_name=INPUT_SCHEMA_FILE_NAME,
             max_col_num=max_col_num,
+            **kwargs,
         )
         self.schema_output = self._populate_schema(
             y_sample,
             schema_file_name=OUTPUT_SCHEMA_FILE_NAME,
             max_col_num=max_col_num,
+            **kwargs,
         )
 
     def _populate_schema(
         self,
         data: Union[list, tuple, pd.Series, np.ndarray, pd.DataFrame],
         schema_file_name: str,
         max_col_num: int,
+        **kwargs,
     ):
         """Populates schema and if the schema exceeds the limit of 32kb, save as a json file to the artifact_dir.
 
         Parameters
         ----------
         data: Union[list, tuple, pd.Series, np.ndarray, pd.DataFrame]
             A sample of input data that will be used to generate input schema.
@@ -397,15 +408,18 @@
         """
         result = None
 
         try:
             if data is not None:
                 data = utils.to_dataframe(data)
                 schema = data.ads.model_schema(max_col_num=max_col_num)
-                schema.to_json_file(os.path.join(self.artifact_dir, schema_file_name))
+                schema.to_json_file(
+                    file_path=os.path.join(self.artifact_dir, schema_file_name),
+                    storage_options=kwargs.pop("auth", {}),
+                )
                 if self._validate_schema_size(schema, schema_file_name):
                     result = schema
         except DataSizeTooWide:
             logger.warning(
                 f"The data has too many columns and "
                 f"the maximum allowable number of columns is `{max_col_num}`. "
                 "The schema was not auto generated. increase allowable number of columns."
```

### Comparing `oracle_ads-2.8.3/ads/common/object_storage_details.py` & `oracle_ads-2.8.4/ads/common/object_storage_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Dict
 from urllib.parse import urlparse
 
 from ads.common import auth as authutil
 from ads.common import oci_client
 
 
-class InvalidObjectStoragePath(Exception):
+class InvalidObjectStoragePath(Exception):   # pragma: no cover
     """Invalid Object Storage Path."""
 
     pass
 
 
 @dataclass
 class ObjectStorageDetails:
@@ -117,7 +117,24 @@
         """Validates the Object Storage URI."""
         if not re.match(r"oci://*@*", uri):
             raise InvalidObjectStoragePath(
                 f"The `{uri}` is not a valid Object Storage path. "
                 "It must follow the pattern `oci://<bucket_name>@<namespace>/<prefix>`."
             )
         return True
+
+    @staticmethod
+    def is_oci_path(uri: str = None) -> bool:
+        """Check if the given path is oci object storage uri.
+
+        Parameters
+        ----------
+        uri: str
+            The URI of the target.
+
+        Returns
+        -------
+        bool: return True if the path is oci object storage uri.
+        """
+        if not uri:
+            return False
+        return uri.startswith("oci://")
```

### Comparing `oracle_ads-2.8.3/ads/common/oci_client.py` & `oracle_ads-2.8.4/ads/common/oci_client.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/oci_datascience.py` & `oracle_ads-2.8.4/ads/common/oci_datascience.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/oci_logging.py` & `oracle_ads-2.8.4/ads/common/oci_logging.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/common/oci_mixin.py` & `oracle_ads-2.8.4/ads/common/oci_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,40 +7,45 @@
 """Contains Mixins for integrating OCI data models
 """
 import inspect
 import json
 import logging
 import os
 import re
+import time
 import traceback
 from datetime import date, datetime
 from typing import Callable, Optional, Union
 from enum import Enum
 
 import oci
 import yaml
 from ads.common import auth
 from ads.common.decorator.utils import class_or_instance_method
-from ads.common.utils import camel_to_snake
+from ads.common.utils import camel_to_snake, get_progress_bar
 from ads.config import COMPARTMENT_OCID
 from dateutil import tz
 from dateutil.parser import parse
 from oci._vendor import six
 
 logger = logging.getLogger(__name__)
 
 LIFECYCLE_STOP_STATE = ("SUCCEEDED", "FAILED", "CANCELED", "DELETED")
+WORK_REQUEST_STOP_STATE = ("SUCCEEDED", "FAILED", "CANCELED")
+DEFAULT_WAIT_TIME = 1200
+DEFAULT_POLL_INTERVAL = 10
+DEFAULT_WORKFLOW_STEPS = 2
 
 
 class MergeStrategy(Enum):
     OVERRIDE = "override"
     MERGE = "merge"
 
 
-class OCIModelNotExists(Exception):
+class OCIModelNotExists(Exception):   # pragma: no cover
     pass
 
 
 class OCIClientMixin:
     """Mixin class for representing OCI resource/service with OCI client.
 
     Most OCI requests requires a client for making the connection.
@@ -927,14 +932,84 @@
         else:
             # This will likely never happen as OCI SDK will raise an error if the HTTP request is not successful.
             raise oci.exceptions.RequestException(
                 f"opc-work-request-id not found in response headers: {response.headers}"
             )
         return work_request_response
 
+    def wait_for_progress(
+        self, 
+        work_request_id: str, 
+        num_steps: int = DEFAULT_WORKFLOW_STEPS, 
+        max_wait_time: int = DEFAULT_WAIT_TIME, 
+        poll_interval: int = DEFAULT_POLL_INTERVAL
+    ):
+        """Waits for the work request progress bar to be completed.
+
+        Parameters
+        ----------
+        work_request_id: str
+            Work Request OCID.
+        num_steps: (int, optional). Defaults to 2.
+            Number of steps for the progress indicator.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
+
+        Returns
+        -------
+        None
+        """
+        work_request_logs = []
+
+        i = 0
+        start_time = time.time()
+        with get_progress_bar(num_steps) as progress:
+            seconds_since = time.time() - start_time
+            exceed_max_time = max_wait_time > 0 and seconds_since >= max_wait_time
+            if exceed_max_time:
+                logger.error(
+                    f"Max wait time ({max_wait_time} seconds) exceeded."
+                )
+            while not exceed_max_time and (not work_request_logs or len(work_request_logs) < num_steps):
+                time.sleep(poll_interval)
+                new_work_request_logs = []
+
+                try:
+                    work_request = self.client.get_work_request(work_request_id).data
+                    work_request_logs = self.client.list_work_request_logs(
+                        work_request_id
+                    ).data
+                except Exception as ex:
+                    logger.warn(ex)
+
+                new_work_request_logs = (
+                    work_request_logs[i:] if work_request_logs else []
+                )
+
+                for wr_item in new_work_request_logs:
+                    progress.update(wr_item.message)
+                    i += 1
+
+                if work_request and work_request.status in WORK_REQUEST_STOP_STATE:
+                    if work_request.status != "SUCCEEDED":
+                        if new_work_request_logs:
+                            raise Exception(new_work_request_logs[-1].message)
+                        else:
+                            raise Exception(
+                                "Error occurred in attempt to perform the operation. "
+                                "Check the service logs to get more details. "
+                                f"{work_request}"
+                            )
+                    else:
+                        break
+            progress.update("Done")
+
 
 class OCIModelWithNameMixin:
     """Mixin class to operate OCI model which contains name property."""
 
     @classmethod
     def from_name(cls, name: str, compartment_id: Optional[str] = None):
         """Initializes an object from name.
```

### Comparing `oracle_ads-2.8.3/ads/common/oci_resource.py` & `oracle_ads-2.8.4/ads/common/oci_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """Contains class wrapping OCI resource search service
 """
 import oci.resource_search
 from ads.common.oci_mixin import OCIClientMixin
 
 
-class ResourceNotFoundError(Exception):
+class ResourceNotFoundError(Exception):   # pragma: no cover
     """Exception when an OCI resource is not found or user does not have permission to access it.
     This could mean the resource does not exist, or
     there is not enough permission to find/access the resource.
     """
 
 
 class SEARCH_TYPE(str):
```

### Comparing `oracle_ads-2.8.3/ads/common/serializer.py` & `oracle_ads-2.8.4/ads/common/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
+import dataclasses
 import json
 from abc import ABC, abstractmethod
-import dataclasses
-from typing import Dict, Union, Optional, List
 from enum import Enum
+from typing import Dict, Optional, Union
+from urllib.parse import urlparse
 
 import fsspec
 import yaml
+
 from ads.common import logger
 
 try:
     from yaml import CSafeDumper as dumper
     from yaml import CSafeLoader as loader
 except:
     from yaml import SafeDumper as dumper
@@ -49,23 +51,27 @@
     from_yaml(cls, yaml_string=None, uri=None, **kwargs)
         Creates an object from YAML string provided or from URI location containing YAML string
     from_string(cls, obj_string=None: str, uri=None, **kwargs)
         Creates an object from string provided or from URI location containing string
     """
 
     @abstractmethod
-    def to_dict(self, **kwargs) -> dict:
-        """Serializes instance of class into a dictionary.
+    def to_dict(self, **kwargs: Dict) -> Dict:
+        """Serializes an instance of class into a dictionary.
+
+        Parameters
+        ----------
+        **kwargs: Dict
+            Additional arguments.
 
         Returns
         -------
         Dict
-            A dictionary.
+            The result dictionary.
         """
-        pass
 
     @classmethod
     @abstractmethod
     def from_dict(cls, obj_dict: dict) -> "Serializable":
         """Returns an instance of the class instantiated by the dictionary provided.
 
         Parameters
@@ -86,45 +92,51 @@
 
         Parameters
         ----------
         s: (string)
             content
         uri: (string)
             URI location to save string s
-
-        kwargs
-        ------
-        keyword arguments to be passed into fsspec.open(). For OCI object storage, this should be config="path/to/.oci/config".
-            For other storage connections consider e.g. host, port, username, password, etc.
+        kwargs : dict
+            keyword arguments to be passed into fsspec.open().
+            For OCI object storage, this can be config="path/to/.oci/config".
 
         Returns
         -------
         None
-            Nothing.
+            Nothing
         """
+
+        overwrite = kwargs.pop("overwrite", True)
+        if not overwrite:
+            dst_path_scheme = urlparse(uri).scheme or "file"
+            if fsspec.filesystem(dst_path_scheme, **kwargs).exists(uri):
+                raise FileExistsError(
+                    f"The `{uri}` is already exists. Set `overwrite` to True "
+                    "if you wish to overwrite."
+                )
+
         with fsspec.open(uri, "w", **kwargs) as f:
             f.write(s)
 
     @staticmethod
     def _read_from_file(uri: str, **kwargs) -> str:
         """Returns contents from location specified by URI
 
         Parameters
         ----------
         uri: (string)
             URI location
-
-        kwargs
-        ------
-        keyword arguments to be passed into fsspec.open(). For OCI object storage, this should be config="path/to/.oci/config".
-            For other storage connections consider e.g. host, port, username, password, etc.
+        kwargs : dict
+            keyword arguments to be passed into fsspec.open().
+            For OCI object storage, this can be config="path/to/.oci/config".
 
         Returns
         -------
-            string: Contents in file specified by URI
+        string: Contents in file specified by URI
         """
         with fsspec.open(uri, "r", **kwargs) as f:
             return f.read()
 
     def to_json(
         self, uri: str = None, encoder: callable = json.JSONEncoder, **kwargs
     ) -> str:
@@ -135,23 +147,31 @@
         uri: (string, optional)
             URI location to save the JSON string. Defaults to None.
         encoder: (callable, optional)
             Encoder for custom data structures. Defaults to JSONEncoder.
 
         kwargs
         ------
-        keyword arguments to be passed into fsspec.open(). For OCI object storage, this should be config="path/to/.oci/config".
-            For other storage connections consider e.g. host, port, username, password, etc.
+        overwrite: (bool, optional). Defaults to True.
+            Whether to overwrite existing file or not.
 
-        Returns:
-            string: Serialized version of object
+        keyword arguments to be passed into fsspec.open().
+        For OCI object storage, this could be config="path/to/.oci/config".
+        For other storage connections consider e.g. host, port, username, password, etc.
+
+        Returns
+        -------
+        Union[str, None]
+            Serialized version of object.
+            `None` in case when `uri` provided.
         """
         json_string = json.dumps(self.to_dict(**kwargs), cls=encoder)
         if uri:
             self._write_to_file(s=json_string, uri=uri, **kwargs)
+            return None
         return json_string
 
     @classmethod
     def from_json(
         cls,
         json_string: str = None,
         uri: str = None,
@@ -186,39 +206,48 @@
         if json_string:
             return cls.from_dict(json.loads(json_string, cls=decoder))
         if uri:
             json_dict = json.loads(cls._read_from_file(uri, **kwargs), cls=decoder)
             return cls.from_dict(json_dict)
         raise ValueError("Must provide either JSON string or URI location")
 
-    def to_yaml(self, uri: str = None, dumper: callable = dumper, **kwargs) -> str:
+    def to_yaml(
+        self, uri: str = None, dumper: callable = yaml.SafeDumper, **kwargs
+    ) -> Union[str, None]:
         """Returns object serialized as a YAML string
 
         Parameters
         ----------
-        uri: (string, optional)
-            URI location to save the YAML string. Defaults to None.
-        dumper: (callable, optional)
-            Custom YAML Dumper. Defaults to CDumper/SafeDumper.
+        uri : str, optional
+            URI location to save the YAML string, by default None
+        dumper : callable, optional
+            Custom YAML Dumper, by default yaml.SafeDumper
+        kwargs : dict
+            overwrite: (bool, optional). Defaults to True.
+                Whether to overwrite existing file or not.
+            note: (str, optional)
+                The note that needs to be added in the beginning of the YAML.
+                It will be added as is without any formatting.
+            side_effect: Optional[SideEffect]
+                side effect to take on the dictionary. The side effect can be either
+                convert the dictionary keys to "lower" (SideEffect.CONVERT_KEYS_TO_LOWER.value)
+                or "upper"(SideEffect.CONVERT_KEYS_TO_UPPER.value) cases.
 
-        kwargs
-        ------
-        side_effect: Optional[SideEffect]
-            side effect to take on the dictionary. The side effect can be either
-            convert the dictionary keys to "lower" (SideEffect.CONVERT_KEYS_TO_LOWER.value)
-            or "upper"(SideEffect.CONVERT_KEYS_TO_UPPER.value) cases.
-        keyword arguments to be passed into fsspec.open(). For OCI object storage, this should be config="path/to/.oci/config".
-            For other storage connections consider e.g. host, port, username, password, etc.
+            The other keyword arguments to be passed into fsspec.open().
+            For OCI object storage, this could be config="path/to/.oci/config".
 
-        Returns:
-            Union[str, None]
-                Serialized version of object.
-                None in case when `uri` provided.
+        Returns
+        -------
+        Union[str, None]
+            Serialized version of object.
+            `None` in case when `uri` provided.
         """
-        yaml_string = yaml.dump(self.to_dict(**kwargs), Dumper=dumper)
+        note = kwargs.pop("note", "")
+
+        yaml_string = f"{note}\n" + yaml.dump(self.to_dict(**kwargs), Dumper=dumper)
         if uri:
             self._write_to_file(s=yaml_string, uri=uri, **kwargs)
             return None
 
         return yaml_string
 
     @classmethod
```

### Comparing `oracle_ads-2.8.3/ads/common/utils.py` & `oracle_ads-2.8.4/ads/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 # dimention of np array which can be converted to pd dataframe
 DIMENSION = 2
 
 # declare custom exception class
 
 
-class FileOverwriteError(Exception):
+class FileOverwriteError(Exception):   # pragma: no cover
     pass
 
 
 def get_cpu_count():
     """
     Returns the number of CPUs available on this machine
     """
@@ -491,17 +491,15 @@
         else:
             module_name, module_pkg = msg, msg
         print(
             f"ERROR: {module_name} module not found. Make sure you have installed {module_pkg} in order to download all of necessary modules."
         )
 
     if is_documentation_mode() and is_notebook():
-
         if display_type.lower() == "tip":
-
             if "\n" in msg:
                 t = "<b>{}:</b>".format(title.upper().strip()) if title else ""
 
                 user_message = "{}{}".format(
                     t,
                     "".join(
                         [
@@ -563,15 +561,14 @@
                 </div>
 
                 """
                 )
             )
 
         elif display_type.startswith("info"):
-
             user_message = msg.strip().replace("\n", "<br>")
 
             if see_also_links:
                 see_also_html = f"""
                 <ul>
                 {'<li>'.join([f"<a src='{url}'>{display_name}</a>"
                               for (display_name, url) in see_also_links])}
@@ -636,15 +633,14 @@
     if isinstance(raw, str):
         return ellipsis_strings([raw], n)[0]
 
     sequence = list(raw) if not isinstance(raw, list) else raw
 
     result = []
     for s in sequence:
-
         if len(str(s)) <= n:
             result.append(s)
         else:
             n2 = int(n) // 2 - 3
             n1 = n - n2 - 3
             result.append("{0}...{1}".format(s[:n1], s[-n2:]))
 
@@ -1132,44 +1128,52 @@
         return False
     else:
         raise TypeError(f"The data type `{type(data)}` is not supported.")
 
     return col_num > max_col_num
 
 
-def get_files(directory: str):
+def get_files(directory: str, auth: Optional[Dict] = None):
     """List out all the file names under this directory.
 
     Parameters
     ----------
     directory: str
         The directory to list out all the files from.
+    auth: (Dict, optional). Defaults to None.
+        The default authentication is set using `ads.set_auth` API. If you need to override the
+        default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
+        authentication signer and kwargs required to instantiate IdentityClient object.
 
     Returns
     -------
     List
         List of the files in the directory.
     """
     directory = directory.rstrip("/")
-    if os.path.exists(os.path.join(directory, ".model-ignore")):
-        ignore_patterns = (
-            Path(os.path.join(directory), ".model-ignore")
-            .read_text()
-            .strip()
-            .split("\n")
-        )
+    path_scheme = urlparse(directory).scheme or "file"
+    storage_options = auth or authutil.default_signer()
+    model_ignore_path = os.path.join(directory, ".model-ignore")
+    if is_path_exists(model_ignore_path, auth=auth):
+        with fsspec.open(model_ignore_path, "r", **storage_options) as f:
+            ignore_patterns = f.read().strip().split("\n")
     else:
         ignore_patterns = []
     file_names = []
-    for root, dirs, files in os.walk(directory):
+    fs = fsspec.filesystem(path_scheme, **storage_options)
+    for root, dirs, files in fs.walk(directory):
         for name in files:
             file_names.append(os.path.join(root, name))
         for name in dirs:
             file_names.append(os.path.join(root, name))
 
+    # return all files in remote directory.
+    if directory.startswith("oci://"):
+        directory = directory.lstrip("oci://")
+
     for ignore in ignore_patterns:
         if not ignore.startswith("#") and ignore.strip() != "":
             matches = []
             for file_name in file_names:
                 if ignore.endswith("/"):
                     ignore = ignore[:-1] + "*"
                 if not re.search(fnmatch.translate("/%s" % ignore.strip()), file_name):
@@ -1224,15 +1228,15 @@
         If this is a directory, the source files will be placed under it.
     unpack : (bool, optional). Defaults to False.
         Indicate if zip or tar.gz file specified by the uri should be unpacked.
         This option has no effect on other files.
     force_overwrite: (bool, optional). Defaults to False.
         Whether to overwrite existing files or not.
     auth: (Dict, optional). Defaults to None.
-        The default authetication is set using `ads.set_auth` API. If you need to override the
+        The default authentication is set using `ads.set_auth` API. If you need to override the
         default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
         authentication signer and kwargs required to instantiate IdentityClient object.
 
     Returns
     -------
     None
         Nothing
@@ -1290,15 +1294,15 @@
     uri_src: str
         The URI of the source file, which can be local path or OCI object storage URI.
     uri_dst: str
         The URI of the destination file, which can be local path or OCI object storage URI.
     force_overwrite: (bool, optional). Defaults to False.
         Whether to overwrite existing files or not.
     auth: (Dict, optional). Defaults to None.
-        The default authetication is set using `ads.set_auth` API. If you need to override the
+        The default authentication is set using `ads.set_auth` API. If you need to override the
         default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
         authentication signer and kwargs required to instantiate IdentityClient object.
     chunk_size: (int, optinal). Defaults to `DEFAULT_BUFFER_SIZE`
         How much data can be copied in one iteration.
 
     Returns
     -------
@@ -1353,15 +1357,15 @@
     Reoves file.
 
     Parameters
     ----------
     file_path: str
         The path of the source file, which can be local path or OCI object storage URI.
     auth: (Dict, optional). Defaults to None.
-        The default authetication is set using `ads.set_auth` API. If you need to override the
+        The default authentication is set using `ads.set_auth` API. If you need to override the
         default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
         authentication signer and kwargs required to instantiate IdentityClient object.
 
     Returns
     -------
     None
         Nothing.
@@ -1566,7 +1570,30 @@
 
     try:
         return json.loads(config.OCI_REGION_METADATA)["regionIdentifier"]
     except:
         pass
 
     return None
+
+
+def is_path_exists(uri: str, auth: Optional[Dict] = None) -> bool:
+    """Check if the given path which can be local path or OCI object storage URI exists.
+
+    Parameters
+    ----------
+    uri: str
+        The URI of the target, which can be local path or OCI object storage URI.
+    auth: (Dict, optional). Defaults to None.
+        The default authentication is set using `ads.set_auth` API. If you need to override the
+        default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
+        authentication signer and kwargs required to instantiate IdentityClient object.
+
+    Returns
+    -------
+    bool: return True if the path exists.
+    """
+    path_scheme = urlparse(uri).scheme or "file"
+    storage_options = auth or authutil.default_signer()
+    if fsspec.filesystem(path_scheme, **storage_options).exists(uri):
+        return True
+    return False
```

### Comparing `oracle_ads-2.8.3/ads/common/word_lists.py` & `oracle_ads-2.8.4/ads/common/word_lists.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/config.py` & `oracle_ads-2.8.4/ads/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,44 @@
 from typing import Dict, Optional
 
 from ads.common.config import DEFAULT_CONFIG_PATH, DEFAULT_CONFIG_PROFILE, Config, Mode
 
 OCI_ODSC_SERVICE_ENDPOINT = os.environ.get("OCI_ODSC_SERVICE_ENDPOINT")
 OCI_IDENTITY_SERVICE_ENDPOINT = os.environ.get("OCI_IDENTITY_SERVICE_ENDPOINT")
 NB_SESSION_COMPARTMENT_OCID = os.environ.get("NB_SESSION_COMPARTMENT_OCID")
-PROJECT_OCID = os.environ.get("PROJECT_OCID")
+PROJECT_OCID = os.environ.get("PROJECT_OCID") or os.environ.get("PIPELINE_PROJECT_OCID")
 NB_SESSION_OCID = os.environ.get("NB_SESSION_OCID")
 USER_OCID = os.environ.get("USER_OCID")
 OCI_RESOURCE_PRINCIPAL_VERSION = os.environ.get("OCI_RESOURCE_PRINCIPAL_VERSION")
 OCI_RESOURCE_PRINCIPAL_RPT_PATH = os.environ.get("OCI_RESOURCE_PRINCIPAL_RPT_PATH")
 OCI_RESOURCE_PRINCIPAL_RPT_ID = os.environ.get("OCI_RESOURCE_PRINCIPAL_RPT_ID")
 TENANCY_OCID = os.environ.get("TENANCY_OCID")
 OCI_REGION_METADATA = os.environ.get("OCI_REGION_METADATA")
 JOB_RUN_OCID = os.environ.get("JOB_RUN_OCID")
 JOB_RUN_COMPARTMENT_OCID = os.environ.get("JOB_RUN_COMPARTMENT_OCID")
+PIPELINE_RUN_OCID = os.environ.get("PIPELINE_RUN_OCID")
+PIPELINE_RUN_COMPARTMENT_OCID = os.environ.get("PIPELINE_RUN_COMPARTMENT_OCID")
+PIPELINE_COMPARTMENT_OCID = os.environ.get("PIPELINE_COMPARTMENT_OCID")
+
 CONDA_BUCKET_NAME = os.environ.get("CONDA_BUCKET_NAME", "service-conda-packs")
 CONDA_BUCKET_NS = os.environ.get("CONDA_BUCKET_NS", "id19sfcrra6z")
 OCI_RESOURCE_PRINCIPAL_RPT_ENDPOINT = os.environ.get(
     "OCI_RESOURCE_PRINCIPAL_RPT_ENDPOINT"
 )
-COMPARTMENT_OCID = NB_SESSION_COMPARTMENT_OCID or JOB_RUN_COMPARTMENT_OCID
+COMPARTMENT_OCID = (
+    NB_SESSION_COMPARTMENT_OCID
+    or JOB_RUN_COMPARTMENT_OCID
+    or PIPELINE_RUN_COMPARTMENT_OCID
+)
 MD_OCID = os.environ.get("MD_OCID")
 DATAFLOW_RUN_OCID = os.environ.get("DATAFLOW_RUN_ID")
+
 RESOURCE_OCID = (
-    NB_SESSION_OCID or JOB_RUN_OCID or MD_OCID
-)  # We can add DATAFLOW_RUN_OCID here. Needs impact analysis
+    NB_SESSION_OCID or JOB_RUN_OCID or MD_OCID or PIPELINE_RUN_OCID or DATAFLOW_RUN_OCID
+)
 NO_CONTAINER = os.environ.get("NO_CONTAINER")
 
 
 def export(
     uri: Optional[str] = DEFAULT_CONFIG_PATH,
     auth: Dict = None,
     force_overwrite: Optional[bool] = False,
```

### Comparing `oracle_ads-2.8.3/ads/data_labeling/__init__.py` & `oracle_ads-2.8.4/ads/data_labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/boundingbox.py` & `oracle_ads-2.8.4/ads/data_labeling/boundingbox.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/constants.py` & `oracle_ads-2.8.4/ads/data_labeling/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/data_labeling_service.py` & `oracle_ads-2.8.4/ads/data_labeling/data_labeling_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/interface/reader.py` & `oracle_ads-2.8.4/ads/data_labeling/interface/reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/loader/file_loader.py` & `oracle_ads-2.8.4/ads/data_labeling/loader/file_loader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/metadata.py` & `oracle_ads-2.8.4/ads/data_labeling/metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/mixin/data_labeling.py` & `oracle_ads-2.8.4/ads/data_labeling/mixin/data_labeling.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/ner.py` & `oracle_ads-2.8.4/ads/data_labeling/ner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/parser/dls_record_parser.py` & `oracle_ads-2.8.4/ads/data_labeling/parser/dls_record_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 )
 from oci.data_labeling_service_dataplane.models.annotation import (
     Annotation as OCIAnnotation,
 )
 from oci.exceptions import ServiceError
 
 
-class ReadAnnotationError(Exception):
+class ReadAnnotationError(Exception):   # pragma: no cover
     def __init__(self, id: str):
         super().__init__(f"Error occurred in attempt to read annotation {id}.")
 
 
-class AnnotationNotFoundError(Exception):
+class AnnotationNotFoundError(Exception):   # pragma: no cover
     def __init__(self, id: str):
         super().__init__(f"{id} not found.")
 
 
-class DLSRecordParser(Parser):
+class DLSRecordParser(Parser):   # pragma: no cover
     """DLSRecordParser class which parses the labels from the record."""
 
     def __init__(
         self,
         dataset_source_path: str,
         auth: dict = None,
         format: str = None,
```

### Comparing `oracle_ads-2.8.3/ads/data_labeling/parser/export_metadata_parser.py` & `oracle_ads-2.8.4/ads/data_labeling/parser/export_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/parser/export_record_parser.py` & `oracle_ads-2.8.4/ads/data_labeling/parser/export_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/dataset_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/dls_record_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/dls_record_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 from ads.common import oci_client
 from ads.data_labeling.interface.reader import Reader
 from oci.data_labeling_service_dataplane.models import AnnotationSummary, RecordSummary
 from oci.exceptions import ServiceError
 from oci.pagination import list_call_get_all_results
 
 
-class ReadRecordsError(Exception):
+class ReadRecordsError(Exception):   # pragma: no cover
     def __init__(self, dataset_id: str):
         super().__init__(
             f"Error occurred in attempt to read records of dataset {dataset_id}."
         )
 
 
-class ReadAnnotationsError(Exception):
+class ReadAnnotationsError(Exception):   # pragma: no cover
     def __init__(self, dataset_id: str):
         super().__init__(
             f"Error occurred in attempt to read annotations of dataset {dataset_id}."
         )
 
 
 @dataclass
```

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/export_record_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/export_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/jsonl_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/metadata_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/metadata_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from ads.data_labeling.interface.reader import Reader
 from ads.data_labeling.metadata import Metadata
 from ads.data_labeling.parser.export_metadata_parser import MetadataParser
 from ads.data_labeling.reader.jsonl_reader import JsonlReader
 from oci.exceptions import ServiceError
 
 
-class EmptyMetadata(Exception):
+class EmptyMetadata(Exception):   # pragma: no cover
     """Empty Metadata."""
 
     pass
 
 
-class ReadDatasetError(Exception):
+class ReadDatasetError(Exception):   # pragma: no cover
     def __init__(self, id: str):
         super().__init__(f"Error occurred in attempt to read dataset {id}.")
 
 
-class DatasetNotFoundError(Exception):
+class DatasetNotFoundError(Exception):   # pragma: no cover
     def __init__(self, id: str):
         super().__init__(f"{id} not found.")
 
 
 class MetadataReader:
     """MetadataReader class which reads and extracts the labeled dataset metadata.
```

### Comparing `oracle_ads-2.8.3/ads/data_labeling/reader/record_reader.py` & `oracle_ads-2.8.4/ads/data_labeling/reader/record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/record.py` & `oracle_ads-2.8.4/ads/data_labeling/record.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/visualizer/image_visualizer.py` & `oracle_ads-2.8.4/ads/data_labeling/visualizer/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/data_labeling/visualizer/text_visualizer.py` & `oracle_ads-2.8.4/ads/data_labeling/visualizer/text_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/database/connection.py` & `oracle_ads-2.8.4/ads/database/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             The ocid of the secret to retrieve from Oracle Cloud Infrastructure Vault.
         key: str, optional
             The key to find the database directory.
         repository_path: str, optional
             The local database information store, default to ~/.database unless specified otherwise.
         kwargs: dict, optional
             Name-value pairs that are to be added to the list of connection parameters.
-            For example, database_name="mydb", database_type="oracle", username = "root", password = "pwd".
+            For example, database_name="mydb", database_type="oracle", username = "root", password = "example-password".
 
         Returns
         -------
         A Connector object.
         """
 
         prio_dict = {}
```

### Comparing `oracle_ads-2.8.3/ads/dataflow/dataflow.py` & `oracle_ads-2.8.4/ads/dataflow/dataflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     v2_4_4 = "2.4.4"
     v3_0_2 = "3.0.2"
 
 
 class DataFlow:
     @deprecated(
         "2.6.3",
-        details="Use ads.jobs.DataFlow class for creating DataFlow applications and runs. Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/apachespark/dataflow.html#create-run-data-flow-application-using-ads-python-sdk",
+        details="Use ads.jobs.DataFlow class for creating Data Flow applications and runs. Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/apachespark/dataflow.html#create-run-data-flow-application-using-ads-python-sdk",
     )
     def __init__(
         self,
         compartment_id=None,
         dataflow_base_folder="/home/datascience/dataflow",
         os_auth=None,
         df_auth=None,
```

### Comparing `oracle_ads-2.8.3/ads/dataflow/dataflowsummary.py` & `oracle_ads-2.8.4/ads/dataflow/dataflowsummary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/classification_dataset.py` & `oracle_ads-2.8.4/ads/dataset/classification_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2020, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import pandas as pd
 import warnings
 
 from ads.common import utils, logger
 from ads.dataset import helper
@@ -18,15 +18,15 @@
 class ClassificationDataset(ADSDatasetWithTarget):
     """
     Dataset for classification task
     """
 
     def __init__(self, df, sampled_df, target, target_type, shape, **kwargs):
         ADSDatasetWithTarget.__init__(
-            self, df, sampled_df, target, target_type, shape, **kwargs
+            self, df=df, sampled_df=sampled_df, target=target, target_type=target_type, shape=shape, **kwargs
         )
 
     def auto_transform(
         self,
         fix_imbalance: bool = True,
         correlation_threshold: float = 0.7,
         frac: float = 1.0,
```

### Comparing `oracle_ads-2.8.3/ads/dataset/correlation.py` & `oracle_ads-2.8.4/ads/dataset/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/correlation_plot.py` & `oracle_ads-2.8.4/ads/dataset/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/dask_series.py` & `oracle_ads-2.8.4/ads/dataset/dask_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/dataframe_transformer.py` & `oracle_ads-2.8.4/ads/dataset/dataframe_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/dataset.py` & `oracle_ads-2.8.4/ads/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2020, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from __future__ import print_function, absolute_import, division
 
 import copy
 import datetime
 import fsspec
 import numpy as np
 import os
 import pandas as pd
 import uuid
 
 from collections import Counter
 from sklearn.preprocessing import FunctionTransformer
-from typing import Iterable, Union
+from typing import Iterable, Tuple, Union
 
 from ads import set_documentation_mode
 from ads.common import utils
 from ads.common.decorator.deprecate import deprecated
 from ads.dataset import helper, logger
 from ads.dataset.dataframe_transformer import DataFrameTransformer
 from ads.dataset.exception import ValidationError
@@ -67,16 +67,16 @@
     """
 
     df_read_functions = ["head", "describe", "_get_numeric_data"]
 
     def __init__(
         self,
         df,
-        sampled_df,
-        shape,
+        sampled_df=None,
+        shape=None,
         name="",
         description=None,
         type_discovery=True,
         types={},
         metadata=None,
         progress=DummyProgressBar(),
         transformer_pipeline=None,
@@ -84,14 +84,25 @@
         **kwargs,
     ):
 
         #
         # to keep performance high and linear no matter the size of the distributed dataset we
         # create a pandas df that's used internally because this has a fixed upper size.
         #
+        if shape is None:
+            shape = df.shape
+
+        if sampled_df is None:
+            sampled_df = generate_sample(
+                df,
+                shape[0],
+                DatasetDefaults.sampling_confidence_level,
+                DatasetDefaults.sampling_confidence_interval,
+                **kwargs,
+            )
         super().__init__(
             sampled_df,
             type_discovery=type_discovery,
             types=types,
             metadata=metadata,
             progress=progress,
         )
@@ -130,14 +141,44 @@
     def __repr__(self):
         rows, cols = self.shape
         return f"{rows:,} rows, {cols:,} columns"
 
     def __len__(self):
         return self.shape[0]
 
+    @staticmethod
+    def from_dataframe(
+        df,
+        sampled_df=None,
+        shape=None,
+        name="",
+        description=None,
+        type_discovery=True,
+        types={},
+        metadata=None,
+        progress=DummyProgressBar(),
+        transformer_pipeline=None,
+        interactive=False,
+        **kwargs,
+    ) -> "ADSDataset":
+        return ADSDataset(
+            df=df,
+            sampled_df=sampled_df,
+            shape=shape,
+            name=name,
+            description=description,
+            type_discovery=type_discovery,
+            types=types,
+            metadata=metadata,
+            progress=progress,
+            transformer_pipeline=transformer_pipeline,
+            interactive=interactive,
+            **kwargs
+        )
+
     @property
     @deprecated(
         "2.5.2", details="The ddf attribute is deprecated. Use the df attribute."
     )
     def ddf(self):
         return self.df
```

### Comparing `oracle_ads-2.8.3/ads/dataset/dataset_browser.py` & `oracle_ads-2.8.4/ads/dataset/dataset_browser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/dataset_with_target.py` & `oracle_ads-2.8.4/ads/dataset/dataset_with_target.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,96 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2020, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from __future__ import absolute_import, print_function
 
 import abc
 import importlib
 from collections import defaultdict
 from numbers import Number
-from typing import Union
+from typing import Tuple, Union
 
 import pandas as pd
 from ads.common import utils, logger
 from ads.common.data import ADSData
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 from ads.dataset import helper
 from ads.dataset.dataset import ADSDataset
 from ads.dataset.feature_engineering_transformer import FeatureEngineeringTransformer
 from ads.dataset.feature_selection import FeatureImportance
-from ads.dataset.helper import deprecate_default_value, deprecate_variable
+from ads.dataset.helper import (
+    DatasetDefaults,
+    deprecate_default_value, 
+    deprecate_variable, 
+    generate_sample,
+    get_target_type,
+    is_text_data,
+)
 from ads.dataset.label_encoder import DataFrameLabelEncoder
 from ads.dataset.pipeline import TransformerPipeline
 from ads.dataset.progress import DummyProgressBar
 from ads.dataset.recommendation import Recommendation
 from ads.dataset.recommendation_transformer import RecommendationTransformer
 from ads.dataset.target import TargetVariable
-from ads.type_discovery.typed_feature import DateTimeTypedFeature
+from ads.type_discovery.typed_feature import (
+    CategoricalTypedFeature,
+    ContinuousTypedFeature,
+    DocumentTypedFeature,
+    GISTypedFeature,
+    OrdinalTypedFeature,
+    TypedFeature,
+    DateTimeTypedFeature, 
+    TypedFeature
+)
 from sklearn.model_selection import train_test_split
 from pandas.io.formats.printing import pprint_thing
 from sklearn.preprocessing import FunctionTransformer
 from abc import ABCMeta
 
 
 class ADSDatasetWithTarget(ADSDataset, metaclass=ABCMeta):
     """
     This class provides APIs for preparing dataset for modeling.
     """
 
     def __init__(
         self,
         df,
-        sampled_df,
         target,
-        target_type,
-        shape,
+        sampled_df=None,
+        shape=None,
+        target_type=None,
         sample_max_rows=-1,
         type_discovery=True,
         types={},
         parent=None,
         name="",
         metadata=None,
         transformer_pipeline=None,
         description=None,
         progress=DummyProgressBar(),
         **kwargs,
     ):
         self.recommendation_transformer = None
+        if shape is None:
+            shape = df.shape
+        if sampled_df is None:
+            sampled_df = generate_sample(
+                df,
+                shape[0],
+                DatasetDefaults.sampling_confidence_level,
+                DatasetDefaults.sampling_confidence_interval,
+                **kwargs,
+            )
 
         if parent is None:
             cols = sampled_df.columns.tolist()
             cols.insert(0, cols.pop(cols.index(target)))
             ADSDataset.__init__(
                 self,
                 df,
@@ -131,24 +157,161 @@
             #
             # after regenerating the sample we need to move the target back to the head
             #
             cols = self.sampled_df.columns.tolist()
             cols.insert(0, cols.pop(cols.index(target)))
             self.sampled_df = self.sampled_df[[*cols]]
 
+        if target_type is None:
+            target_type = get_target_type(target, sampled_df, **kwargs)
         self.target = TargetVariable(self, target, target_type)
 
         # remove target from type discovery conversion
         for step in self.transformer_pipeline.steps:
             if (
                 step[0] == "type_discovery"
                 and self.target.name in step[1].kw_args["dtypes"]
             ):
                 step[1].kw_args["dtypes"].pop(self.target.name)
 
+    @staticmethod
+    def from_dataframe(
+        df: pd.DataFrame,
+        target: str,
+        sampled_df: pd.DataFrame = None,
+        shape: Tuple[int, int] = None,
+        target_type: TypedFeature = None,
+        positive_class=None,
+        **init_kwargs,
+    ):
+        from ads.dataset.classification_dataset import (
+            BinaryClassificationDataset, 
+            BinaryTextClassificationDataset, 
+            MultiClassClassificationDataset, 
+            MultiClassTextClassificationDataset
+        )
+        from ads.dataset.forecasting_dataset import ForecastingDataset
+        from ads.dataset.regression_dataset import RegressionDataset
+
+        if sampled_df is None:
+            sampled_df = generate_sample(
+                df,
+                (shape or df.shape)[0],
+                DatasetDefaults.sampling_confidence_level,
+                DatasetDefaults.sampling_confidence_interval,
+                **init_kwargs,
+            )
+            
+        if target_type is None:
+            target_type = get_target_type(target, sampled_df, **init_kwargs)
+
+        if len(df[target].dropna()) == 0:
+            logger.warning(
+                "It is not recommended to use an empty column as the target variable."
+            )
+            raise ValueError(
+                f"We do not support using empty columns as the chosen target"
+            )
+        if utils.is_same_class(target_type, ContinuousTypedFeature):
+            return RegressionDataset(
+                df=df,
+                sampled_df=sampled_df,
+                target=target,
+                target_type=target_type,
+                shape=shape,
+                **init_kwargs,
+            )
+        elif utils.is_same_class(
+            target_type, DateTimeTypedFeature
+        ) or df.index.dtype.name.startswith("datetime"):
+            return ForecastingDataset(
+                df=df,
+                sampled_df=sampled_df,
+                target=target,
+                target_type=target_type,
+                shape=shape,
+                **init_kwargs,
+            )
+
+        # Adding ordinal typed feature, but ultimately we should rethink how we want to model this type
+        elif utils.is_same_class(target_type, CategoricalTypedFeature) or utils.is_same_class(
+            target_type, OrdinalTypedFeature
+        ):
+            if target_type.meta_data["internal"]["unique"] == 2:
+                if is_text_data(sampled_df, target):
+                    return BinaryTextClassificationDataset(
+                        df=df,
+                        sampled_df=sampled_df,
+                        target=target,
+                        shape=shape,
+                        target_type=target_type,
+                        positive_class=positive_class,
+                        **init_kwargs,
+                    )
+
+                return BinaryClassificationDataset(
+                    df=df,
+                    sampled_df=sampled_df,
+                    target=target,
+                    shape=shape,
+                    target_type=target_type,
+                    positive_class=positive_class,
+                    **init_kwargs,
+                )
+            else:
+                if is_text_data(sampled_df, target):
+                    return MultiClassTextClassificationDataset(
+                        df=df,
+                        sampled_df=sampled_df,
+                        target=target,
+                        target_type=target_type,
+                        shape=shape,
+                        **init_kwargs,
+                    )
+                return MultiClassClassificationDataset(
+                    df=df,
+                    sampled_df=sampled_df,
+                    target=target,
+                    target_type=target_type,
+                    shape=shape,
+                    **init_kwargs,
+                )
+        elif (
+            utils.is_same_class(target, DocumentTypedFeature)
+            or "text" in target_type["type"]
+            or "text" in target
+        ):
+            raise ValueError(
+                f"The column {target} cannot be used as the target column."
+            )
+        elif (
+            utils.is_same_class(target_type, GISTypedFeature)
+            or "coord" in target_type["type"]
+            or "coord" in target
+        ):
+            raise ValueError(
+                f"The column {target} cannot be used as the target column."
+            )
+        # This is to catch constant columns that are boolean. Added as a fix for pd.isnull(), and datasets with a
+        #   binary target, but only data on one instance
+        elif target_type and target_type["low_level_type"] == "bool":
+            return BinaryClassificationDataset(
+                df=df,
+                sampled_df=sampled_df,
+                target=target,
+                shape=shape,
+                target_type=target_type,
+                positive_class=positive_class,
+                **init_kwargs,
+            )
+        raise ValueError(
+            f"Unable to identify problem type. Specify the data type of {target} using 'types'. "
+            f"For example, types = {{{target}: 'category'}}"
+        )
+
     def rename_columns(self, columns):
         """
         Returns a dataset with columns renamed.
         """
         if isinstance(columns, list):
             assert len(columns) == len(
                 self.columns.values
```

### Comparing `oracle_ads-2.8.3/ads/dataset/exception.py` & `oracle_ads-2.8.4/ads/dataset/exception.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/factory.py` & `oracle_ads-2.8.4/ads/dataset/factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/feature_engineering_transformer.py` & `oracle_ads-2.8.4/ads/dataset/feature_engineering_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/feature_selection.py` & `oracle_ads-2.8.4/ads/dataset/feature_selection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/forecasting_dataset.py` & `oracle_ads-2.8.4/ads/dataset/forecasting_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class ForecastingDataset(ADSDatasetWithTarget):
     def __init__(self, df, sampled_df, target, target_type, shape, **kwargs):
         # index on target
         if isinstance(target, DateTimeTypedFeature):
             df = df.set_index(target)
         ADSDatasetWithTarget.__init__(
-            self, df, sampled_df, target, target_type, shape, **kwargs
+            self, df=df, sampled_df=sampled_df, target=target, target_type=target_type, shape=shape, **kwargs
         )
 
     def select_best_features(self, score_func=None, k=12):
         """
         Not yet implemented
         """
         raise NotImplementedError(
```

### Comparing `oracle_ads-2.8.3/ads/dataset/helper.py` & `oracle_ads-2.8.4/ads/dataset/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2020, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import ast
 import base64
 import html
 import io
 import math
@@ -828,7 +828,24 @@
         return var
 
 
 def _log_yscale_not_set():
     logger.info(
         "`yscale` parameter is not set. Valid values are `'linear'`, `'log'`, `'symlog'`."
     )
+
+def infer_target_type(target, target_series, discover_target_type=True):
+    # if type discovery is turned off, infer type from pandas dtype
+    if discover_target_type:
+        target_type = TypeDiscoveryDriver().discover(
+            target, target_series, is_target=True
+        )
+    else:
+        target_type = get_feature_type(target, target_series)
+    return target_type
+
+def get_target_type(target, sampled_df, **init_kwargs):
+    discover_target_type = init_kwargs.get("type_discovery", True)
+    if target in init_kwargs.get("types", {}):
+        sampled_df[target] = sampled_df[target].astype(init_kwargs.get("types")[target])
+        discover_target_type = False
+    return infer_target_type(target, sampled_df[target], discover_target_type)
```

### Comparing `oracle_ads-2.8.3/ads/dataset/label_encoder.py` & `oracle_ads-2.8.4/ads/dataset/label_encoder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/pipeline.py` & `oracle_ads-2.8.4/ads/dataset/pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/plot.py` & `oracle_ads-2.8.4/ads/dataset/plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/progress.py` & `oracle_ads-2.8.4/ads/dataset/progress.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/recommendation.py` & `oracle_ads-2.8.4/ads/dataset/recommendation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/recommendation_transformer.py` & `oracle_ads-2.8.4/ads/dataset/recommendation_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/regression_dataset.py` & `oracle_ads-2.8.4/ads/dataset/regression_dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 
 from ads.dataset.dataset_with_target import ADSDatasetWithTarget
 
 
 class RegressionDataset(ADSDatasetWithTarget):
     def __init__(self, df, sampled_df, target, target_type, shape, **kwargs):
         ADSDatasetWithTarget.__init__(
-            self, df, sampled_df, target, target_type, shape, **kwargs
+            self, df=df, sampled_df=sampled_df, target=target, target_type=target_type, shape=shape, **kwargs
         )
```

### Comparing `oracle_ads-2.8.3/ads/dataset/sampled_dataset.py` & `oracle_ads-2.8.4/ads/dataset/sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/target.py` & `oracle_ads-2.8.4/ads/dataset/target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dataset/timeseries.py` & `oracle_ads-2.8.4/ads/dataset/timeseries.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/dbmixin/db_pandas_accessor.py` & `oracle_ads-2.8.4/ads/dbmixin/db_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/environment/ml_runtime.py` & `oracle_ads-2.8.4/ads/environment/ml_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/evaluations/__init__.py` & `oracle_ads-2.8.4/ads/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/evaluations/evaluation_plot.py` & `oracle_ads-2.8.4/ads/evaluations/evaluation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/evaluations/evaluator.py` & `oracle_ads-2.8.4/ads/evaluations/evaluator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/evaluations/statistical_metrics.py` & `oracle_ads-2.8.4/ads/evaluations/statistical_metrics.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/base_explainer.py` & `oracle_ads-2.8.4/ads/explanations/base_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/explainer.py` & `oracle_ads-2.8.4/ads/explanations/explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/mlx_global_explainer.py` & `oracle_ads-2.8.4/ads/explanations/mlx_global_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/mlx_interface.py` & `oracle_ads-2.8.4/ads/explanations/mlx_interface.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/mlx_local_explainer.py` & `oracle_ads-2.8.4/ads/explanations/mlx_local_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/explanations/mlx_whatif_explainer.py` & `oracle_ads-2.8.4/ads/explanations/mlx_whatif_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/__init__.py` & `oracle_ads-2.8.4/ads/feature_engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/dataframe_accessor.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/dataframe_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/correlation.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/eda_mixin.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/eda_mixin_series.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/eda_mixin_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/feature_types_mixin.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/feature_types_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/mixin/utils.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/mixin/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/accessor/series_accessor.py` & `oracle_ads-2.8.4/ads/feature_engineering/accessor/series_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsimage/image.py` & `oracle_ads-2.8.4/ads/feature_engineering/adsimage/image.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsimage/image_reader.py` & `oracle_ads-2.8.4/ads/feature_engineering/adsimage/image_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsstring/common_regex_mixin.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/base.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/nltk_parser.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import functools
 import nltk
 import pandas as pd
 from nltk import FreqDist, ngrams, pos_tag
 from nltk.stem import SnowballStemmer
 from nltk.tokenize import sent_tokenize, word_tokenize
-from ads.feature_engineering.adsstring.parsers.base import Parser
+from ads.feature_engineering.feature_type.adsstring.parsers.base import Parser
 from typing import List
 
 if "CONDA_PREFIX" in os.environ:
     nltk.data.path.append(f"{os.environ['CONDA_PREFIX']}/nltk")
 
 
 class NLTKParser(Parser):
```

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsstring/parsers/spacy_parser.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import itertools
 from collections import Counter
 from typing import List, Sequence, Tuple
 import os
 import functools
 import pandas as pd
 
-from ads.feature_engineering.adsstring.parsers.base import Parser
+from ads.feature_engineering.feature_type.adsstring.parsers.base import Parser
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 
 
 # This module is only used when user installed spacy. spacy has conflicts with oci-cli.
```

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/adsstring/string.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/string.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 # Copyright (c) 2021, 2022 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import functools
 
 from typing import Any, Callable
-from ads.feature_engineering.adsstring.common_regex_mixin import (
+from ads.feature_engineering.feature_type.base import FeatureType
+from ads.feature_engineering.feature_type.adsstring.common_regex_mixin import (
     CommonRegexMixin,
 )
-from ads.feature_engineering.adsstring.oci_language import OCILanguage
+from ads.feature_engineering.feature_type.adsstring.oci_language import OCILanguage
 from ads.common.decorator.runtime_dependency import OptionalDependency
+from ads.feature_engineering.feature_type.adsstring.oci_language import OCILanguage
 
 
 def to_adsstring(func: Callable) -> Callable:
     """Decorator that converts output of a function to `ADSString` if it returns a string.
 
     Parameters
     ----------
@@ -52,27 +54,27 @@
     Callable
         class decorator
     """
 
     def decorate(cls):
         for attr in dir(cls):
             if (
-                callable(getattr(cls, attr))
-                and not attr.startswith("__")
+                not attr.startswith("__")
                 and not attr.startswith("_")
+                and callable(getattr(cls, attr))
             ):
                 setattr(cls, attr, decorator(getattr(cls, attr)))
         return cls
 
     return decorate
 
 
 @wrap_output_string(to_adsstring)
-class ADSString(str, CommonRegexMixin):
-    """Defines an enhanced string class for the purporse of performing NLP tasks.
+class ADSString(str, FeatureType, CommonRegexMixin):
+    """Defines an enhanced string class for the purpose of performing NLP tasks.
     Its functionalities can be extended by registering plugins.
 
     Attributes
     ----------
     plugins: List
         list of plugins that add functionalities to the class.
     string: str
@@ -80,25 +82,26 @@
 
     Example
     -------
     >>> ADSString.nlp_backend('nltk')
     >>> s = ADSString("Walking my dog on a breezy day is the best.")
     >>> s.lower() # regular string methods still work
     >>> s.replace("a", "e")
-    >>> s.nouns
-    >>> s.parts_of_speech
+    >>> s.noun
+    >>> s.pos #parts of speech
     >>> s = ADSString("get in touch with my associate at john.smith@gmail.com to schedule")
-    >>> s.emails
+    >>> s.email
     >>> ADSString.plugin_register(OCILanguage)
     >>> s = ADSString("This movie is awesome.")
     >>> s.absa
     """
 
     plugins = []
     language_model_cache = dict()
+    description = "Type representing enhanced string class."
 
     def __init__(self, text: str, language="english") -> None:
         """Initialze the class and register plugins.
 
         Parameters
         ----------
         text : str
@@ -169,25 +172,25 @@
             try:
                 import spacy
             except:
                 raise ModuleNotFoundError(
                     f"The `spacy` module was not found. Please run "
                     f"`pip install {OptionalDependency.TEXT}`."
                 )
-            from ads.feature_engineering.adsstring.parsers.spacy_parser import (
+            from ads.feature_engineering.feature_type.adsstring.parsers.spacy_parser import (
                 SpacyParser,
             )
 
             cls.plugin_register(SpacyParser)
         elif backend == "nltk":
             try:
                 import nltk
             except:
                 raise ModuleNotFoundError("nltk must be installed.")
-            from ads.feature_engineering.adsstring.parsers.nltk_parser import (
+            from ads.feature_engineering.feature_type.adsstring.parsers.nltk_parser import (
                 NLTKParser,
             )
 
             cls.plugin_register(NLTKParser)
         else:
             raise ValueError(
                 "Currently only `nltk` and `spacy` are supported. Default uses `nltk`."
```

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/data_schema.json` & `oracle_ads-2.8.4/ads/feature_engineering/data_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/dataset/zip_code_data.py` & `oracle_ads-2.8.4/ads/feature_engineering/dataset/zip_code_data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/exceptions.py` & `oracle_ads-2.8.4/ads/feature_engineering/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/__init__.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/address.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/adsstring/oci_language.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/adsstring/oci_language.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/base.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/boolean.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/boolean.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/category.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/category.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/constant.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/constant.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/continuous.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/continuous.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/creditcard.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/creditcard.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/datetime.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/datetime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/discrete.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/discrete.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/document.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/document.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/gis.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/gis.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/feature_validator.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/feature_warning.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/feature_warning.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/handler/warnings.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/handler/warnings.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/integer.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/integer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address_v4.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v4.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/ip_address_v6.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ip_address_v6.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/lat_long.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/lat_long.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/object.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/object.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/ordinal.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/ordinal.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/phone_number.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/phone_number.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/string.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/text.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/text.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/unknown.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/unknown.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type/zip_code.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type/zip_code.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/feature_type_manager.py` & `oracle_ads-2.8.4/ads/feature_engineering/feature_type_manager.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/schema.py` & `oracle_ads-2.8.4/ads/feature_engineering/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
 # Copyright (c) 2021, 2022 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
+import asteval
+import fsspec
+import json
+import os
+import sys
+import yaml
 from abc import ABC, abstractmethod
+from cerberus import Validator
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional
-from copy import deepcopy
-
-import yaml
+from string import Template
+from os import path
 from ads.common.serializer import DataClassSerializable
+from ads.common.object_storage_details import ObjectStorageDetails
 
 try:
     from yaml import CDumper as dumper
     from yaml import CLoader as loader
 except:
     from yaml import Dumper as dumper
     from yaml import Loader as loader
 
-import json
-import os
-import asteval
-from os import path
-
-import fsspec
-import yaml
-from cerberus import Validator
-import sys
-from string import Template
-
-
 SCHEMA_VALIDATOR_NAME = "data_schema.json"
 INPUT_OUTPUT_SCHENA_SIZE_LIMIT = 32000
 SCHEMA_VERSION = "1.1"
 DEFAULT_SCHEMA_VERSION = "1.0"
 SCHEMA_KEY = "schema"
 SCHEMA_VERSION_KEY = "version"
+DEFAULT_STORAGE_OPTIONS = None
 
 
 class SchemaSizeTooLarge(ValueError):
     def __init__(self, size: int):
         super().__init__(
             f"The schema `{size}` bytes and "
             f"the maximum allowable schema size is `{INPUT_OUTPUT_SCHENA_SIZE_LIMIT}` bytes. "
@@ -681,39 +678,49 @@
         Returns
         -------
         str
             The json representation of data schema.
         """
         return json.dumps(self.to_dict()).replace("NaN", "null")
 
-    def to_json_file(self, file_path):
+    def to_json_file(self, file_path, storage_options: dict = None):
         """Saves the data schema into a json file.
 
         Parameters
         ----------
         file_path : str
             File Path to store the schema in json format.
+        storage_options: dict. Default None
+            Parameters passed on to the backend filesystem class.
+            Defaults to `storage_options` set using `DatasetFactory.set_default_storage()`.
 
         Returns
         -------
         None
             Nothing.
         """
         directory = os.path.expanduser(os.path.dirname(file_path))
         basename = os.path.expanduser(os.path.basename(file_path))
         assert os.path.splitext(file_path)[-1].lower() in [
             ".json"
         ], f"The file `{basename}` is not a valid JSON file. The `{file_path}` must have the extension .json."
         if directory and not os.path.exists(directory):
-            try:
-                os.mkdir(directory)
-            except:
-                raise Exception(f"Error creating the directory.")
-        with open(os.path.join(directory, basename), "w") as json_file:
-            json.dump(self.to_dict(), json_file)
+            if not ObjectStorageDetails.is_oci_path(directory):
+                try:
+                    os.mkdir(directory)
+                except:
+                    raise Exception(f"Error creating the directory.")
+        if not storage_options:
+            storage_options = DEFAULT_STORAGE_OPTIONS or {"config": {}}
+        with fsspec.open(
+            os.path.join(directory, basename),
+            mode="w",
+            **(storage_options),
+        ) as f:
+            f.write(json.dumps(self.to_dict()))
 
     def to_yaml_file(self, file_path):
         """Saves the data schema into a yaml file.
         Parameters
         ----------
         file_path : str
             File Path to store the schema in yaml format.
```

### Comparing `oracle_ads-2.8.3/ads/feature_engineering/utils.py` & `oracle_ads-2.8.4/ads/feature_engineering/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/_imports.py` & `oracle_ads-2.8.4/ads/hpo/_imports.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/ads_search_space.py` & `oracle_ads-2.8.4/ads/hpo/ads_search_space.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/distributions.py` & `oracle_ads-2.8.4/ads/hpo/distributions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/objective.py` & `oracle_ads-2.8.4/ads/hpo/objective.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/search_cv.py` & `oracle_ads-2.8.4/ads/hpo/search_cv.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,42 +63,42 @@
     INITIATED = auto()
     RUNNING = auto()
     HALTED = auto()
     TERMINATED = auto()
     COMPLETED = auto()
 
 
-class InvalidStateTransition(Exception):
+class InvalidStateTransition(Exception):   # pragma: no cover
     """
     `Invalid State Transition` is raised when an invalid transition request is made, such as calling
     halt without a running process.
     """
 
     pass
 
 
-class ExitCriterionError(Exception):
+class ExitCriterionError(Exception):   # pragma: no cover
     """
     `ExitCriterionError` is raised when an attempt is made to check exit status for a different exit
     type than the tuner was initialized with. For example, if an HPO study has an exit criteria based
     on the number of trials and a request is made for the time remaining, which is a different exit
     criterion, an exception is raised.
     """
 
     pass
 
 
-class DuplicatedStudyError(Exception):
+class DuplicatedStudyError(Exception):   # pragma: no cover
     """
     `DuplicatedStudyError` is raised when a new tuner process is created with a study name that
     already exists in storage.
     """
 
 
-class NoRestartError(Exception):
+class NoRestartError(Exception):   # pragma: no cover
     """
     `NoRestartError` is raised when an attempt is made to check how many seconds have transpired since
     the HPO process was last resumed from a halt. This can happen if the process has been terminated
     or it was never halted and then resumed to begin with.
     """
 
     pass
```

### Comparing `oracle_ads-2.8.3/ads/hpo/stopping_criterion.py` & `oracle_ads-2.8.4/ads/hpo/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/tuner_artifact.py` & `oracle_ads-2.8.4/ads/hpo/tuner_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ads.common import logger
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 
 
-class NotPickableError(Exception):
+class NotPickableError(Exception):   # pragma: no cover
     def __init__(self, message):
         self.message = message
 
 
 class UploadTunerArtifact:
     def __init__(self, tuner, file_uri, metadata, auth=None):
         self.tuner = tuner
```

### Comparing `oracle_ads-2.8.3/ads/hpo/utils.py` & `oracle_ads-2.8.4/ads/hpo/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/validation.py` & `oracle_ads-2.8.4/ads/hpo/validation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_contour.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_contour.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_edf.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_edf.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_intermediate_values.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_optimization_history.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_optimization_history.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_parallel_coordinate.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/hpo/visualization/_param_importances.py` & `oracle_ads-2.8.4/ads/hpo/visualization/_param_importances.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/__init__.py` & `oracle_ads-2.8.4/ads/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/ads_job.py` & `oracle_ads-2.8.4/ads/jobs/ads_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
-from typing import List, Union
+from typing import List, Union, Dict
 from urllib.parse import urlparse
 
 import fsspec
 from ads.common.auth import default_signer
 from ads.jobs.builders.base import Builder
 from ads.jobs.builders.infrastructure.dataflow import DataFlow, DataFlowRun
 from ads.jobs.builders.infrastructure.dsc_job import DataScienceJob, DataScienceJobRun
@@ -70,14 +70,17 @@
                 # The entrypoint should be a path relative to the working dir.
                 # Here my_script.py is a file in the code_dir/my_package directory
                 .with_entrypoint("my_package/my_script.py")
                 # Add an additional Python path, relative to the working dir (code_dir/other_packages).
                 .with_python_path("other_packages")
                 # Copy files in "code_dir/output" to object storage after job finishes.
                 .with_output("output", "oci://bucket_name@namespace/path/to/dir")
+                # Tags
+                .with_freeform_tag(my_tag="my_value")
+                .with_defined_tag(**{"Operations": {"CostCenter": "42"}})
             )
         )
         # Create and Run the job
         run = job.create().run()
         # Stream the job run outputs
         run.watch()
 
@@ -352,14 +355,16 @@
         Job
             The job instance (self)
         """
         return self.set_spec("name", name)
 
     def build(self) -> "Job":
         """Load default values from the environment for the job infrastructure."""
+        super().build()
+
         build_method = getattr(self.infrastructure, "build", None)
         if build_method and callable(build_method):
             build_method()
         else:
             raise NotImplementedError
         return self
 
@@ -450,27 +455,35 @@
         Returns
         -------
         str
             Status of the job
         """
         return getattr(self.infrastructure, "status", None)
 
-    def to_dict(self) -> dict:
+    def to_dict(self, **kwargs: Dict) -> Dict:
         """Serialize the job specifications to a dictionary.
 
+        Parameters
+        ----------
+        **kwargs: Dict
+            The additional arguments.
+            - filter_by_attribute_map: bool
+                If True, then in the result will be included only the fields
+                presented in the `attribute_map`.
+
         Returns
         -------
-        dict
+        Dict
             A dictionary containing job specifications.
         """
         spec = {"name": self.name}
         if self.runtime:
-            spec["runtime"] = self.runtime.to_dict()
+            spec["runtime"] = self.runtime.to_dict(**kwargs)
         if self.infrastructure:
-            spec["infrastructure"] = self.infrastructure.to_dict()
+            spec["infrastructure"] = self.infrastructure.to_dict(**kwargs)
         if self.id:
             spec["id"] = self.id
         return {
             "kind": self.kind,
             # "apiVersion": self.api_version,
             "spec": spec,
         }
@@ -488,15 +501,15 @@
         -------
         Job
             A job instance
 
         Raises
         ------
         NotImplementedError
-            If the type of the intrastructure or runtime is not supported.
+            If the type of the infrastructure or runtime is not supported.
         """
         if not isinstance(config, dict):
             raise ValueError("The config data for initializing the job is invalid.")
         spec = config.get("spec")
 
         mappings = {
             "infrastructure": cls._INFRASTRUCTURE_MAPPING,
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/base.py` & `oracle_ads-2.8.4/ads/jobs/builders/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """Special type to represent the current enclosed class.
 
 This type is used by factory class method or when a method returns ``self``.
 """
 
 
 class Builder(Serializable):
-
     attribute_map = {}
 
     def __init__(self, spec: Dict = None, **kwargs) -> None:
         """To initialize the object,
         user can either pass in the specification as a dictionary or through keyword arguments.
 
         Parameters
@@ -107,17 +106,33 @@
         """The type of the object as showing in YAML.
 
         This implementation returns the class name with the first letter coverted to lower case.
         """
         class_name = self.__class__.__name__
         return class_name[0].lower() + class_name[1:] if len(class_name) > 1 else ""
 
-    def to_dict(self) -> dict:
-        """Converts the object to dictionary with kind, type and spec as keys."""
-        spec = copy.deepcopy(self._spec)
+    def to_dict(self, **kwargs) -> dict:
+        """Converts the object to dictionary with kind, type and spec as keys.
+
+        Parameters
+        ----------
+        **kwargs: Dict
+            The additional arguments.
+            - filter_by_attribute_map: bool
+                If True, then in the result will be included only the fields
+                presented in the `attribute_map`.
+        """
+        filter_by_attribute_map = kwargs.pop("filter_by_attribute_map", False)
+
+        spec = {
+            key: value
+            for key, value in copy.deepcopy(self._spec).items()
+            if not filter_by_attribute_map or key in self.attribute_map
+        }
+
         for key, value in spec.items():
             if hasattr(value, "to_dict"):
                 value = value.to_dict()
             spec[key] = value
 
         return {
             "kind": self.kind,
@@ -129,7 +144,13 @@
     def from_dict(cls: Type[Self], obj_dict: dict) -> Self:
         """Initialize the object from a Python dictionary"""
         return cls(spec=obj_dict.get("spec"))
 
     def __repr__(self) -> str:
         """Displays the object as YAML."""
         return self.to_yaml()
+
+    def build(self) -> Self:
+        """Load default values from the environment for the job infrastructure.
+        Should be implemented on the child level.
+        """
+        return self
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/infrastructure/base.py` & `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,28 +57,31 @@
 
     def run(
         self,
         name: str = None,
         args: str = None,
         env_var: dict = None,
         freeform_tags: dict = None,
+        defined_tags: dict = None,
         wait: bool = False,
     ):
         """Runs a job on the infrastructure.
 
         Parameters
         ----------
         name : str, optional
             The name of the job run, by default None
         args : str, optional
             Command line arguments for the job run, by default None.
         env_var : dict, optional
-            Environment variable for the job run, by default None
+            Environment variable for the job run, by default None.
         freeform_tags : dict, optional
-            Freeform tags for the job run, by default None
+            Freeform tags for the job run, by default None.
+        defined_tags : dict, optional
+            Defined tags for the job run, by default None.
         wait : bool, optional
             Indicate if this method should wait for the run to finish before it returns, by default False.
         """
         raise NotImplementedError()
 
     def delete(self):
         """Deletes a job from the infrastructure."""
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dataflow.py` & `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dataflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,26 @@
 from ads.jobs.builders.infrastructure.base import Infrastructure, RunInstance
 from ads.jobs.builders.infrastructure.utils import normalize_config
 from ads.jobs.builders.runtimes.python_runtime import DataFlowRuntime
 from ads.model.runtime.env_info import InferenceEnvInfo
 from oci.data_flow.models import CreateApplicationDetails, CreateRunDetails
 from tqdm import tqdm
 
+from ads.config import NB_SESSION_COMPARTMENT_OCID, NB_SESSION_OCID
+
 logger = logging.getLogger(__name__)
 
 CONDA_PACK_SUFFIX = "#conda"
 SLEEP_INTERVAL = 3
 
+DEFAULT_LANGUAGE = "PYTHON"
+DEFAULT_SPARK_VERSION = "3.2.1"
+DEFAULT_NUM_EXECUTORS = 1
+DEFAULT_SHAPE = "VM.Standard.E3.Flex"
+
 
 def conda_pack_name_to_dataflow_config(conda_uri):
     return {
         "spark.archives": conda_uri + CONDA_PACK_SUFFIX,
         "dataflow.auth": "resource_principal",
     }
 
@@ -356,15 +363,14 @@
 
     @property
     def executor(self):
         return _DataFlowLog(run_id=self.run_id, src_type="EXECUTOR")
 
 
 class DataFlow(Infrastructure):
-
     CONST_COMPARTMENT_ID = "compartment_id"
     CONST_CONFIG = "configuration"
     CONST_EXECUTE = "execute"
     CONST_DRIVER_SHAPE = "driver_shape"
     CONST_EXECUTOR_SHAPE = "executor_shape"
     CONST_LANGUAGE = "language"
     CONST_METASTORE_ID = "metastore_id"
@@ -413,65 +419,69 @@
             defaults.update(spec)
             super().__init__(defaults, **kwargs)
 
         self.df_app = DataFlowApp(**self._spec)
         self.runtime = None
         self._name = None
 
-    @staticmethod
-    def _load_default_properties() -> dict:
+    def _load_default_properties(self) -> Dict:
         """
         Load default properties from environment variables, notebook session, etc.
 
         Returns
         -------
         dict
             a dictionary of default properties
         """
         defaults = {}
-        if "NB_SESSION_COMPARTMENT_OCID" in os.environ:
-            defaults["compartment_id"] = os.environ["NB_SESSION_COMPARTMENT_OCID"]
-        if "NB_SESSION_OCID" in os.environ:
+        if NB_SESSION_COMPARTMENT_OCID:
+            defaults[self.CONST_COMPARTMENT_ID] = NB_SESSION_COMPARTMENT_OCID
+        if NB_SESSION_OCID:
             dsc_client = OCIClientFactory(**default_signer()).data_science
             try:
-                nb_session = dsc_client.get_notebook_session(
-                    os.environ["NB_SESSION_OCID"]
-                ).data
+                nb_session = dsc_client.get_notebook_session(NB_SESSION_OCID).data
                 nb_config = nb_session.notebook_session_configuration_details
-                defaults["driver_shape"] = nb_config.shape
+
+                defaults[self.CONST_DRIVER_SHAPE] = nb_config.shape
                 logger.debug(f"Set driver shape to {nb_config.shape}")
-                defaults["executor_shape"] = nb_config.shape
+
+                defaults[self.CONST_EXECUTOR_SHAPE] = nb_config.shape
                 logger.debug(f"Set executor shape to {nb_config.shape}")
+
                 if nb_config.notebook_session_shape_config_details:
                     notebook_shape_config_details = oci_util.to_dict(
                         nb_config.notebook_session_shape_config_details
                     )
-                    defaults["driver_shape_config"] = copy.deepcopy(
+
+                    defaults[self.CONST_DRIVER_SHAPE_CONFIG] = copy.deepcopy(
                         notebook_shape_config_details
                     )
                     logger.debug(
                         f"Set driver shape config to {nb_config.notebook_session_shape_config_details}"
                     )
-                    defaults["executor_shape_config"] = copy.deepcopy(
+
+                    defaults[self.CONST_EXECUTOR_SHAPE_CONFIG] = copy.deepcopy(
                         notebook_shape_config_details
                     )
                     logger.debug(
                         f"Set executor shape config to {nb_config.notebook_session_shape_config_details}"
                     )
 
             except Exception as e:
                 logger.warning(
                     f"Error fetching details about Notebook session: {os.environ['NB_SESSION_OCID']}. {e}"
                 )
 
-        defaults["language"] = "PYTHON"
-        defaults["spark_version"] = "3.2.1"
-        defaults["num_executors"] = 1
-        logger.debug("Set spark version to be 3.2.1.")
-        logger.debug("Set number of executors to be 1.")
+        defaults["language"] = DEFAULT_LANGUAGE
+        defaults["spark_version"] = DEFAULT_SPARK_VERSION
+        defaults["num_executors"] = DEFAULT_NUM_EXECUTORS
+
+        logger.debug(f"Set spark version to be {defaults['spark_version']}")
+        logger.debug(f"Set number of executors to be {defaults['num_executors']}")
+
         return defaults
 
     @property
     def name(self) -> str:
         """Display name of the job"""
         return self._name
 
@@ -1030,15 +1040,15 @@
             list of Data Flow jobs
         """
         return [
             cls.from_id(job.id)
             for job in DataFlowApp.list_resource(compartment_id, **kwargs)
         ]
 
-    def to_dict(self) -> dict:
+    def to_dict(self, **kwargs) -> dict:
         """
         Serialize job to a dictionary.
 
         Returns
         -------
         dict
             serialized job as a dictionary
@@ -1109,16 +1119,34 @@
                     if converted_key:
                         temp_maps[converted_key] = value
                     else:
                         temp_maps[key] = value
                 spec[shape_config] = copy.deepcopy(temp_maps)
         return spec
 
-    def to_yaml(self) -> str:
+    def to_yaml(self, **kwargs) -> str:
         """Serializes the object into YAML string.
 
         Returns
         -------
         str
             YAML stored in a string.
         """
-        return yaml.safe_dump(self.to_dict())
+        return yaml.safe_dump(self.to_dict(**kwargs))
+
+    def init(self) -> "DataFlow":
+        """Initializes a starter specification for the DataFlow.
+
+        Returns
+        -------
+        DataFlow
+            The DataFlow instance (self)
+        """
+        return (
+            self.build()
+            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
+            .with_language(self.language or DEFAULT_LANGUAGE)
+            .with_spark_version(self.spark_version or DEFAULT_SPARK_VERSION)
+            .with_num_executors(self.num_executors or DEFAULT_NUM_EXECUTORS)
+            .with_driver_shape(self.driver_shape or DEFAULT_SHAPE)
+            .with_executor_shape(self.executor_shape or DEFAULT_SHAPE)
+        )
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dsc_job.py` & `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 from __future__ import annotations
 
 import datetime
 import logging
+import oci
 import os
 import time
 import traceback
 import uuid
 from io import DEFAULT_BUFFER_SIZE
 from string import Template
 from typing import Any, Dict, List, Optional, Union
@@ -30,18 +31,22 @@
     DataScienceJobRuntimeManager,
 )
 from ads.jobs.builders.infrastructure.utils import get_value
 from ads.jobs.builders.runtimes.artifact import Artifact
 from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
 from ads.jobs.builders.runtimes.python_runtime import GitPythonRuntime
 
+from ads.common.dsc_file_system import OCIFileStorage, DSCFileSystemManager
+
 logger = logging.getLogger(__name__)
 
 SLEEP_INTERVAL = 3
 WAIT_SECONDS_AFTER_FINISHED = 90
+MAXIMUM_MOUNT_COUNT = 5
+FILE_STORAGE_TYPE = "FILE_STORAGE"
 
 
 class DSCJob(OCIDataScienceMixin, oci.data_science.models.Job):
     """Represents an OCI Data Science Job
     This class contains all attributes of the oci.data_science.models.Job.
     The main purpose of this class is to link the oci.data_science.models.Job model and the related client methods.
     Mainly, linking the Job model (payload) to Create/Update/Get/List/Delete methods.
@@ -433,14 +438,16 @@
             Keyword arguments for initializing a Data Science Job Run.
             The keys can be any keys in supported by OCI JobConfigurationDetails and JobRun, including:
             * hyperparameter_values: dict(str, str)
             * environment_variables: dict(str, str)
             * command_line_arguments: str
             * maximum_runtime_in_minutes: int
             * display_name: str
+            * freeform_tags: dict(str, str)
+            * defined_tags: dict(str, dict(str, object))
 
         If display_name is not specified, it will be generated as "<JOB_NAME>-run-<TIMESTAMP>".
 
         Returns
         -------
         DSCJobRun
             An instance of DSCJobRun, which can be used to monitor the job run.
@@ -829,14 +836,24 @@
             .with_project_id("<project_ocid>")
             .with_subnet_id("<subnet_ocid>")
             .with_shape_name("VM.Standard.E3.Flex")
             # Shape config details are applicable only for the flexible shapes.
             .with_shape_config_details(memory_in_gbs=16, ocpus=1)
             # Minimum/Default block storage size is 50 (GB).
             .with_block_storage_size(50)
+            # A list of file systems to be mounted
+            .with_storage_mount(
+                {
+                    "src" : "<mount_target_ip_address>:<export_path>",
+                    "dest" : "<destination_directory_name>"
+                }
+            )
+            # Tags
+            .with_freeform_tag(my_tag="my_value")
+            .with_defined_tag(**{"Operations": {"CostCenter": "42"}})
         )
 
     """
 
     CONST_PROJECT_ID = "projectId"
     CONST_COMPARTMENT_ID = "compartmentId"
     CONST_DISPLAY_NAME = "displayName"
@@ -846,27 +863,33 @@
     CONST_BLOCK_STORAGE = "blockStorageSize"
     CONST_SUBNET_ID = "subnetId"
     CONST_SHAPE_CONFIG_DETAILS = "shapeConfigDetails"
     CONST_MEMORY_IN_GBS = "memoryInGBs"
     CONST_OCPUS = "ocpus"
     CONST_LOG_ID = "logId"
     CONST_LOG_GROUP_ID = "logGroupId"
+    CONST_STORAGE_MOUNT = "storageMount"
+    CONST_FREEFORM_TAGS = "freeformTags"
+    CONST_DEFINED_TAGS = "definedTags"
 
     attribute_map = {
         CONST_PROJECT_ID: "project_id",
         CONST_COMPARTMENT_ID: "compartment_id",
         CONST_DISPLAY_NAME: "display_name",
         CONST_JOB_TYPE: "job_type",
         CONST_JOB_INFRA: "job_infrastructure_type",
         CONST_SHAPE_NAME: "shape_name",
         CONST_BLOCK_STORAGE: "block_storage_size",
         CONST_SUBNET_ID: "subnet_id",
         CONST_SHAPE_CONFIG_DETAILS: "shape_config_details",
         CONST_LOG_ID: "log_id",
         CONST_LOG_GROUP_ID: "log_group_id",
+        CONST_STORAGE_MOUNT: "storage_mount",
+        CONST_FREEFORM_TAGS: "freeform_tags",
+        CONST_DEFINED_TAGS: "defined_tags",
     }
 
     shape_config_details_attribute_map = {
         CONST_MEMORY_IN_GBS: "memory_in_gbs",
         CONST_OCPUS: "ocpus",
     }
 
@@ -884,34 +907,40 @@
         CONST_LOG_GROUP_ID: "job_log_configuration_details.log_group_id",
     }
 
     snake_to_camel_map = {
         v.split(".", maxsplit=1)[-1]: k for k, v in payload_attribute_map.items()
     }
 
+    storage_mount_type_dict = {FILE_STORAGE_TYPE: OCIFileStorage}
+
     @staticmethod
     def standardize_spec(spec):
         if not spec:
             return {}
 
         attribute_map = {
             **DataScienceJob.attribute_map,
             **DataScienceJob.shape_config_details_attribute_map,
         }
         snake_to_camel_map = {v: k for k, v in attribute_map.items()}
+        snake_to_camel_map = {
+            **{v: k for k, v in attribute_map.items()},
+            **DataScienceJob.snake_to_camel_map,
+        }
 
         for key in list(spec.keys()):
-            if key not in attribute_map and key in snake_to_camel_map:
+            if key not in attribute_map and key.lower() in snake_to_camel_map:
                 value = spec.pop(key)
                 if isinstance(value, dict):
-                    spec[snake_to_camel_map[key]] = DataScienceJob.standardize_spec(
-                        value
-                    )
+                    spec[
+                        snake_to_camel_map[key.lower()]
+                    ] = DataScienceJob.standardize_spec(value)
                 else:
-                    spec[snake_to_camel_map[key]] = value
+                    spec[snake_to_camel_map[key.lower()]] = value
         return spec
 
     def __init__(self, spec: Dict = None, **kwargs) -> None:
         """Initializes a data science job infrastructure
 
         Parameters
         ----------
@@ -1208,14 +1237,82 @@
         Returns
         -------
         str
             Log group OCID
         """
         return self.get_spec(self.CONST_LOG_GROUP_ID)
 
+    def with_storage_mount(self, *storage_mount: List[dict]) -> DataScienceJob:
+        """Sets the file systems to be mounted for the data science job.
+        A maximum number of 5 file systems are allowed to be mounted for a single data science job.
+
+        Parameters
+        ----------
+        storage_mount : List[dict]
+            A list of file systems to be mounted.
+
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        storage_mount_list = []
+        for item in storage_mount:
+            if not isinstance(item, dict):
+                raise ValueError(
+                    "Parameter `storage_mount` should be a list of dictionaries."
+                )
+            storage_mount_list.append(item)
+        if len(storage_mount_list) > MAXIMUM_MOUNT_COUNT:
+            raise ValueError(
+                f"A maximum number of {MAXIMUM_MOUNT_COUNT} file systems are allowed to be mounted at this time for a job."
+            )
+        return self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount_list)
+
+    @property
+    def storage_mount(self) -> List[dict]:
+        """Files systems that have been mounted for the data science job
+
+        Returns
+        -------
+        list
+            A list of file systems that have been mounted
+        """
+        return self.get_spec(self.CONST_STORAGE_MOUNT, [])
+
+    def with_freeform_tag(self, **kwargs) -> DataScienceJob:
+        """Sets freeform tags
+
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        return self.set_spec(self.CONST_FREEFORM_TAGS, kwargs)
+
+    def with_defined_tag(self, **kwargs) -> DataScienceJob:
+        """Sets defined tags
+
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        return self.set_spec(self.CONST_DEFINED_TAGS, kwargs)
+
+    @property
+    def freeform_tags(self) -> dict:
+        """Freeform tags"""
+        return self.get_spec(self.CONST_FREEFORM_TAGS, {})
+
+    @property
+    def defined_tags(self) -> dict:
+        """Defined tags"""
+        return self.get_spec(self.CONST_DEFINED_TAGS, {})
+
     def _prepare_log_config(self) -> dict:
         if not self.log_group_id and not self.log_id:
             return None
         # Look up log group ID if only the log ID is specified
         if self.log_id and not self.log_group_id:
             try:
                 log_obj = OCILog.from_ocid(self.log_id)
@@ -1281,14 +1378,50 @@
                     sub_value = get_value(value, sub_dsc_attr)
                     if not sub_value:
                         continue
                     if overwrite or not sub_spec.get(sub_infra_attr):
                         sub_spec[sub_infra_attr] = sub_value
                 if sub_spec:
                     self._spec[infra_attr] = sub_spec
+
+        self._update_storage_mount_from_dsc_model(dsc_job, overwrite)
+        return self
+
+    def _update_storage_mount_from_dsc_model(
+        self, dsc_job: oci.data_science.models.Job, overwrite: bool = True
+    ) -> DataScienceJob:
+        """Update the mount storage properties from an OCI data science job model.
+
+        Parameters
+        ----------
+        dsc_job: oci.data_science.models.Job
+            An OCI data science job model.
+
+        overwrite: bool
+            Whether to overwrite the existing values.
+            If this is set to False, only the empty/None properties will be updated.
+
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        storage_mount_list = get_value(
+            dsc_job, "job_storage_mount_configuration_details_list"
+        )
+        if storage_mount_list:
+            storage_mount = [
+                self.storage_mount_type_dict[
+                    file_system.storage_type
+                ].update_from_dsc_model(file_system)
+                for file_system in storage_mount_list
+                if file_system.storage_type in self.storage_mount_type_dict
+            ]
+            if overwrite or not self.get_spec(self.CONST_STORAGE_MOUNT):
+                self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount)
         return self
 
     def _update_job_infra(self, dsc_job: DSCJob) -> DataScienceJob:
         """Updates the job infrastructure from a DSCJob object.
 
         Parameters
         ----------
@@ -1317,21 +1450,48 @@
             if value:
                 dsc_job.job_infrastructure_configuration_details[camel_attr] = value
 
         if dsc_job.job_infrastructure_configuration_details.get("subnetId"):
             dsc_job.job_infrastructure_configuration_details[
                 "jobInfrastructureType"
             ] = JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE
+
+        if self.storage_mount:
+            if not hasattr(
+                oci.data_science.models, "JobStorageMountConfigurationDetails"
+            ):
+                raise EnvironmentError(
+                    "Storage mount hasn't been supported in the current OCI SDK installed."
+                )
+            dsc_job.job_storage_mount_configuration_details_list = [
+                DSCFileSystemManager.initialize(file_system)
+                for file_system in self.storage_mount
+            ]
         return self
 
     def build(self) -> DataScienceJob:
         self.dsc_job.load_defaults()
         self._update_from_dsc_model(self.dsc_job, overwrite=False)
         return self
 
+    def init(self) -> DataScienceJob:
+        """Initializes a starter specification for the DataScienceJob.
+
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        return (
+            self.build()
+            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
+            .with_project_id(self.project_id or "{Provide a project OCID}")
+            .with_subnet_id(self.subnet_id or "{Provide a subnet OCID or remove this field if you use a default networking}")
+        )
+
     def create(self, runtime, **kwargs) -> DataScienceJob:
         """Creates a job with runtime.
 
         Parameters
         ----------
         runtime : Runtime
             An ADS job runtime.
@@ -1357,69 +1517,89 @@
         ):
             display_name = utils.get_random_name_for_resource()
         else:
             display_name = None
 
         payload["display_name"] = display_name
         payload["job_log_configuration_details"] = self._prepare_log_config()
+        if not payload.get("freeform_tags"):
+            payload["freeform_tags"] = self.freeform_tags
+        if not payload.get("defined_tags"):
+            payload["defined_tags"] = self.defined_tags
 
         self.dsc_job = DSCJob(**payload)
         # Set Job infra to user values after DSCJob initialized the defaults
         self._update_job_infra(self.dsc_job)
         self.dsc_job.create()
         # Update the model from infra after job creation.
         self._update_from_dsc_model(self.dsc_job)
         return self
 
     def run(
-        self, name=None, args=None, env_var=None, freeform_tags=None, wait=False
+        self,
+        name=None,
+        args=None,
+        env_var=None,
+        freeform_tags=None,
+        defined_tags=None,
+        wait=False,
     ) -> DataScienceJobRun:
         """Runs a job on OCI Data Science job
 
         Parameters
         ----------
         name : str, optional
             The name of the job run, by default None.
         args : str, optional
             Command line arguments for the job run, by default None.
         env_var : dict, optional
             Environment variable for the job run, by default None
         freeform_tags : dict, optional
             Freeform tags for the job run, by default None
+        defined_tags : dict, optional
+            Defined tags for the job run, by default None
         wait : bool, optional
             Indicate if this method should wait for the run to finish before it returns, by default False.
 
         Returns
         -------
         DataScienceJobRun
             A Data Science Job Run instance.
 
         """
         # Runtime in the infrastructure will be None if the job is not created.
         if not self.runtime:
             raise RuntimeError(
                 "Job is not created. Call create() to create the job first."
             )
-        tags = self.runtime.freeform_tags
-        if not tags:
-            tags = {}
-        if freeform_tags:
-            tags.update(freeform_tags)
+
+        if not freeform_tags:
+            freeform_tags = {}
+        runtime_freeform_tags = self.runtime.freeform_tags
+        if runtime_freeform_tags:
+            freeform_tags.update(runtime_freeform_tags)
+
+        if not defined_tags:
+            defined_tags = {}
+        runtime_defined_tags = self.runtime.defined_tags
+        if runtime_defined_tags:
+            defined_tags.update(runtime_defined_tags)
 
         if name:
             envs = self.runtime.envs
             if env_var:
                 envs.update(env_var)
             name = Template(name).safe_substitute(envs)
 
         return self.dsc_job.run(
             display_name=name,
             command_line_arguments=args,
             environment_variables=env_var,
-            freeform_tags=tags,
+            freeform_tags=freeform_tags,
+            defined_tags=defined_tags,
             wait=wait,
         )
 
     def delete(self) -> None:
         """Deletes a job"""
         self.dsc_job.delete()
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/infrastructure/dsc_job_runtime.py` & `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/dsc_job_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     NotebookArtifact,
     PythonArtifact,
     GitPythonArtifact,
 )
 from ads.jobs.builders.infrastructure.utils import get_value
 
 
-class IncompatibleRuntime(Exception):
+class IncompatibleRuntime(Exception):  # pragma: no cover
     """Represents an exception when runtime is not compatible with the OCI data science job configuration.
     This exception is designed to be raised during the extraction of a runtime from OCI data science job.
     The data science job does not explicitly contain information of the type of the ADS runtime.
     Each runtime handler should determine if the configuration of the job can be converted to the runtime.
     This exception should be raised during the extract() call if the configuration cannot be converted.
     The RuntimeManager uses this exception to determine if the conversion is successful.
     """
@@ -100,14 +100,16 @@
             JSON payload for defining a Data Science Job with OCI API
         """
         payload = {}
         payload["artifact"] = self._translate_artifact(runtime)
         payload["job_configuration_details"] = self._translate_config(runtime)
         if runtime.freeform_tags:
             payload["freeform_tags"] = runtime.freeform_tags
+        if runtime.defined_tags:
+            payload["defined_tags"] = runtime.defined_tags
         self.data_science_job.runtime = runtime
         return payload
 
     def _translate_artifact(self, runtime: Runtime):
         """Translate the runtime artifact.
         OCI data science requires an artifact file to be uploaded before the job is created.
         For Python runtime, the artifact is the script for running the job.
@@ -349,18 +351,22 @@
             The data science job containing runtime information.
 
         Returns
         -------
         dict
             A runtime specification dictionary for initializing a runtime.
         """
+        tags = {}
         value = get_value(dsc_job, "freeform_tags")
         if value:
-            return {Runtime.CONST_TAG: value}
-        return {}
+            tags[Runtime.CONST_FREEFORM_TAGS] = value
+        value = get_value(dsc_job, "defined_tags")
+        if value:
+            tags[Runtime.CONST_DEFINED_TAGS] = value
+        return tags
 
     def _extract_artifact(self, dsc_job):
         """Extract the job artifact from data science job.
 
         This is the base method which does not extract the job artifact.
         Sub-class should implement the extraction if needed.
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/infrastructure/utils.py` & `oracle_ads-2.8.4/ads/jobs/builders/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/runtimes/artifact.py` & `oracle_ads-2.8.4/ads/jobs/builders/runtimes/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/runtimes/base.py` & `oracle_ads-2.8.4/ads/jobs/builders/runtimes/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 class Runtime(Builder):
     """Base class for job runtime"""
 
     # Constant strings
     CONST_ENV_VAR = "env"
     CONST_ARGS = "args"
     CONST_MAXIMUM_RUNTIME_IN_MINUTES = "maximumRuntimeInMinutes"
-    CONST_TAG = "freeformTags"
+    CONST_FREEFORM_TAGS = "freeformTags"
+    CONST_DEFINED_TAGS = "definedTags"
 
     attribute_map = {
-        CONST_TAG: "freeform_tags",
+        CONST_FREEFORM_TAGS: "freeform_tags",
+        CONST_DEFINED_TAGS: "defined_tags",
         CONST_ENV_VAR: CONST_ENV_VAR,
     }
 
     def __init__(self, spec: Dict = None, **kwargs) -> None:
         env = {}
         if spec and "env" in spec and isinstance(spec["env"], dict):
             env = spec.pop("env", {})
@@ -160,22 +162,32 @@
         """
         if not kwargs:
             return self
         envs = [{"name": k, "value": v} for k, v in kwargs.items()]
         return self.set_spec(self.CONST_ENV_VAR, envs)
 
     def with_freeform_tag(self: Self, **kwargs) -> Self:
-        """Sets freeform tag
+        """Sets freeform tags
 
         Returns
         -------
         Self
             This method returns self to support chaining methods.
         """
-        return self.set_spec(self.CONST_TAG, kwargs)
+        return self.set_spec(self.CONST_FREEFORM_TAGS, kwargs)
+
+    def with_defined_tag(self: Self, **kwargs) -> Self:
+        """Sets defined tags
+
+        Returns
+        -------
+        Self
+            This method returns self to support chaining methods.
+        """
+        return self.set_spec(self.CONST_DEFINED_TAGS, kwargs)
 
     def with_maximum_runtime_in_minutes(
         self: Self, maximum_runtime_in_minutes: int
     ) -> Self:
         """Sets maximum runtime in minutes
 
         Returns
@@ -205,19 +217,38 @@
     @property
     def envs(self) -> dict:
         """Environment variables"""
         return self.environment_variables
 
     @property
     def freeform_tags(self) -> dict:
-        """freeform_tags"""
-        return self.get_spec(self.CONST_TAG, {})
+        """Freeform tags"""
+        return self.get_spec(self.CONST_FREEFORM_TAGS, {})
+
+    @property
+    def defined_tags(self) -> dict:
+        """Defined tags"""
+        return self.get_spec(self.CONST_DEFINED_TAGS, {})
 
     @property
     def args(self) -> list:
         """Command line arguments"""
         return self.get_spec(self.CONST_ARGS, [])
 
     @property
     def maximum_runtime_in_minutes(self) -> int:
         """Maximum runtime in minutes"""
         return self.get_spec(self.CONST_MAXIMUM_RUNTIME_IN_MINUTES)
+
+    def init(self) -> Self:
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        Self
+            This method returns self to support chaining methods.
+        """
+        return (
+            self.with_environment_variable(env_name="env_value")
+            .with_freeform_tag(tag_name="tag_value")
+            .with_argument(key1="val1")
+        )
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/runtimes/container_runtime.py` & `oracle_ads-2.8.4/ads/jobs/builders/runtimes/container_runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,7 +118,23 @@
         Returns
         -------
         ContainerRuntime
             The runtime instance.
         """
         self._spec[self.CONST_CMD] = cmd
         return self
+
+    def init(self) -> "ContainerRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        ContainerRuntime
+            The runtime instance.
+        """
+        super().init()
+
+        return self.with_image(
+            image="iad.ocir.io/namespace/image:tag",
+            entrypoint=["bash", "--login", "-c"],
+            cmd="{Container CMD. For MLFlow, it will be replaced with the Project CMD}",
+        )
```

### Comparing `oracle_ads-2.8.3/ads/jobs/builders/runtimes/python_runtime.py` & `oracle_ads-2.8.4/ads/jobs/builders/runtimes/python_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 from __future__ import annotations
 
-import json
 import os
-from typing import Any, Dict
+from typing import Dict
 
-from ads.jobs.builders.runtimes.base import Runtime
 from ads.common.auth import default_signer
+from ads.jobs.builders.runtimes.base import Runtime
 from ads.opctl.config.utils import convert_notebook
 
 
 class CondaRuntime(Runtime):
     """Represents a job runtime with conda pack
     This is the base class for Runtime using conda environment.
     The ``CondaRuntime`` is not designed to be used directly when creating a job.
@@ -113,14 +112,28 @@
             self.CONST_CONDA_TYPE: self.CONST_CONDA_TYPE_CUSTOM,
             self.CONST_CONDA_URI: uri,
         }
         if region:
             conda_spec[self.CONST_CONDA_REGION] = region
         return self.set_spec(self.CONST_CONDA, conda_spec)
 
+    def init(self) -> "CondaRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        CondaRuntime
+            The runtime instance.
+        """
+        super().init()
+        return self.with_custom_conda(
+            "{Path to the custom conda environment. "
+            "Example: oci://your_bucket@namespace/object_name"
+        )
+
 
 class ScriptRuntime(CondaRuntime):
     """Represents job runtime with scripts and conda pack.
 
     This runtime is designed to define job artifacts and configurations supported by OCI Data Science Jobs natively.
     It can be used with any script types that is supported by the OCI Data Science Jobs,
     including shell scripts and python scripts.
@@ -229,14 +242,33 @@
         Returns
         -------
         self
             The runtime instance.
         """
         return self.set_spec(self.CONST_ENTRYPOINT, entrypoint)
 
+    def init(self) -> "ScriptRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        ScriptRuntime
+            The runtime instance.
+        """
+        super().init()
+        return (
+            self.with_entrypoint(
+                "{Entrypoint script. For MLflow, it will be replaced with the CMD}"
+            )
+            .with_script(
+                "{Path to the script. For MLflow, it will be replaced with the path to the project}"
+            )
+            .with_argument(key1="val1")
+        )
+
 
 class _PythonRuntimeMixin(Runtime):
     CONST_OUTPUT_DIR = "outputDir"
     CONST_OUTPUT_URI = "outputUri"
     CONST_PYTHON_PATH = "pythonPath"
     CONST_ENTRYPOINT = "entrypoint"
     CONST_ENTRY_FUNCTION = "entryFunction"
@@ -399,14 +431,33 @@
 
     """
 
     attribute_map = {}
     attribute_map.update(ScriptRuntime.attribute_map)
     attribute_map.update(_PythonRuntimeMixin.attribute_map)
 
+    def init(self) -> "PythonRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        PythonRuntime
+            The runtime instance.
+        """
+        super().init()
+        return (
+            self.with_working_dir("{For MLflow the project folder will be used.}")
+            .with_entrypoint(
+                "{Entrypoint script. For MLflow, it will be replaced with the CMD}"
+            )
+            .with_script(
+                "{Path to the script. For MLflow, it will be replaced with the path to the project}"
+            )
+        )
+
 
 class NotebookRuntime(CondaRuntime):
     """Represents a job runtime with Jupyter notebook
 
     To run a job with a single Jupyter notebook,
     you can define the run time as::
 
@@ -568,14 +619,28 @@
         return self.get_spec(self.CONST_SOURCE)
 
     @property
     def notebook(self) -> str:
         """The path of the notebook relative to the source."""
         return self.get_spec(self.CONST_ENTRYPOINT)
 
+    def init(self) -> "NotebookRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        NotebookRuntime
+            The runtime instance.
+        """
+        super().init()
+        return self.with_source(
+            uri="{Path to the source code directory. For MLflow, it will be replaced with the path to the project}",
+            notebook="{Entrypoint notebook. For MLflow, it will be replaced with the CMD}",
+        ).with_exclude_tag("tag1")
+
 
 class GitPythonRuntime(CondaRuntime, _PythonRuntimeMixin):
     """Represents a job runtime with source code from git repository
 
     Example::
 
         runtime = (
@@ -675,17 +740,31 @@
         return self.get_spec(self.CONST_COMMIT)
 
     @property
     def ssh_secret_ocid(self) -> str:
         """The OCID of the OCI Vault secret storing the Git SSH key."""
         return self.get_spec(self.CONST_GIT_SSH_SECRET_ID)
 
+    def init(self) -> "GitPythonRuntime":
+        """Initializes a starter specification for the runtime.
 
-class DataFlowRuntime(CondaRuntime):
+        Returns
+        -------
+        GitPythonRuntime
+            The runtime instance.
+        """
+        super().init()
+        return self.with_source(
+            "{Git URI. For MLflow, it will be replaced with the Project URI}"
+        ).with_entrypoint(
+            "{Entrypoint script. For MLflow, it will be replaced with the CMD}"
+        )
 
+
+class DataFlowRuntime(CondaRuntime):
     CONST_SCRIPT_BUCKET = "scriptBucket"
     CONST_ARCHIVE_BUCKET = "archiveBucket"
     CONST_ARCHIVE_URI = "archiveUri"
     CONST_SCRIPT_PATH = "scriptPathURI"
     CONST_CONFIGURATION = "configuration"
     CONST_CONDA_AUTH_TYPE = "condaAuthType"
     CONST_OVERWRITE = "overwrite"
@@ -884,14 +963,36 @@
     def overwrite(self) -> str:
         """Whether to overwrite the existing script in object storage (script bucket)."""
         return self.get_spec(self.CONST_OVERWRITE)
 
     def convert(self, **kwargs):
         pass
 
+    def init(self) -> "DataFlowRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        DataFlowRuntime
+            The runtime instance.
+        """
+        super().init()
+        self._spec.pop(self.CONST_ENV_VAR, None)
+        return (
+            self.with_script_uri(
+                "{Path to the executable script. For MLflow, it will be replaced with the CMD}"
+            )
+            .with_script_bucket(
+                "{The object storage bucket to save a script. "
+                "Example: oci://<bucket_name>@<tenancy>/<prefix>}"
+            )
+            .with_overwrite(True)
+            .with_configuration({"spark.driverEnv.env_key": "env_value"})
+        )
+
 
 class DataFlowNotebookRuntime(DataFlowRuntime, NotebookRuntime):
     def convert(self, overwrite=False):
         if self.output_uri:
             path = os.path.join(
                 self.output_uri,
                 str(os.path.basename(self.notebook_uri)).replace(".ipynb", ".py"),
```

### Comparing `oracle_ads-2.8.3/ads/jobs/cli.py` & `oracle_ads-2.8.4/ads/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/env_var_parser.py` & `oracle_ads-2.8.4/ads/jobs/env_var_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/extension.py` & `oracle_ads-2.8.4/ads/jobs/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 
-import os
-import tempfile
 import json
+import os
 import shlex
+import tempfile
+import warnings
 from getopt import gnu_getopt
 
-from ads.opctl.constants import (
-    ADS_DATAFLOW_CONFIG_FILE_NAME,
-    DEFAULT_ADS_CONFIG_FOLDER,
-)
-from ads.jobs import Job, DataFlow, DataFlowRuntime, DataFlowRun
+from ads.common.decorator.runtime_dependency import (OptionalDependency,
+                                                     runtime_dependency)
+from ads.jobs import DataFlow, DataFlowRun, DataFlowRuntime, Job
 from ads.jobs.utils import get_dataflow_config
-from ads.common.decorator.runtime_dependency import (
-    runtime_dependency,
-    OptionalDependency,
-)
+from ads.opctl.constants import (ADS_DATAFLOW_CONFIG_FILE_NAME,
+                                 DEFAULT_ADS_CONFIG_FOLDER)
 
 
 def dataflow(line, cell=None):
     opts, args = gnu_getopt(
         shlex.split(line),
         "f:a:c:t:n:hwo",
         longopts=[
@@ -87,29 +84,35 @@
         script_name = options["--file"]
     else:
         script_name = "script.py"
     if "-a" in options:
         archive_name = options["-a"]
     elif "--archive" in options:
         archive_name = options["--archive"]
+    elif hasattr(dataflow_config, "archive_uri") and dataflow_config.archive_uri:
+        archive_name = dataflow_config.archive_uri
     else:
         archive_name = None
     with tempfile.TemporaryDirectory() as td:
         file = os.path.join(td, script_name)
         with open(file, "w") as f:
             f.write(cell)
         rt_spec = {
             "scriptPathURI": file,
             "scriptBucket": dataflow_config.pop("script_bucket"),
         }
         if len(args) > 1:
             rt_spec["args"] = args[1:]
         if archive_name:
             rt_spec["archiveUri"] = archive_name
-            rt_spec["archiveBucket"] = dataflow_config.pop("archive_bucket")
+            rt_spec["archiveBucket"] = dataflow_config.pop("archive_bucket", None)
+            if not archive_name.startswith("oci://") and not rt_spec["archiveBucket"]:
+                raise ValueError(
+                    "`archiveBucket` has to be set in the config if `archive` is a local path."
+                )
         rt = DataFlowRuntime(rt_spec)
         infra = DataFlow(spec=dataflow_config)
         if "-o" in options or "--overwrite" in options:
             df = infra.create(rt, overwrite=True)
         else:
             df = infra.create(rt)
         print("DataFlow App ID", df.id)
```

### Comparing `oracle_ads-2.8.3/ads/jobs/schema/infrastructure_schema.json` & `oracle_ads-2.8.4/ads/jobs/schema/infrastructure_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/schema/job_schema.json` & `oracle_ads-2.8.4/ads/jobs/schema/job_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/schema/runtime_schema.json` & `oracle_ads-2.8.4/ads/jobs/schema/runtime_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666666%*

 * *Differences: {"'type'": "{'allowed': {insert: [(7, 'dataFlowNotebook')]}}"}*

```diff
@@ -170,13 +170,14 @@
         "allowed": [
             "python",
             "container",
             "notebook",
             "gitPython",
             "operator",
             "script",
-            "dataFlow"
+            "dataFlow",
+            "dataFlowNotebook"
         ],
         "required": true,
         "type": "string"
     }
 }
```

### Comparing `oracle_ads-2.8.3/ads/jobs/schema/validator.py` & `oracle_ads-2.8.4/ads/jobs/schema/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/serializer.py` & `oracle_ads-2.8.4/ads/jobs/serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 import json
 from abc import ABC, abstractmethod
-from typing import Union, TypeVar, Type
+from typing import Type, TypeVar, Union, Dict
+from urllib.parse import urlparse
 
 import fsspec
 import yaml
 
-
 Self = TypeVar("Self", bound="Serializable")
 """Special type to represent the current enclosed class.
 
 This type is used by factory class method or when a method returns ``self``.
 """
 
 
 class Serializable(ABC):
     """Base class that represents a serializable item."""
 
     @abstractmethod
-    def to_dict(self) -> dict:
-        """Serializes an instance of class into a dictionary"""
+    def to_dict(self, **kwargs: Dict) -> Dict:
+        """Serializes an instance of class into a dictionary.
+
+        Parameters
+        ----------
+        **kwargs: Dict
+            Additional arguments.
+
+        Returns
+        -------
+        Dict
+            The result dictionary.
+        """
 
     @classmethod
     @abstractmethod
     def from_dict(cls, obj_dict: dict):
         """Initialize an instance of the class from a dictionary
 
         Parameters
@@ -46,14 +57,24 @@
             The content to be written.
         uri : str
             URI of the file to save the content.
         kwargs : dict
             keyword arguments to be passed into fsspec.open().
             For OCI object storage, this can be config="path/to/.oci/config".
         """
+
+        overwrite = kwargs.pop("overwrite", True)
+        if not overwrite:
+            dst_path_scheme = urlparse(uri).scheme or "file"
+            if fsspec.filesystem(dst_path_scheme, **kwargs).exists(uri):
+                raise FileExistsError(
+                    f"The `{uri}` is already exists. Set `overwrite` to True "
+                    "if you wish to overwrite."
+                )
+
         with fsspec.open(uri, "w", **kwargs) as f:
             f.write(s)
 
     @staticmethod
     def _read_from_file(uri: str, **kwargs) -> str:
         """Returns contents from a file specified by URI
 
@@ -78,25 +99,30 @@
         Parameters
         ----------
         uri : str, optional
             URI location to save the JSON string, by default None
         encoder : callable, optional
             Encoder for custom data structures, by default json.JSONEncoder
         kwargs : dict
-            keyword arguments to be passed into fsspec.open().
-            For OCI object storage, this can be config="path/to/.oci/config".
+            overwrite: (bool, optional). Defaults to True.
+                Whether to overwrite existing file or not.
+
+            The other keyword arguments to be passed into fsspec.open().
+            For OCI object storage, this could be config="path/to/.oci/config".
 
         Returns
         -------
-        str
-            object serialized as a JSON string
+        Union[str, None]
+            Serialized version of object.
+            `None` in case when `uri` provided.
         """
-        json_string = json.dumps(self.to_dict(), cls=encoder)
+        json_string = json.dumps(self.to_dict(**kwargs), cls=encoder)
         if uri:
             self._write_to_file(s=json_string, uri=uri, **kwargs)
+            return None
         return json_string
 
     @classmethod
     def from_json(
         cls: Type[Self],
         json_string: str = None,
         uri: str = None,
@@ -156,24 +182,32 @@
         Parameters
         ----------
         uri : str, optional
             URI location to save the YAML string, by default None
         dumper : callable, optional
             Custom YAML Dumper, by default yaml.SafeDumper
         kwargs : dict
-            keyword arguments to be passed into fsspec.open().
-            For OCI object storage, this can be config="path/to/.oci/config".
+            overwrite: (bool, optional). Defaults to True.
+                Whether to overwrite existing file or not.
+            note: (str, optional)
+                The note that needs to be added in the beginning of the YAML.
+                It will be added as is without any formatting.
+
+            The other keyword arguments to be passed into fsspec.open().
+            For OCI object storage, this could be config="path/to/.oci/config".
 
         Returns
         -------
         Union[str, None]
-            If uri is specified, None will be returned.
-            Otherwise, the yaml content will be returned.
+            Serialized version of object.
+            `None` in case when `uri` provided.
         """
-        yaml_string = yaml.dump(self.to_dict(), Dumper=dumper)
+        note = kwargs.pop("note", "")
+
+        yaml_string = f"{note}\n" + yaml.dump(self.to_dict(**kwargs), Dumper=dumper)
         if uri:
             self._write_to_file(s=yaml_string, uri=uri, **kwargs)
             return None
 
         return yaml_string
 
     @classmethod
```

### Comparing `oracle_ads-2.8.3/ads/jobs/templates/driver_notebook.py` & `oracle_ads-2.8.4/ads/jobs/templates/driver_notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/templates/driver_oci.py` & `oracle_ads-2.8.4/ads/jobs/templates/driver_oci.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/templates/driver_python.py` & `oracle_ads-2.8.4/ads/jobs/templates/driver_python.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/templates/driver_utils.py` & `oracle_ads-2.8.4/ads/jobs/templates/driver_utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/jobs/utils.py` & `oracle_ads-2.8.4/ads/jobs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 
 import os
 import json
 
 from oci.data_flow.models import Application
@@ -39,15 +39,15 @@
                 f"Dataflow configuration with profile {oci_profile} not found."
             )
             raise ValueError(
                 f"Dataflow configuration with profile {oci_profile} not found."
             )
         return config
     else:
-        logger.error(f"{dataflow_config_file_path} not found.")
+        logger.warning(f"{dataflow_config_file_path} not found. Follow this link https://accelerated-data-science.readthedocs.io/en/latest/user_guide/apachespark/dataflow.html to set up the config.")
         return {}
 
 
 class DataFlowConfig(Application):
     def __init__(self, path: str = None, oci_profile: str = None):
         """Create a DataFlowConfig object. If a path to config file is given it is loaded from the path.
```

### Comparing `oracle_ads-2.8.3/ads/model/__init__.py` & `oracle_ads-2.8.4/ads/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/artifact.py` & `oracle_ads-2.8.4/ads/model/artifact.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,46 +7,48 @@
 import fnmatch
 import importlib
 import os
 import sys
 import shutil
 import tempfile
 import uuid
+import fsspec
 from typing import Dict, Optional, Tuple
 from ads.common import auth as authutil
 from ads.common import logger, utils
+from ads.common.object_storage_details import ObjectStorageDetails
 from ads.config import CONDA_BUCKET_NAME, CONDA_BUCKET_NS
 from ads.model.runtime.env_info import EnvInfo, InferenceEnvInfo, TrainingEnvInfo
 from ads.model.runtime.runtime_info import RuntimeInfo
 from jinja2 import Environment, PackageLoader
 import warnings
 from ads import __version__
 from datetime import datetime
 
 MODEL_ARTIFACT_VERSION = "3.0"
 REQUIRED_ARTIFACT_FILES = ("runtime.yaml", "score.py")
 SCORE_VERSION = "1.0"
 ADS_VERSION = __version__
 
 
-class ArtifactNestedFolderError(Exception):
+class ArtifactNestedFolderError(Exception):   # pragma: no cover
     def __init__(self, folder: str):
         self.folder = folder
         super().__init__("The required artifact files placed in a nested folder.")
 
 
-class ArtifactRequiredFilesError(Exception):
+class ArtifactRequiredFilesError(Exception):   # pragma: no cover
     def __init__(self, required_files: Tuple[str]):
         super().__init__(
             "Not all required files presented in artifact folder. "
             f"Required files for conda runtime: {required_files}. If you are using container runtime, set `ignore_conda_error=True`."
         )
 
 
-class AritfactFolderStructureError(Exception):
+class AritfactFolderStructureError(Exception):   # pragma: no cover
     def __init__(self, required_files: Tuple[str]):
         super().__init__(
             "The artifact folder has a wrong structure. "
             f"Required files: {required_files}"
         )
 
 
@@ -112,46 +114,67 @@
 
     def __init__(
         self,
         artifact_dir: str,
         model_file_name: str = None,
         reload: Optional[bool] = False,
         ignore_conda_error: Optional[bool] = False,
+        local_copy_dir: str = None,
+        auth: dict = None,
     ):
         """Initializes a ModelArtifact instance.
 
         Parameters
         ----------
         artifact_dir: str
-            The local artifact folder to store the files needed for deployment.
+            The artifact folder to store the files needed for deployment.
         model_file_name: (str, optional). Defaults to `None`.
             The file name of the serialized model.
         reload: (bool, optional). Defaults to False.
             Determine whether will reload the Model into the env.
+        ignore_conda_error: (bool, optional). Defaults to False.
+            Parameter to ignore error when collecting conda information.
+        local_copy_dir: (str, optional). Defaults to None.
+            The local back up directory of the model artifacts.
+        auth :(Dict, optional). Defaults to None.
+            The default authetication is set using `ads.set_auth` API. If you need to override the
+            default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
+            authentication signer and kwargs required to instantiate IdentityClient object.
 
         Returns
         -------
         ModelArtifact
             A ModelArtifact instance.
 
         Raises
         ------
         ValueError
             If `artifact_dir` not provided.
         """
         if not artifact_dir:
             raise ValueError("The `artifact_dir` needs to be provided.")
 
+        self.artifact_dir = (
+            artifact_dir
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else os.path.abspath(os.path.expanduser(artifact_dir))
+        )
+        self.local_copy_dir = (
+            local_copy_dir or tempfile.mkdtemp()
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else artifact_dir
+        )
+
         self.score = None
-        self.artifact_dir = os.path.abspath(os.path.expanduser(artifact_dir))
         sys.path.insert(0, self.artifact_dir)
         self.model_file_name = model_file_name
         self._env = Environment(loader=PackageLoader("ads", "templates"))
         self.ignore_conda_error = ignore_conda_error
         self.model = None
+        self.auth = auth or authutil.default_signer()
         if reload and not ignore_conda_error:
             self.reload()
             # Extracts the model_file_name from the score.py.
             if (
                 not self.model_file_name
                 and self.score
                 and hasattr(self.score, "model_name")
@@ -211,15 +234,15 @@
         """
         runtime_info = RuntimeInfo.from_env()
         runtime_info.model_artifact_version = MODEL_ARTIFACT_VERSION
         if ignore_conda_error:
             runtime_info.model_provenance.training_code.artifact_directory = (
                 self.artifact_dir
             )
-            runtime_info.save()
+            runtime_info.save(storage_options=auth)
             return runtime_info
         inference_conda_env = ModelArtifact._populate_env_info(
             InferenceEnvInfo,
             conda_pack=inference_conda_env,
             bucketname=bucketname,
             namespace=namespace,
             auth=auth,
@@ -255,15 +278,15 @@
         runtime_file_path = os.path.join(self.artifact_dir, "runtime.yaml")
         if os.path.exists(runtime_file_path) and not force_overwrite:
             raise ValueError(
                 "runtime.yaml already exists. "
                 "Set `force_overwrite` to True to overwrite all the files."
             )
         else:
-            runtime_info.save()
+            runtime_info.save(storage_options=auth)
         return runtime_info
 
     @staticmethod
     def _populate_env_info(
         clss: EnvInfo,
         conda_pack: str,
         bucketname: str = None,
@@ -341,36 +364,49 @@
 
         context = {
             "model_file_name": self.model_file_name,
             "SCORE_VERSION": SCORE_VERSION,
             "ADS_VERSION": ADS_VERSION,
             "time_created": time_suffix,
         }
+        storage_options = kwargs.pop("auth", {})
+        storage_options = storage_options if storage_options else {}
         context.update(kwargs)
-        with open(os.path.join(self.artifact_dir, "score.py"), "w") as sfl:
-            sfl.write(scorefn_template.render(context))
+        with fsspec.open(
+            os.path.join(self.artifact_dir, "score.py"), "w", **storage_options
+        ) as f:
+            f.write(scorefn_template.render(context))
 
     def reload(self):
         """Syncs the `score.py` to reload the model and predict function.
 
         Returns
         -------
         None
             Nothing
+
         """
+        if ObjectStorageDetails.is_oci_path(self.artifact_dir):
+            utils.copy_from_uri(
+                uri=self.artifact_dir,
+                to_path=self.local_copy_dir,
+                force_overwrite=True,
+                auth=self.auth,
+            )
+
         spec = importlib.util.spec_from_file_location(
-            "score%s" % uuid.uuid4(), os.path.join(self.artifact_dir, "score.py")
+            "score%s" % uuid.uuid4(), os.path.join(self.local_copy_dir, "score.py")
         )
         self.score = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(self.score)
         self.model = self.score.load_model()  # load model in cache
         # remove the cache files.
         for dir in [
-            os.path.join(self.artifact_dir, "__pycache__"),
-            os.path.join(self.artifact_dir, ".ipynb_checkpoints"),
+            os.path.join(self.local_copy_dir, "__pycache__"),
+            os.path.join(self.local_copy_dir, ".ipynb_checkpoints"),
         ]:
             if os.path.exists(dir):
                 shutil.rmtree(dir, ignore_errors=True)
 
     @classmethod
     def from_uri(
         cls,
@@ -406,50 +442,79 @@
         ModelArtifact
             A `ModelArtifact` instance
 
         Raises
         ------
         ValueError
             If `uri` is equal to `artifact_dir`, and it not exists.
+            If `artifact_dir` is not provided.
         """
-        artifact_dir = os.path.join(
-            os.path.abspath(os.path.expanduser(artifact_dir)), ""
+        if not artifact_dir:
+            raise ValueError("The `artifact_dir` needs to be provided.")
+
+        artifact_dir = (
+            artifact_dir
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else os.path.join(os.path.abspath(os.path.expanduser(artifact_dir)), "")
         )
 
-        if artifact_dir == os.path.join(
-            os.path.abspath(os.path.expanduser(uri)).rstrip("/"), ""
-        ):
-            if not os.path.exists(artifact_dir):
+        if not ObjectStorageDetails.is_oci_path(uri):
+            uri = os.path.join(os.path.abspath(os.path.expanduser(uri)).rstrip("/"), "")
+        auth = auth or authutil.default_signer()
+
+        to_path = (
+            tempfile.mkdtemp()
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else artifact_dir
+        )
+        force_overwrite = (
+            True if ObjectStorageDetails.is_oci_path(artifact_dir) else force_overwrite
+        )
+        if artifact_dir == uri and not ObjectStorageDetails.is_oci_path(artifact_dir):
+            if not utils.is_path_exists(artifact_dir, auth=auth):
                 raise ValueError("Provided `uri` doesn't exist.")
         else:
-            auth = auth or authutil.default_signer()
             utils.copy_from_uri(
                 uri=uri,
-                to_path=artifact_dir,
+                to_path=to_path,
                 unpack=True,
                 force_overwrite=force_overwrite,
                 auth=auth,
             )
+
         if not ignore_conda_error:
             try:
-                _validate_artifact_dir(artifact_dir)
+                _validate_artifact_dir(to_path)
             except ArtifactNestedFolderError as exc:
                 with tempfile.TemporaryDirectory() as temp_dir:
                     utils.copy_from_uri(
                         uri=exc.folder, to_path=temp_dir, force_overwrite=True
                     )
                     utils.copy_from_uri(
-                        uri=temp_dir, to_path=artifact_dir, force_overwrite=True
+                        uri=temp_dir, to_path=to_path, force_overwrite=True
+                    )
+
+        if ObjectStorageDetails.is_oci_path(artifact_dir):
+            for root, dirs, files in os.walk(to_path):
+                prefix = (os.path.abspath(root).split(to_path)[-1]).lstrip("/")
+                for file in files:
+                    path = os.path.join(prefix, file)
+                    utils.copy_file(
+                        uri_src=os.path.join(root, file),
+                        uri_dst=os.path.join(artifact_dir, path),
+                        force_overwrite=True,
+                        auth=auth,
                     )
 
         return cls(
-            artifact_dir,
-            model_file_name,
+            artifact_dir=artifact_dir,
+            model_file_name=model_file_name,
             reload=True,
             ignore_conda_error=ignore_conda_error,
+            local_copy_dir=to_path,
         )
 
     def __getattr__(self, item):
         """Makes the functions in `score.py` directly accessable by ModelArtifact class."""
 
         try:
             return getattr(self.score, item)
```

### Comparing `oracle_ads-2.8.3/ads/model/artifact_downloader.py` & `oracle_ads-2.8.4/ads/model/artifact_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         None
 
         Raises
         ------
         ValueError
             If target directory does not exist.
         """
-        if os.path.exists(self.target_dir):
+        if os.path.exists(self.target_dir) and len(os.listdir(self.target_dir)) > 0:
             if not self.force_overwrite:
                 raise ValueError(
                     f"The `{self.target_dir}` directory already exists. "
                     "Set `force_overwrite` to `True` if you wish to overwrite."
                 )
             shutil.rmtree(self.target_dir)
         with utils.get_progress_bar(
```

### Comparing `oracle_ads-2.8.3/ads/model/artifact_uploader.py` & `oracle_ads-2.8.4/ads/model/artifact_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/common/.model-ignore` & `oracle_ads-2.8.4/ads/model/common/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/common/utils.py` & `oracle_ads-2.8.4/ads/model/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import json
 import os
 import tempfile
+import yaml
 from typing import Any, Dict, Optional
 from zipfile import ZipFile
-
-import yaml
-
 from ads.common import utils
 
 
 DEPRECATE_AS_ONNX_WARNING = "This attribute `as_onnx` will be deprecated in the future. You can choose specific format by setting `model_save_serializer`."
 DEPRECATE_USE_TORCH_SCRIPT_WARNING = "This attribute `use_torch_script` will be deprecated in the future. You can choose specific format by setting `model_save_serializer`."
```

### Comparing `oracle_ads-2.8.3/ads/model/datascience_model.py` & `oracle_ads-2.8.4/ads/model/datascience_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 _MAX_ARTIFACT_SIZE_IN_BYTES = 2147483648  # 2GB
 
 
-class ModelArtifactSizeError(Exception):
+class ModelArtifactSizeError(Exception):   # pragma: no cover
     def __init__(self, max_artifact_size: str):
         super().__init__(
             f"The model artifacts size is greater than `{max_artifact_size}`. "
             "The `bucket_uri` needs to be specified to "
             "copy artifacts to the object storage bucket. "
             "Example: `bucket_uri=oci://<bucket_name>@<namespace>/prefix/`"
         )
```

### Comparing `oracle_ads-2.8.3/ads/model/deployment/__init__.py` & `oracle_ads-2.8.4/ads/model/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/deployment/common/utils.py` & `oracle_ads-2.8.4/ads/model/deployment/common/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,36 +115,31 @@
         dry_run (bool, optional): Defaults to False.
         is_json_payload (bool, optional): Indicate whether to send data with a `application/json` MIME TYPE. Defaults to False.
         header (dict, optional): A dictionary of HTTP headers to send to the specified url. Defaults to {}.
 
     Returns:
         A JSON representive of a requests.Response object.
     """
-    headers = dict()
     if is_json_payload:
-        headers["Content-Type"] = (
-            header.get("content_type") or DEFAULT_CONTENT_TYPE_JSON
-        )
+        header["Content-Type"] =  header.pop("content_type", DEFAULT_CONTENT_TYPE_JSON) or DEFAULT_CONTENT_TYPE_JSON
         request_kwargs = {"json": data}
     else:
-        headers["Content-Type"] = (
-            header.get("content_type") or DEFAULT_CONTENT_TYPE_BYTES
-        )
+        header["Content-Type"] = header.pop("content_type", DEFAULT_CONTENT_TYPE_BYTES) or DEFAULT_CONTENT_TYPE_BYTES
         request_kwargs = {"data": data}  # should pass bytes when using data
-
-    request_kwargs["headers"] = headers
+    
+    request_kwargs["headers"] = header
 
     if dry_run:
         request_kwargs["headers"]["Accept"] = "*/*"
         req = requests.Request("POST", endpoint, **request_kwargs).prepare()
         if is_json_payload:
             return json.loads(req.body)
         return req.body
     else:
-        request_kwargs["auth"] = header.get("signer")
+        request_kwargs["auth"] = header.pop("signer")
         return requests.post(endpoint, **request_kwargs).json()
 
 
 # State Constants
 class State(Enum):
     ACTIVE = auto()
     CREATING = auto()
```

### Comparing `oracle_ads-2.8.3/ads/model/deployment/model_deployer.py` & `oracle_ads-2.8.4/ads/model/deployment/model_deployer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/deployment/model_deployment.py` & `oracle_ads-2.8.4/ads/model/deployment/model_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import time
 from typing import Dict, List, Union, Any
 
 import oci.loggingsearch
 from ads.common import auth as authutil
 import pandas as pd
 from ads.model.serde.model_input import JsonModelInputSERDE
-from ads.common import auth, oci_client
 from ads.common.oci_logging import (
     LOG_INTERVAL,
     LOG_RECORDS_LIMIT,
     ConsolidatedLog,
     OCILog,
 )
 from ads.config import COMPARTMENT_OCID, PROJECT_OCID
@@ -59,14 +58,15 @@
 DELETE_WORKFLOW_STEPS = 2
 DEACTIVATE_WORKFLOW_STEPS = 2
 DEFAULT_RETRYING_REQUEST_ATTEMPTS = 3
 TERMINAL_STATES = [State.ACTIVE, State.FAILED, State.DELETED, State.INACTIVE]
 
 MODEL_DEPLOYMENT_KIND = "deployment"
 MODEL_DEPLOYMENT_TYPE = "modelDeployment"
+MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON = "TRITON"
 
 MODEL_DEPLOYMENT_INSTANCE_SHAPE = "VM.Standard.E4.Flex"
 MODEL_DEPLOYMENT_INSTANCE_OCPUS = 1
 MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS = 16
 MODEL_DEPLOYMENT_INSTANCE_COUNT = 1
 MODEL_DEPLOYMENT_BANDWIDTH_MBPS = 10
 
@@ -77,19 +77,19 @@
 
 
 class ModelDeploymentMode:
     HTTPS = "HTTPS_ONLY"
     STREAM = "STREAM_ONLY"
 
 
-class LogNotConfiguredError(Exception):
+class LogNotConfiguredError(Exception):  # pragma: no cover
     pass
 
 
-class ModelDeploymentFailedError(Exception):
+class ModelDeploymentFailedError(Exception):  # pragma: no cover
     pass
 
 
 class ModelDeployment(Builder):
     """
     A class used to represent a Model Deployment.
 
@@ -824,14 +824,16 @@
 
     def predict(
         self,
         json_input=None,
         data: Any = None,
         serializer: "ads.model.ModelInputSerializer" = model_input_serializer,
         auto_serialize_data: bool = False,
+        model_name: str = None,
+        model_version: str = None,
         **kwargs,
     ) -> dict:
         """Returns prediction of input data run against the model deployment endpoint.
 
         Examples
         --------
         >>> import numpy as np
@@ -856,14 +858,18 @@
         serializer: ads.model.ModelInputSerializer
             Defaults to ads.model.JsonModelInputSerializer.
         auto_serialize_data: bool
             Defaults to False. Indicate whether to auto serialize input data using `serializer`.
             If `auto_serialize_data=False`, `data` required to be bytes or json serializable
             and `json_input` required to be json serializable. If `auto_serialize_data` set
             to True, data will be serialized before sending to model deployment endpoint.
+        model_name: str
+            Defaults to None. When the `inference_server="triton"`, the name of the model to invoke.
+        model_version: str
+            Defaults to None. When the `inference_server="triton"`, the version of the model to invoke.
         kwargs:
             content_type: str
                 Used to indicate the media type of the resource.
                 By default, it will be `application/octet-stream` for bytes input and `application/json` otherwise.
                 The content-type header will be set to this value when calling the model deployment endpoint.
 
         Returns
@@ -874,14 +880,15 @@
         """
         endpoint = f"{self.url}/predict"
         signer = authutil.default_signer()["signer"]
         header = {
             "signer": signer,
             "content_type": kwargs.get("content_type", None),
         }
+        header.update(kwargs.pop("headers", {}))
 
         if data is None and json_input is None:
             raise AttributeError(
                 "Neither `data` nor `json_input` are provided. You need to provide one of them."
             )
         if data is not None and json_input is not None:
             raise AttributeError(
@@ -912,17 +919,26 @@
             data = json_input
 
         is_json_payload = _is_json_serializable(data)
         if not isinstance(data, bytes) and not is_json_payload:
             raise TypeError(
                 "`data` is not bytes or json serializable. Set `auto_serialize_data` to `True` to serialize the input data."
             )
-
+        if model_name and model_version:
+            header["model-name"] = model_name
+            header["model-version"] = model_version
+        elif bool(model_version) ^ bool(model_name):
+            raise ValueError(
+                "`model_name` and `model_version` have to be provided together."
+            )
         prediction = send_request(
-            data=data, endpoint=endpoint, is_json_payload=is_json_payload, header=header
+            data=data,
+            endpoint=endpoint,
+            is_json_payload=is_json_payload,
+            header=header,
         )
         return prediction
 
     def activate(
         self,
         wait_for_completion: bool = True,
         max_wait_time: int = DEFAULT_WAIT_TIME,
@@ -1319,15 +1335,15 @@
                     key, mapping[child_config.get("type")].from_dict(child_config)
                 )
             else:
                 model_deployment.set_spec(key, value)
 
         return model_deployment
 
-    def to_dict(self) -> Dict:
+    def to_dict(self, **kwargs) -> Dict:
         """Serializes model deployment to a dictionary.
 
         Returns
         -------
         dict
             The model deployment serialized as a dictionary.
         """
@@ -1386,14 +1402,22 @@
         )
 
         self._extract_from_oci_model(runtime, oci_model_instance)
         infrastructure.set_spec(
             infrastructure.CONST_WEB_CONCURRENCY,
             runtime.env.get("WEB_CONCURRENCY", None),
         )
+        if (
+            runtime.env.get("CONTAINER_TYPE", None)
+            == MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
+        ):
+            runtime.set_spec(
+                runtime.CONST_INFERENCE_SERVER,
+                MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON.lower(),
+            )
 
         self.set_spec(self.CONST_INFRASTRUCTURE, infrastructure)
         self.set_spec(self.CONST_RUNTIME, runtime)
 
         return self
 
     @staticmethod
@@ -1513,17 +1537,23 @@
                 infrastructure.CONST_OCPUS: infrastructure.shape_config_details.get(
                     "ocpus", None
                 )
                 or MODEL_DEPLOYMENT_INSTANCE_OCPUS,
                 infrastructure.CONST_MEMORY_IN_GBS: infrastructure.shape_config_details.get(
                     "memory_in_gbs", None
                 )
+                or infrastructure.shape_config_details.get(
+                    "memoryInGBs", None
+                )
                 or MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS,
             }
 
+        if infrastructure.subnet_id:
+            instance_configuration[infrastructure.CONST_SUBNET_ID] = infrastructure.subnet_id
+
         scaling_policy = {
             infrastructure.CONST_POLICY_TYPE: "FIXED_SIZE",
             infrastructure.CONST_INSTANCE_COUNT: infrastructure.replica
             or MODEL_DEPLOYMENT_INSTANCE_COUNT,
         }
 
         if not runtime.model_uri:
@@ -1562,14 +1592,24 @@
 
         environment_variables = runtime.env
         if infrastructure.web_concurrency:
             environment_variables["WEB_CONCURRENCY"] = str(
                 infrastructure.web_concurrency
             )
             runtime.set_spec(runtime.CONST_ENV, environment_variables)
+        if (
+            hasattr(runtime, "inference_server")
+            and runtime.inference_server
+            and runtime.inference_server.upper()
+            == MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
+        ):
+            environment_variables[
+                "CONTAINER_TYPE"
+            ] = MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
+            runtime.set_spec(runtime.CONST_ENV, environment_variables)
         environment_configuration_details = {
             runtime.CONST_ENVIRONMENT_CONFIG_TYPE: runtime.environment_config_type,
             runtime.CONST_ENVIRONMENT_VARIABLES: runtime.env,
         }
 
         if runtime.environment_config_type == OCIModelDeploymentRuntimeType.CONTAINER:
             if not hasattr(
@@ -1665,7 +1705,16 @@
             Dict contains model deployment spec related keyword arguments.
         """
         spec_kwargs = {}
         for attribute in self.initialize_spec_attributes:
             if attribute in kwargs:
                 spec_kwargs[attribute] = kwargs[attribute]
         return spec_kwargs
+
+    def build(self) -> "ModelDeployment":
+        """Load default values from the environment for the job infrastructure."""
+        build_method = getattr(self.infrastructure, "build", None)
+        if build_method and callable(build_method):
+            build_method()
+        else:
+            raise NotImplementedError
+        return self
```

### Comparing `oracle_ads-2.8.3/ads/model/deployment/model_deployment_infrastructure.py` & `oracle_ads-2.8.4/ads/model/deployment/model_deployment_infrastructure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/from typing import Dict
 
 
+import copy
+import logging
+import traceback
 from typing import Any, Dict
+
+import oci.util as oci_util
+
+from ads.common.oci_datascience import DSCNotebookSession
+from ads.config import COMPARTMENT_OCID, NB_SESSION_OCID, PROJECT_OCID
 from ads.jobs.builders.base import Builder
 
 MODEL_DEPLOYMENT_INFRASTRUCTURE_TYPE = "datascienceModelDeployment"
 MODEL_DEPLOYMENT_INFRASTRUCTURE_KIND = "infrastructure"
 
+DEFAULT_BANDWIDTH_MBPS = 10
+DEFAULT_WEB_CONCURRENCY = 10
+DEFAULT_REPLICA = 1
+DEFAULT_SHAPE_NAME = "VM.Standard.E2.4"
+
+logger = logging.getLogger(__name__)
+
 
 class ModelDeploymentInfrastructure(Builder):
     """A class used to represent a Model Deployment Infrastructure.
 
     Attributes
     ----------
     compartment_id: str
@@ -35,14 +50,16 @@
         The predict log of model deployment
     log_group_id: str
         The access and predict log group id of model deployment
     log_id: str
         The access and predict log id of model deployment
     web_concurrency: int
         The web concurrency of model deployment
+    subnet_id: str
+        The subnet id of model deployment
 
     Methods
     -------
     with_compartment_id(compartment_id)
         Sets the compartment id of model deployment
     with_project_id(project_id)
         Sets the project id of model deployment
@@ -60,14 +77,16 @@
         Sets the predict log of model deployment
     with_log_group_id(log_group_id)
         Sets the access and predict log group id of model deployment
     with_log_id(log_id)
         Sets the access and predict log id of model deployment
     with_web_concurrency(web_concurrency)
         Sets the web concurrency of model deployment
+    with_subnet_id(subnet_id)
+        Sets the subnet id of model deployment
 
     Example
     -------
     Build infrastructure from builder apis:
     >>> infrastructure = ModelDeploymentInfrastructure()
     ...        .with_project_id(<project_id>)
     ...        .with_compartment_id(<compartment_id>)
@@ -75,14 +94,15 @@
     ...        .with_shape_config_details(
     ...            ocpus=1,
     ...            memory_in_gbs=16
     ...        )
     ...        .with_replica(1)
     ...        .with_bandwidth_mbps(10)
     ...        .with_web_concurrency(10)
+    ...        .with_subnet_id(<subnet_id>)
     ...        .with_access_log(
     ...            log_group_id=<log_group_id>,
     ...            log_id=<log_id>
     ...        )
     ...        .with_predict_log(
     ...            log_group_id=<log_group_id>,
     ...            log_id=<log_id>
@@ -117,14 +137,15 @@
     CONST_ACCESS = "access"
     CONST_PREDICT_LOG = "predictLog"
     CONST_PREDICT = "predict"
     CONST_LOG_ID = "logId"
     CONST_LOG_GROUP_ID = "logGroupId"
     CONST_WEB_CONCURRENCY = "webConcurrency"
     CONST_STREAM_CONFIG_DETAILS = "streamConfigurationDetails"
+    CONST_SUBNET_ID = "subnetId"
 
     attribute_map = {
         CONST_PROJECT_ID: "project_id",
         CONST_COMPARTMENT_ID: "compartment_id",
         CONST_SHAPE_NAME: "shape_name",
         CONST_SHAPE_CONFIG_DETAILS: "shape_config_details",
         CONST_OCPUS: "ocpus",
@@ -132,14 +153,15 @@
         CONST_REPLICA: "replica",
         CONST_BANDWIDTH_MBPS: "bandwidth_mbps",
         CONST_ACCESS_LOG: "access_log",
         CONST_PREDICT_LOG: "predict_log",
         CONST_LOG_ID: "log_id",
         CONST_LOG_GROUP_ID: "log_group_id",
         CONST_WEB_CONCURRENCY: "web_concurrency",
+        CONST_SUBNET_ID: "subnet_id",
     }
 
     shape_config_details_attribute_map = {
         CONST_MEMORY_IN_GBS: "memory_in_gbs",
         CONST_OCPUS: "ocpus",
     }
 
@@ -158,14 +180,15 @@
     )
 
     payload_attribute_map = {
         CONST_PROJECT_ID: "project_id",
         CONST_COMPARTMENT_ID: "compartment_id",
         CONST_SHAPE_NAME: f"{MODEL_CONFIG_DETAILS_PATH}.instance_configuration.instance_shape_name",
         CONST_SHAPE_CONFIG_DETAILS: f"{MODEL_CONFIG_DETAILS_PATH}.instance_configuration.model_deployment_instance_shape_config_details",
+        CONST_SUBNET_ID: f"{MODEL_CONFIG_DETAILS_PATH}.instance_configuration.subnet_id",
         CONST_REPLICA: f"{MODEL_CONFIG_DETAILS_PATH}.scaling_policy.instance_count",
         CONST_BANDWIDTH_MBPS: f"{MODEL_CONFIG_DETAILS_PATH}.bandwidth_mbps",
         CONST_ACCESS_LOG: "category_log_details.access",
         CONST_PREDICT_LOG: "category_log_details.predict",
         CONST_DEPLOYMENT_TYPE: "model_deployment_configuration_details.deployment_type",
         CONST_POLICY_TYPE: f"{MODEL_CONFIG_DETAILS_PATH}.scaling_policy.policy_type",
     }
@@ -175,14 +198,55 @@
         CONST_ACCESS_LOG: access_log_attribute_map,
         CONST_PREDICT_LOG: predict_log_attribute_map,
     }
 
     def __init__(self, spec: Dict = None, **kwargs) -> None:
         super().__init__(spec, **kwargs)
 
+    def _load_default_properties(self) -> Dict:
+        """Load default properties from environment variables, notebook session, etc.
+
+        Returns
+        -------
+        Dict
+            A dictionary of default properties.
+        """
+        defaults = super()._load_default_properties()
+        if COMPARTMENT_OCID:
+            defaults[self.CONST_COMPARTMENT_ID] = COMPARTMENT_OCID
+        if PROJECT_OCID:
+            defaults[self.CONST_PROJECT_ID] = PROJECT_OCID
+
+        defaults[self.CONST_BANDWIDTH_MBPS] = DEFAULT_BANDWIDTH_MBPS
+        defaults[self.CONST_WEB_CONCURRENCY] = DEFAULT_WEB_CONCURRENCY
+        defaults[self.CONST_REPLICA] = DEFAULT_REPLICA
+
+        if NB_SESSION_OCID:
+            try:
+                nb_session = DSCNotebookSession.from_ocid(NB_SESSION_OCID)
+                nb_config = nb_session.notebook_session_configuration_details
+                defaults[self.CONST_SHAPE_NAME] = nb_config.shape
+
+                if nb_config.notebook_session_shape_config_details:
+                    notebook_shape_config_details = oci_util.to_dict(
+                        nb_config.notebook_session_shape_config_details
+                    )
+                    defaults[self.CONST_SHAPE_CONFIG_DETAILS] = copy.deepcopy(
+                        notebook_shape_config_details
+                    )
+
+            except Exception as e:
+                logger.warning(
+                    f"Error fetching details about Notebook "
+                    f"session: {NB_SESSION_OCID}. {e}"
+                )
+                logger.debug(traceback.format_exc())
+
+        return defaults
+
     @property
     def kind(self) -> str:
         """The kind of the object as showing in YAML.
 
         Returns
         -------
         str
@@ -514,7 +578,51 @@
 
         Returns
         -------
         ModelDeploymentInfrastructure
             The ModelDeploymentInfrastructure instance (self).
         """
         return self.set_spec(self.CONST_WEB_CONCURRENCY, web_concurrency)
+
+    def with_subnet_id(self, subnet_id: str) -> "ModelDeploymentInfrastructure":
+        """Sets the subnet id of model deployment.
+
+        Parameters
+        ----------
+        subnet_id : str
+            The subnet id of model deployment.
+
+        Returns
+        -------
+        ModelDeploymentInfrastructure
+            The ModelDeploymentInfrastructure instance (self).
+        """
+        return self.set_spec(self.CONST_SUBNET_ID, subnet_id)
+
+    @property
+    def subnet_id(self) -> str:
+        """The model deployment subnet id.
+
+        Returns
+        -------
+        str
+            The model deployment subnet id.
+        """
+        return self.get_spec(self.CONST_SUBNET_ID, None)
+
+    def init(self) -> "ModelDeploymentInfrastructure":
+        """Initializes a starter specification for the ModelDeploymentInfrastructure.
+
+        Returns
+        -------
+        ModelDeploymentInfrastructure
+            The ModelDeploymentInfrastructure instance (self)
+        """
+        return (
+            self.build()
+            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
+            .with_project_id(self.project_id or "{Provide a project OCID}")
+            .with_bandwidth_mbps(self.bandwidth_mbps or DEFAULT_BANDWIDTH_MBPS)
+            .with_web_concurrency(self.web_concurrency or DEFAULT_WEB_CONCURRENCY)
+            .with_replica(self.replica or DEFAULT_REPLICA)
+            .with_shape_name(self.shape_name or DEFAULT_SHAPE_NAME)
+        )
```

### Comparing `oracle_ads-2.8.3/ads/model/deployment/model_deployment_properties.py` & `oracle_ads-2.8.4/ads/model/deployment/model_deployment_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/deployment/model_deployment_runtime.py` & `oracle_ads-2.8.4/ads/model/deployment/model_deployment_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -233,14 +233,28 @@
         Returns
         -------
         ModelDeploymentRuntime
             The ModelDeploymentRuntime instance (self).
         """
         return self.set_spec(self.CONST_MODEL_URI, model_uri)
 
+    def init(self) -> "ModelDeploymentRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        Self
+            This method returns self to support chaining methods.
+        """
+        return (
+            self.with_env({"key": "value"})
+            .with_deployment_mode("HTTPS_ONLY")
+            .with_model_uri("<MODEL_URI>")
+        )
+
 
 class ModelDeploymentCondaRuntime(ModelDeploymentRuntime):
     """A class used to represent a Model Deployment Conda Runtime.
 
     Examples
     --------
     >>> conda_runtime = ModelDeploymentCondaRuntime()
@@ -268,14 +282,24 @@
         Returns
         -------
         str
             DEFAULT
         """
         return OCIModelDeploymentRuntimeType.CONDA
 
+    def init(self) -> "ModelDeploymentCondaRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        CondaRuntime
+            The runtime instance.
+        """
+        return super().init()
+
 
 class ModelDeploymentContainerRuntime(ModelDeploymentRuntime):
     """A class used to represent a Model Deployment Container Runtime.
 
     Attributes
     ----------
     image: str
@@ -326,23 +350,25 @@
 
     CONST_IMAGE = "image"
     CONST_IMAGE_DIGEST = "imageDigest"
     CONST_CMD = "cmd"
     CONST_ENTRYPOINT = "entrypoint"
     CONST_SERVER_PORT = "serverPort"
     CONST_HEALTH_CHECK_PORT = "healthCheckPort"
+    CONST_INFERENCE_SERVER = "inferenceServer"
 
     attribute_map = {
         **ModelDeploymentRuntime.attribute_map,
         CONST_IMAGE: "image",
         CONST_IMAGE_DIGEST: "image_digest",
         CONST_CMD: "cmd",
         CONST_ENTRYPOINT: "entrypoint",
         CONST_SERVER_PORT: "server_port",
         CONST_HEALTH_CHECK_PORT: "health_check_port",
+        CONST_INFERENCE_SERVER: "inference_server",
     }
 
     payload_attribute_map = {
         **ModelDeploymentRuntime.payload_attribute_map,
         CONST_IMAGE: f"{ModelDeploymentRuntime.ENVIRONMENT_CONFIG_DETAILS_PATH}.image",
         CONST_IMAGE_DIGEST: f"{ModelDeploymentRuntime.ENVIRONMENT_CONFIG_DETAILS_PATH}.image_digest",
         CONST_CMD: f"{ModelDeploymentRuntime.ENVIRONMENT_CONFIG_DETAILS_PATH}.cmd",
@@ -528,7 +554,80 @@
 
         Returns
         -------
         ModelDeploymentContainerRuntime
             The ModelDeploymentContainerRuntime instance (self).
         """
         return self.set_spec(self.CONST_HEALTH_CHECK_PORT, health_check_port)
+
+    @property
+    def inference_server(self) -> str:
+        """Returns the inference server.
+
+        Returns
+        -------
+        str
+            The inference server.
+        """
+        return self.get_spec(self.CONST_INFERENCE_SERVER, None)
+
+    def with_inference_server(
+        self, inference_server: str = "triton"
+    ) -> "ModelDeploymentRuntime":
+        """Sets the inference server. Current supported inference server is "triton".
+        Note if you are using byoc, you do not need to set the inference server.
+
+        Parameters
+        ----------
+        inference_server: str
+            Set the inference server.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+
+        Example
+        -------
+        >>> from ads.model.deployment import ModelDeployment, ModelDeploymentContainerRuntime, ModelDeploymentInfrastructure
+        >>> import ads
+        >>> ads.set_auth("resource_principal")
+        >>> infrastructure = ModelDeploymentInfrastructure()\
+        ...                 .with_project_id(<project_id>)\
+        ...                 .with_compartment_id(<comparment_id>)\
+        ...                 .with_shape_name("VM.Standard.E4.Flex")\
+        ...                 .with_replica(2)\
+        ...                 .with_bandwidth_mbps(10)\
+        ...                 .with_access_log(log_group_id=<deployment_log_group_id>, log_id=<deployment_access_log_id>)\
+        ...                 .with_predict_log(log_group_id=<deployment_log_group_id>, log_id=<deployment_predict_log_id>)
+
+        >>> runtime = ModelDeploymentContainerRuntime()\
+        ...                 .with_image(<container_image>)\
+        ...                 .with_server_port(<server_port>)\
+        ...                 .with_health_check_port(<health_check_port>)\
+        ...                 .with_model_uri(<model_id>)\
+        ...                 .with_env({"key":"value", "key2":"value2"})\
+        ...                 .with_inference_server("triton")
+        >>> deployment = ModelDeployment()\
+        ...                 .with_display_name("Triton Example")\
+        ...                 .with_infrastructure(infrastructure)\
+        ...                 .with_runtime(runtime)
+        >>> deployment.deploy()
+        """
+        return self.set_spec(self.CONST_INFERENCE_SERVER, inference_server.lower())
+
+    def init(self) -> "ModelDeploymentContainerRuntime":
+        """Initializes a starter specification for the runtime.
+
+        Returns
+        -------
+        CondaRuntime
+            The runtime instance.
+        """
+        super().init()
+        return (
+            self.with_image("iad.ocir.io/<namespace>/<image>:<tag>")
+            .with_image_digest("<IMAGE_DIGEST>")
+            .with_entrypoint(["python", "/opt/ds/model/deployed_model/api.py"])
+            .with_server_port(5000)
+            .with_health_check_port(5000)
+        )
```

### Comparing `oracle_ads-2.8.3/ads/model/extractor/automl_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/automl_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/huggingface_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/huggingface_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/keras_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/keras_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/lightgbm_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/lightgbm_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/model_info_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/model_info_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/model_info_extractor_factory.py` & `oracle_ads-2.8.4/ads/model/extractor/model_info_extractor_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/pytorch_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/pytorch_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/sklearn_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/sklearn_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/spark_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/spark_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/tensorflow_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/tensorflow_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/extractor/xgboost_extractor.py` & `oracle_ads-2.8.4/ads/model/extractor/xgboost_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/automl_model.py` & `oracle_ads-2.8.4/ads/model/framework/automl_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/huggingface_model.py` & `oracle_ads-2.8.4/ads/model/framework/huggingface_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/lightgbm_model.py` & `oracle_ads-2.8.4/ads/model/framework/lightgbm_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/pytorch_model.py` & `oracle_ads-2.8.4/ads/model/framework/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/sklearn_model.py` & `oracle_ads-2.8.4/ads/model/framework/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/spark_model.py` & `oracle_ads-2.8.4/ads/model/framework/spark_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import os
-from typing import Any, Callable, Dict, List, Optional, Union, Tuple
-
 import numpy as np
 import pandas as pd
-from ads.common import logger
+import fsspec
+from typing import Any, Callable, Dict, List, Optional, Union, Tuple
+from ads.common import logger, utils
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
+from ads.common.object_storage_details import ObjectStorageDetails
 from ads.model.extractor.spark_extractor import SparkExtractor
 from ads.model.serde.model_input import SparkModelInputSerializerType
 from ads.model.serde.model_serializer import SparkModelSerializerType
 from ads.model.generic_model import (
     FrameworkSpecificModel,
     DEFAULT_MODEL_FOLDER_NAME,
+    _prepare_artifact_dir,
 )
 from ads.model.model_properties import ModelProperties
 from ads.model.serde.common import SERDE
 
 SPARK_DATAFRAME_SCHEMA_PATH = "_input_data_schema.json"
 
 
@@ -148,15 +150,15 @@
         Initiates a SparkPipelineModel instance.
 
         Parameters
         ----------
         estimator: Callable
             SparkPipelineModel
         artifact_dir: str
-            Directory for generate artifact.
+            The URI for the generated artifact, which can be local path or OCI object storage URI.
         properties: (ModelProperties, optional). Defaults to None.
             ModelProperties object required to save and deploy model.
         auth :(Dict, optional). Defaults to None.
             The default authetication is set using `ads.set_auth` API. If you need to override the
             default, use the `ads.common.auth.api_keys` or `ads.common.auth.resource_principal` to create appropriate
             authentication signer and kwargs required to instantiate IdentityClient object.
         model_save_serializer: (SERDE or str, optional). Defaults to None.
@@ -204,31 +206,34 @@
             artifact_dir=artifact_dir,
             properties=properties,
             auth=auth,
             model_save_serializer=model_save_serializer,
             model_input_serializer=model_input_serializer,
             **kwargs,
         )
+
         self._extractor = SparkExtractor(estimator)
         self.framework = self._extractor.framework
         self.algorithm = self._extractor.algorithm
         self.version = self._extractor.version
         self.hyperparameter = self._extractor.hyperparameter
 
     @staticmethod
-    def _handle_model_file_name(as_onnx: bool, model_file_name: str):
+    def _handle_model_file_name(
+        as_onnx: bool, model_file_name: Optional[str] = DEFAULT_MODEL_FOLDER_NAME
+    ):
         """
         Process folder name for saving model.
 
         Parameters
         ----------
         as_onnx: bool
             To convert to onnx format
-        model_file_name: str
-            File name for saving model.
+        model_file_name: Optional[str]
+            File name for saving model. Default value is `model`.
 
         Returns
         -------
         str
             Processed file name. (Folder in the case of spark serialization)
         """
         if as_onnx:
@@ -303,14 +308,19 @@
             data_type,
             schema,
         ) = self.get_data_serializer()._serialize_via_spark(X_sample)
         if not schema:
             raise TypeError(
                 f"Data type: {data_type} unsupported. Please use `pyspark.sql.DataFrame`, `pyspark.pandas.DataFrame`, or `pandas.DataFrame`."
             )
-        with open(input_schema_path, "w") as f:
+        storage_options = kwargs.get("auth", {})
+        with fsspec.open(
+            input_schema_path,
+            mode="w",
+            **(storage_options),
+        ) as f:
             f.write(schema.json())
 
         if isinstance(X_sample, sql.DataFrame):
             X_sample = X_sample.toPandas()
 
         return X_sample, y_sample
```

### Comparing `oracle_ads-2.8.3/ads/model/framework/tensorflow_model.py` & `oracle_ads-2.8.4/ads/model/framework/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/framework/xgboost_model.py` & `oracle_ads-2.8.4/ads/model/framework/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/generic_model.py` & `oracle_ads-2.8.4/ads/model/generic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import yaml
 from PIL import Image
 
 from ads.common import auth as authutil
 from ads.common import logger, utils
 from ads.common.decorator.utils import class_or_instance_method
 from ads.common.utils import DATA_SCHEMA_MAX_COL_NUM, get_files
+from ads.common.object_storage_details import ObjectStorageDetails
 from ads.config import (
     CONDA_BUCKET_NS,
     JOB_RUN_COMPARTMENT_OCID,
     JOB_RUN_OCID,
     NB_SESSION_COMPARTMENT_OCID,
     NB_SESSION_OCID,
     PROJECT_OCID,
@@ -131,32 +132,32 @@
 
 
 class DataScienceModelType(str, metaclass=ExtendedEnumMeta):
     MODEL_DEPLOYMENT = "datasciencemodeldeployment"
     MODEL = "datasciencemodel"
 
 
-class NotActiveDeploymentError(Exception):
+class NotActiveDeploymentError(Exception):   # pragma: no cover
     def __init__(self, state: str):
         msg = (
             "To perform a prediction the deployed model needs to be in an active state. "
             f"The current state is: {state}."
         )
         super().__init__(msg)
 
 
-class SerializeModelNotImplementedError(NotImplementedError):
+class SerializeModelNotImplementedError(NotImplementedError):   # pragma: no cover
     pass
 
 
-class SerializeInputNotImplementedError(NotImplementedError):
+class SerializeInputNotImplementedError(NotImplementedError):   # pragma: no cover
     pass
 
 
-class RuntimeInfoInconsistencyError(Exception):
+class RuntimeInfoInconsistencyError(Exception):   # pragma: no cover
     pass
 
 
 def _prepare_artifact_dir(artifact_dir: str = None) -> str:
     """Prepares artifact dir for the model.
 
     Parameters
@@ -165,14 +166,17 @@
         The artifact dir that needs to be normalized.
 
     Returns
     -------
     str
         The artifact dir.
     """
+    if artifact_dir and ObjectStorageDetails.is_oci_path(artifact_dir):
+        return artifact_dir
+
     if artifact_dir and isinstance(artifact_dir, str):
         return os.path.abspath(os.path.expanduser(artifact_dir))
 
     artifact_dir = tempfile.mkdtemp()
     logger.info(
         f"The `artifact_dir` was not provided and "
         f"automatically set to: {artifact_dir}"
@@ -340,28 +344,49 @@
             Whether to serialize the model to pkl file by default. If False, you need to serialize the model manually,
             save it under artifact_dir and update the score.py manually.
         model_save_serializer: (SERDE or str, optional). Defaults to None.
             Instance of ads.model.SERDE. Used for serialize/deserialize model.
         model_input_serializer: (SERDE or str, optional). Defaults to None.
             Instance of ads.model.SERDE. Used for serialize/deserialize model input.
         """
+        if (
+            artifact_dir
+            and ObjectStorageDetails.is_oci_path(artifact_dir)
+            and not self._PREFIX == "spark"
+        ):
+            raise ValueError(
+                f"Unsupported value of `artifact_dir`: {artifact_dir}. "
+                "Only SparkPipelineModel framework supports object storage path as `artifact_dir`."
+            )
 
         self.estimator = estimator
         self.auth = auth or authutil.default_signer()
         self.dsc_model = (
             DataScienceModel()
             .with_custom_metadata_list(ModelCustomMetadata())
             .with_provenance_metadata(ModelProvenanceMetadata())
             .with_defined_metadata_list(ModelTaxonomyMetadata())
             .with_input_schema(Schema())
             .with_output_schema(Schema())
         )
 
         self.model_file_name = None
-        self.artifact_dir = _prepare_artifact_dir(artifact_dir)
+        self.artifact_dir = (
+            artifact_dir
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else _prepare_artifact_dir(artifact_dir)
+        )
+        self.local_copy_dir = (
+            _prepare_artifact_dir()
+            if ObjectStorageDetails.is_oci_path(artifact_dir)
+            else self.artifact_dir
+        )
+        if ObjectStorageDetails.is_oci_path(self.artifact_dir):
+            os.environ["OCI_DEPLOYMENT_PATH"] = self.artifact_dir
+
         self.model_artifact = None
         self.framework = None
         self.algorithm = None
         self.version = None
         self.hyperparameter = None
         self._introspect = ModelIntrospect(self)
         self.model_deployment = (
@@ -679,21 +704,20 @@
             X_sample=X_sample,
             initial_types=initial_types,
             **kwargs,
         )
 
     def _check_model_file(self, model_file_name, force_overwrite):
         model_path = os.path.join(self.artifact_dir, model_file_name)
-
-        if os.path.exists(model_path) and not force_overwrite:
+        if utils.is_path_exists(uri=model_path, auth=self.auth) and not force_overwrite:
             raise ValueError(
                 f"The {model_path} already exists, set force_overwrite to True if you wish to overwrite."
             )
-
-        os.makedirs(self.artifact_dir, exist_ok=True)
+        if not ObjectStorageDetails.is_oci_path(self.artifact_dir):
+            os.makedirs(self.artifact_dir, exist_ok=True)
         return model_path
 
     def _handle_model_file_name(self, as_onnx: bool, model_file_name: str = None):
         if as_onnx:
             self._set_model_save_serializer_to_onnx()
 
         if not model_file_name:
@@ -785,14 +809,15 @@
         X_sample: Union[list, tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         y_sample: Union[list, tuple, pd.DataFrame, pd.Series, np.ndarray] = None,
         training_script_path: str = None,
         training_id: str = _TRAINING_RESOURCE_ID,
         ignore_pending_changes: bool = True,
         max_col_num: int = DATA_SCHEMA_MAX_COL_NUM,
         ignore_conda_error: bool = False,
+        score_py_uri: str = None,
         **kwargs: Dict,
     ) -> "GenericModel":
         """Prepare and save the score.py, serialized model and runtime.yaml file.
 
         Parameters
         ----------
         inference_conda_env: (str, optional). Defaults to None.
@@ -837,14 +862,18 @@
         ignore_pending_changes: bool. Defaults to False.
             whether to ignore the pending changes in the git.
         max_col_num: (int, optional). Defaults to utils.DATA_SCHEMA_MAX_COL_NUM.
             Do not generate the input schema if the input has more than this
             number of features(columns).
         ignore_conda_error: (bool, optional). Defaults to False.
             Parameter to ignore error when collecting conda information.
+        score_py_uri: (str, optional). Defaults to None.
+            The uri of the customized score.py, which can be local path or OCI object storage URI.
+            When provide with this attibute, the `score.py` will not be auto generated, and the
+            provided `score.py` will be added into artifact_dir.
         kwargs:
             impute_values: (dict, optional).
                 The dictionary where the key is the column index(or names is accepted
                 for pandas dataframe) and the value is the impute value for the corresponding column.
 
         Raises
         ------
@@ -908,28 +937,30 @@
         )
         if (
             not isinstance(self.model_file_name, str)
             or self.model_file_name.strip() == ""
         ):
             raise ValueError("The `model_file_name` needs to be provided.")
 
-        os.makedirs(self.artifact_dir, exist_ok=True)
+        if not ObjectStorageDetails.is_oci_path(self.artifact_dir):
+            os.makedirs(self.artifact_dir, exist_ok=True)
 
         # Bring in .model-ignore file
-        shutil.copyfile(
-            os.path.join(
-                os.path.dirname(os.path.realpath(__file__)),
-                "common/.model-ignore",
-            ),
-            os.path.join(self.artifact_dir, ".model-ignore"),
+        uri_src = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)),
+            "common/.model-ignore",
         )
+        uri_dst = os.path.join(self.artifact_dir, ".model-ignore")
+        utils.copy_file(uri_src=uri_src, uri_dst=uri_dst, force_overwrite=True)
 
         self.model_artifact = ModelArtifact(
             artifact_dir=self.artifact_dir,
             model_file_name=self.model_file_name,
+            auth=self.auth,
+            local_copy_dir=self.local_copy_dir,
         )
         self.runtime_info = self.model_artifact.prepare_runtime_yaml(
             inference_conda_env=self.properties.inference_conda_env,
             inference_python_version=self.properties.inference_python_version,
             training_conda_env=self.properties.training_conda_env,
             training_python_version=self.properties.training_python_version,
             force_overwrite=force_overwrite,
@@ -958,16 +989,17 @@
                     X_sample=X_sample,
                     **kwargs,
                 )
                 self._summary_status.update_status(
                     detail="Serialized model", status=ModelState.DONE.value
                 )
             except SerializeModelNotImplementedError as e:
-                if not os.path.exists(
-                    os.path.join(self.artifact_dir, self.model_file_name)
+                if not utils.is_path_exists(
+                    uri=os.path.join(self.artifact_dir, self.model_file_name),
+                    auth=self.auth,
                 ):
                     self._summary_status.update_action(
                         detail="Serialized model",
                         action=(
                             "Model is not automatically serialized. "
                             f"Serialize the model as `{self.model_file_name}` and "
                             f"save to the {self.artifact_dir}."
@@ -997,35 +1029,46 @@
                 jinja_template_filename = "score_" + self.framework
                 if self.framework == "transformers":
                     jinja_template_filename = "score_" + "huggingface_pipeline"
             else:
                 jinja_template_filename = (
                     "score-pkl" if self._serialize else "score_generic"
                 )
-        self.model_artifact.prepare_score_py(
-            jinja_template_filename=jinja_template_filename,
-            model_file_name=self.model_file_name,
-            data_deserializer=self.model_input_serializer.name,
-            model_serializer=self.model_save_serializer.name,
-            **{**kwargs, **self._score_args},
-        )
+
+        if score_py_uri:
+            utils.copy_file(
+                uri_src=score_py_uri,
+                uri_dst=os.path.join(self.artifact_dir, "score.py"),
+                force_overwrite=force_overwrite,
+                auth=self.auth,
+            )
+        else:
+            self.model_artifact.prepare_score_py(
+                jinja_template_filename=jinja_template_filename,
+                model_file_name=self.model_file_name,
+                data_deserializer=self.model_input_serializer.name,
+                model_serializer=self.model_save_serializer.name,
+                auth=self.auth,
+                **{**kwargs, **self._score_args},
+            )
 
         self._summary_status.update_status(
             detail="Generated score.py", status=ModelState.DONE.value
         )
 
         self.populate_metadata(
             use_case_type=use_case_type,
             X_sample=X_sample,
             y_sample=y_sample,
             training_script_path=self.properties.training_script_path,
             training_id=self.properties.training_id,
             ignore_pending_changes=ignore_pending_changes,
             max_col_num=max_col_num,
             ignore_conda_error=self.ignore_conda_error,
+            auth=self.auth,
         )
 
         self._summary_status.update_status(
             detail="Populated metadata(Custom, Taxonomy and Provenance)",
             status=ModelState.DONE.value,
         )
 
@@ -1279,20 +1322,29 @@
             An instance of `GenericModel` class.
 
         Raises
         ------
         ValueError
             If `model_file_name` not provided.
         """
+        if (
+            cls._PREFIX is not "spark"
+            and artifact_dir
+            and ObjectStorageDetails.is_oci_path(artifact_dir)
+        ):
+            raise ValueError(
+                f"Unsupported value of `artifact_dir`: {artifact_dir}. "
+                "Only SparkPipelineModel framework supports object storage path as artifact_dir."
+            )
 
         local_vars = _extract_locals(locals())
         properties = properties or ModelProperties()
         properties.with_dict(local_vars)
-        artifact_dir = _prepare_artifact_dir(artifact_dir)
         auth = auth or authutil.default_signer()
+        artifact_dir = _prepare_artifact_dir(artifact_dir)
         model_artifact = ModelArtifact.from_uri(
             uri=uri,
             artifact_dir=artifact_dir,
             model_file_name=model_file_name,
             force_overwrite=force_overwrite,
             auth=auth,
             ignore_conda_error=ignore_conda_error,
@@ -1301,14 +1353,15 @@
             estimator=model_artifact.model,
             artifact_dir=artifact_dir,
             auth=auth,
             properties=properties,
             **kwargs,
         )
         model.model_file_name = model_file_name or model_artifact.model_file_name
+        model.local_copy_dir = model_artifact.local_copy_dir
         model.model_artifact = model_artifact
         model.ignore_conda_error = ignore_conda_error
         model.reload_runtime_info()
         model._summary_status.update_status(
             detail="Generated score.py",
             status=ModelState.DONE.value,
         )
@@ -1376,33 +1429,51 @@
                 By default the value will be extracted from the `OCI_REGION_METADATA` environment variables.
 
         Returns
         -------
         Self
             An instance of GenericModel class.
         """
+        if (
+            cls._PREFIX is not "spark"
+            and artifact_dir
+            and ObjectStorageDetails.is_oci_path(artifact_dir)
+        ):
+            raise ValueError(
+                f"Unsupported value of `artifact_dir`: {artifact_dir}. "
+                "Only SparkPipelineModel framework supports object storage path as artifact_dir."
+            )
+
         local_vars = _extract_locals(locals())
         properties = properties or ModelProperties()
         properties.with_dict(local_vars)
         properties.compartment_id = properties.compartment_id or _COMPARTMENT_OCID
         auth = auth or authutil.default_signer()
         artifact_dir = _prepare_artifact_dir(artifact_dir)
 
+        target_dir = (
+            artifact_dir
+            if not ObjectStorageDetails.is_oci_path(artifact_dir)
+            else tempfile.mkdtemp()
+        )
+        bucket_uri = bucket_uri or (
+            artifact_dir if ObjectStorageDetails.is_oci_path(artifact_dir) else None
+        )
         dsc_model = DataScienceModel.from_id(model_id)
         dsc_model.download_artifact(
-            target_dir=artifact_dir,
+            target_dir=target_dir,
             force_overwrite=force_overwrite,
             bucket_uri=bucket_uri,
             remove_existing_artifact=remove_existing_artifact,
             auth=auth,
             region=kwargs.pop("region", None),
             timeout=kwargs.pop("timeout", None),
         )
         result_model = cls.from_model_artifact(
-            uri=artifact_dir,
+            uri=target_dir,
             model_file_name=model_file_name,
             artifact_dir=artifact_dir,
             auth=auth,
             force_overwrite=force_overwrite,
             properties=properties,
             ignore_conda_error=ignore_conda_error,
             **kwargs,
@@ -1480,14 +1551,24 @@
                 By default the value will be extracted from the `OCI_REGION_METADATA` environment variables.
 
         Returns
         -------
         Self
             An instance of GenericModel class.
         """
+        if (
+            cls._PREFIX is not "spark"
+            and artifact_dir
+            and ObjectStorageDetails.is_oci_path(artifact_dir)
+        ):
+            raise ValueError(
+                f"Unsupported value of `artifact_dir`: {artifact_dir}. "
+                "Only SparkPipelineModel framework supports object storage path as `artifact_dir`."
+            )
+
         model_deployment = ModelDeployer(config=auth).get_model_deployment(
             model_deployment_id=model_deployment_id
         )
 
         current_state = model_deployment.state.name.upper()
         if current_state != ModelDeploymentState.ACTIVE.name:
             raise NotActiveDeploymentError(current_state)
@@ -1685,23 +1766,25 @@
         Returns
         -------
         None
             Nothing.
         """
         # reload runtime.yaml
         runtime_yaml_file = os.path.join(self.artifact_dir, "runtime.yaml")
-        if not os.path.exists(runtime_yaml_file):
+        if not utils.is_path_exists(runtime_yaml_file, auth=self.auth):
             if self.ignore_conda_error:
                 return self.runtime_info
             else:
                 raise FileNotFoundError(
                     f"`runtime.yaml` does not exist in {self.artifact_dir}. "
                     "Use `RuntimeInfo` class to populate it."
                 )
-        self.runtime_info = RuntimeInfo.from_yaml(uri=runtime_yaml_file)
+        self.runtime_info = RuntimeInfo.from_yaml(
+            uri=runtime_yaml_file, storage_options=self.auth or {}
+        )
 
     def reload(self) -> "GenericModel":
         """Reloads the model artifact files: `score.py` and the `runtime.yaml`.
 
         Returns
         -------
         GenericModel
@@ -1793,15 +1876,15 @@
         self.properties.compartment_id = (
             self.properties.compartment_id or _COMPARTMENT_OCID
         )
         self.properties.project_id = self.properties.project_id or PROJECT_OCID
 
         # check if the runtime_info sync with the runtime.yaml.
         try:
-            runtime_file_path = os.path.join(self.artifact_dir, "runtime.yaml")
+            runtime_file_path = os.path.join(self.local_copy_dir, "runtime.yaml")
             runtime_info_from_yaml = RuntimeInfo.from_yaml(uri=runtime_file_path)
             if self.runtime_info != runtime_info_from_yaml:
                 raise RuntimeInfoInconsistencyError(
                     "`.runtime_info` does not sync with runtime.yaml file. Call "
                     "`.runtime_info.save()` if you updated `runtime_info`. "
                     "Call `.reload()` if you updated runtime.yaml file."
                 )
@@ -1844,15 +1927,15 @@
         self.dsc_model = (
             self.dsc_model.with_compartment_id(self.properties.compartment_id)
             .with_project_id(self.properties.project_id)
             .with_display_name(display_name)
             .with_description(description)
             .with_freeform_tags(**(freeform_tags or {}))
             .with_defined_tags(**(defined_tags or {}))
-            .with_artifact(self.artifact_dir)
+            .with_artifact(self.local_copy_dir)
             .with_model_version_set_id(model_version_set_id)
             .with_version_label(version_label)
         ).create(
             bucket_uri=bucket_uri,
             overwrite_existing_artifact=overwrite_existing_artifact,
             remove_existing_artifact=remove_existing_artifact,
             **kwargs,
@@ -1876,22 +1959,23 @@
         """List out all the file names under the artifact_dir.
 
         Returns
         -------
         List
             List of the files in the artifact_dir.
         """
-        return get_files(self.artifact_dir)
+        return get_files(self.artifact_dir, auth=self.auth)
 
     def deploy(
         self,
         wait_for_completion: Optional[bool] = True,
         display_name: Optional[str] = None,
         description: Optional[str] = None,
         deployment_instance_shape: Optional[str] = None,
+        deployment_instance_subnet_id: Optional[str] = None,
         deployment_instance_count: Optional[int] = None,
         deployment_bandwidth_mbps: Optional[int] = None,
         deployment_log_group_id: Optional[str] = None,
         deployment_access_log_id: Optional[str] = None,
         deployment_predict_log_id: Optional[str] = None,
         deployment_memory_in_gbs: Optional[float] = None,
         deployment_ocpus: Optional[float] = None,
@@ -1932,14 +2016,16 @@
             The name of the model. If a display_name is not provided in kwargs,
             a randomly generated easy to remember name with timestamp will be generated,
             like 'strange-spider-2022-08-17-23:55.02'.
         description: (str, optional). Defaults to None.
             The description of the model.
         deployment_instance_shape: (str, optional). Default to `VM.Standard2.1`.
             The shape of the instance used for deployment.
+        deployment_instance_subnet_id: (str, optional). Default to None.
+            The subnet id of the instance used for deployment.
         deployment_instance_count: (int, optional). Defaults to 1.
             The number of instance used for deployment.
         deployment_bandwidth_mbps: (int, optional). Defaults to 10.
             The bandwidth limit on the load balancer in Mbps.
         deployment_memory_in_gbs: (float, optional). Defaults to None.
             Specifies the size of the memory of the model deployment instance in GBs.
         deployment_ocpus: (float, optional). Defaults to None.
@@ -2066,14 +2152,18 @@
                 self.properties.deployment_bandwidth_mbps
                 or existing_infrastructure.bandwidth_mbps
             )
             .with_shape_name(
                 self.properties.deployment_instance_shape
                 or existing_infrastructure.shape_name
             )
+            .with_subnet_id(
+                self.properties.deployment_instance_subnet_id
+                or existing_infrastructure.subnet_id
+            )
             .with_replica(
                 self.properties.deployment_instance_count
                 or existing_infrastructure.replica
             )
             .with_web_concurrency(web_concurrency)
         )
 
@@ -2235,14 +2325,15 @@
         model_freeform_tags: Optional[dict] = None,
         model_defined_tags: Optional[dict] = None,
         ignore_introspection: Optional[bool] = False,
         wait_for_completion: Optional[bool] = True,
         deployment_display_name: Optional[str] = None,
         deployment_description: Optional[str] = None,
         deployment_instance_shape: Optional[str] = None,
+        deployment_instance_subnet_id: Optional[str] = None,
         deployment_instance_count: Optional[int] = None,
         deployment_bandwidth_mbps: Optional[int] = None,
         deployment_log_group_id: Optional[str] = None,
         deployment_access_log_id: Optional[str] = None,
         deployment_predict_log_id: Optional[str] = None,
         deployment_memory_in_gbs: Optional[float] = None,
         deployment_ocpus: Optional[float] = None,
@@ -2322,14 +2413,16 @@
             The name of the model deployment. If a deployment_display_name is not provided in kwargs,
             a randomly generated easy to remember name with timestamp will be generated,
             like 'strange-spider-2022-08-17-23:55.02'.
         description: (str, optional). Defaults to None.
             The description of the model.
         deployment_instance_shape: (str, optional). Default to `VM.Standard2.1`.
             The shape of the instance used for deployment.
+        deployment_instance_subnet_id: (str, optional). Default to None.
+            The subnet id of the instance used for deployment.
         deployment_instance_count: (int, optional). Defaults to 1.
             The number of instance used for deployment.
         deployment_bandwidth_mbps: (int, optional). Defaults to 10.
             The bandwidth limit on the load balancer in Mbps.
         deployment_log_group_id: (str, optional). Defaults to None.
             The oci logging group id. The access log and predict log share the same log group.
         deployment_access_log_id: (str, optional). Defaults to None.
@@ -2463,14 +2556,15 @@
             deployment_display_name = utils.get_random_name_for_resource()
 
         self.deploy(
             wait_for_completion=wait_for_completion,
             display_name=deployment_display_name,
             description=deployment_description,
             deployment_instance_shape=self.properties.deployment_instance_shape,
+            deployment_instance_subnet_id=self.properties.deployment_instance_subnet_id,
             deployment_instance_count=self.properties.deployment_instance_count,
             deployment_bandwidth_mbps=self.properties.deployment_bandwidth_mbps,
             deployment_log_group_id=self.properties.deployment_log_group_id,
             deployment_access_log_id=self.properties.deployment_access_log_id,
             deployment_predict_log_id=self.properties.deployment_predict_log_id,
             deployment_memory_in_gbs=self.properties.deployment_memory_in_gbs,
             deployment_ocpus=self.properties.deployment_ocpus,
@@ -2479,14 +2573,15 @@
         )
         return self.model_deployment
 
     def predict(
         self,
         data: Any = None,
         auto_serialize_data: bool = False,
+        local: bool = False,
         **kwargs,
     ) -> Dict[str, Any]:
         """Returns prediction of input data run against the model deployment endpoint.
 
         Examples
         --------
         >>> uri = "https://github.com/pytorch/hub/raw/master/images/dog.jpg"
@@ -2503,14 +2598,16 @@
         data: Any
             Data for the prediction for onnx models, for local serialization
             method, data can be the data types that each framework support.
         auto_serialize_data: bool.
             Whether to auto serialize input data. Defauls to `False` for GenericModel, and `True` for other frameworks.
             `data` required to be json serializable if `auto_serialize_data=False`.
             If `auto_serialize_data` set to True, data will be serialized before sending to model deployment endpoint.
+        local: bool.
+            Whether to invoke the prediction locally. Default to False.
         kwargs:
             content_type: str, used to indicate the media type of the resource.
             image: PIL.Image Object or uri for the image.
                A valid string path for image file can be local path, http(s), oci, s3, gs.
             storage_options: dict
                Passed to `fsspec.open` for a particular storage connection.
                Please see `fsspec` (https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.open) for more details.
@@ -2521,18 +2618,29 @@
             Dictionary with the predicted values.
 
         Raises
         ------
         NotActiveDeploymentError
             If model deployment process was not started or not finished yet.
         ValueError
-            If `data` is empty or not JSON serializable.
+            If model is not deployed yet or the endpoint information is not available.
         """
-        if not self.model_deployment:
-            raise ValueError("Use `deploy()` method to start model deployment.")
+        if local:
+            return self.verify(
+                data=data, auto_serialize_data=auto_serialize_data, **kwargs
+            )
+
+        if not (self.model_deployment and self.model_deployment.url):
+            raise ValueError(
+                "Error invoking the remote endpoint as the model is not "
+                "deployed yet or the endpoint information is not available. "
+                "Use `deploy()` method to start model deployment. "
+                "If you intend to invoke inference using locally available "
+                "model artifact, set parameter `local=True`"
+            )
 
         current_state = self.model_deployment.state.name.upper()
         if current_state != ModelDeploymentState.ACTIVE.name:
             raise NotActiveDeploymentError(current_state)
 
         data = self._handle_input_data(data, auto_serialize_data, **kwargs)
         prediction = self.model_deployment.predict(
```

### Comparing `oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py` & `oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/model_artifact_boilerplate/score.py` & `oracle_ads-2.8.4/ads/model/model_artifact_boilerplate/score.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/model_metadata.py` & `oracle_ads-2.8.4/ads/model/model_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import oci.data_science.models
 import pandas as pd
 import yaml
 from ads.common import logger
 from ads.common.error import ChangesNotCommitted
 from ads.common.extended_enum import ExtendedEnumMeta
 from ads.common.serializer import DataClassSerializable
+from ads.common.object_storage_details import ObjectStorageDetails
 from oci.util import to_dict
 
 try:
     from yaml import CDumper as dumper
 except:
     from yaml import Dumper as dumper
 
@@ -1650,14 +1651,17 @@
         ChangesNotCommitted: if there are changes not being commited.
 
         Returns
         -------
         None
             Nothing.
         """
+        if ObjectStorageDetails.is_oci_path(path):
+            return
+
         if self.repo is not None and not ignore:
             path_abs = os.path.abspath(path)
             if (
                 os.path.commonpath([path_abs, self.repo.working_dir])
                 == self.repo.working_dir
             ):
                 path_relpath = os.path.relpath(path_abs, self.repo.working_dir)
```

### Comparing `oracle_ads-2.8.3/ads/model/model_properties.py` & `oracle_ads-2.8.4/ads/model/model_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     training_id: str = None
     compartment_id: str = None
     project_id: str = None
     bucket_uri: str = None
     remove_existing_artifact: bool = None
     overwrite_existing_artifact: bool = None
     deployment_instance_shape: str = None
+    deployment_instance_subnet_id: str = None
     deployment_instance_count: int = None
     deployment_bandwidth_mbps: int = None
     deployment_log_group_id: str = None
     deployment_access_log_id: str = None
     deployment_predict_log_id: str = None
     deployment_memory_in_gbs: Union[float, int] = None
     deployment_ocpus: Union[float, int] = None
```

### Comparing `oracle_ads-2.8.3/ads/model/model_version_set.py` & `oracle_ads-2.8.4/ads/model/model_version_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,32 +378,32 @@
             UpdateModelDetails(
                 model_version_set_id=self.id, version_label=version_label
             ),
             **kwargs,
         )
 
     @classmethod
-    def _load_default_properties(cls) -> Dict:
+    def _load_default_properties(self) -> Dict:
         """
         Load default properties from environment variables, notebook session, etc.
 
         Returns
         -------
         Dict
             A dictionary of default properties.
         """
         defaults = {}
-        compartment_ocid = COMPARTMENT_OCID
-        if compartment_ocid:
-            defaults[cls.CONST_COMPARTMENT_ID] = compartment_ocid
+
+        if COMPARTMENT_OCID:
+            defaults[self.CONST_COMPARTMENT_ID] = COMPARTMENT_OCID
         if PROJECT_OCID:
-            defaults[cls.CONST_PROJECT_ID] = PROJECT_OCID
+            defaults[self.CONST_PROJECT_ID] = PROJECT_OCID
 
         timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M")
-        defaults[cls.CONST_NAME] = f"model-version-set-{timestamp}"
+        defaults[self.CONST_NAME] = f"model-version-set-{timestamp}"
 
         return defaults
 
     @property
     def id(self) -> Optional[str]:
         """The OCID of the model version set."""
         if self.dsc_model_version_set:
```

### Comparing `oracle_ads-2.8.3/ads/model/runtime/env_info.py` & `oracle_ads-2.8.4/ads/model/runtime/env_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/runtime/model_deployment_details.py` & `oracle_ads-2.8.4/ads/model/runtime/model_deployment_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/runtime/model_provenance_details.py` & `oracle_ads-2.8.4/ads/model/runtime/model_provenance_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/runtime/runtime_info.py` & `oracle_ads-2.8.4/ads/model/runtime/runtime_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import os
 from dataclasses import dataclass, field
 from typing import Dict
 
 from ads.common.serializer import DataClassSerializable, SideEffect
@@ -58,21 +58,24 @@
         -------
         RuntimeInfo
             A RuntimeInfo instance.
         """
         runtime_info = cls(model_artifact_version="3.0")
         return runtime_info
 
-    def save(self):
+    def save(self, storage_options=None):
         """Save the RuntimeInfo object into runtime.yaml file under the artifact directory.
 
         Returns
         -------
         None
             Nothing.
         """
         runtime_file_path = os.path.join(
             self.model_provenance.training_code.artifact_directory, "runtime.yaml"
         )
+        storage_options = storage_options or {}
         self.to_yaml(
-            uri=runtime_file_path, side_effect=SideEffect.CONVERT_KEYS_TO_UPPER.value
+            uri=runtime_file_path,
+            side_effect=SideEffect.CONVERT_KEYS_TO_UPPER.value,
+            storage_options=storage_options,
         )
```

### Comparing `oracle_ads-2.8.3/ads/model/runtime/schemas/model_provenance_schema.yaml` & `oracle_ads-2.8.4/ads/model/runtime/schemas/model_provenance_schema.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/runtime/utils.py` & `oracle_ads-2.8.4/ads/model/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/serde/common.py` & `oracle_ads-2.8.4/ads/model/serde/common.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/serde/model_input.py` & `oracle_ads-2.8.4/ads/model/serde/model_input.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/serde/model_serializer.py` & `oracle_ads-2.8.4/ads/model/serde/model_serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/model/service/oci_datascience_model.py` & `oracle_ads-2.8.4/ads/model/service/oci_datascience_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 _REQUEST_INTERVAL_IN_SEC = 3
 
 MODEL_NEEDS_TO_BE_SAVED = (
     "Model needs to be saved to the Model Catalog before it can be accessed."
 )
 
 
-class ModelProvenanceNotFoundError(Exception):
+class ModelProvenanceNotFoundError(Exception):   # pragma: no cover
     pass
 
 
-class ModelArtifactNotFoundError(Exception):
+class ModelArtifactNotFoundError(Exception):   # pragma: no cover
     pass
 
 
-class ModelNotSavedError(Exception):
+class ModelNotSavedError(Exception):   # pragma: no cover
     pass
 
 
-class ModelWithActiveDeploymentError(Exception):
+class ModelWithActiveDeploymentError(Exception):   # pragma: no cover
     pass
 
 
 def check_for_model_id(msg: str = MODEL_NEEDS_TO_BE_SAVED):
     """The decorator helping to check if the ID attribute sepcified for a datascience model.
 
     Parameters
```

### Comparing `oracle_ads-2.8.3/ads/model/service/oci_datascience_model_deployment.py` & `oracle_ads-2.8.4/ads/model/service/oci_datascience_model_deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from functools import wraps
-import json
-import time
 import logging
 from typing import Callable, List
 from ads.common.oci_datascience import OCIDataScienceMixin
-from ads.common import utils as progress_bar_utils
+from ads.common.oci_mixin import OCIWorkRequestMixin
 from ads.config import PROJECT_OCID
-from ads.model.deployment.common import utils
 from ads.model.deployment.common.utils import OCIClientManager, State
 import oci
 
 from oci.data_science.models import (
     CreateModelDeploymentDetails,
     UpdateModelDeploymentDetails,
 )
@@ -70,24 +67,25 @@
             return func(self, *args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
-class MissingModelDeploymentIdError(Exception):
+class MissingModelDeploymentIdError(Exception):   # pragma: no cover
     pass
 
 
-class MissingModelDeploymentWorkflowIdError(Exception):
+class MissingModelDeploymentWorkflowIdError(Exception):   # pragma: no cover
     pass
 
 
 class OCIDataScienceModelDeployment(
     OCIDataScienceMixin,
+    OCIWorkRequestMixin,
     oci.data_science.models.ModelDeployment,
 ):
     """Represents an OCI Data Science Model Deployment.
     This class contains all attributes of the `oci.data_science.models.ModelDeployment`.
     The main purpose of this class is to link the `oci.data_science.models.ModelDeployment`
     and the related client methods.
     Linking the `ModelDeployment` (payload) to Create/Update/Delete/Activate/Deactivate methods.
@@ -176,44 +174,54 @@
             Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
         OCIDataScienceModelDeployment
             The `OCIDataScienceModelDeployment` instance (self).
         """
-        logger.info(f"Activating model deployment `{self.id}`.")
-        response = self.client.activate_model_deployment(
-            self.id,
-        )
+        dsc_model_deployment = OCIDataScienceModelDeployment.from_id(self.id)
+        if (
+            dsc_model_deployment.lifecycle_state
+            == self.LIFECYCLE_STATE_ACTIVE
+        ):
+            raise Exception(
+                f"Model deployment {dsc_model_deployment.id} is already in active state."
+            )
 
-        if wait_for_completion:
+        if (
+            dsc_model_deployment.lifecycle_state
+            == self.LIFECYCLE_STATE_INACTIVE
+        ):
+            logger.info(f"Activating model deployment `{self.id}`.")
+            response = self.client.activate_model_deployment(
+                self.id,
+            )
 
-            self.workflow_req_id = response.headers.get("opc-work-request-id", None)
-            oci_model_deployment_object = self.client.get_model_deployment(self.id).data
-            current_state = State._from_str(oci_model_deployment_object.lifecycle_state)
-            model_deployment_id = self.id
+            if wait_for_completion:
 
-            try:
-                self._wait_for_progress_completion(
-                    State.ACTIVE.name,
-                    ACTIVATE_WORKFLOW_STEPS,
-                    [State.FAILED.name, State.INACTIVE.name],
-                    self.workflow_req_id,
-                    current_state,
-                    model_deployment_id,
-                    max_wait_time,
-                    poll_interval,
-                )
-            except Exception as e:
-                logger.error(
-                    f"Error while trying to activate model deployment: {self.id}"
-                )
-                raise e
+                self.workflow_req_id = response.headers.get("opc-work-request-id", None)
 
-        return self.sync()
+                try:
+                    self.wait_for_progress(
+                        self.workflow_req_id, 
+                        ACTIVATE_WORKFLOW_STEPS, 
+                        max_wait_time, 
+                        poll_interval
+                    )
+                except Exception as e:
+                    logger.error(
+                        f"Error while trying to activate model deployment: {self.id}"
+                    )
+                    raise e
+
+            return self.sync()
+        else:
+            raise Exception(
+                f"Can't activate model deployment {dsc_model_deployment.id} when it's in {dsc_model_deployment.lifecycle_state} state."
+            )
 
     def create(
         self,
         create_model_deployment_details: CreateModelDeploymentDetails,
         wait_for_completion: bool = True,
         max_wait_time: int = DEFAULT_WAIT_TIME,
         poll_interval: int = DEFAULT_POLL_INTERVAL,
@@ -239,28 +247,21 @@
         response = self.client.create_model_deployment(create_model_deployment_details)
         self.update_from_oci_model(response.data)
         logger.info(f"Creating model deployment `{self.id}`.")
 
         if wait_for_completion:
 
             self.workflow_req_id = response.headers.get("opc-work-request-id", None)
-            res_payload = json.loads(str(response.data))
-            current_state = State._from_str(res_payload["lifecycle_state"])
-            model_deployment_id = self.id
 
             try:
-                self._wait_for_progress_completion(
-                    State.ACTIVE.name,
-                    CREATE_WORKFLOW_STEPS,
-                    [State.FAILED.name, State.INACTIVE.name],
-                    self.workflow_req_id,
-                    current_state,
-                    model_deployment_id,
-                    max_wait_time,
-                    poll_interval,
+                self.wait_for_progress(
+                    self.workflow_req_id, 
+                    CREATE_WORKFLOW_STEPS, 
+                    max_wait_time, 
+                    poll_interval
                 )
             except Exception as e:
                 logger.error(
                     f"Error while trying to create model deployment: {self.id}"
                 )
                 raise e
 
@@ -289,44 +290,54 @@
             Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
         OCIDataScienceModelDeployment
             The `OCIDataScienceModelDeployment` instance (self).
         """
-        logger.info(f"Deactivating model deployment `{self.id}`.")
-        response = self.client.deactivate_model_deployment(
-            self.id,
-        )
+        dsc_model_deployment = OCIDataScienceModelDeployment.from_id(self.id)
+        if (
+            dsc_model_deployment.lifecycle_state
+            == self.LIFECYCLE_STATE_INACTIVE
+        ):
+            raise Exception(
+                f"Model deployment {dsc_model_deployment.id} is already in inactive state."
+            )
 
-        if wait_for_completion:
+        if (
+            dsc_model_deployment.lifecycle_state
+            == self.LIFECYCLE_STATE_ACTIVE
+        ):
+            logger.info(f"Deactivating model deployment `{self.id}`.")
+            response = self.client.deactivate_model_deployment(
+                self.id,
+            )
 
-            self.workflow_req_id = response.headers.get("opc-work-request-id", None)
-            oci_model_deployment_object = self.client.get_model_deployment(self.id).data
-            current_state = State._from_str(oci_model_deployment_object.lifecycle_state)
-            model_deployment_id = self.id
+            if wait_for_completion:
 
-            try:
-                self._wait_for_progress_completion(
-                    State.INACTIVE.name,
-                    DEACTIVATE_WORKFLOW_STEPS,
-                    [State.FAILED.name],
-                    self.workflow_req_id,
-                    current_state,
-                    model_deployment_id,
-                    max_wait_time,
-                    poll_interval,
-                )
-            except Exception as e:
-                logger.error(
-                    f"Error while trying to deactivate model deployment: {self.id}"
-                )
-                raise e
+                self.workflow_req_id = response.headers.get("opc-work-request-id", None)
 
-        return self.sync()
+                try:
+                    self.wait_for_progress(
+                        self.workflow_req_id, 
+                        DEACTIVATE_WORKFLOW_STEPS, 
+                        max_wait_time, 
+                        poll_interval
+                    )
+                except Exception as e:
+                    logger.error(
+                        f"Error while trying to deactivate model deployment: {self.id}"
+                    )
+                    raise e
+
+            return self.sync()
+        else:
+            raise Exception(
+                f"Can't deactivate model deployment {dsc_model_deployment.id} when it's in {dsc_model_deployment.lifecycle_state} state."
+            )
 
     @check_for_model_deployment_id(
         msg="Model deployment needs to be deployed before it can be deleted."
     )
     def delete(
         self,
         wait_for_completion: bool = True,
@@ -347,36 +358,45 @@
             Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
         OCIDataScienceModelDeployment
             The `OCIDataScienceModelDeployment` instance (self).
         """
+        dsc_model_deployment = OCIDataScienceModelDeployment.from_id(self.id)
+        if dsc_model_deployment.lifecycle_state in [
+            self.LIFECYCLE_STATE_DELETED,
+            self.LIFECYCLE_STATE_DELETING
+        ]:
+            raise Exception(
+                f"Model deployment {dsc_model_deployment.id} is either deleted or being deleted."
+            )
+        if dsc_model_deployment.lifecycle_state not in [
+            self.LIFECYCLE_STATE_ACTIVE,
+            self.LIFECYCLE_STATE_FAILED,
+            self.LIFECYCLE_STATE_INACTIVE,
+        ]:
+            raise Exception(
+                f"Can't delete model deployment {dsc_model_deployment.id} when it's in {dsc_model_deployment.lifecycle_state} state."
+            )
         logger.info(f"Deleting model deployment `{self.id}`.")
         response = self.client.delete_model_deployment(
             self.id,
         )
 
         if wait_for_completion:
 
             self.workflow_req_id = response.headers.get("opc-work-request-id", None)
-            oci_model_deployment_object = self.client.get_model_deployment(self.id).data
-            current_state = State._from_str(oci_model_deployment_object.lifecycle_state)
-            model_deployment_id = self.id
 
             try:
-                self._wait_for_progress_completion(
-                    State.DELETED.name,
-                    DELETE_WORKFLOW_STEPS,
-                    [State.FAILED.name, State.INACTIVE.name],
-                    self.workflow_req_id,
-                    current_state,
-                    model_deployment_id,
-                    max_wait_time,
-                    poll_interval,
+                self.wait_for_progress(
+                    self.workflow_req_id, 
+                    DELETE_WORKFLOW_STEPS, 
+                    max_wait_time, 
+                    poll_interval
                 )
             except Exception as e:
                 logger.error(
                     f"Error while trying to delete model deployment: {self.id}"
                 )
                 raise e
 
@@ -507,94 +527,7 @@
 
         Returns
         -------
         OCIDataScienceModelDeployment
             An instance of `OCIDataScienceModelDeployment`.
         """
         return super().from_ocid(model_deployment_id)
-
-    def _wait_for_progress_completion(
-        self,
-        final_state: str,
-        work_flow_step: int,
-        disallowed_final_states: List[str],
-        work_flow_request_id: str,
-        state: State,
-        model_deployment_id: str,
-        max_wait_time: int = DEFAULT_WAIT_TIME,
-        poll_interval: int = DEFAULT_POLL_INTERVAL,
-    ):
-        """_wait_for_progress_completion blocks until progress is completed.
-
-        Parameters
-        ----------
-        final_state: str
-            Final state of model deployment aimed to be reached.
-        work_flow_step: int
-            Number of work flow step of the request.
-        disallowed_final_states: list[str]
-            List of disallowed final state to be reached.
-        work_flow_request_id: str
-            The id of work flow request.
-        state: State
-            The current state of model deployment.
-        model_deployment_id: str
-            The ocid of model deployment.
-        max_wait_time: int
-            Maximum amount of time to wait in seconds (Defaults to 1200).
-            Negative implies infinite wait time.
-        poll_interval: int
-            Poll interval in seconds (Defaults to 10).
-        """
-
-        start_time = time.time()
-        prev_message = ""
-        prev_workflow_stage_len = 0
-        current_state = state or State.UNKNOWN
-        with progress_bar_utils.get_progress_bar(work_flow_step) as progress:
-            if max_wait_time > 0 and utils.seconds_since(start_time) >= max_wait_time:
-                utils.get_logger().error(
-                    f"Max wait time ({max_wait_time} seconds) exceeded."
-                )
-            while (
-                max_wait_time < 0 or utils.seconds_since(start_time) < max_wait_time
-            ) and current_state.name.upper() != final_state:
-                if current_state.name.upper() in disallowed_final_states:
-                    utils.get_logger().info(
-                        f"Operation failed due to deployment reaching state {current_state.name.upper()}. Use Deployment ID for further steps."
-                    )
-                    break
-
-                prev_state = current_state.name
-                try:
-                    model_deployment_payload = json.loads(
-                        str(self.client.get_model_deployment(model_deployment_id).data)
-                    )
-                    current_state = (
-                        State._from_str(model_deployment_payload["lifecycle_state"])
-                        if "lifecycle_state" in model_deployment_payload
-                        else State.UNKNOWN
-                    )
-                    workflow_payload = self.client.list_work_request_logs(
-                        work_flow_request_id
-                    ).data
-                    if isinstance(workflow_payload, list) and len(workflow_payload) > 0:
-                        if prev_message != workflow_payload[-1].message:
-                            for _ in range(
-                                len(workflow_payload) - prev_workflow_stage_len
-                            ):
-                                progress.update(workflow_payload[-1].message)
-                            prev_workflow_stage_len = len(workflow_payload)
-                            prev_message = workflow_payload[-1].message
-                            prev_workflow_stage_len = len(workflow_payload)
-                    if prev_state != current_state.name:
-                        utils.get_logger().info(
-                            f"Status Update: {current_state.name} in {utils.seconds_since(start_time)} seconds"
-                        )
-                except Exception as e:
-                    # utils.get_logger().warning(
-                    #     "Unable to update deployment status. Details: %s", format(
-                    #         e)
-                    # )
-                    pass
-                time.sleep(poll_interval)
-            progress.update("Done")
```

### Comparing `oracle_ads-2.8.3/ads/model/service/oci_datascience_model_version_set.py` & `oracle_ads-2.8.4/ads/model/service/oci_datascience_model_version_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 from oci.data_science.models import (
     CreateModelVersionSetDetails,
     UpdateModelVersionSetDetails,
 )
 
 
-class ModelVersionSetNotExists(Exception):
+class ModelVersionSetNotExists(Exception):   # pragma: no cover
     pass
 
 
-class ModelVersionSetNotSaved(Exception):
+class ModelVersionSetNotSaved(Exception):   # pragma: no cover
     pass
 
 
 class DataScienceModelVersionSet(
     OCIDataScienceMixin,
     OCIModelWithNameMixin,
     OCIWorkRequestMixin,
```

### Comparing `oracle_ads-2.8.3/ads/model/transformer/onnx_transformer.py` & `oracle_ads-2.8.4/ads/model/transformer/onnx_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/mysqldb/mysql_db.py` & `oracle_ads-2.8.4/ads/mysqldb/mysql_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/backend/ads_ml_job.py` & `oracle_ads-2.8.4/ads/opctl/backend/ads_ml_job.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,41 @@
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import copy
 import os
+import shlex
 import shutil
 import tempfile
 from distutils import dir_util
-from typing import Tuple, Dict
-import shlex
+from typing import Dict, Tuple, Union
+
+from jinja2 import Environment, PackageLoader
 
-import ads
-from ads.common.auth import create_signer, AuthContext
+from ads.common.auth import AuthContext, create_signer
 from ads.common.oci_client import OCIClientFactory
 from ads.jobs import (
-    Job,
-    DataScienceJobRun,
+    ContainerRuntime,
     DataScienceJob,
+    DataScienceJobRun,
+    GitPythonRuntime,
+    Job,
+    NotebookRuntime,
+    PythonRuntime,
     ScriptRuntime,
-    ContainerRuntime,
 )
 from ads.opctl import logger
-from ads.opctl.backend.base import Backend
+from ads.opctl.backend.base import (
+    Backend,
+    RuntimeFactory,
+)
 from ads.opctl.config.resolver import ConfigResolver
 from ads.opctl.constants import DEFAULT_IMAGE_SCRIPT_DIR
-from jinja2 import Environment, PackageLoader
 from ads.opctl.distributed.common.cluster_config_helper import (
     ClusterConfigToJobSpecConverter,
 )
 
 REQUIRED_FIELDS = [
     "project_id",
     "compartment_id",
@@ -56,14 +62,74 @@
             config["execution"].get("oci_config", None),
             config["execution"].get("oci_profile", None),
         )
         self.auth_type = config["execution"].get("auth")
         self.profile = config["execution"].get("oci_profile", None)
         self.client = OCIClientFactory(**self.oci_auth).data_science
 
+    def init(
+        self,
+        uri: Union[str, None] = None,
+        overwrite: bool = False,
+        runtime_type: Union[str, None] = None,
+        **kwargs: Dict,
+    ) -> Union[str, None]:
+        """Generates a starter YAML specification for a Data Science Job.
+
+        Parameters
+        ----------
+        overwrite: (bool, optional). Defaults to False.
+            Overwrites the result specification YAML if exists.
+        uri: (str, optional), Defaults to None.
+            The filename to save the resulting specification template YAML.
+        runtime_type: (str, optional). Defaults to None.
+                The resource runtime type.
+        **kwargs: Dict
+            The optional arguments.
+
+        Returns
+        -------
+        Union[str, None]
+            The YAML specification for the given resource if `uri` was not provided.
+            `None` otherwise.
+        """
+
+        with AuthContext(auth=self.auth_type, profile=self.profile):
+            # define a job
+            job = (
+                Job()
+                .with_name(
+                    "{Job name. For MLflow, it will be replaced with the Project name}"
+                )
+                .with_infrastructure(
+                    DataScienceJob(
+                        **(self.config.get("infrastructure", {}) or {})
+                    ).init()
+                )
+                .with_runtime(
+                    JobRuntimeFactory.get_runtime(
+                        key=runtime_type or PythonRuntime().type
+                    ).init()
+                )
+            )
+
+            note = (
+                "# This YAML specification was auto generated by the `ads opctl init` command.\n"
+                "# The more details about the jobs YAML specification can be found in the ADS documentation:\n"
+                "# https://accelerated-data-science.readthedocs.io/en/latest/user_guide/jobs/index.html \n\n"
+            )
+
+            return job.to_yaml(
+                uri=uri,
+                overwrite=overwrite,
+                note=note,
+                filter_by_attribute_map=True,
+                **kwargs,
+            )
+
     def apply(self) -> None:
         """
         Create Job and Job Run from YAML.
         """
         with AuthContext(auth=self.auth_type, profile=self.profile):
             job = Job.from_dict(self.config)
             job.create()
@@ -473,7 +539,19 @@
                         jobrun = job.run(
                             worker_jobrun_conf.get("name"),
                             env_var=conf["envVars"],
                         )
                         worker_jobruns.append(jobrun)
                 self.job = job
                 return job, main_jobrun, worker_jobruns
+
+
+class JobRuntimeFactory(RuntimeFactory):
+    """Job runtime factory."""
+
+    _MAP = {
+        ContainerRuntime().type: ContainerRuntime,
+        ScriptRuntime().type: ScriptRuntime,
+        PythonRuntime().type: PythonRuntime,
+        NotebookRuntime().type: NotebookRuntime,
+        GitPythonRuntime().type: GitPythonRuntime,
+    }
```

### Comparing `oracle_ads-2.8.3/ads/opctl/backend/ads_model_deployment.py` & `oracle_ads-2.8.4/ads/opctl/backend/ads_model_deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
-from typing import Dict
-import ads
-from ads.common.auth import create_signer, AuthContext
+import json
+from typing import Dict, Union
+from ads.common.auth import AuthContext, create_signer
 from ads.common.oci_client import OCIClientFactory
-from ads.opctl.backend.base import Backend
-from ads.model.deployment import ModelDeployment
-
-from oci.data_science.models import ModelDeployment as OCIModelDeployment
+from ads.model.deployment import ModelDeployment, ModelDeploymentInfrastructure
+from ads.model.deployment.model_deployment_runtime import (
+    ModelDeploymentCondaRuntime,
+    ModelDeploymentContainerRuntime,
+)
+from ads.opctl.backend.base import Backend, RuntimeFactory
 
 
 class ModelDeploymentBackend(Backend):
     def __init__(self, config: Dict) -> None:
         """
         Initialize a ModelDeployment object given config dictionary.
 
@@ -30,14 +32,73 @@
             config["execution"].get("oci_config", None),
             config["execution"].get("oci_profile", None),
         )
         self.auth_type = config["execution"].get("auth")
         self.profile = config["execution"].get("oci_profile", None)
         self.client = OCIClientFactory(**self.oci_auth).data_science
 
+    def init(
+        self,
+        uri: Union[str, None] = None,
+        overwrite: bool = False,
+        runtime_type: Union[str, None] = None,
+        **kwargs: Dict,
+    ) -> Union[str, None]:
+        """Generates a starter YAML specification for a Data Science Job.
+
+        Parameters
+        ----------
+        overwrite: (bool, optional). Defaults to False.
+            Overwrites the result specification YAML if exists.
+        uri: (str, optional), Defaults to None.
+            The filename to save the resulting specification template YAML.
+        runtime_type: (str, optional). Defaults to None.
+                The resource runtime type.
+        **kwargs: Dict
+            The optional arguments.
+
+        Returns
+        -------
+        Union[str, None]
+            The YAML specification for the given resource if `uri` was not provided.
+            `None` otherwise.
+        """
+        with AuthContext(auth=self.auth_type, profile=self.profile):
+            # define a job
+            object = (
+                ModelDeployment()
+                .with_display_name("Model Deployment")
+                .with_description("The model deployment description")
+                .with_freeform_tags(key1="value1")
+                .with_infrastructure(
+                    ModelDeploymentInfrastructure(
+                        **(self.config.get("infrastructure", {}) or {})
+                    ).init()
+                )
+                .with_runtime(
+                    ModelDeploymentRuntimeFactory.get_runtime(
+                        key=runtime_type or ModelDeploymentCondaRuntime().type
+                    ).init()
+                )
+            )
+
+            note = (
+                "# This YAML specification was auto generated by the `ads opctl init` command.\n"
+                "# The more details about the jobs YAML specification can be found in the ADS documentation:\n"
+                "# https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/model_deploy_byoc.html \n\n"
+            )
+
+            return object.to_yaml(
+                uri=uri,
+                overwrite=overwrite,
+                note=note,
+                filter_by_attribute_map=True,
+                **kwargs,
+            )
+
     def apply(self) -> None:
         """
         Deploy model deployment from YAML.
         """
         wait_for_completion = self.config["execution"].get("wait_for_completion")
         max_wait_time = self.config["execution"].get("max_wait_time")
         poll_interval = self.config["execution"].get("poll_interval")
@@ -56,30 +117,14 @@
         """
         model_deployment_id = self.config["execution"].get("run_id")
         wait_for_completion = self.config["execution"].get("wait_for_completion")
         max_wait_time = self.config["execution"].get("max_wait_time")
         poll_interval = self.config["execution"].get("poll_interval")
         with AuthContext(auth=self.auth_type, profile=self.profile):
             model_deployment = ModelDeployment.from_id(model_deployment_id)
-            if model_deployment.lifecycle_state in [
-                OCIModelDeployment.LIFECYCLE_STATE_DELETED
-                or OCIModelDeployment.LIFECYCLE_STATE_DELETING
-            ]:
-                print(
-                    f"Model deployment {model_deployment.model_deployment_id} is either deleted or being deleted."
-                )
-                return
-            if model_deployment.lifecycle_state not in [
-                OCIModelDeployment.LIFECYCLE_STATE_ACTIVE,
-                OCIModelDeployment.LIFECYCLE_STATE_FAILED,
-                OCIModelDeployment.LIFECYCLE_STATE_INACTIVE,
-            ]:
-                raise Exception(
-                    f"Can't delete model deployment {model_deployment.model_deployment_id} when it's in {model_deployment.lifecycle_state} state."
-                )
             model_deployment.delete(
                 wait_for_completion=wait_for_completion,
                 max_wait_time=max_wait_time,
                 poll_interval=poll_interval,
             )
             print(
                 f"Model Deployment {model_deployment.model_deployment_id} has been deleted."
@@ -91,82 +136,74 @@
         """
         model_deployment_id = self.config["execution"].get("run_id")
         wait_for_completion = self.config["execution"].get("wait_for_completion")
         max_wait_time = self.config["execution"].get("max_wait_time")
         poll_interval = self.config["execution"].get("poll_interval")
         with AuthContext(auth=self.auth_type, profile=self.profile):
             model_deployment = ModelDeployment.from_id(model_deployment_id)
-            if (
-                model_deployment.lifecycle_state
-                == OCIModelDeployment.LIFECYCLE_STATE_ACTIVE
-            ):
-                print(
-                    f"Model deployment {model_deployment.model_deployment_id} is already active."
-                )
-                return
-
-            if (
-                model_deployment.lifecycle_state
-                == OCIModelDeployment.LIFECYCLE_STATE_INACTIVE
-            ):
-                model_deployment.activate(
-                    wait_for_completion=wait_for_completion,
-                    max_wait_time=max_wait_time,
-                    poll_interval=poll_interval,
-                )
-                print(
-                    f"Model Deployment {model_deployment.model_deployment_id} has been activated."
-                )
-            else:
-                raise Exception(
-                    f"Can't activate model deployment {model_deployment.model_deployment_id} when it's in {model_deployment.lifecycle_state} state."
-                )
+            model_deployment.activate(
+                wait_for_completion=wait_for_completion,
+                max_wait_time=max_wait_time,
+                poll_interval=poll_interval,
+            )
+            print(
+                f"Model Deployment {model_deployment.model_deployment_id} has been activated."
+            )
 
     def deactivate(self) -> None:
         """
         Deactivate model deployment from OCID.
         """
         model_deployment_id = self.config["execution"].get("run_id")
         wait_for_completion = self.config["execution"].get("wait_for_completion")
         max_wait_time = self.config["execution"].get("max_wait_time")
         poll_interval = self.config["execution"].get("poll_interval")
         with AuthContext(auth=self.auth_type, profile=self.profile):
             model_deployment = ModelDeployment.from_id(model_deployment_id)
-            if (
-                model_deployment.lifecycle_state
-                == OCIModelDeployment.LIFECYCLE_STATE_INACTIVE
-            ):
-                print(
-                    f"Model deployment {model_deployment.model_deployment_id} is already inactive."
-                )
-                return
-
-            if (
-                model_deployment.lifecycle_state
-                == OCIModelDeployment.LIFECYCLE_STATE_ACTIVE
-            ):
-                model_deployment.deactivate(
-                    wait_for_completion=wait_for_completion,
-                    max_wait_time=max_wait_time,
-                    poll_interval=poll_interval,
-                )
-                print(
-                    f"Model Deployment {model_deployment.model_deployment_id} has been deactivated."
-                )
-            else:
-                raise Exception(
-                    f"Can't deactivate model deployment {model_deployment.model_deployment_id} when it's in {model_deployment.lifecycle_state} state."
-                )
+            model_deployment.deactivate(
+                wait_for_completion=wait_for_completion,
+                max_wait_time=max_wait_time,
+                poll_interval=poll_interval,
+            )
+            print(
+                f"Model Deployment {model_deployment.model_deployment_id} has been deactivated."
+            )
 
     def watch(self) -> None:
         """
         Watch Model Deployment from OCID.
         """
         model_deployment_id = self.config["execution"].get("run_id")
         log_type = self.config["execution"].get("log_type")
         interval = self.config["execution"].get("interval")
         log_filter = self.config["execution"].get("log_filter")
         with AuthContext(auth=self.auth_type, profile=self.profile):
             model_deployment = ModelDeployment.from_id(model_deployment_id)
             model_deployment.watch(
                 log_type=log_type, interval=interval, log_filter=log_filter
             )
+
+    def predict(self) -> None:
+        ocid = self.config["execution"].get("ocid")
+        data = self.config["execution"].get("payload")
+        model_name = self.config["execution"].get("model_name")
+        model_version = self.config["execution"].get("model_version")
+        with AuthContext(auth=self.auth_type, profile=self.profile):
+            model_deployment = ModelDeployment.from_id(ocid)
+            try:
+                data = json.loads(data)
+            except:
+                pass
+            print(
+                model_deployment.predict(
+                    data=data, model_name=model_name, model_version=model_version
+                )
+            )
+
+
+class ModelDeploymentRuntimeFactory(RuntimeFactory):
+    """Mode Deployment runtime factory."""
+
+    _MAP = {
+        ModelDeploymentCondaRuntime().type: ModelDeploymentCondaRuntime,
+        ModelDeploymentContainerRuntime().type: ModelDeploymentContainerRuntime,
+    }
```

### Comparing `oracle_ads-2.8.3/ads/opctl/backend/local.py` & `oracle_ads-2.8.4/ads/opctl/backend/local.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,58 +6,73 @@
 
 import copy
 import json
 import os
 import tempfile
 from concurrent.futures import Future, ThreadPoolExecutor
 from time import sleep
-from typing import List, Dict
+from typing import Dict, List
 
+from oci.data_science.models import PipelineStepRun
+
+from ads.common.auth import create_signer
+from ads.common.decorator.runtime_dependency import (
+    OptionalDependency,
+    runtime_dependency,
+)
+
+from ads.model.model_metadata import ModelCustomMetadata
+from ads.model.runtime.runtime_info import RuntimeInfo
 from ads.opctl import logger
 from ads.opctl.backend.base import Backend
+from ads.opctl.conda.cmds import _install
 from ads.opctl.config.resolver import ConfigResolver
-from ads.opctl.distributed.cmds import local_run, load_ini
 from ads.opctl.constants import (
-    ML_JOB_IMAGE,
-    ML_JOB_GPU_IMAGE,
+    DEFAULT_IMAGE_CONDA_DIR,
     DEFAULT_IMAGE_HOME_DIR,
     DEFAULT_IMAGE_SCRIPT_DIR,
-    DEFAULT_IMAGE_CONDA_DIR,
+    DEFAULT_MODEL_FOLDER,
     DEFAULT_NOTEBOOK_SESSION_CONDA_DIR,
     DEFAULT_NOTEBOOK_SESSION_SPARK_CONF_DIR,
+    ML_JOB_GPU_IMAGE,
+    ML_JOB_IMAGE,
+    DEFAULT_MODEL_DEPLOYMENT_FOLDER,
 )
-from ads.opctl.utils import get_docker_client, is_in_notebook_session
-from ads.opctl.utils import build_image, run_container, run_command
+from ads.opctl.distributed.cmds import load_ini, local_run
+from ads.opctl.model.cmds import _download_model
 from ads.opctl.spark.cmds import (
-    generate_core_site_properties_str,
     generate_core_site_properties,
+    generate_core_site_properties_str,
 )
-from ads.common.decorator.runtime_dependency import (
-    runtime_dependency,
-    OptionalDependency,
+from ads.opctl.utils import (
+    build_image,
+    get_docker_client,
+    is_in_notebook_session,
+    run_command,
+    run_container,
 )
 from ads.pipeline.ads_pipeline import Pipeline, PipelineStep
-from oci.data_science.models import PipelineStepRun
+from ads.common.oci_client import OCIClientFactory
+from ads.config import NO_CONTAINER
 
-
-class CondaPackNotFound(Exception):
+class CondaPackNotFound(Exception):  # pragma: no cover
     pass
 
 
 class LocalBackend(Backend):
     def __init__(self, config: Dict) -> None:
         """
         Initialize a LocalBackend object with given config.
 
         Parameters
         ----------
         config: dict
             dictionary of configurations
         """
-        self.config = config
+        super().__init__(config=config)
 
     def run(self):
         if self.config.get("version") == "v1.0":
             docker_image = self.config["spec"]["Infrastructure"]["spec"]["dockerImage"]
             # TODO: don't hard code api keys
             bind_volumes = {
                 os.path.expanduser("~/.oci"): {
@@ -142,15 +157,15 @@
             else:
                 dev_container = {
                     "image": image,
                     "mounts": [],
                     "extensions": ["ms-python.python"],
                 }
 
-        dev_container["containerEnv"] = self.config["execution"]["env_vars"]
+        dev_container["containerEnv"] = self.config["execution"].get("env_vars", {})
         for k, v in self.config["execution"]["volumes"].items():
             dev_container["mounts"].append(
                 f"source={os.path.abspath(k)},target={v['bind']},type=bind"
             )
 
         try:
             client = get_docker_client()
@@ -174,39 +189,46 @@
                 f.write(json.dumps(dev_container, indent=2))
             print(f"File {os.path.join(source_folder, '.devcontainer.json')} created.")
         else:
             with open(os.path.abspath(".devcontainer.json"), "w") as f:
                 f.write(json.dumps(dev_container, indent=2))
             print(f"File {os.path.abspath('.devcontainer.json')} created.")
 
-    def _run_with_conda_pack(self, bind_volumes: Dict) -> int:
-        env_vars = self.config["execution"]["env_vars"]
+    def _run_with_conda_pack(
+        self,
+        bind_volumes: Dict,
+        extra_cmd: str = "",
+        install: bool = False,
+        conda_uri: str = "",
+    ) -> int:
+        env_vars = self.config["execution"].get("env_vars", {})
         slug = self.config["execution"]["conda_slug"]
-        image = self.config["execution"]["image"]
+        image = self.config["execution"].get("image", None)
 
         # bind_volumes is modified in-place and does not need to be returned
         # it is returned just to be explicit that it is changed during this function call
         bind_volumes, env_vars = self._check_conda_pack_and_install_if_applicable(
-            slug, bind_volumes, env_vars
+            slug, bind_volumes, env_vars, install=install, conda_uri=conda_uri
         )
         bind_volumes = self._mount_source_folder_if_exists(bind_volumes)
-        command = self._build_command_for_conda_run()
+        command = self._build_command_for_conda_run(extra_cmd)
         if is_in_notebook_session():
             run_command(command, shell=True)
         else:
             conda_pack_path = os.path.join(
                 os.path.expanduser(self.config["execution"]["conda_pack_folder"]), slug
             )
             if os.path.exists(os.path.join(conda_pack_path, "spark-defaults.conf")):
                 env_vars["SPARK_CONF_DIR"] = os.path.join(DEFAULT_IMAGE_CONDA_DIR, slug)
+            logger.info(f"Running with conda pack in a container with command {command}")
             return self._activate_conda_env_and_run(
                 image, slug, command, bind_volumes, env_vars
             )
 
-    def _build_command_for_conda_run(self) -> str:
+    def _build_command_for_conda_run(self, extra_cmd: str = "") -> str:
         if ConfigResolver(self.config)._is_ads_operator():
             if is_in_notebook_session():
                 curr_dir = os.path.dirname(os.path.abspath(__file__))
                 script = os.path.abspath(
                     os.path.join(curr_dir, "..", "operators", "run.py")
                 )
             else:
@@ -248,14 +270,15 @@
                 logger.warn(
                     "ML Job only support .py and .sh files."
                     "If you intend to submit to ML Job later, please update file extension."
                 )
                 command = f"cd {source_folder} && {entry_script} "
         if self.config["execution"].get("command"):
             command += f"{self.config['execution']['command']}"
+        command += extra_cmd
         return command
 
     def _run_with_image(self, bind_volumes: Dict) -> int:
         env_vars = self.config["execution"]["env_vars"]
         image = self.config["execution"]["image"]
         if ConfigResolver(self.config)._is_ads_operator():
             # running operators
@@ -268,14 +291,15 @@
         else:
             # in case of running a user image, entrypoint is not required
             entrypoint = self.config["execution"].get("entrypoint", None)
             command = self.config["execution"].get("command", None)
         if self.config["execution"].get("source_folder", None):
             bind_volumes.update(self._mount_source_folder_if_exists(bind_volumes))
         bind_volumes.update(self.config["execution"]["volumes"])
+
         return run_container(image, bind_volumes, env_vars, command, entrypoint)
 
     def _run_with_image_v1(self, bind_volumes: Dict) -> int:
         env_vars = [
             str(d["name"]) + "=" + str(d["value"])
             for d in self.config["spec"]["Runtime"]["spec"]["environmentVariables"]
         ]
@@ -290,23 +314,41 @@
             bind_volumes=bind_volumes,
             env_vars=env_vars,
             command=command,
             entrypoint=entrypoint,
         )
 
     def _check_conda_pack_and_install_if_applicable(
-        self, slug: str, bind_volumes: Dict, env_vars: Dict
+        self,
+        slug: str,
+        bind_volumes: Dict,
+        env_vars: Dict,
+        install: bool = False,
+        conda_uri: str = None,
     ) -> Dict:
-        conda_pack_path = os.path.join(
-            os.path.expanduser(self.config["execution"]["conda_pack_folder"]), slug
+        conda_pack_folder = os.path.abspath(
+            os.path.expanduser(self.config["execution"]["conda_pack_folder"])
         )
+        conda_pack_path = os.path.join(conda_pack_folder, slug)
         if not os.path.exists(conda_pack_path):
-            raise CondaPackNotFound(
-                f"Conda pack {conda_pack_path} not found. Please run `ads opctl conda create` or `ads opctl conda install`."
-            )
+            if install:
+                logger.info(
+                    f"Downloading a `{slug}` to the `{conda_pack_folder}`. If this conda pack is already installed locally in a different location, pass in `conda_pack_folder` to avoid downloading it again."
+                )
+                _install(
+                    conda_uri=conda_uri,
+                    conda_pack_folder=conda_pack_folder,
+                    oci_config=self.oci_config,
+                    oci_profile=self.profile,
+                    auth_type=self.auth_type,
+                )
+            else:
+                raise CondaPackNotFound(
+                    f"Conda pack {conda_pack_path} not found. Please run `ads opctl conda create` or `ads opctl conda install`."
+                )
         if os.path.exists(os.path.join(conda_pack_path, "spark-defaults.conf")):
             if not is_in_notebook_session():
                 env_vars["SPARK_CONF_DIR"] = os.path.join(DEFAULT_IMAGE_CONDA_DIR, slug)
             # write core_site.xml
             if self.config["execution"]["auth"] == "api_key":
                 properties = generate_core_site_properties(
                     "api_key",
@@ -606,7 +648,162 @@
 
         Parameters
         ----------
         str: str
             The message to log
         """
         logger.info(f"{self.LOG_PREFIX}: {str}")
+
+
+class LocalModelDeploymentBackend(LocalBackend):
+    def __init__(self, config: Dict) -> None:
+        """
+        Initialize a LocalModelDeploymentBackend object with given config.
+
+        Parameters
+        ----------
+        config: dict
+            dictionary of configurations
+        """
+        super().__init__(config)
+        self.oci_auth = create_signer(
+            self.auth_type,
+            self.oci_config,
+            self.profile,
+        )
+        self.client = OCIClientFactory(**self.oci_auth).data_science
+
+    def predict(self) -> None:
+        """
+        Conducts local verify.
+
+        Returns
+        -------
+        None
+            Nothing.
+        """
+        
+        # model artifact in artifact directory
+        artifact_directory = self.config["execution"].get("artifact_directory")
+        ocid = self.config["execution"].get("ocid")
+        
+        model_folder = os.path.expanduser(
+            self.config["execution"].get("model_save_folder", DEFAULT_MODEL_FOLDER)
+        )
+        artifact_directory = artifact_directory or os.path.join(model_folder, str(ocid))
+        if ocid and (
+            not os.path.exists(artifact_directory)
+            or len(os.listdir(artifact_directory)) == 0
+        ):
+            region = self.config["execution"].get("region", None)
+            bucket_uri = self.config["execution"].get("bucket_uri", None)
+            timeout = self.config["execution"].get("timeout", None)
+            logger.info(
+                f"No cached model found. Downloading the model {ocid} to {artifact_directory}. If you already have a copy of the model, specify `artifact_directory` instead of `ocid`. You can specify `model_save_folder` to decide where to store the model artifacts."
+            )
+
+            _download_model(
+                auth=self.auth_type,
+                profile=self.profile,
+                ocid=ocid,
+                artifact_directory=artifact_directory,
+                region=region,
+                bucket_uri=bucket_uri,
+                timeout=timeout,
+                force_overwrite=True,
+            )
+                
+        # conda
+        conda_slug, conda_path = self.config["execution"].get("conda_slug"), self.config["execution"].get("conda_path")
+        if not conda_slug and not conda_path and ocid:
+            conda_slug, conda_path = self._get_conda_info_from_custom_metadata(ocid)
+        if not conda_slug and not conda_path:
+            conda_slug, conda_path = self._get_conda_info_from_runtime(
+                artifact_dir=artifact_directory
+            )
+        if 'conda_slug' not in self.config["execution"]:
+            self.config["execution"]["conda_slug"] = conda_path.split("/")[-1] if conda_path else conda_slug 
+
+        self.config["execution"]["image"] = ML_JOB_IMAGE
+        
+        # bind_volumnes
+        bind_volumes = {}
+        SCRIPT = "script.py"
+        dir_path = os.path.dirname(os.path.realpath(__file__))
+        if not is_in_notebook_session():
+            bind_volumes = {
+                os.path.expanduser(
+                    os.path.dirname(self.config["execution"]["oci_config"])
+                ): {"bind": os.path.join(DEFAULT_IMAGE_HOME_DIR, ".oci")}
+            }
+            
+            self.config["execution"]["source_folder"] = os.path.abspath(
+                os.path.join(dir_path, "..")
+            )
+            self.config["execution"]["entrypoint"] = SCRIPT
+            bind_volumes[artifact_directory] = {"bind": DEFAULT_MODEL_DEPLOYMENT_FOLDER}
+        
+        # extra cmd
+        data = self.config["execution"].get("payload")
+        extra_cmd = f"--payload '{data}' " + f"--auth {self.auth_type} "
+        if self.auth_type != "resource_principal":
+            extra_cmd += f"--profile {self.profile}"
+        
+        if is_in_notebook_session() or NO_CONTAINER:
+            # _run_with_conda_pack has code to handle notebook session case,
+            # however, it activate the conda pack and then run the script. 
+            # For the deployment, we just take the current conda env and run it.
+            # Hence we just handle the notebook case directly here.
+            script_path = os.path.join(os.path.join(dir_path, ".."), SCRIPT)
+            cmd = f"python {script_path} " + f"--artifact-directory {artifact_directory} " + extra_cmd
+            logger.info(f"Running in a notebook or NO_CONTAINER with command {cmd}")
+            run_command(cmd=cmd, shell=True)
+        else:
+            extra_cmd = f"--artifact-directory {DEFAULT_MODEL_DEPLOYMENT_FOLDER} "+ extra_cmd
+            exit_code = self._run_with_conda_pack(
+                    bind_volumes, extra_cmd, install=True, conda_uri=conda_path
+                )
+            if exit_code != 0:
+                raise RuntimeError(
+                    f"`predict` did not complete successfully. Exit code: {exit_code}. "
+                    f"Run with the --debug argument to view container logs."
+                )
+                
+    def _get_conda_info_from_custom_metadata(self, ocid):
+        """
+        Get conda env info from custom metadata from model catalog.
+
+        Returns
+        -------
+        (str, str)
+            conda slug and conda path.
+        """
+        response = self.client.get_model(ocid)
+        custom_metadata = ModelCustomMetadata._from_oci_metadata(
+            response.data.custom_metadata_list
+        )
+        conda_slug, conda_path = None, None
+        if "CondaEnvironmentPath" in custom_metadata.keys:
+            conda_path = custom_metadata["CondaEnvironmentPath"].value
+        if "SlugName" in custom_metadata.keys:
+            conda_slug = custom_metadata["SlugName"].value
+        return conda_slug, conda_path
+
+    @staticmethod
+    def _get_conda_info_from_runtime(artifact_dir):
+        """
+        Get conda env info from runtime yaml file.
+
+        Returns
+        -------
+        (str, str)
+            conda slug and conda path.
+        """
+        runtime_yaml_file = os.path.join(artifact_dir, "runtime.yaml")
+        runtime_info = RuntimeInfo.from_yaml(uri=runtime_yaml_file)
+        conda_slug = (
+            runtime_info.model_deployment.inference_conda_env.inference_env_slug
+        )
+        conda_path = (
+            runtime_info.model_deployment.inference_conda_env.inference_env_path
+        )
+        return conda_slug, conda_path
```

### Comparing `oracle_ads-2.8.3/ads/opctl/cli.py` & `oracle_ads-2.8.4/ads/opctl/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
-import fsspec
 import os
+from typing import Any, Dict
 
 import click
+import fsspec
 import yaml
 
-from ads.common.auth import AuthType
+import ads.opctl.conda.cli
+import ads.opctl.distributed.cli
+import ads.opctl.model.cli
+import ads.opctl.spark.cli
 from ads.common import auth as authutil
+from ads.common.auth import AuthType
 from ads.opctl.cmds import activate as activate_cmd
 from ads.opctl.cmds import cancel as cancel_cmd
-from ads.opctl.cmds import deactivate as deactivate_cmd
 from ads.opctl.cmds import configure as configure_cmd
+from ads.opctl.cmds import deactivate as deactivate_cmd
 from ads.opctl.cmds import delete as delete_cmd
+from ads.opctl.cmds import init as init_cmd
+from ads.opctl.cmds import init_operator as init_operator_cmd
 from ads.opctl.cmds import init_vscode as init_vscode_cmd
+from ads.opctl.cmds import predict as predict_cmd
 from ads.opctl.cmds import run as run_cmd
 from ads.opctl.cmds import run_diagnostics as run_diagnostics_cmd
 from ads.opctl.cmds import watch as watch_cmd
-from ads.opctl.cmds import init_operator as init_operator_cmd
+from ads.opctl.config.merger import ConfigMerger
+from ads.opctl.constants import (BACKEND_NAME, DEFAULT_MODEL_FOLDER,
+                                 RESOURCE_TYPE, RUNTIME_TYPE)
 from ads.opctl.utils import build_image as build_image_cmd
 from ads.opctl.utils import publish_image as publish_image_cmd
 from ads.opctl.utils import suppress_traceback
-from ads.opctl.config.merger import ConfigMerger
-from ads.opctl.constants import BACKEND_NAME
-
-import ads.opctl.conda.cli
-import ads.opctl.spark.cli
-import ads.opctl.distributed.cli
 
 
 @click.group("opctl")
 @click.help_option("--help", "-h")
 def commands():
     pass
 
@@ -495,15 +499,143 @@
 def deactivate(**kwargs):
     """
     Deactivates a data science service.
     """
     suppress_traceback(kwargs["debug"])(deactivate_cmd)(**kwargs)
 
 
+@commands.command()
+@click.argument(
+    "resource-type",
+    type=click.Choice(RESOURCE_TYPE.values()),
+    required=True,
+)
+@click.help_option("--help", "-h")
+@click.option("--debug", "-d", help="Set debug mode", is_flag=True, default=False)
+@click.option(
+    "--runtime-type",
+    type=click.Choice(RUNTIME_TYPE.values()),
+    help="The runtime type",
+    required=False,
+)
+@click.option(
+    "--output",
+    help=f"The filename to save the resulting specification template YAML",
+    required=False,
+    default=None,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    help="Overwrite result file if it already exists",
+    is_flag=True,
+    default=False,
+)
+@click.option(
+    "--ads-config",
+    help="The folder where the ADS opctl config located",
+    required=False,
+    default=None,
+)
+def init(debug: bool, **kwargs: Dict[str, Any]) -> None:
+    """Generates a starter specification template YAML for the Data Science resources."""
+    suppress_traceback(debug)(init_cmd)(**kwargs)
+
+
+@commands.command()
+@click.option(
+    "--ocid",
+    nargs=1,
+    required=False,
+    help="This can be either a model id or model deployment id. When model id is passed, it conducts a local predict/test. This is designed for local dev purpose in order to test whether deployment will be successful locally. When you pass in `model_save_folder`, the model artifact will be downloaded and saved to a subdirectory of `model_save_folder` where model id is the name of subdirectory. Or you can pass in a model deployment id and this will invoke the remote endpoint and conduct a prediction on the server.",
+)
+@click.option(
+    "--model-save-folder",
+    nargs=1,
+    required=False,
+    default=DEFAULT_MODEL_FOLDER,
+    help="Which location to store model artifact folders. Defaults to ~/.ads_ops/models. This is only used when model id is passed to `ocid` and a local predict is conducted.",
+)
+@click.option(
+    "--conda-pack-folder",
+    nargs=1,
+    required=False,
+    help="Which location to store the conda pack locally. Defaults to ~/.ads_ops/conda. This is only used when model id is passed to `ocid` and a local predict is conducted.",
+)
+@click.option(
+    "--bucket-uri",
+    nargs=1,
+    required=False,
+    help="The OCI Object Storage URI where model artifacts will be copied to. The `bucket_uri` is only necessary for uploading large artifacts which size is greater than 2GB. Example: `oci://<bucket_name>@<namespace>/prefix/`. This is only used when the model id is passed.",
+)
+@click.option(
+    "--region",
+    nargs=1,
+    required=False,
+    help="The destination Object Storage bucket region. By default the value will be extracted from the `OCI_REGION_METADATA` environment variables. This is only used when the model id is passed.",
+)
+@click.option(
+    "--timeout",
+    nargs=1,
+    required=False,
+    help="The connection timeout in seconds for the client. This is only used when the model id is passed.",
+)
+@click.option(
+    "--artifact-directory",
+    nargs=1,
+    required=False,
+    default=None,
+    help="The artifact directory where stores your models, score.py and etc. This is used when you have a model artifact locally and have not saved it to the model catalog yet. In this case, you dont need to pass in model ",
+)
+@click.option(
+    "--payload",
+    nargs=1,
+    help="The payload sent to the model for prediction. For example, --payload '[[-1.68671955,-0.27358368,0.82731396,-0.14530245,0.80733585]]'.",
+)
+@click.option(
+    "--conda-slug",
+    nargs=1,
+    required=False,
+    help="The conda slug used to load the model and conduct the prediction. This is only used when model id is passed to `ocid` and a local predict is conducted. It should match the inference conda env specified in the runtime.yaml file which is the conda pack being used when conducting real model deployment.",
+)
+@click.option(
+    "--conda-path",
+    nargs=1,
+    required=False,
+    help="The conda path used to load the model and conduct the prediction. This is only used when model id is passed to `ocid` and a local predict is conducted. It should match the inference conda env specified in the runtime.yaml file which is the conda pack being used when conducting real model deployment.",
+)
+@click.option(
+    "--model-version",
+    nargs=1,
+    required=False,
+    help="When the `inference_server='triton'`, the version of the model to invoke. This can only be used when model deployment id is passed in. For the other cases, it will be ignored.",
+)
+@click.option(
+    "--model-name",
+    nargs=1,
+    required=False,
+    help="When the `inference_server='triton'`, the name of the model to invoke. This can only be used when model deployment id is passed in. For the other cases, it will be ignored.",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
+def predict(**kwargs):
+    """
+    Make prediction using the model with the payload.
+    """
+    suppress_traceback(kwargs["debug"])(predict_cmd)(**kwargs)
+
+
 commands.add_command(ads.opctl.conda.cli.commands)
+commands.add_command(ads.opctl.model.cli.commands)
 commands.add_command(ads.opctl.spark.cli.commands)
 commands.add_command(ads.opctl.distributed.cli.commands)
-
-# @commands.command()
-# @click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
-# def list(debug):
-#     print(json.dumps(suppress_traceback(debug)(_list_ads_operators)(), indent=2))
```

### Comparing `oracle_ads-2.8.3/ads/opctl/cmds.py` & `oracle_ads-2.8.4/ads/opctl/cmds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
-import os
 import configparser
+import os
+from typing import Dict, List, Union
+
 import click
+import fsspec
+import yaml
 
 import ads
-
-from typing import Dict, List
-
-from ads.common.auth import AuthContext
-from ads.common.oci_datascience import DSCNotebookSession
+from ads.common.auth import AuthContext, AuthType
 from ads.common.extended_enum import ExtendedEnumMeta
+from ads.common.oci_datascience import DSCNotebookSession
+from ads.opctl import logger
+from ads.opctl.backend.ads_dataflow import DataFlowBackend
 from ads.opctl.backend.ads_ml_job import MLJobBackend, MLJobDistributedBackend
+from ads.opctl.backend.ads_ml_pipeline import PipelineBackend
 from ads.opctl.backend.ads_model_deployment import ModelDeploymentBackend
 from ads.opctl.backend.local import (
     LocalBackend,
     LocalBackendDistributed,
+    LocalModelDeploymentBackend,
     LocalPipelineBackend,
 )
-from ads.opctl.backend.ads_dataflow import DataFlowBackend
-from ads.opctl.backend.ads_ml_pipeline import PipelineBackend
 from ads.opctl.config.base import ConfigProcessor
 from ads.opctl.config.merger import ConfigMerger
 from ads.opctl.config.resolver import ConfigResolver
 from ads.opctl.config.utils import read_from_ini
 from ads.opctl.config.validator import ConfigValidator
 from ads.opctl.config.yaml_parsers import YamlSpecParser
-import fsspec
-from ads.common.auth import AuthType
-
-from ads.opctl.distributed.cmds import (
-    update_ini,
-    increment_tag_in_ini,
-    docker_build_cmd,
-    update_image,
-    verify_and_publish_image,
-    update_config_image,
-)
 from ads.opctl.constants import (
-    DEFAULT_OCI_CONFIG_FILE,
-    DEFAULT_PROFILE,
-    DEFAULT_CONDA_PACK_FOLDER,
-    DEFAULT_ADS_CONFIG_FOLDER,
     ADS_CONFIG_FILE_NAME,
-    ADS_JOBS_CONFIG_FILE_NAME,
     ADS_DATAFLOW_CONFIG_FILE_NAME,
-    ADS_ML_PIPELINE_CONFIG_FILE_NAME,
+    ADS_JOBS_CONFIG_FILE_NAME,
     ADS_LOCAL_BACKEND_CONFIG_FILE_NAME,
+    ADS_ML_PIPELINE_CONFIG_FILE_NAME,
+    ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME,
     BACKEND_NAME,
+    DEFAULT_ADS_CONFIG_FOLDER,
+    DEFAULT_CONDA_PACK_FOLDER,
+    DEFAULT_OCI_CONFIG_FILE,
+    DEFAULT_PROFILE,
+    RESOURCE_TYPE,
 )
-from ads.opctl.utils import (
-    is_in_notebook_session,
-    get_service_pack_prefix,
+from ads.opctl.distributed.cmds import (
+    docker_build_cmd,
+    increment_tag_in_ini,
+    update_config_image,
+    update_image,
+    update_ini,
+    verify_and_publish_image,
 )
-import yaml
+from ads.opctl.utils import get_service_pack_prefix, is_in_notebook_session
 
 
 class DataScienceResource(str, metaclass=ExtendedEnumMeta):
     JOB = "datasciencejob"
     DATAFLOW = "dataflowapplication"
     PIPELINE = "datasciencepipeline"
     MODEL_DEPLOYMENT = "datasciencemodeldeployment"
+    MODEL = "datasciencemodel"
 
 
 class DataScienceResourceRun(str, metaclass=ExtendedEnumMeta):
     JOB_RUN = "datasciencejobrun"
     DATAFLOW_RUN = "dataflowrun"
     PIPELINE_RUN = "datasciencepipelinerun"
     MODEL_DEPLOYMENT = "datasciencemodeldeployment"
@@ -78,14 +77,15 @@
     DataScienceResource.JOB: "job",
     DataScienceResourceRun.JOB_RUN: "job",
     DataScienceResource.DATAFLOW: "dataflow",
     DataScienceResourceRun.DATAFLOW_RUN: "dataflow",
     DataScienceResource.PIPELINE: "pipeline",
     DataScienceResourceRun.PIPELINE_RUN: "pipeline",
     DataScienceResourceRun.MODEL_DEPLOYMENT: "deployment",
+    DataScienceResource.MODEL: "deployment",
 }
 
 DATA_SCIENCE_RESOURCE_RUN_BACKEND_MAP = {
     DataScienceResourceRun.JOB_RUN: "job",
     DataScienceResourceRun.DATAFLOW_RUN: "dataflow",
     DataScienceResourceRun.PIPELINE_RUN: "pipeline",
     DataScienceResourceRun.MODEL_DEPLOYMENT: "deployment",
@@ -99,14 +99,15 @@
         BACKEND_NAME.PIPELINE.value: PipelineBackend,
         BACKEND_NAME.MODEL_DEPLOYMENT.value: ModelDeploymentBackend,
     }
 
     LOCAL_BACKENDS_MAP = {
         BACKEND_NAME.JOB.value: LocalBackend,
         BACKEND_NAME.PIPELINE.value: LocalPipelineBackend,
+        BACKEND_NAME.MODEL_DEPLOYMENT.value: LocalModelDeploymentBackend,
     }
 
     def __init__(self, config: Dict):
         self.config = config
         self._backend = config["execution"].pop("backend", None)
         if self._backend is None:
             raise RuntimeError("Please specify backend.")
@@ -137,15 +138,15 @@
     """Saves job run info YAML to a local file.
 
     Parameters
     ----------
     yaml_content : str
         YAML content as string.
     """
-    if kwargs["job_info"]:
+    if kwargs.get("job_info"):
         yaml_path = os.path.abspath(os.path.expanduser(kwargs["job_info"]))
         if os.path.isfile(yaml_path):
             overwrite = input(
                 f"File {yaml_path} already exists. Overwrite the file? [yN]: "
             )
             if overwrite not in ["y", "Y"]:
                 return
@@ -206,15 +207,15 @@
             backend = LocalBackendDistributed(config)
             backend.run()
         elif mode == BACKEND_NAME.DATAFLOW.value:
             raise RuntimeError(
                 "backend operator for distributed training can either be local or job"
             )
         else:
-            if not kwargs["dry_run"]:
+            if not kwargs["dry_run"] and not kwargs["nobuild"]:
                 verify_and_publish_image(kwargs["nopush"], config)
                 print("running image: " + config["spec"]["cluster"]["spec"]["image"])
             cluster_def = YamlSpecParser.parse_content(config)
 
             backend = MLJobDistributedBackend(p.config)
 
             # Define job first,
@@ -281,15 +282,14 @@
     Returns
     -------
     Dict
         dictionary of job id and run id in case of ML Job run, else empty if running locally
     """
     p = ConfigProcessor(config).step(ConfigMerger, **kwargs)
     if config.get("kind") == "distributed":  # TODO: add kind factory
-
         config = update_config_image(config)
         cluster_def = YamlSpecParser.parse_content(config)
 
         backend = MLJobDistributedBackend(p.config)
 
         # Define job first,
         # Then Run
@@ -454,14 +454,35 @@
     kwargs["run_id"] = kwargs.pop("ocid")
     if not kwargs.get("backend"):
         kwargs["backend"] = _get_backend_from_run_id(kwargs["run_id"])
     p = ConfigProcessor().step(ConfigMerger, **kwargs)
     return _BackendFactory(p.config).backend.deactivate()
 
 
+def predict(**kwargs) -> None:
+    """
+    Make prediction using the model with the payload.
+
+    Parameters
+    ----------
+    kwargs: dict
+        keyword argument, stores command line args
+
+    Returns
+    -------
+    None
+    """
+    p = ConfigProcessor().step(ConfigMerger, **kwargs)
+    if "datasciencemodeldeployment" in p.config["execution"].get("ocid", ""):
+        return ModelDeploymentBackend(p.config).predict()
+    else:
+        # model ocid or artifact directory
+        return LocalModelDeploymentBackend(p.config).predict()
+
+
 def init_vscode(**kwargs) -> None:
     """
     Create a .devcontainer.json file for local development.
 
     Parameters
     ----------
     kwargs
@@ -549,17 +570,18 @@
     )
     config_parser["CONDA"]["conda_pack_os_prefix"] = conda_os_prefix
 
     with open(os.path.join(os.path.expanduser(folder), ADS_CONFIG_FILE_NAME), "w") as f:
         config_parser.write(f)
     print(f"Configuration saved at {os.path.join(folder, ADS_CONFIG_FILE_NAME)}")
 
-    print("==== Setting configuration for OCI Jobs ====")
+    print("==== Setting configuration for Data Science Jobs ====")
     if click.confirm(
-        f"Do you want to set up or update OCI Jobs configuration?", default=True
+        f"Do you want to set up or update Data Science Jobs configuration?",
+        default=True,
     ):
         required_fields = [
             ("compartment_id", ""),
             ("project_id", ""),
             ("subnet_id", ""),
             ("shape_name", ""),
             ("block_storage_size_in_GBs", ""),
@@ -576,17 +598,17 @@
             required_fields,
             optional_fields,
             folder,
             oci_config_path,
             is_in_notebook_session(),
         )
 
-    print("==== Setting configuration for OCI DataFlow ====")
+    print("==== Setting configuration for OCI Data Flow ====")
     if click.confirm(
-        f"Do you want to set up or update OCI DataFlow configuration?", default=True
+        f"Do you want to set up or update OCI Data Flow configuration?", default=True
     ):
         required_fields = [
             ("compartment_id", ""),
             ("driver_shape", ""),
             ("executor_shape", ""),
             ("logs_bucket_uri", ""),
             ("script_bucket", "in the format oci://<bucket>@<namespace>/<path>"),
@@ -624,14 +646,42 @@
             required_fields,
             optional_fields,
             folder,
             oci_config_path,
             is_in_notebook_session(),
         )
 
+    print("==== Setting configuration for Data Science Model Deployment ====")
+    if click.confirm(
+        f"Do you want to set up or update Data Science Model Deployment configuration?",
+        default=True,
+    ):
+        required_fields = [
+            ("compartment_id", ""),
+            ("project_id", ""),
+            ("shape_name", ""),
+        ]
+
+        optional_fields = [
+            ("log_group_id", ""),
+            ("log_id", ""),
+            ("bandwidth_mbps", ""),
+            ("replica", ""),
+            ("web_concurrency", ""),
+        ]
+
+        _set_service_configurations(
+            ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME,
+            required_fields,
+            optional_fields,
+            folder,
+            oci_config_path,
+            is_in_notebook_session(),
+        )
+
     print("==== Setting configuration for local backend ====")
     if click.confirm(
         f"Do you want to set up or update local backend configuration?", default=True
     ):
         required_fields = [
             ("max_parallel_containers", str(min(os.cpu_count(), 4))),
             ("pipeline_status_poll_interval_seconds", str(5)),
@@ -733,7 +783,67 @@
 
 
 def _get_backend_from_run_id(ocid: str) -> str:
     for value in DataScienceResourceRun.values():
         if value in ocid:
             return DATA_SCIENCE_RESOURCE_RUN_BACKEND_MAP[value]
     raise ValueError("Must provide a resource run OCID.")
+
+
+def init(
+    resource_type: str,
+    runtime_type: Union[str, None] = None,
+    output: Union[str, None] = None,
+    overwrite: bool = False,
+    ads_config: str = DEFAULT_ADS_CONFIG_FOLDER,
+    **kwargs,
+) -> Union[str, None]:
+    """
+    Generates a starter specification template YAML for the Data Science resource.
+
+    Parameters
+    ----------
+    resource_type: str
+        The resource type to generate the specification YAML.
+    runtime_type: (str, optional). Defaults to None.
+        The resource runtime type.
+    output: (str, optional). Defaults to None.
+        The path to the file to save the resulting specification template YAML.
+    overwrite: (bool, optional). Defaults to False.
+        Whether to overwrite the result specification YAML if exists.
+    ads_config: (str, optional)
+        The folder where the ads opctl config located.
+    kwargs: (Dict, optional).
+        Any optional kwargs arguments.
+
+    Returns
+    -------
+    Union[str, None]
+        The YAML specification for the given resource if `output` was not provided,
+        path to the specification otherwise.
+
+    Raises
+    ------
+    ValueError
+        If `resource_type` not specified.
+    """
+    if not resource_type:
+        raise ValueError(
+            f"The `resource_type` must be specified. Supported values: {RESOURCE_TYPE.values()}"
+        )
+
+    # get config info form INI files
+    p = ConfigProcessor({"execution": {"backend": resource_type}}).step(
+        ConfigMerger, ads_config=ads_config or DEFAULT_ADS_CONFIG_FOLDER, **kwargs
+    )
+
+    # generate YAML specification template
+    spec_yaml = _BackendFactory(p.config).backend.init(
+        uri=output, overwrite=overwrite, runtime_type=runtime_type, **kwargs
+    )
+
+    print("#" * 100)
+
+    if spec_yaml:
+        print(spec_yaml)
+    else:
+        print(output)
```

### Comparing `oracle_ads-2.8.3/ads/opctl/conda/cli.py` & `oracle_ads-2.8.4/ads/opctl/conda/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/conda/cmds.py` & `oracle_ads-2.8.4/ads/opctl/conda/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,18 @@
     auth_type : str
         authentication method
     Returns
     -------
     None
     """
     ns, bucket, path, slug = parse_conda_uri(conda_uri)
+    if bucket == "service-conda-packs":
+        raise ValueError(
+            "Download service conda pack is not allowed. Only custom conda pack can be downloaded to local machine. You need to publish it to your own bucket first."
+        )
     os.makedirs(conda_pack_folder, exist_ok=True)
     pack_path = os.path.join(os.path.expanduser(conda_pack_folder), slug + ".tar.gz")
     pack_folder_path = os.path.join(os.path.expanduser(conda_pack_folder), slug)
 
     if not (is_in_notebook_session() or NO_CONTAINER):
         _check_job_image_exists(gpu=False)
```

### Comparing `oracle_ads-2.8.3/ads/opctl/conda/config.yaml` & `oracle_ads-2.8.4/ads/opctl/conda/config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/conda/multipart_uploader.py` & `oracle_ads-2.8.4/ads/opctl/conda/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/conda/pack.py` & `oracle_ads-2.8.4/ads/opctl/conda/pack.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/base.py` & `oracle_ads-2.8.4/ads/opctl/config/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml` & `oracle_ads-2.8.4/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/merger.py` & `oracle_ads-2.8.4/ads/opctl/config/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     DEFAULT_CONDA_PACK_FOLDER,
     DEFAULT_ADS_CONFIG_FOLDER,
     ADS_JOBS_CONFIG_FILE_NAME,
     ADS_CONFIG_FILE_NAME,
     ADS_ML_PIPELINE_CONFIG_FILE_NAME,
     ADS_DATAFLOW_CONFIG_FILE_NAME,
     ADS_LOCAL_BACKEND_CONFIG_FILE_NAME,
+    ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME,
     DEFAULT_NOTEBOOK_SESSION_CONDA_DIR,
     BACKEND_NAME,
 )
 
 
 class ConfigMerger(ConfigProcessor):
     """Merge configurations from command line args, YAML, ini and default configs.
@@ -174,17 +175,19 @@
                 f"{os.path.join(ads_config_folder, 'config.ini')} does not exist. No config loaded."
             )
             return {}
 
     def _get_service_config(self, oci_profile: str, ads_config_folder: str) -> Dict:
         backend = self.config["execution"].get("backend", None)
         backend_config = {
+            BACKEND_NAME.JOB.value: ADS_JOBS_CONFIG_FILE_NAME,
             BACKEND_NAME.DATAFLOW.value: ADS_DATAFLOW_CONFIG_FILE_NAME,
             BACKEND_NAME.PIPELINE.value: ADS_ML_PIPELINE_CONFIG_FILE_NAME,
             BACKEND_NAME.LOCAL.value: ADS_LOCAL_BACKEND_CONFIG_FILE_NAME,
+            BACKEND_NAME.MODEL_DEPLOYMENT.value: ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME,
         }
         config_file = backend_config.get(backend, ADS_JOBS_CONFIG_FILE_NAME)
 
         if os.path.exists(os.path.join(ads_config_folder, config_file)):
             parser = read_from_ini(os.path.join(ads_config_folder, config_file))
             if oci_profile in parser:
                 return parser[oci_profile]
```

### Comparing `oracle_ads-2.8.3/ads/opctl/config/resolver.py` & `oracle_ads-2.8.4/ads/opctl/config/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,19 @@
                 )
             else:
                 self.config["execution"]["source_folder"] = None
 
     def _resolve_entry_script(self) -> None:
         # this should be run after _resolve_source_folder_path
         if not self._is_ads_operator():
-            if os.path.splitext(self.config["execution"]["entrypoint"])[1] == ".ipynb":
+            if (
+                self.config["execution"].get("entrypoint")
+                and os.path.splitext(self.config["execution"]["entrypoint"])[1]
+                == ".ipynb"
+            ):
                 input_path = os.path.join(
                     self.config["execution"]["source_folder"],
                     self.config["execution"]["entrypoint"],
                 )
                 exclude_tags = self.config["execution"].get("exclude_tag")
                 self.config["execution"]["entrypoint"] = os.path.basename(
                     convert_notebook(
```

### Comparing `oracle_ads-2.8.3/ads/opctl/config/utils.py` & `oracle_ads-2.8.4/ads/opctl/config/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 import fsspec
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 
 
-class OperatorNotFound(Exception):
+class OperatorNotFound(Exception):   # pragma: no cover
     pass
 
 
-class CondaPackInfoNotProvided(Exception):
+class CondaPackInfoNotProvided(Exception):   # pragma: no cover
     pass
 
 
-class NotSupportedError(Exception):
+class NotSupportedError(Exception):   # pragma: no cover
     pass
 
 
 class _DefaultNoneDict(dict):
     def __missing__(self, key):
         return ""
```

### Comparing `oracle_ads-2.8.3/ads/opctl/config/validator.py` & `oracle_ads-2.8.4/ads/opctl/config/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/versioner.py` & `oracle_ads-2.8.4/ads/opctl/config/versioner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/base.py` & `oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py` & `oracle_ads-2.8.4/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/constants.py` & `oracle_ads-2.8.4/ads/opctl/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,59 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
-from enum import Enum
+from ads.common.extended_enum import ExtendedEnum
 
 DEFAULT_OCI_CONFIG_FILE = "~/.oci/config"
 DEFAULT_PROFILE = "DEFAULT"
 DEFAULT_CONDA_PACK_FOLDER = "~/conda"
+DEFAULT_MODEL_FOLDER = "~/.ads_ops/models"
 CONDA_PACK_OS_PREFIX_FORMAT = "oci://<bucket>@<namespace>/<prefix>"
 DEFAULT_ADS_CONFIG_FOLDER = "~/.ads_ops"
 OPS_IMAGE_BASE = "ads-operators-base"
 ML_JOB_IMAGE = "ml-job"
 ML_JOB_GPU_IMAGE = "ml-job-gpu"
 OPS_IMAGE_GPU_BASE = "ads-operators-gpu-base"
 DEFAULT_MANIFEST_VERSION = "1.0"
 ADS_CONFIG_FILE_NAME = "config.ini"
 ADS_JOBS_CONFIG_FILE_NAME = "ml_job_config.ini"
 ADS_DATAFLOW_CONFIG_FILE_NAME = "dataflow_config.ini"
 ADS_ML_PIPELINE_CONFIG_FILE_NAME = "ml_pipeline.ini"
 ADS_LOCAL_BACKEND_CONFIG_FILE_NAME = "local_backend.ini"
+ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME = "model_deployment_config.ini"
 DEFAULT_IMAGE_HOME_DIR = "/home/datascience"
 DEFAULT_IMAGE_SCRIPT_DIR = "/etc/datascience"
 DEFAULT_IMAGE_CONDA_DIR = "/opt/conda/envs"
 DEFAULT_NOTEBOOK_SESSION_SPARK_CONF_DIR = "/home/datascience/spark_conf_dir"
 DEFAULT_NOTEBOOK_SESSION_CONDA_DIR = "/home/datascience/conda"
+DEFAULT_SPECIFICATION_FILE_NAME = "oci-datascience-template.yaml"
+DEFAULT_MODEL_DEPLOYMENT_FOLDER = "/opt/ds/model/deployed_model/"
 
 
-class BACKEND_NAME(Enum):
+class RUNTIME_TYPE(ExtendedEnum):
+    PYTHON = "python"
+    CONTAINER = "container"
+    NOTEBOOK = "notebook"
+    GITPYTHON = "gitPython"
+    OPERATOR = "operator"
+    SCRIPT = "script"
+    DATAFLOW = "dataFlow"
+    DATAFLOWNOTEBOOK = "dataFlowNotebook"
+    CONDA = "conda"
+
+
+class RESOURCE_TYPE(ExtendedEnum):
+    JOB = "job"
+    DATAFLOW = "dataflow"
+    PIPELINE = "pipeline"
+    MODEL_DEPLOYMENT = "deployment"
+
+
+class BACKEND_NAME(ExtendedEnum):
     JOB = "job"
     DATAFLOW = "dataflow"
     PIPELINE = "pipeline"
     MODEL_DEPLOYMENT = "deployment"
     LOCAL = "local"
```

### Comparing `oracle_ads-2.8.3/ads/opctl/diagnostics/__main__.py` & `oracle_ads-2.8.4/ads/opctl/diagnostics/__main__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/diagnostics/check_distributed_job_requirements.py` & `oracle_ads-2.8.4/ads/opctl/diagnostics/check_distributed_job_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/diagnostics/check_requirements.py` & `oracle_ads-2.8.4/ads/opctl/diagnostics/check_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/certificates.py` & `oracle_ads-2.8.4/ads/opctl/distributed/certificates.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/cli.py` & `oracle_ads-2.8.4/ads/opctl/distributed/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/cmds.py` & `oracle_ads-2.8.4/ads/opctl/distributed/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/abstract_cluster_provider.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_cluster_provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/abstract_framework_spec_builder.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/abstract_framework_spec_builder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_config_helper.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_config_helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_provider_factory.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_provider_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/cluster_runner.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/cluster_runner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/distributed/common/framework_factory.py` & `oracle_ads-2.8.4/ads/opctl/distributed/common/framework_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/docker/Dockerfile` & `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.gpu` & `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.job` & `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/docker/Dockerfile.job.gpu` & `oracle_ads-2.8.4/ads/opctl/docker/Dockerfile.job.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/docker/merge_dependencies.py` & `oracle_ads-2.8.4/ads/opctl/docker/merge_dependencies.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/spark/cli.py` & `oracle_ads-2.8.4/ads/opctl/spark/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/spark/cmds.py` & `oracle_ads-2.8.4/ads/opctl/spark/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/spec/abstract_operator_spec.py` & `oracle_ads-2.8.4/ads/opctl/spec/abstract_operator_spec.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/spec/operator_spec_factory.py` & `oracle_ads-2.8.4/ads/opctl/spec/operator_spec_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/templates/diagnostic_report_template.jinja2` & `oracle_ads-2.8.4/ads/opctl/templates/diagnostic_report_template.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/opctl/utils.py` & `oracle_ads-2.8.4/ads/opctl/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 
 import functools
 import logging
 import os
 import subprocess
 import sys
+import shlex
 import tempfile
 import urllib.parse
 from distutils import dir_util
 from subprocess import Popen, PIPE, STDOUT
 from typing import Union, List, Tuple, Dict
-import shlex
 import yaml
 
 import ads
 from ads.common.oci_client import OCIClientFactory
 from ads.opctl import logger
 from ads.opctl.constants import (
     ML_JOB_IMAGE,
@@ -29,14 +29,17 @@
 )
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 
 
+CONTAINER_NETWORK = "CONTAINER_NETWORK"
+
+
 def get_service_pack_prefix() -> Dict:
     curr_dir = os.path.dirname(os.path.abspath(__file__))
     service_config_file = os.path.join(curr_dir, "conda", "config.yaml")
     with open(service_config_file) as f:
         service_config = yaml.safe_load(f.read())
     if all(key in os.environ for key in ["CONDA_BUCKET_NS", "CONDA_BUCKET_NAME"]):
         bucket_info = {
@@ -171,19 +174,21 @@
             command += ["--target", target]
         if os.environ.get("no_proxy"):
             command += ["--build-arg", f"no_proxy={os.environ['no_proxy']}"]
         if os.environ.get("http_proxy"):
             command += ["--build-arg", f"http_proxy={os.environ['http_proxy']}"]
         if os.environ.get("https_proxy"):
             command += ["--build-arg", f"https_proxy={os.environ['https_proxy']}"]
+        if os.environ.get(CONTAINER_NETWORK):
+            command += ["--network", os.environ[CONTAINER_NETWORK]]
         command += [os.path.abspath(curr_dir)]
-        logger.info(f"Build image with command {command}")
+        logger.info("Build image with command %s", command)
         proc = run_command(command)
     if proc.returncode != 0:
-        raise RuntimeError(f"Docker build failed.")
+        raise RuntimeError("Docker build failed.")
 
 
 def _get_image_name_dockerfile_target(type: str, gpu: bool) -> str:
     look_up = {
         ("job-local", False): (ML_JOB_IMAGE, "Dockerfile.job", None),
         ("job-local", True): (ML_JOB_GPU_IMAGE, "Dockerfile.job.gpu", None),
         ("ads-ops-base", False): (OPS_IMAGE_BASE, "Dockerfile", "base"),
@@ -317,31 +322,55 @@
         ads.opctl.logger.setLevel(logging.INFO)
     logger.info(f"Running container with image: {image}")
     logger.info(f"bind_volumes: {bind_volumes}")
     logger.info(f"env_vars: {env_vars}")
     logger.info(f"command: {command}")
     logger.info(f"entrypoint: {entrypoint}")
 
+    # Print out the equivalent docker run command for debugging purpose
+    docker_run_cmd = [">>> docker run --rm"]
+    if entrypoint:
+        docker_run_cmd.append(f"--entrypoint {entrypoint}")
+    if env_vars:
+        docker_run_cmd.extend([f"-e {key}={val}" for key, val in env_vars.items()])
+    if bind_volumes:
+        docker_run_cmd.extend(
+            [f'-v {source}:{bind.get("bind")}' for source, bind in bind_volumes.items()]
+        )
+    docker_run_cmd.append(image)
+    if command:
+        docker_run_cmd.append(command)
+    logger.debug(" ".join(docker_run_cmd))
+
     client = get_docker_client()
     try:
         client.api.inspect_image(image)
     except docker.errors.ImageNotFound:
-        logger.warn(f"Image {image} not found. Try pulling it now....")
+        logger.warning(f"Image {image} not found. Try pulling it now....")
         run_command(["docker", "pull", f"{image}"], None)
-    container = client.containers.run(
-        image=image,
-        volumes=bind_volumes,
-        command=shlex.split(command) if command else None,
-        environment=env_vars,
-        detach=True,
-        entrypoint=entrypoint,
-        user=0,
-        # auto_remove=True,
-    )
-    logger.info(f"Container ID: {container.id}")
-
-    for line in container.logs(stream=True, follow=True):
-        logger.info(line.decode("utf-8").strip())
-
-    result = container.wait()
-    container.remove()
-    return result.get("StatusCode", -1)
+    try:
+        kwargs = {}
+        if CONTAINER_NETWORK in os.environ:
+            kwargs["network_mode"] = os.environ[CONTAINER_NETWORK]
+        container = client.containers.run(
+            image=image,
+            volumes=bind_volumes,
+            command=shlex.split(command) if command else None,
+            environment=env_vars,
+            detach=True,
+            entrypoint=entrypoint,
+            user=0,
+            **kwargs
+            # auto_remove=True,
+        )
+        logger.info("Container ID: %s", container.id)
+        for line in container.logs(stream=True, follow=True):
+            print(line.decode("utf-8"), end="")
+
+        result = container.wait()
+        return result.get("StatusCode", -1)
+    except docker.errors.APIError as ex:
+        logger.error(ex.explanation)
+        return -1
+    finally:
+        # Remove the container
+        container.remove()
```

### Comparing `oracle_ads-2.8.3/ads/oracledb/oracle_db.py` & `oracle_ads-2.8.4/ads/oracledb/oracle_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/__init__.py` & `oracle_ads-2.8.4/ads/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/ads_pipeline.py` & `oracle_ads-2.8.4/ads/pipeline/ads_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 # Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import copy
 import datetime
 import logging
 import os
+import traceback
+from typing import Any, Dict, List, Optional
+
 import fsspec
 import oci
-from typing import Any, Dict, List, Optional
-from ads.common.oci_datascience import OCIDataScienceMixin
+import oci.util as oci_util
+
+from ads.common import utils
+from ads.common.oci_datascience import DSCNotebookSession, OCIDataScienceMixin
 from ads.common.oci_logging import OCILog
 from ads.common.oci_resource import ResourceNotFoundError
-from ads.common import utils
+from ads.config import COMPARTMENT_OCID, NB_SESSION_OCID, PROJECT_OCID
 from ads.jobs.builders.base import Builder
-from ads.jobs.builders.infrastructure.dsc_job import DSCJob, DataScienceJob
+from ads.jobs.builders.infrastructure.dsc_job import DataScienceJob, DSCJob
 from ads.jobs.builders.infrastructure.dsc_job_runtime import (
     DataScienceJobRuntimeManager,
 )
 from ads.jobs.builders.runtimes.artifact import Artifact
-from ads.pipeline.ads_pipeline_step import PipelineStep
-from ads.pipeline.ads_pipeline_run import PipelineRun
-from ads.pipeline.visualizer.base import PipelineVisualizer, GraphOrientation
-from ads.pipeline.visualizer.graph_renderer import PipelineGraphRenderer
 from ads.jobs.builders.runtimes.python_runtime import (
-    CondaRuntime,
-    ScriptRuntime,
-    PythonRuntime,
-    NotebookRuntime,
     GitPythonRuntime,
+    NotebookRuntime,
+    PythonRuntime,
+    ScriptRuntime,
 )
+from ads.pipeline.ads_pipeline_run import PipelineRun
+from ads.pipeline.ads_pipeline_step import PipelineStep
+from ads.pipeline.visualizer.base import GraphOrientation, PipelineVisualizer
+from ads.pipeline.visualizer.graph_renderer import PipelineGraphRenderer
 
 logger = logging.getLogger(__name__)
 
 MAXIMUM_TIMEOUT = 1800
 DEFAULT_WAITER_KWARGS = {"max_wait_seconds": MAXIMUM_TIMEOUT}
 DEFAULT_OPERATION_KWARGS = {
     "delete_related_pipeline_runs": True,
@@ -351,14 +355,54 @@
         if "dag" in kwargs:
             self.with_dag(kwargs.get("dag"))
         elif spec and "dag" in spec:
             self.with_dag(spec.get("dag"))
         self.data_science_pipeline = None
         self.service_logging = None
 
+    def _load_default_properties(self) -> Dict:
+        """Load default properties from environment variables, notebook session, etc.
+
+        Returns
+        -------
+        Dict
+            A dictionary of default properties.
+        """
+        defaults = super()._load_default_properties()
+        if COMPARTMENT_OCID:
+            defaults[self.CONST_COMPARTMENT_ID] = COMPARTMENT_OCID
+        if PROJECT_OCID:
+            defaults[self.CONST_PROJECT_ID] = PROJECT_OCID
+
+        if NB_SESSION_OCID:
+            try:
+                nb_session = DSCNotebookSession.from_ocid(NB_SESSION_OCID)
+                nb_config = nb_session.notebook_session_configuration_details
+                defaults[self.CONST_SHAPE_NAME] = nb_config.shape
+                defaults[
+                    self.CONST_BLOCK_STORAGE_SIZE
+                ] = nb_config.block_storage_size_in_gbs
+
+                if nb_config.notebook_session_shape_config_details:
+                    notebook_shape_config_details = oci_util.to_dict(
+                        nb_config.notebook_session_shape_config_details
+                    )
+                    defaults[self.CONST_SHAPE_CONFIG_DETAILS] = copy.deepcopy(
+                        notebook_shape_config_details
+                    )
+
+            except Exception as e:
+                logger.warning(
+                    f"Error fetching details about Notebook "
+                    f"session: {NB_SESSION_OCID}. {e}"
+                )
+                logger.debug(traceback.format_exc())
+
+        return defaults
+
     @property
     def kind(self) -> str:
         """The kind of the object as showing in YAML.
 
         Returns
         -------
         str
@@ -959,23 +1003,23 @@
         Returns
         -------
         str:
             The service log id of pipeline.
         """
         return self.get_spec(self.CONST_SERVICE_LOG_ID)
 
-    def to_dict(self) -> dict:
+    def to_dict(self, **kwargs) -> dict:
         """Serializes the pipeline specifications to a dictionary.
 
         Returns
         -------
         dict
             A dictionary containing pipeline specifications.
         """
-        dict_details = copy.deepcopy(super().to_dict())
+        dict_details = copy.deepcopy(super().to_dict(**kwargs))
         dict_details["spec"][self.CONST_DAG] = self.get_spec(self.CONST_DAG)
 
         step_details_list = []
         if self.step_details:
             for step in self.step_details:
                 if isinstance(step, PipelineStep):
                     step = step.to_dict()
@@ -1933,14 +1977,29 @@
         str
             Status of the pipeline.
         """
         if self.data_science_pipeline:
             return self.data_science_pipeline.lifecycle_state
         return None
 
+    def init(self) -> "Pipeline":
+        """Initializes a starter specification for the Pipeline.
+
+        Returns
+        -------
+        Pipeline
+            The Pipeline instance (self)
+        """
+        return (
+            self.build()
+            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
+            .with_project_id(self.project_id or "{Provide a project OCID}")
+        )
+
+
 
 class DataSciencePipeline(OCIDataScienceMixin, oci.data_science.models.Pipeline):
     @classmethod
     def from_ocid(cls, ocid: str) -> "DataSciencePipeline":
         """Gets a datascience pipeline by OCID.
 
         Parameters
@@ -2214,8 +2273,8 @@
             wait_for_states=[
                 oci.data_science.models.WorkRequest.STATUS_SUCCEEDED,
                 oci.data_science.models.WorkRequest.STATUS_FAILED,
             ],
             operation_kwargs=operation_kwargs,
             waiter_kwargs=waiter_kwargs,
         )
-        return self.sync()
+        return self.sync()
```

### Comparing `oracle_ads-2.8.3/ads/pipeline/ads_pipeline_run.py` & `oracle_ads-2.8.4/ads/pipeline/ads_pipeline_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 class StepType(str, metaclass=ExtendedEnumMeta):
     ML_JOB = "ML_JOB"
     CUSTOM_SCRIPT = "CUSTOM_SCRIPT"
 
 
-class LogNotConfiguredError(Exception):
+class LogNotConfiguredError(Exception):   # pragma: no cover
     pass
 
 
 class PipelineRun(
     OCIDataScienceMixin, oci.data_science.models.PipelineRun, RunInstance
 ):
     """
```

### Comparing `oracle_ads-2.8.3/ads/pipeline/ads_pipeline_step.py` & `oracle_ads-2.8.4/ads/pipeline/ads_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/builders/infrastructure/custom_script.py` & `oracle_ads-2.8.4/ads/pipeline/builders/infrastructure/custom_script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/cli.py` & `oracle_ads-2.8.4/ads/pipeline/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/extension.py` & `oracle_ads-2.8.4/ads/pipeline/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/visualizer/base.py` & `oracle_ads-2.8.4/ads/pipeline/visualizer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datetime import datetime, timezone
 from typing import ByteString, Dict, List, Optional, Union
 
 import fsspec
 from oci.data_science.models.pipeline_step_run import PipelineStepRun
 
 
-class PipelineVisualizerError(Exception):
+class PipelineVisualizerError(Exception):   # pragma: no cover
     pass
 
 
 class StepStatus:
     WAITING = "WAITING"
     ACCEPTED = "ACCEPTED"
     IN_PROGRESS = "IN_PROGRESS"
```

### Comparing `oracle_ads-2.8.3/ads/pipeline/visualizer/graph_renderer.py` & `oracle_ads-2.8.4/ads/pipeline/visualizer/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/pipeline/visualizer/text_renderer.py` & `oracle_ads-2.8.4/ads/pipeline/visualizer/text_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/adb.py` & `oracle_ads-2.8.4/ads/secrets/adb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/auth_token.py` & `oracle_ads-2.8.4/ads/secrets/auth_token.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/big_data_service.py` & `oracle_ads-2.8.4/ads/secrets/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/mysqldb.py` & `oracle_ads-2.8.4/ads/secrets/mysqldb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/oracledb.py` & `oracle_ads-2.8.4/ads/secrets/oracledb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/secrets/secrets.py` & `oracle_ads-2.8.4/ads/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/telemetry/telemetry.py` & `oracle_ads-2.8.4/ads/telemetry/telemetry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 #!/usr/bin/env python
-# -*- coding: utf-8; -*-
+# -*- coding: utf-8 -*--
 
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
-from ads import __version__
+
+import os
 from enum import Enum, auto
+from typing import Any, Dict, Optional
 
 import ads.config
+from ads import __version__
+from ads.common import logger
 
+LIBRARY = "Oracle-ads"
 EXTRA_USER_AGENT_INFO = "EXTRA_USER_AGENT_INFO"
 USER_AGENT_KEY = "additional_user_agent"
-ENV_MD_OCID = "MD_OCID"
 UNKNOWN = "UNKNOWN"
 
 
 class Surface(Enum):
     """
-    An Enum class for labeling the surface where ADS is being used
+    An Enum class for labeling the surface where ADS is being used.
     """
 
     WORKSTATION = auto()
     DATASCIENCE_JOB = auto()
     DATASCIENCE_NOTEBOOK = auto()
     DATASCIENCE_MODEL_DEPLOYMENT = auto()
     DATAFLOW = auto()
     OCI_SERVICE = auto()
+    DATASCIENCE_PIPELINE = auto()
 
     @classmethod
     def surface(cls):
         surface = cls.WORKSTATION
         if (
             ads.config.OCI_RESOURCE_PRINCIPAL_VERSION
             or ads.config.OCI_RESOURCE_PRINCIPAL_RPT_PATH
@@ -39,16 +44,37 @@
                 surface = cls.DATASCIENCE_JOB
             elif ads.config.NB_SESSION_OCID:
                 surface = cls.DATASCIENCE_NOTEBOOK
             elif ads.config.MD_OCID:
                 surface = cls.DATASCIENCE_MODEL_DEPLOYMENT
             elif ads.config.DATAFLOW_RUN_OCID:
                 surface = cls.DATAFLOW
+            elif ads.config.PIPELINE_RUN_OCID:
+                surface = cls.DATASCIENCE_PIPELINE
         return surface
 
 
-def update_oci_client_config(config={}):
-    if not config.get(USER_AGENT_KEY):
-        config[
-            USER_AGENT_KEY
-        ] = f"Oracle-ads/version={__version__}/surface={Surface.surface().name}"  # To be enabled in future - /api={os.environ.get(EXTRA_USER_AGENT_INFO,UNKNOWN)}"
+def update_oci_client_config(config: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
+    """Adds user agent information to the config if it is not setup yet.
+
+    Returns
+    -------
+    Dict
+        The updated configuration.
+    """
+
+    try:
+        config = config or {}
+        if not config.get(USER_AGENT_KEY):
+            config.update(
+                {
+                    USER_AGENT_KEY: (
+                        f"{LIBRARY}/version={__version__}#"
+                        f"surface={Surface.surface().name}#"
+                        f"api={os.environ.get(EXTRA_USER_AGENT_INFO,UNKNOWN) or UNKNOWN}"
+                    )
+                }
+            )
+    except Exception as ex:
+        logger.debug(ex)
+
     return config
```

### Comparing `oracle_ads-2.8.3/ads/templates/score-pkl.jinja2` & `oracle_ads-2.8.4/ads/templates/score-pkl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score.jinja2` & `oracle_ads-2.8.4/ads/templates/score.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_generic.jinja2` & `oracle_ads-2.8.4/ads/templates/score_generic.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_huggingface_pipeline.jinja2` & `oracle_ads-2.8.4/ads/templates/score_huggingface_pipeline.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_lightgbm.jinja2` & `oracle_ads-2.8.4/ads/templates/score_lightgbm.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_onnx.jinja2` & `oracle_ads-2.8.4/ads/templates/score_onnx.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_onnx_new.jinja2` & `oracle_ads-2.8.4/ads/templates/score_onnx_new.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_oracle_automl.jinja2` & `oracle_ads-2.8.4/ads/templates/score_oracle_automl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_pyspark.jinja2` & `oracle_ads-2.8.4/ads/templates/score_pyspark.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -28,18 +28,17 @@
     """
     Loads model from the serialized format
 
     Returns
     -------
     model:  a model instance on which predict API can be invoked
     """
-    model_dir = os.path.dirname(os.path.realpath(__file__))
+    model_dir = os.environ.get("OCI_DEPLOYMENT_PATH", os.path.dirname(os.path.realpath(__file__)))
     if model_dir not in sys.path:
         sys.path.insert(0, model_dir)
-    contents = os.listdir(model_dir)
     try:
         print(f'Start loading {model_file_name} from model directory {model_dir} ...')
         loaded_model = PipelineModel.load(os.path.join(model_dir, model_file_name))
         print("Model is successfully loaded.")
         return loaded_model
     except Exception as e:
         error_msg = f"Failed to load the model and gave the exception: {e}."
```

### Comparing `oracle_ads-2.8.3/ads/templates/score_pytorch.jinja2` & `oracle_ads-2.8.4/ads/templates/score_pytorch.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,29 @@
 import json
 from typing import Dict, List
 import numpy as np
 import pandas as pd
 from io import BytesIO
 import base64
 import logging
+from random import randint
+
+
+def get_torch_device():
+    num_devices = torch.cuda.device_count()
+    if num_devices == 0:
+        return "cpu"
+    if num_devices == 1:
+        return "cuda:0"
+    else:
+        return f"cuda:{randint(0, num_devices-1)}"
+
 
 model_name = '{{model_file_name}}'
+device = torch.device(get_torch_device())
 
 """
    Inference script. This script is used for prediction by scoring server when schema is known.
 """
 
 @lru_cache(maxsize=10)
 def load_model(model_file_name=model_name):
@@ -55,14 +68,15 @@
 
     the_model.eval()
 {% else %}
     raise NotImplementedError("`load_model()` needs to be implemented.")
 
 {% endif %}
     print("Model is successfully loaded.")
+    the_model = the_model.to(device)
     return the_model
 
 @lru_cache(maxsize=1)
 def fetch_data_type_from_schema(input_schema_path=os.path.join(os.path.dirname(os.path.realpath(__file__)), "input_schema.json")):
     """
     Returns data type information fetch from input_schema.json.
 
@@ -154,14 +168,15 @@
     Returns
     -------
     data: Data format after any processing.
     """
     data = deserialize(data, input_schema_path)
 
     # Add further data preprocessing if needed
+    data = data.to(device)
     return data
 
 def post_inference(yhat):
     """
     Post-process the model results.
 
     Parameters
@@ -195,10 +210,10 @@
         Format: {'prediction': output from model.predict method}
 
     """
     inputs = pre_inference(data, input_schema_path)
 
     with torch.no_grad():
         yhat = post_inference(
-        model(inputs)
+        model(inputs).to("cpu")
     )
     return {'prediction': yhat}
```

### Comparing `oracle_ads-2.8.3/ads/templates/score_scikit-learn.jinja2` & `oracle_ads-2.8.4/ads/templates/score_scikit-learn.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/templates/score_spark.jinja2` & `oracle_ads-2.8.4/ads/templates/score_xgboost.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,53 @@
+# score.py {{SCORE_VERSION}} generated by ADS {{ADS_VERSION}} on {{time_created}}
+import json
 import os
 import sys
-import json
+import xgboost as xgb
+import pandas as pd
+import numpy as np
 from functools import lru_cache
-from collections.abc import Iterable
+from io import BytesIO
+import base64
+import logging
+
+model_name = '{{model_file_name}}'
 
-# Importing pyspark libraries
-from pyspark.ml.pipeline import PipelineModel
-from pyspark.sql import SparkSession
-from pyspark.sql.types import StructType
 
 """
    Inference script. This script is used for prediction by scoring server when schema is known.
 """
 
-model_name = '{{model_file_name}}'
-spark_input_schema = model_name + "_input_data_schema.json"
-
-spark = SparkSession \
-    .builder \
-    .appName('Spark Model Inference') \
-    .getOrCreate()
-
 
 @lru_cache(maxsize=10)
 def load_model(model_file_name=model_name):
     """
     Loads model from the serialized format
 
     Returns
     -------
     model:  a model instance on which predict API can be invoked
     """
+    model_xgb = xgb.Booster()
     model_dir = os.path.dirname(os.path.realpath(__file__))
     if model_dir not in sys.path:
         sys.path.insert(0, model_dir)
     contents = os.listdir(model_dir)
-    try:
-        print(f'Start loading {model_file_name} from model directory {model_dir} ...')
-        loaded_model = PipelineModel.load(os.path.join(model_dir, model_file_name))
-        print("Model is successfully loaded.")
-        return loaded_model
-    except Exception as e:
-        error_msg = f"Failed to load the model and gave the exception: {e}."
-        raise Exception(error_msg)
+    if model_file_name not in contents:
+        raise Exception(f'{model_file_name} is not found in model directory {model_dir}')
+
+{% if model_serializer == "xgboost" %}
+    print(f'Start loading {model_file_name} from model directory {model_dir} ...')
+    model_xgb.load_model(os.path.join(os.path.dirname(os.path.realpath(__file__)), model_file_name))
+    print("Model is successfully loaded.")
+    return model_xgb
+
+{% else %}
+    raise NotImplementedError("`load_model()` needs to be implemented.")
+{% endif %}
 
 @lru_cache(maxsize=1)
 def fetch_data_type_from_schema(input_schema_path=os.path.join(os.path.dirname(os.path.realpath(__file__)), "input_schema.json")):
     """
     Returns data type information fetch from input_schema.json.
 
     Parameters
@@ -60,46 +61,73 @@
     """
     data_type = {}
     if os.path.exists(input_schema_path):
         schema = json.load(open(input_schema_path))
         for col in schema['schema']:
             data_type[col['name']] = col['dtype']
     else:
-        print("input_schema has to be passed in in order to recover the same data type. pass `X_sample` in `ads.model.framework.spark_model.SparkPipelineModel.prepare` function to generate the input_schema. Otherwise, the data type might be changed after serialization/deserialization.")
+        print("input_schema has to be passed in in order to recover the same data type. pass `X_sample` in `ads.model.framework.xgboost_model.XGBoostModel.prepare` function to generate the input_schema. Otherwise, the data type might be changed after serialization/deserialization.")
     return data_type
 
+
 def deserialize(data, input_schema_path):
     """
     Deserialize json serialization data to data in original type when sent to predict.
 
     Parameters
     ----------
     data: serialized input data.
     input_schema_path: path of input schema.
 
     Returns
     -------
     data: deserialized input data.
 
     """
+{% if data_deserializer == "json" %}
+    if isinstance(data, bytes):
+        logging.warning(
+            "bytes are passed directly to the model. If the model expects a specific data format, you need to write the conversion logic in `deserialize()` yourself."
+        )
+        return data
+
     data_type = data.get('data_type', '') if isinstance(data, dict) else ''
     json_data = data.get('data', data) if isinstance(data, dict) else data
 
-    spark_schema_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), spark_input_schema)
-    with open(spark_schema_path) as f:
-        spark_schema = StructType.fromJson(json.loads(f.read()))
+    if "numpy.ndarray" in data_type:
+        load_bytes = BytesIO(base64.b64decode(json_data.encode('utf-8')))
+        return np.load(load_bytes, allow_pickle=True)
+    if "pandas.core.series.Series" in data_type:
+        return pd.Series(json_data)
+    if "pandas.core.frame.DataFrame" in data_type or isinstance(json_data, str):
+        return pd.read_json(json_data, dtype=fetch_data_type_from_schema(input_schema_path))
+    if isinstance(json_data, dict):
+        return pd.DataFrame.from_dict(json_data)
+
+    return json_data
+
+{% elif data_deserializer == "cloudpickle" %}
+    import cloudpickle
+    from pickle import UnpicklingError
+    deserialized_data = data
+    try:
+        deserialized_data = cloudpickle.loads(data)
+    except TypeError:
+        pass
+    except UnpicklingError:
+        logger.warning(
+            "bytes are passed directly to the model. If the model expects a specific data format, you need to write the conversion logic in `deserialize()` yourself."
+        )
 
-    if isinstance(json_data, str) or not isinstance(json_data, Iterable):
-        json_data = [json_data]
+    return deserialized_data
 
-    try:
-        rdd_data = spark.sparkContext.parallelize(json_data)
-        return spark.read.json(rdd_data, schema=spark_schema)
-    except:
-        raise TypeError(f"Unsupported data_type: {data_type} or failed to load data with provided spark schema: {spark_schema}. Only supported data types are: pyspark.sql.dataframe.DataFrame, pyspark.pandas.dataframe.DataFrame, pandas.DataFrame, json")
+{% else %}
+    # Add further data deserialization if needed
+    return data
+{% endif %}
 
 def pre_inference(data, input_schema_path):
     """
     Preprocess data
 
     Parameters
     ----------
@@ -110,45 +138,41 @@
     -------
     data: Data format after any processing.
 
     """
     data = deserialize(data, input_schema_path)
     return data
 
-def post_inference(yhat, input_cols):
+def post_inference(yhat):
     """
     Post-process the model results
 
     Parameters
     ----------
     yhat: Data format after calling model.predict.
 
     Returns
     -------
     yhat: Data format after any processing.
 
     """
-    return yhat.toPandas()['prediction'].to_list()
+    return yhat.tolist()
 
 def predict(data, model=load_model(), input_schema_path=os.path.join(os.path.dirname(os.path.realpath(__file__)), "input_schema.json")):
     """
     Returns prediction given the model and data to predict
 
     Parameters
     ----------
     model: Model instance returned by load_model API
-    data: Data format as expected by the predict API of the core estimator. For eg. in case of sckit models it could be numpy array/List of list/Pandas DataFrame
+    data: Data format as expected by the predict API of the core estimator. For eg. in case xgboost models it could be numpy array/List of list/Pandas DataFrame
     input_schema_path: path of input schema.
 
     Returns
     -------
     predictions: Output from scoring server
         Format: {'prediction': output from model.predict method}
 
     """
-
-    input = pre_inference(data, input_schema_path)
-    input_cols = input.columns
-    print("Dataset Count: " + str(input.count()))
-
-    yhat = post_inference(model.transform(input), input_cols)
-    return {'prediction': yhat}
+    data = pre_inference(data, input_schema_path)
+    data = xgb.DMatrix(data)
+    return {'prediction': post_inference(model.predict(data))}
```

### Comparing `oracle_ads-2.8.3/ads/templates/score_tensorflow.jinja2` & `oracle_ads-2.8.4/ads/templates/score_tensorflow.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/backends.py` & `oracle_ads-2.8.4/ads/text_dataset/backends.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/dataset.py` & `oracle_ads-2.8.4/ads/text_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/extractor.py` & `oracle_ads-2.8.4/ads/text_dataset/extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/options.py` & `oracle_ads-2.8.4/ads/text_dataset/options.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/udfs.py` & `oracle_ads-2.8.4/ads/text_dataset/udfs.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/text_dataset/utils.py` & `oracle_ads-2.8.4/ads/text_dataset/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2021, 2022 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import functools
 import os
 
 
-class NotSupportedError(Exception):
+class NotSupportedError(Exception):   # pragma: no cover
     pass
 
 
 def experimental(cls):
     @functools.wraps(cls)
     def wrapper(*args, **kwargs):
         instance = cls(*args, **kwargs)
```

### Comparing `oracle_ads-2.8.3/ads/type_discovery/abstract_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/abstract_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/constant_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/constant_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/continuous_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/continuous_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/credit_card_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/credit_card_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/datetime_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/datetime_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/discrete_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/discrete_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/document_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/document_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/ip_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/ip_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/latlon_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/latlon_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/phone_number_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/phone_number_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/type_discovery_driver.py` & `oracle_ads-2.8.4/ads/type_discovery/type_discovery_driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/typed_feature.py` & `oracle_ads-2.8.4/ads/type_discovery/typed_feature.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/unknown_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/unknown_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/type_discovery/zipcode_detector.py` & `oracle_ads-2.8.4/ads/type_discovery/zipcode_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/ads/vault/vault.py` & `oracle_ads-2.8.4/ads/vault/vault.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.3/oracle_ads.egg-info/PKG-INFO` & `oracle_ads-2.8.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: oracle-ads
-Version: 2.8.3
+Name: oracle_ads
+Version: 2.8.4
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,141 +19,141 @@
 Description-Content-Type: text/markdown
 Provides-Extra: boosted
 Provides-Extra: notebook
 Provides-Extra: text
 Provides-Extra: viz
 Provides-Extra: data
 Provides-Extra: opctl
-Provides-Extra: mysql
 Provides-Extra: bds
 Provides-Extra: spark
 Provides-Extra: huggingface
 Provides-Extra: torch
 Provides-Extra: tensorflow
 Provides-Extra: geo
 Provides-Extra: onnx
 Provides-Extra: optuna
 Provides-Extra: complete
 Provides-Extra: all-optional
 Provides-Extra: all-public
 
-# Oracle Accelerated Data Science SDK (ADS)
+# Oracle Accelerated Data Science (ADS)
 
-[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=plastic)](https://pypi.org/project/oracle-ads/)
+[![PyPI](https://img.shields.io/pypi/v/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Python](https://img.shields.io/pypi/pyversions/oracle-ads.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/oracle-ads/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://github.com/ambv/black)
 
-The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
+
+The [Oracle Accelerated Data Science (ADS) SDK](https://accelerated-data-science.readthedocs.io/en/latest/index.html) is maintained by the Oracle Cloud Infrastructure (OCI) [Data Science service](https://docs.oracle.com/en-us/iaas/data-science/using/data-science.htm) team. It speeds up common data science activities by providing tools that automate and simplify common data science tasks. Additionally, provides data scientists a friendly pythonic interface to OCI services. Some of the more notable services are OCI Data Science, Model Catalog, Model Deployment, Jobs, ML Pipelines, Data Flow, Object Storage, Vault, Big Data Service, Data Catalog, and the Autonomous Database. ADS gives you an interface to manage the life cycle of machine learning models, from data acquisition to model evaluation, interpretation, and model deployment.
 
 With ADS you can:
 
- - Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
- - Use feature types to characterize your data, create meaning summary statistics and plot. Use the warning and validation system to test the quality of your data.
- - Tune models using hyperparameter optimization with the `ADSTuner` tool.
- - Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
- - Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
- - Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
- - Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
- - Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
- - Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
+- Read datasets from Oracle Object Storage, Oracle RDBMS (ATP/ADW/On-prem), AWS S3 and other sources into `Pandas dataframes`.
+- Tune models using hyperparameter optimization with the `ADSTuner` tool.
+- Generate detailed evaluation reports of your model candidates with the `ADSEvaluator` module.
+- Save machine learning models to the [OCI Data Science Model Catalog](https://docs.oracle.com/en-us/iaas/data-science/using/models-about.htm).
+- Deploy models as HTTP endpoints with [Model Deployment](https://docs.oracle.com/en-us/iaas/data-science/using/model-dep-about.htm).
+- Launch distributed ETL, data processing, and model training jobs in Spark with [OCI Data Flow](https://docs.oracle.com/en-us/iaas/data-flow/using/home.htm).
+- Train machine learning models in OCI Data Science [Jobs](https://docs.oracle.com/en-us/iaas/data-science/using/jobs-about.htm).
+- Define and run an end-to-end machine learning orchestration covering all the steps of machine learning lifecycle in a repeatable, continuous [ML Pipelines](https://accelerated-data-science.readthedocs.io/en/latest/user_guide/pipeline/overview.html#).
+- Manage the life cycle of conda environments through the `ads conda` command line interface (CLI).
 
 ## Installation
 
 You have various options when installing ADS.
 
 ### Installing the oracle-ads base package
 
 ```bash
-  $ python3 -m pip install oracle-ads
+  python3 -m pip install oracle-ads
 ```
 
 ### Installing extras libraries
 
-The `all-optional` module will install all optional dependencies.
+The `all-optional` module will install all optional dependencies. Note the single quotes around installation of extra libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[all-optional]
+  python3 -m pip install 'oracle-ads[all-optional]'
 ```
 
 To work with gradient boosting models, install the `boosted` module. This module includes XGBoost and LightGBM model classes.
 
 ```bash
-  $ python3 -m pip install oracle-ads[boosted]
+  python3 -m pip install 'oracle-ads[boosted]'
 ```
 
 For big data use cases using Oracle Big Data Service (BDS), install the `bds` module. It includes the following libraries, `ibis-framework[impala]`, `hdfs[kerberos]` and `sqlalchemy`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[bds]
+  python3 -m pip install 'oracle-ads[bds]'
 ```
 
 To work with a broad set of data formats (for example, Excel, Avro, etc.) install the `data` module. It includes the `fastavro`, `openpyxl`, `pandavro`, `asteval`, `datefinder`, `htmllistparse`, and `sqlalchemy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[data]
+  python3 -m pip install 'oracle-ads[data]'
 ```
 
 To work with geospatial data install the `geo` module. It includes the `geopandas` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[geo]
+  python3 -m pip install 'oracle-ads[geo]'
 ```
 
 Install the `notebook` module to use ADS within a OCI Data Science service [notebook session](https://docs.oracle.com/en-us/iaas/data-science/using/manage-notebook-sessions.htm). This module installs `ipywidgets` and `ipython` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[notebook]
+  python3 -m pip install 'oracle-ads[notebook]'
 ```
 
 To work with ONNX-compatible run times and libraries designed to maximize performance and model portability, install the `onnx` module. It includes the following libraries, `onnx`, `onnxruntime`, `onnxmltools`, `skl2onnx`, `xgboost`, `lightgbm` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[onnx]
+  python3 -m pip install 'oracle-ads[onnx]'
 ```
 
 For infrastructure tasks, install the `opctl` module. It includes the following libraries, `oci-cli`, `docker`, `conda-pack`, `nbconvert`, `nbformat`, and `inflection`.
 
 ```bash
-  $ python3 -m pip install oracle-ads[opctl]
+  python3 -m pip install 'oracle-ads[opctl]'
 ```
 
 For hyperparameter optimization tasks install the `optuna` module. It includes the `optuna` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[optuna]
+  python3 -m pip install 'oracle-ads[optuna]'
 ```
 
 Install the `tensorflow` module to include `tensorflow` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[tensorflow]
+  python3 -m pip install 'oracle-ads[tensorflow]'
 ```
 
 For text related tasks, install the `text` module. This will include the `wordcloud`, `spacy` libraries.
 
 ```bash
-  $ python3 -m pip install oracle-ads[text]
+  python3 -m pip install 'oracle-ads[text]'
 ```
 
 Install the `torch` module to include `pytorch` and libraries from the `viz` module.
 
 ```bash
-  $ python3 -m pip install oracle-ads[torch]
+  python3 -m pip install 'oracle-ads[torch]'
 ```
 
 Install the `viz` module to include libraries for visualization tasks. Some of the key packages are `bokeh`, `folium`, `seaborn` and related packages.
 
 ```bash
-  $ python3 -m pip install oracle-ads[viz]
+  python3 -m pip install 'oracle-ads[viz]'
 ```
 
 **Note**
 
 Multiple extra dependencies can be installed together. For example:
 
 ```bash
-  $ python3 -m pip install  oracle-ads[notebook,viz,text]
+  python3 -m pip install  'oracle-ads[notebook,viz,text]'
 ```
 
 ## Documentation
 
   - [Oracle Accelerated Data Science SDK (ADS) Documentation](https://accelerated-data-science.readthedocs.io/en/latest/index.html)
   - [OCI Data Science and AI services Examples](https://github.com/oracle/oci-data-science-ai-samples)
   - [Oracle AI & Data Science Blog](https://blogs.oracle.com/ai-and-datascience/)
@@ -201,20 +200,18 @@
       bind_variables={ max_rows : 100 },
       connection_parameters=connection_parameters,
   )
 ```
 
 ## Contributing
 
-This project welcomes contributions from the community. Before submitting a pull request, please review our contribution guide [CONTRIBUTING.md](https://github.com/oracle/accelerated-data-science/blob/main/CONTRIBUTING.md).
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
 Find Getting Started instructions for developers in [README-development.md](https://github.com/oracle/accelerated-data-science/blob/main/README-development.md)
 
 ## Security
 
 Consult the security guide [SECURITY.md](https://github.com/oracle/accelerated-data-science/blob/main/SECURITY.md) for our responsible security vulnerability disclosure process.
 
 ## License
 
 Copyright (c) 2020, 2022 Oracle and/or its affiliates. Licensed under the [Universal Permissive License v1.0](https://oss.oracle.com/licenses/upl/)
-
-
```

### Comparing `oracle_ads-2.8.3/oracle_ads.egg-info/SOURCES.txt` & `oracle_ads-2.8.4/oracle_ads.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,26 @@
 ads/catalog/model.py
 ads/catalog/notebook.py
 ads/catalog/project.py
 ads/catalog/summary.py
 ads/common/__init__.py
 ads/common/analyzer.py
 ads/common/auth.py
-ads/common/base_properties.py
 ads/common/card_identifier.py
 ads/common/config.py
 ads/common/data.py
-ads/common/data_serializer.py
+ads/common/dsc_file_system.py
 ads/common/error.py
 ads/common/extended_enum.py
 ads/common/ipython.py
 ads/common/model.py
 ads/common/model_artifact.py
 ads/common/model_artifact_schema.json
 ads/common/model_export_util.py
-ads/common/model_introspect.py
 ads/common/model_metadata.py
-ads/common/model_metadata_mixin.py
 ads/common/object_storage_details.py
 ads/common/oci_client.py
 ads/common/oci_datascience.py
 ads/common/oci_logging.py
 ads/common/oci_mixin.py
 ads/common/oci_resource.py
 ads/common/serializer.py
@@ -149,22 +146,15 @@
 ads/feature_engineering/accessor/mixin/utils.py
 ads/feature_engineering/adsimage/__init__.py
 ads/feature_engineering/adsimage/image.py
 ads/feature_engineering/adsimage/image_reader.py
 ads/feature_engineering/adsimage/interface/__init__.py
 ads/feature_engineering/adsimage/interface/reader.py
 ads/feature_engineering/adsstring/__init__.py
-ads/feature_engineering/adsstring/common_regex_mixin.py
-ads/feature_engineering/adsstring/oci_language.py
-ads/feature_engineering/adsstring/string.py
 ads/feature_engineering/adsstring/oci_language/__init__.py
-ads/feature_engineering/adsstring/parsers/__init__.py
-ads/feature_engineering/adsstring/parsers/base.py
-ads/feature_engineering/adsstring/parsers/nltk_parser.py
-ads/feature_engineering/adsstring/parsers/spacy_parser.py
 ads/feature_engineering/adsstring/string/__init__.py
 ads/feature_engineering/dataset/__init__.py
 ads/feature_engineering/dataset/zip_code_data.py
 ads/feature_engineering/feature_type/__init__.py
 ads/feature_engineering/feature_type/address.py
 ads/feature_engineering/feature_type/base.py
 ads/feature_engineering/feature_type/boolean.py
@@ -266,15 +256,14 @@
 ads/model/deployment/__init__.py
 ads/model/deployment/model_deployer.py
 ads/model/deployment/model_deployment.py
 ads/model/deployment/model_deployment_infrastructure.py
 ads/model/deployment/model_deployment_properties.py
 ads/model/deployment/model_deployment_runtime.py
 ads/model/deployment/common/__init__.py
-ads/model/deployment/common/progress_bar.py
 ads/model/deployment/common/utils.py
 ads/model/extractor/__init__.py
 ads/model/extractor/automl_extractor.py
 ads/model/extractor/huggingface_extractor.py
 ads/model/extractor/keras_extractor.py
 ads/model/extractor/lightgbm_extractor.py
 ads/model/extractor/model_info_extractor.py
@@ -312,25 +301,22 @@
 ads/model/serde/model_serializer.py
 ads/model/service/__init__.py
 ads/model/service/oci_datascience_model.py
 ads/model/service/oci_datascience_model_deployment.py
 ads/model/service/oci_datascience_model_version_set.py
 ads/model/transformer/__init__.py
 ads/model/transformer/onnx_transformer.py
-ads/model_artifact_boilerplate/__init__.py
-ads/model_artifact_boilerplate/score.py
-ads/model_artifact_boilerplate/artifact_introspection_test/__init__.py
-ads/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
 ads/mysqldb/__init__.py
 ads/mysqldb/mysql_db.py
 ads/opctl/__init__.py
 ads/opctl/cli.py
 ads/opctl/cmds.py
 ads/opctl/constants.py
 ads/opctl/index.yaml
+ads/opctl/script.py
 ads/opctl/utils.py
 ads/opctl/backend/__init__.py
 ads/opctl/backend/ads_dataflow.py
 ads/opctl/backend/ads_ml_job.py
 ads/opctl/backend/ads_ml_pipeline.py
 ads/opctl/backend/ads_model_deployment.py
 ads/opctl/backend/base.py
@@ -373,14 +359,17 @@
 ads/opctl/distributed/common/framework_factory.py
 ads/opctl/docker/Dockerfile
 ads/opctl/docker/Dockerfile.gpu
 ads/opctl/docker/Dockerfile.job
 ads/opctl/docker/Dockerfile.job.gpu
 ads/opctl/docker/cuda.repo
 ads/opctl/docker/merge_dependencies.py
+ads/opctl/model/__init__.py
+ads/opctl/model/cli.py
+ads/opctl/model/cmds.py
 ads/opctl/spark/__init__.py
 ads/opctl/spark/cli.py
 ads/opctl/spark/cmds.py
 ads/opctl/spec/__init__.py
 ads/opctl/spec/abstract_operator_spec.py
 ads/opctl/spec/operator_spec_factory.py
 ads/opctl/spec/utils.py
@@ -393,17 +382,14 @@
 ads/pipeline/ads_pipeline_step.py
 ads/pipeline/cli.py
 ads/pipeline/extension.py
 ads/pipeline/builders/__init__.py
 ads/pipeline/builders/infrastructure/__init__.py
 ads/pipeline/builders/infrastructure/custom_script.py
 ads/pipeline/schema/__init__.py
-ads/pipeline/schema/cs_step_schema.json
-ads/pipeline/schema/ml_step_schema.json
-ads/pipeline/schema/pipeline_schema.json
 ads/pipeline/visualizer/__init__.py
 ads/pipeline/visualizer/base.py
 ads/pipeline/visualizer/graph_renderer.py
 ads/pipeline/visualizer/text_renderer.py
 ads/secrets/__init__.py
 ads/secrets/adb.py
 ads/secrets/auth_token.py
@@ -423,15 +409,14 @@
 ads/templates/score_lightgbm.jinja2
 ads/templates/score_onnx.jinja2
 ads/templates/score_onnx_new.jinja2
 ads/templates/score_oracle_automl.jinja2
 ads/templates/score_pyspark.jinja2
 ads/templates/score_pytorch.jinja2
 ads/templates/score_scikit-learn.jinja2
-ads/templates/score_spark.jinja2
 ads/templates/score_tensorflow.jinja2
 ads/templates/score_xgboost.jinja2
 ads/text_dataset/__init__.py
 ads/text_dataset/backends.py
 ads/text_dataset/dataset.py
 ads/text_dataset/extractor.py
 ads/text_dataset/options.py
```

### Comparing `oracle_ads-2.8.3/oracle_ads.egg-info/requires.txt` & `oracle_ads-2.8.4/oracle_ads.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 fastavro>=0.24.2
 openpyxl>=3.0.7
 pandavro>=1.6.0
 datefinder>=0.7.1
 htmllistparse>=0.6.0
 sqlalchemy<=1.4.46,>=1.4.1
 oracledb>=1.0
-mysql-connector-python
 ibis-framework[impala]
 hdfs[kerberos]
 sqlalchemy
 pyspark>=3.0.0
 transformers
 torch
 torchvision
@@ -75,15 +74,14 @@
 oracledb>=1.0
 oci-cli
 docker
 conda-pack
 nbconvert
 nbformat
 inflection
-mysql-connector-python
 ibis-framework[impala]
 hdfs[kerberos]
 sqlalchemy
 pyspark>=3.0.0
 transformers
 torch
 torchvision
@@ -121,15 +119,14 @@
 htmllistparse>=0.6.0
 ibis-framework[impala]
 inflection
 ipython<8.0,>=7.23.1
 ipywidgets~=7.6.3
 lightgbm
 lightgbm==3.3.1
-mysql-connector-python
 nbconvert
 nbformat
 oci-cli
 onnx>=1.12.0
 onnxmltools>=1.10.0
 onnxruntime>=1.10.0
 openpyxl>=3.0.7
@@ -169,17 +166,14 @@
 scipy>=1.5.4
 seaborn>=0.11.0
 geopandas
 
 [huggingface]
 transformers
 
-[mysql]
-mysql-connector-python
-
 [notebook]
 ipywidgets~=7.6.3
 ipython<8.0,>=7.23.1
 
 [onnx]
 bokeh<=2.4.3,>=2.3.0
 folium>=0.12.1
```

### Comparing `oracle_ads-2.8.3/setup.py` & `oracle_ads-2.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         "oci-cli",
         "docker",
         "conda-pack",
         "nbconvert",
         "nbformat",
         "inflection",
     ],
-    "mysql": ["mysql-connector-python"],
     "bds": ["ibis-framework[impala]", "hdfs[kerberos]", "sqlalchemy"],
     "spark": ["pyspark>=3.0.0"],
     "huggingface": ["transformers"],
 }
 
 this_directory = Path(__file__).parent
```

