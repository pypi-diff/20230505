# Comparing `tmp/gempyp-1.0.60b2.tar.gz` & `tmp/gempyp-1.0.70b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.60b2.tar", max compression
+gzip compressed data, was "gempyp-1.0.70b0.tar", max compression
```

## Comparing `gempyp-1.0.60b2.tar` & `gempyp-1.0.70b0.tar`

### file list

```diff
@@ -1,137 +1,94 @@
--rw-r--r--   0        0        0       23 2022-10-03 07:28:23.246552 gempyp-1.0.60b2/gempyp/__init__.py
--rw-r--r--   0        0        0      108 2022-10-03 07:28:23.246552 gempyp-1.0.60b2/gempyp/cli.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.249546 gempyp-1.0.60b2/gempyp/config/__init__.py
--rw-r--r--   0        0        0      156 2022-10-04 08:37:21.600854 gempyp-1.0.60b2/gempyp/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5438 2023-03-01 12:46:57.624255 gempyp-1.0.60b2/gempyp/config/__pycache__/baseConfig.cpython-310.pyc
--rw-r--r--   0        0        0     1422 2023-03-01 12:46:57.778000 gempyp-1.0.60b2/gempyp/config/__pycache__/DefaultSettings.cpython-310.pyc
--rw-r--r--   0        0        0     1842 2023-03-01 12:47:01.228577 gempyp-1.0.60b2/gempyp/config/__pycache__/GitLinkXML.cpython-310.pyc
--rw-r--r--   0        0        0     3650 2023-03-01 12:46:56.370587 gempyp-1.0.60b2/gempyp/config/__pycache__/xmlConfig.cpython-310.pyc
--rw-r--r--   0        0        0     7387 2023-03-22 09:03:31.739771 gempyp-1.0.60b2/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0     1481 2023-03-22 09:03:14.609820 gempyp-1.0.60b2/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2022-10-03 07:28:23.252108 gempyp-1.0.60b2/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2023-03-01 12:31:26.370749 gempyp-1.0.60b2/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2022-12-22 11:08:44.796327 gempyp-1.0.60b2/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2022-10-03 07:28:23.252911 gempyp-1.0.60b2/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2022-10-03 07:28:23.252911 gempyp-1.0.60b2/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     3607 2023-03-22 09:03:14.611989 gempyp-1.0.60b2/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.254385 gempyp-1.0.60b2/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.255739 gempyp-1.0.60b2/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2023-01-09 14:28:43.265339 gempyp-1.0.60b2/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2023-03-01 12:31:26.377729 gempyp-1.0.60b2/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2022-10-03 07:28:23.257527 gempyp-1.0.60b2/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.259374 gempyp-1.0.60b2/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2022-10-03 07:28:23.260585 gempyp-1.0.60b2/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2022-10-03 07:28:23.260585 gempyp-1.0.60b2/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.261656 gempyp-1.0.60b2/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2022-10-03 07:28:23.262838 gempyp-1.0.60b2/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.261656 gempyp-1.0.60b2/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2022-10-03 07:28:23.263837 gempyp-1.0.60b2/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.263837 gempyp-1.0.60b2/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2022-10-03 07:28:23.265569 gempyp-1.0.60b2/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2022-10-03 07:28:23.265569 gempyp-1.0.60b2/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2022-10-03 07:28:23.266610 gempyp-1.0.60b2/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2022-10-03 07:28:23.266610 gempyp-1.0.60b2/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2022-10-03 07:28:23.268693 gempyp-1.0.60b2/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2022-10-03 07:28:23.269690 gempyp-1.0.60b2/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.269690 gempyp-1.0.60b2/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2023-03-01 12:31:26.379723 gempyp-1.0.60b2/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.271440 gempyp-1.0.60b2/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.271440 gempyp-1.0.60b2/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0        0 2022-12-22 11:08:44.857151 gempyp-1.0.60b2/gempyp/dv/__init__.py
--rw-r--r--   0        0        0      152 2022-12-23 06:48:14.204422 gempyp-1.0.60b2/gempyp/dv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1334 2023-01-09 13:41:46.649087 gempyp-1.0.60b2/gempyp/dv/__pycache__/dvObj.cpython-310.pyc
--rw-r--r--   0        0        0     2773 2023-01-17 12:12:50.557058 gempyp-1.0.60b2/gempyp/dv/__pycache__/dvReporting.cpython-310.pyc
--rw-r--r--   0        0        0    18438 2023-01-20 12:49:15.489404 gempyp-1.0.60b2/gempyp/dv/__pycache__/dvRunner.cpython-310.pyc
--rw-r--r--   0        0        0    10694 2023-03-22 09:03:14.613581 gempyp-1.0.60b2/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2023-03-22 09:03:14.614808 gempyp-1.0.60b2/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0     7466 2023-03-22 09:03:31.741761 gempyp-1.0.60b2/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2023-03-22 09:03:14.619794 gempyp-1.0.60b2/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2023-03-22 09:03:14.620790 gempyp-1.0.60b2/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    21427 2023-03-22 09:21:07.033839 gempyp-1.0.60b2/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.272422 gempyp-1.0.60b2/gempyp/engine/__init__.py
--rw-r--r--   0        0        0      156 2022-10-04 08:37:22.333335 gempyp-1.0.60b2/gempyp/engine/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4717 2023-01-16 06:49:35.361493 gempyp-1.0.60b2/gempyp/engine/__pycache__/baseTemplate.cpython-310.pyc
--rw-r--r--   0        0        0     5395 2023-03-01 12:46:57.825755 gempyp-1.0.60b2/gempyp/engine/__pycache__/dataUpload.cpython-310.pyc
--rw-r--r--   0        0        0    20554 2023-01-17 13:46:52.032559 gempyp-1.0.60b2/gempyp/engine/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     3572 2023-01-16 10:34:24.275424 gempyp-1.0.60b2/gempyp/engine/__pycache__/runner.cpython-310.pyc
--rw-r--r--   0        0        0     3125 2023-01-16 06:49:35.340581 gempyp-1.0.60b2/gempyp/engine/__pycache__/simpleTestcase.cpython-310.pyc
--rw-r--r--   0        0        0     4972 2023-01-10 09:10:23.061010 gempyp-1.0.60b2/gempyp/engine/__pycache__/testData.cpython-310.pyc
--rw-r--r--   0        0        0     5092 2023-03-22 09:03:31.747097 gempyp-1.0.60b2/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     7603 2023-03-22 09:03:14.623782 gempyp-1.0.60b2/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    36744 2023-03-22 09:03:14.637205 gempyp-1.0.60b2/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.285178 gempyp-1.0.60b2/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2022-10-03 07:28:23.293594 gempyp-1.0.60b2/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2022-10-03 07:28:23.294753 gempyp-1.0.60b2/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5418 2023-03-01 12:31:26.398835 gempyp-1.0.60b2/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5537 2023-03-22 09:03:31.748997 gempyp-1.0.60b2/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    11590 2023-03-22 09:03:14.640159 gempyp-1.0.60b2/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2023-01-02 09:27:07.313658 gempyp-1.0.60b2/gempyp/final_report.html
--rw-r--r--   0        0        0     3959 2023-03-22 09:03:14.641115 gempyp-1.0.60b2/gempyp/gemPyp.py
--rw-r--r--   0        0        0        0 2022-12-22 11:08:44.882370 gempyp-1.0.60b2/gempyp/jira/__init__.py
--rw-r--r--   0        0        0      154 2022-12-23 06:48:14.487669 gempyp-1.0.60b2/gempyp/jira/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1965 2023-01-13 14:34:24.138949 gempyp-1.0.60b2/gempyp/jira/__pycache__/jiraIntegration.cpython-310.pyc
--rw-r--r--   0        0        0     2037 2022-12-20 08:41:31.802132 gempyp-1.0.60b2/gempyp/jira/__pycache__/jiraIntegration_copy.cpython-310.pyc
--rw-r--r--   0        0        0     2337 2023-03-01 12:31:26.404796 gempyp-1.0.60b2/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2023-03-01 12:31:26.406788 gempyp-1.0.60b2/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.303946 gempyp-1.0.60b2/gempyp/libs/__init__.py
--rw-r--r--   0        0        0      154 2022-10-04 08:37:21.990917 gempyp-1.0.60b2/gempyp/libs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7827 2023-03-01 12:46:57.694109 gempyp-1.0.60b2/gempyp/libs/__pycache__/common.cpython-310.pyc
--rw-r--r--   0        0        0      844 2022-12-14 06:21:29.903977 gempyp-1.0.60b2/gempyp/libs/__pycache__/custom_s3.cpython-310.pyc
--rw-r--r--   0        0        0     3049 2023-03-01 12:47:01.196387 gempyp-1.0.60b2/gempyp/libs/__pycache__/gem_s3_common.cpython-310.pyc
--rw-r--r--   0        0        0     1800 2023-03-01 12:47:01.300339 gempyp-1.0.60b2/gempyp/libs/__pycache__/logConfig.cpython-310.pyc
--rw-r--r--   0        0        0      886 2023-03-01 12:46:57.661182 gempyp-1.0.60b2/gempyp/libs/__pycache__/parsers.cpython-310.pyc
--rw-r--r--   0        0        0     9061 2023-03-22 09:03:31.750992 gempyp-1.0.60b2/gempyp/libs/common.py
--rw-r--r--   0        0        0      418 2022-12-15 14:58:50.001421 gempyp-1.0.60b2/gempyp/libs/enums/__pycache__/run_modes.cpython-310.pyc
--rw-r--r--   0        0        0      418 2022-12-23 06:48:13.622155 gempyp-1.0.60b2/gempyp/libs/enums/__pycache__/run_types.cpython-310.pyc
--rw-r--r--   0        0        0      447 2022-12-20 10:06:05.923546 gempyp-1.0.60b2/gempyp/libs/enums/__pycache__/status.cpython-310.pyc
--rw-r--r--   0        0        0      131 2022-12-22 11:08:44.916232 gempyp-1.0.60b2/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2023-03-01 14:39:26.016033 gempyp-1.0.60b2/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2022-10-03 07:28:23.307330 gempyp-1.0.60b2/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2023-03-22 09:03:31.753042 gempyp-1.0.60b2/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2023-03-01 12:31:26.439278 gempyp-1.0.60b2/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1420 2023-03-01 12:31:26.440317 gempyp-1.0.60b2/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.310440 gempyp-1.0.60b2/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0      157 2022-10-04 08:37:32.773116 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5074 2023-01-09 14:36:17.184000 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/apiCommon.cpython-310.pyc
--rw-r--r--   0        0        0      728 2022-10-10 09:59:10.201853 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/beforeAfterSample.cpython-310.pyc
--rw-r--r--   0        0        0     7130 2023-01-09 14:36:17.327024 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/compareFunctions.cpython-310.pyc
--rw-r--r--   0        0        0     5731 2022-12-23 06:48:14.175657 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/keyCheck.cpython-310.pyc
--rw-r--r--   0        0        0     8111 2023-01-16 06:49:37.756287 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/legacyComparison.cpython-310.pyc
--rw-r--r--   0        0        0     1622 2023-01-09 14:36:17.336000 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/miscVariables.cpython-310.pyc
--rw-r--r--   0        0        0     6316 2022-12-23 06:48:14.197441 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/postAssertion.cpython-310.pyc
--rw-r--r--   0        0        0     2254 2022-10-04 08:37:34.374350 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/postVariables.cpython-310.pyc
--rw-r--r--   0        0        0     6661 2023-01-16 06:49:37.367307 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/predefinedFunctions.cpython-310.pyc
--rw-r--r--   0        0        0     3128 2023-01-16 06:49:37.339840 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/preVariables.cpython-310.pyc
--rw-r--r--   0        0        0    18925 2023-01-16 06:49:35.456399 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/pypRest.cpython-310.pyc
--rw-r--r--   0        0        0     3222 2023-01-16 10:19:21.601214 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/reporting.cpython-310.pyc
--rw-r--r--   0        0        0      933 2022-10-04 08:37:34.456519 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/restObj.cpython-310.pyc
--rw-r--r--   0        0        0     4338 2022-10-13 13:41:28.627315 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     4391 2023-01-16 06:49:37.636530 gempyp-1.0.60b2/gempyp/pyprest/__pycache__/variableReplacement.cpython-310.pyc
--rw-r--r--   0        0        0     9844 2023-03-01 12:31:26.442912 gempyp-1.0.60b2/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2022-10-03 07:28:23.312576 gempyp-1.0.60b2/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    13694 2023-03-22 09:03:31.754997 gempyp-1.0.60b2/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13567 2023-03-22 09:03:31.755994 gempyp-1.0.60b2/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2023-03-22 09:03:31.757989 gempyp-1.0.60b2/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2023-03-01 12:31:26.448255 gempyp-1.0.60b2/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10792 2023-03-22 09:03:31.759482 gempyp-1.0.60b2/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     4195 2022-10-03 07:28:23.319137 gempyp-1.0.60b2/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2023-03-01 12:31:26.452244 gempyp-1.0.60b2/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     3873 2023-03-01 12:31:26.450250 gempyp-1.0.60b2/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    36175 2023-03-22 09:03:31.761072 gempyp-1.0.60b2/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4333 2023-03-22 09:03:14.650977 gempyp-1.0.60b2/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2023-03-22 09:03:14.651974 gempyp-1.0.60b2/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2023-03-22 09:03:31.763022 gempyp-1.0.60b2/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2022-10-13 13:39:16.436921 gempyp-1.0.60b2/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     5463 2023-03-22 09:03:31.764983 gempyp-1.0.60b2/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2022-10-03 07:28:23.327074 gempyp-1.0.60b2/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0      158 2022-10-04 08:37:31.431991 gempyp-1.0.60b2/gempyp/reporter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6010 2023-01-20 14:57:58.641899 gempyp-1.0.60b2/gempyp/reporter/__pycache__/reportGenerator.cpython-310.pyc
--rw-r--r--   0        0        0     7076 2023-03-22 09:03:14.653297 gempyp-1.0.60b2/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    11919 2023-03-22 09:03:14.654965 gempyp-1.0.60b2/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     2301 2023-03-22 09:03:14.655993 gempyp-1.0.60b2/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2022-10-03 07:28:23.334228 gempyp-1.0.60b2/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2022-10-03 07:28:23.238461 gempyp-1.0.60b2/LICENSE
--rw-r--r--   0        0        0     1377 2023-03-22 09:22:55.757961 gempyp-1.0.60b2/pyproject.toml
--rw-r--r--   0        0        0     3161 2022-10-13 13:39:14.273863 gempyp-1.0.60b2/README.md
--rw-r--r--   0        0        0     5087 1970-01-01 00:00:00.000000 gempyp-1.0.60b2/setup.py
--rw-r--r--   0        0        0     4791 1970-01-01 00:00:00.000000 gempyp-1.0.60b2/PKG-INFO
+-rw-r--r--   0        0        0      258 2023-05-05 14:21:56.330590 gempyp-1.0.70b0/gempyp/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-05 14:21:56.330590 gempyp-1.0.70b0/gempyp/Annotations.py
+-rw-r--r--   0        0        0      108 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/__init__.py
+-rw-r--r--   0        0        0     7387 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/baseConfig.py
+-rw-r--r--   0        0        0      198 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/customParser.py
+-rw-r--r--   0        0        0     1778 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/DefaultSettings.py
+-rw-r--r--   0        0        0       62 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/gempyp.conf
+-rw-r--r--   0        0        0     2145 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/GitLinkXML.py
+-rw-r--r--   0        0        0    21143 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/Result.html
+-rw-r--r--   0        0        0       26 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/suite_conf.json
+-rw-r--r--   0        0        0       28 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/testcase_conf.json
+-rw-r--r--   0        0        0     4007 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/xmlConfig.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/common/__init__.py
+-rw-r--r--   0        0        0     3627 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/common/common_functions.py
+-rw-r--r--   0        0        0      956 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/compare.py
+-rw-r--r--   0        0        0      149 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/config/dvm.json
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/__init__.py
+-rw-r--r--   0        0        0     4635 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/configurator.py
+-rw-r--r--   0        0        0      320 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/validator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/__init__.py
+-rw-r--r--   0        0        0      589 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/comparator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/Compare.py
+-rw-r--r--   0        0        0    10157 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/python_obj_comparator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/__init__.py
+-rw-r--r--   0        0        0     5498 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/data.py
+-rw-r--r--   0        0        0      869 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/database.py
+-rw-r--r--   0        0        0     1903 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/db_mysql.py
+-rw-r--r--   0        0        0     2646 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/db_oracle.py
+-rw-r--r--   0        0        0     2436 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/db_postgre.py
+-rw-r--r--   0        0        0     1999 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/db_sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/file_processor.py
+-rw-r--r--   0        0        0    11161 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data_comp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/tools/__init__.py
+-rw-r--r--   0        0        0     3034 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/data_uploader.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/__init__.py
+-rw-r--r--   0        0        0     2285 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dfOperations.py
+-rw-r--r--   0        0        0    10230 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvCompare.py
+-rw-r--r--   0        0        0      682 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvDatabases.py
+-rw-r--r--   0        0        0     9470 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvDataframe.py
+-rw-r--r--   0        0        0     1441 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvObj.py
+-rw-r--r--   0        0        0     3789 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvReporting.py
+-rw-r--r--   0        0        0    23248 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvRunner.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/__init__.py
+-rw-r--r--   0        0        0     5092 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/baseTemplate.py
+-rw-r--r--   0        0        0     8414 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/dataUpload.py
+-rw-r--r--   0        0        0    40521 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/executors/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-05 14:21:30.372942 gempyp-1.0.70b0/gempyp/engine/executors/baseExecutor.py
+-rw-r--r--   0        0        0      656 2023-05-05 14:21:30.373956 gempyp-1.0.70b0/gempyp/engine/gempypHelper.py
+-rw-r--r--   0        0        0     5418 2023-05-05 14:21:30.374954 gempyp-1.0.70b0/gempyp/engine/runner.py
+-rw-r--r--   0        0        0     5537 2023-05-05 14:21:30.374954 gempyp-1.0.70b0/gempyp/engine/simpleTestcase.py
+-rw-r--r--   0        0        0    12428 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/testData.py
+-rw-r--r--   0        0        0    64741 2023-05-05 14:21:30.376963 gempyp-1.0.70b0/gempyp/final_report.html
+-rw-r--r--   0        0        0     4724 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/gemPyp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.379963 gempyp-1.0.70b0/gempyp/jira/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-05 14:21:30.380963 gempyp-1.0.70b0/gempyp/jira/jiraIntegration.py
+-rw-r--r--   0        0        0     4474 2023-05-05 14:21:30.380963 gempyp-1.0.70b0/gempyp/jira/jiraIntegrationCopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.381963 gempyp-1.0.70b0/gempyp/libs/__init__.py
+-rw-r--r--   0        0        0     9045 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/libs/common.py
+-rw-r--r--   0        0        0      131 2023-05-05 14:21:30.383963 gempyp-1.0.70b0/gempyp/libs/enums/run_types.py
+-rw-r--r--   0        0        0      318 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/libs/enums/status.py
+-rw-r--r--   0        0        0       47 2023-05-05 14:21:30.384963 gempyp-1.0.70b0/gempyp/libs/exceptions/__init__.py
+-rw-r--r--   0        0        0     4352 2023-05-05 14:21:30.385646 gempyp-1.0.70b0/gempyp/libs/gem_s3_common.py
+-rw-r--r--   0        0        0     2642 2023-05-05 14:21:30.386656 gempyp-1.0.70b0/gempyp/libs/logConfig.py
+-rw-r--r--   0        0        0     1465 2023-05-05 14:21:30.386656 gempyp-1.0.70b0/gempyp/libs/parsers.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.387656 gempyp-1.0.70b0/gempyp/pyprest/__init__.py
+-rw-r--r--   0        0        0     9844 2023-05-05 14:21:30.388723 gempyp-1.0.70b0/gempyp/pyprest/apiCommon.py
+-rw-r--r--   0        0        0      491 2023-05-05 14:21:30.389602 gempyp-1.0.70b0/gempyp/pyprest/beforeAfterSample.py
+-rw-r--r--   0        0        0    13694 2023-05-05 14:21:30.390435 gempyp-1.0.70b0/gempyp/pyprest/compareFunctions.py
+-rw-r--r--   0        0        0    13567 2023-05-05 14:21:30.391447 gempyp-1.0.70b0/gempyp/pyprest/keyCheck.py
+-rw-r--r--   0        0        0    15661 2023-05-05 14:21:30.392445 gempyp-1.0.70b0/gempyp/pyprest/legacyComparison.py
+-rw-r--r--   0        0        0     1933 2023-05-05 14:21:30.393446 gempyp-1.0.70b0/gempyp/pyprest/miscVariables.py
+-rw-r--r--   0        0        0    10792 2023-05-05 14:21:30.393446 gempyp-1.0.70b0/gempyp/pyprest/postAssertion.py
+-rw-r--r--   0        0        0     4195 2023-05-05 14:21:30.394437 gempyp-1.0.70b0/gempyp/pyprest/postVariables.py
+-rw-r--r--   0        0        0     8271 2023-05-05 14:21:30.396448 gempyp-1.0.70b0/gempyp/pyprest/predefinedFunctions.py
+-rw-r--r--   0        0        0     3873 2023-05-05 14:21:30.395446 gempyp-1.0.70b0/gempyp/pyprest/preVariables.py
+-rw-r--r--   0        0        0    36175 2023-05-05 14:21:30.397446 gempyp-1.0.70b0/gempyp/pyprest/pypRest.py
+-rw-r--r--   0        0        0     4333 2023-05-05 14:21:30.398445 gempyp-1.0.70b0/gempyp/pyprest/reporting.py
+-rw-r--r--   0        0        0     2725 2023-05-05 14:21:30.398445 gempyp-1.0.70b0/gempyp/pyprest/restEngine.py
+-rw-r--r--   0        0        0     1031 2023-05-05 14:21:30.399475 gempyp-1.0.70b0/gempyp/pyprest/restObj.py
+-rw-r--r--   0        0        0     6308 2023-05-05 14:21:30.400514 gempyp-1.0.70b0/gempyp/pyprest/utils.py
+-rw-r--r--   0        0        0     5463 2023-05-05 14:21:30.400514 gempyp-1.0.70b0/gempyp/pyprest/variableReplacement.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.401512 gempyp-1.0.70b0/gempyp/reporter/__init__.py
+-rw-r--r--   0        0        0     6959 2023-05-05 14:21:56.358422 gempyp-1.0.70b0/gempyp/reporter/reportGenerator.py
+-rw-r--r--   0        0        0    12721 2023-05-05 14:21:56.360429 gempyp-1.0.70b0/gempyp/sdk/executor.py
+-rw-r--r--   0        0        0     2508 2023-05-05 14:21:56.361432 gempyp-1.0.70b0/gempyp/sdk/worker.py
+-rw-r--r--   0        0        0    11547 2023-05-05 14:21:30.404588 gempyp-1.0.70b0/gempyp/testcase.html
+-rw-r--r--   0        0        0        2 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/LICENSE
+-rw-r--r--   0        0        0     1371 2023-05-05 14:30:57.265844 gempyp-1.0.70b0/pyproject.toml
+-rw-r--r--   0        0        0     3161 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/README.md
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 gempyp-1.0.70b0/PKG-INFO
```

### Comparing `gempyp-1.0.60b2/gempyp/config/baseConfig.py` & `gempyp-1.0.70b0/gempyp/config/baseConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/config/DefaultSettings.py` & `gempyp-1.0.70b0/gempyp/config/DefaultSettings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 from gempyp.engine import dataUpload
 import traceback
 import logging
+import re
+import sys
 
 # have to discuss about the default location
 DEFAULT_GEMPYP_FOLDER = os.getcwd()
 DEBUG = True
 THREADS = 8
+encrypt_key = b'sEKTykqMLP_iCwlMtiBR_9SQ0v9N1OT3ajVAAaI4AkQ='
 _VERSION = "1.0.0"
 apiSuccess = False
 project_id = "Test_id"
 default_baseurl="https://apis.gemecosystem.com"
 urls = {"data":{} }
 # for getting urls using url tag from config file
 def getEnterPoint(url, bridge_token, user_name):
@@ -19,16 +22,19 @@
         url = checkUrl(url)
         response = dataUpload._sendData(" ", url, bridge_token, user_name,"GET")
         if response.status_code == 200:
             url_enter_point = response.json()
             urls["data"]=url_enter_point["data"]
             global apiSuccess
             apiSuccess = True
-        else:
+        elif re.search('50[0-9]',str(response.status_code)):
             logging.warning("Error Occurs While Getting the BASE_URLs")
+        else:
+            logging.info("Some Error From the Client Side, Maybe username or bridgeToken, Therefore terminating execution")
+            sys.exit()
     except Exception as e:
             traceback.print_exc()
             logging.warning("Error Occurs While Getting the BASE_URLs")
 
 # for sending urls to dataupload file
 def getUrls(apiName):
     return urls["data"].get(apiName, None)
```

### Comparing `gempyp-1.0.60b2/gempyp/config/GitLinkXML.py` & `gempyp-1.0.70b0/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/config/Result.html` & `gempyp-1.0.70b0/gempyp/config/Result.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/config/xmlConfig.py` & `gempyp-1.0.70b0/gempyp/config/xmlConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,41 @@
 from gempyp.config.baseConfig import AbstarctBaseConfig
 from gempyp.libs.parsers import xmlToDict, xmlToList
 from gempyp.libs.logConfig import LoggingConfig
 import sys, os
 import warnings
 import uuid
 import json
-
+from gempyp.config.customParser import CustomXMLParser
+from lxml import etree
 class XmlConfig(AbstarctBaseConfig):
     def __init__(self, filePath: str, s_run_id):
         
         # code pushed in parse function to make run_id working
         self.s_run_id = s_run_id
         super().__init__(filePath)
         # do any xml specific validatioins here
+
+    def ignore_comments_and_parse(xml_file):
+        parser = et.XMLParser(target=et.TreeBuilder(), comment_handler=lambda *args: None)
+        tree = et.parse(xml_file, parser=parser)
+        return tree
        
 
     def parse(self, filePath):
 
         logging.info("-------- Xml file path: {filePath} ----------".format(filePath=filePath))
         path_list = filePath.split(os.sep)[0:-1]
         newfilePath = os.sep.join(path_list)
         sys.path.append({"XMLConfigDir":newfilePath})
         logging.info("-------- Started the Xml parsing in XmlConfig ---------")
         filePath=self.handleSpecialSymbols(filePath)
-        data = et.parse(filePath)
+        # data = et.parse(filePath)
+        parser = CustomXMLParser(remove_comments=True)
+        data = etree.parse(filePath, parser=parser)
         
         
         self._CONFIG["SUITE_DATA"] = self._getSuiteData(data)        
 
         self.log_dir = str(os.path.join(tempfile.gettempdir(), 'logs'))
         if not os.path.exists(self.log_dir):
             os.makedirs(self.log_dir)
```

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.70b0/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/compare.py` & `gempyp-1.0.70b0/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.70b0/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.70b0/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.70b0/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/data.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/database.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.70b0/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/data_compare/data_comp.py` & `gempyp-1.0.70b0/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvCompare.py` & `gempyp-1.0.70b0/gempyp/dv/dvCompare.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,21 @@
         src_key_values = src_df.index.values
         tgt_key_values = tgt_df.index.values
         common_keys = list(set(src_key_values) & set(tgt_key_values))
         keys_only_in_src = list(set(src_key_values) - set(tgt_key_values))
         keys_only_in_tgt = list(set(tgt_key_values) - set(src_key_values))
         src_df.drop(keys_only_in_src, inplace=True)
         tgt_df.drop(keys_only_in_tgt, inplace=True)
-        if 'SKIP_COLUMN' in configData:
-            try:
-                skip_column = configData["SKIP_COLUMN"].split(',')
-                flag = False
-                for i in key:
-                    if i in skip_column:
-                        flag = True
-                        break
-                if flag:
-                    reporter.addRow("Column Given for Skip are Present in Keys Tag","Aborting Skip Columns",status.INFO)
-                else:
-                    src_df.drop(skip_column,axis=1,inplace=True)
-                    tgt_df.drop(skip_column,axis=1,inplace=True)
-                    headers = list(set(headers)-set(skip_column))
-            except Exception as e:
-                reporter.addRow("While Skipping Columns",get_reason_of_failure(traceback.format_exc(), e),status.INFO)
+        # if 'SKIP_COLUMN' in configData:
+        #     try:
+            # skip_column = configData["SKIP_COLUMN"].split(',')
+        
+            # headers = list(set(headers)-set(skip_column))
+        #     except Exception as e:
+        #         reporter.addRow("While Skipping Columns",get_reason_of_failure(traceback.format_exc(), e),status.INFO)
         """calling src and tgt for getting different keys"""
         src_key_dict = addDiffKeysDict(keys_only_in_src, "Source", key, logger)
         tgt_key_dict = addDiffKeysDict(keys_only_in_tgt, "Target", key, logger)
         # for keys in src_key_dict.keys():
         #     src_key_dict[keys] = src_key_dict[keys] + tgt_key_dict[keys]
         diff_keys_dict = collections.defaultdict(list)
         for keys, val in itertools.chain(src_key_dict.items(), tgt_key_dict.items()):
```

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvDatabases.py` & `gempyp-1.0.70b0/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvDataframe.py` & `gempyp-1.0.70b0/gempyp/dv/dvDataframe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import importlib
 from gempyp.libs.common import readPath, download_common_file, get_reason_of_failure
 from gempyp.libs.enums.status import status
 from gempyp.dv.dvDatabases import Databases
 import traceback
 import pandas as pd
 import mysql.connector
-# import snowflake.connector
+import snowflake.connector
 import pg8000
 import re
+import time
+import pymongo
+import json
+import ast
 
 
 class Dataframe:
     def __init__(self) -> None:
         pass
 
     def getSourceDataFrame(self, data, logger, reporter, sourceCred):
@@ -104,72 +108,113 @@
             raise Exception(f"Could not read file, {e}")
 
     def dbOperations(self, cred, db):
         try:
             log = f"----Connecting to {db}DB----"
             self.logger.info(log)
             myDB = self.connectingDB(db, cred)
-            myCursor = myDB.cursor()
         except Exception as e:
             self.reporter.addRow(
                 f"Connection to {db}DB: ", "Exception Occurred", status.ERR)
             self.logger.error(str(e))
+            
             # self.reporter.addMisc(
             #         "REASON OF FAILURE", get_reason_of_failure(traceback.format_exc(), e))
 
             raise Exception(e)
 
         try:
             self.logger.info(f"----Executing the {db}SQL----")
-            sql = f"{db}_SQL"
-            myCursor.execute(self.configData[sql])
-            self.reporter.addRow(
-                f"Executing {db} SQL", f"{self.configData[sql]}{db} SQL executed Successfull", status.PASS)
-            columns = [i[0] for i in myCursor.description]
+            # checking whether it is mongodb object by checking mongoclient in starting of the object
+            x = re.search("^MongoClient.*", str(myDB))
+            if x:
+                try:
+                    db_name = f'{db}_DB'
+                    db_details = ast.literal_eval(self.configData[db_name])
+                    sql = f'{db}_SQL'
+                    conn = myDB[db_details['database']]
+                    list_of_collections = conn.list_collection_names()
+                    if db_details['collection'] not in list_of_collections:
+                        raise Exception
+                    conn = conn[db_details['collection']]
+                except Exception:
+                    self.reporter.addRow("Finding Database and Collection","Not Found in Source_db or Target_db",status.ERR)
+                    raise Exception("Database and Collection not Found in Source_db or Target_db")
+                try:
+                    query = json.loads(self.configData[sql])
+                except Exception:
+                    self.reporter.addRow("Fetching Query","Not Present in JSON Format",status.ERR)
+                    raise Exception("Mongo Query not Present in JSON Format")
+                results = list(conn.find(query))
+                db_1 = pd.DataFrame(results)
+                columns = list(db_1.columns)
+            else:
+                myCursor = myDB.cursor()
+                sql = f"{db}_SQL"
+                myCursor.execute(self.configData[sql])
+                self.reporter.addRow(
+                    f"Executing {db} SQL", f"{self.configData[sql]}<br>{db} SQL executed Successfull", status.PASS)
+                columns = [i[0] for i in myCursor.description]
+                results = myCursor.fetchall()
+                db_1 = pd.DataFrame(results,columns=columns)
         except Exception as e:
             self.logger.error(str(e))
             # self.reporter.addMisc(
             #         "REASON OF FAILURE", get_reason_of_failure(traceback.format_exc(), e))
 
             self.reporter.addRow(
                 f"Executing {db} SQL", "Exception Occurred", status.ERR)
             raise e
-
-        results = myCursor.fetchall()
-        db_1 = pd.DataFrame(results,
-                            columns=columns)
+        
         myDB.close()
         return db_1, columns
 
     def connectingDB(self, dbType, cred):
         
         db = f'{dbType}_DB'
-        if self.configData[db].lower() == 'custom':
+        is_dict = True
+        try:
+            db_details = ast.literal_eval(self.configData[db])
+        except Exception:
+            is_dict = False
+        if is_dict == True:
+            db_type = db_details.get('type')
+        else:
+            db_type = self.configData[db]
+                    
+        if db_type.lower() == 'custom':
             conn = f"{dbType}_CONN"
             db = self.configData[conn]
             myDB = eval(db)
             # this is just to check whether connection is established or not
-            dbCursor = myDB.cursor()
+            x = re.search("^MongoClient.*", str(myDB))
+            if x:
+                myDB.server_info()
+            else:
+                dbCursor = myDB.cursor()
             self.reporter.addRow(
                 f"Connection to {dbType}DB:", f"Connection to {dbType}DB is Successfull", status.PASS)
         else:
             dv = Databases()
             lib, connect = Databases.getConnectionString(
-                dv, self.configData[db])
+                dv, db_type)
             lib = importlib.import_module(lib)
             connection = getattr(lib, connect)
             myDB = connection(**cred)
+            x = re.search("^MongoClient.*", str(myDB))
+            if x:
+                myDB.server_info()
             connDetails = self.getHostDetails(cred)
             self.reporter.addRow(
                 f"Connection to {dbType}DB: {connDetails}", f"Connection to {dbType}DB is Successfull", status.PASS)
         return myDB
 
     def getHostDetails(self, details):
 
         li = list(details.keys())
         for i in li:
             if re.search("user", i) != None:
                 del details[i]
                 continue
             if re.search("password", i) != None:
                 del details[i]
-        return details
+        return details
```

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvObj.py` & `gempyp-1.0.70b0/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvReporting.py` & `gempyp-1.0.70b0/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/dv/dvRunner.py` & `gempyp-1.0.70b0/gempyp/dv/dvRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 import pg8000
 from gempyp.dv.dvObj import DvObj
 from gempyp.libs.common import download_common_file,get_reason_of_failure
 from gempyp.engine.runner import getError
 from gempyp.libs import common
 from gempyp.dv.dvDataframe import Dataframe
 from gempyp.dv.dvCompare import df_compare
+from gempyp.dv.dfOperations import dateFormatHandling, columnCompare, skipColumn
 import re
+import json
+import ast
 
 
 class DvRunner(Base):
 
     def __init__(self, data):
 
         self.data = data
@@ -89,14 +92,18 @@
             if "COLUMN_MAP" in self.configData:
                 self.target_df.rename(columns=eval(
                     self.configData["COLUMN_MAP"]), inplace=True)
                 self.target_columns = list(self.target_df.columns)
             self.matchKeys(self.source_columns, "SOURCE")
             self.matchKeys(self.target_columns, "TARGET")
 
+            if 'SKIP_COLUMN' in self.configData:
+                self.source_df, self.target_df = skipColumn(self.configData.get('SKIP_COLUMN'),self.source_df,self.target_df,self.keys,self.reporter)
+                self.source_columns = list(self.source_df.columns)
+                self.target_columns = list(self.target_df.columns)
             #calling getDuplicatekeysDf function to get dataframe of duplicate keys 
             source_duplicates_df, src_dup_len = self.getDuplicateKeysDf(self.source_df, "SOURCE")
             target_duplicates_df, tgt_dup_len = self.getDuplicateKeysDf(self.target_df, "TARGET")
             dup_keys_length = src_dup_len + tgt_dup_len
             duplicate_keys_df = pd.concat([source_duplicates_df , target_duplicates_df ], axis=0, ignore_index=True)
 
             if self.source_columns == self.target_columns:
@@ -110,19 +117,30 @@
 
             """deleting duplicates from df and keeping last ones"""
             self.logger.info("Removing Duplicates Rows")
             self.source_df.drop_duplicates(
                 subset=self.keys, keep='last', inplace=True)
             self.target_df.drop_duplicates(
                 subset=self.keys, keep='last', inplace=True)
+            
+            #calling compare column
+            if "COMPARE_COLUMN" in self.configData:
+                compare_column = self.configData.get("COMPARE_COLUMN",'').split(',')
+                self.source_df, self.target_df = columnCompare(self.source_df, self.target_df, self.keys, compare_column)
             # hadling case insensitivity
             if 'MATCH_CASE' in self.configData:
                 self.matchCase()
+
+            # date format handling
+            self.source_df, self.target_df = dateFormatHandling(self.source_df, self.target_df)
+            
+            #checking column compare
             value_dict, key_dict, keys_length = df_compare(
                 self.source_df, self.target_df, self.keys, self.logger, self.reporter, self.configData)
+            
             self.writeExcel(value_dict, key_dict, keys_length, duplicate_keys_df, dup_keys_length)
             self.reporter.finalizeReport()
             output = writeToReport(self)
             return output, None
         except Exception as e:
             self.reporter.addMisc(
                     "REASON OF FAILURE", get_reason_of_failure(traceback.format_exc(), e))
@@ -132,28 +150,47 @@
             return output, None
 
     def dbConnParser(self):
         """checking db type and fetching credentials or connection details accordingly"""
         try:
             if 'SOURCE_DB' in self.configData:
                 if 'SOURCE_CONN' in self.configData: 
-                    if self.configData["SOURCE_DB"].lower() == 'custom':
+                    is_dict = True
+                    try:
+                        db_details = ast.literal_eval(self.configData["SOURCE_DB"])
+                    except Exception:
+                        is_dict = False
+                    if is_dict == True:
+                        db_type = db_details.get('type')
+                    else:
+                        db_type = self.configData["SOURCE_DB"]
+                    if db_type.lower() == 'custom':
                         self.sourceCred = self.configData['SOURCE_CONN']
                     else:
                         if re.search("^{.*}$", self.configData["SOURCE_CONN"]):
                             self.sourceCred = eval(self.configData["SOURCE_CONN"])
                         else:
                             self.logger.info("----Parsing the Config File For Source Connections----")
                             self.sourceCred = dict(self.configur.items(
                                 self.configData["SOURCE_CONN"]))
                             self.sourceCred=self.parseConfigDict(self.sourceCred)
             
             if 'TARGET_DB' in self.configData:
                 if 'TARGET_CONN' in self.configData:
-                    if self.configData["TARGET_DB"].lower() == 'custom':
+                    is_dict = True
+                    try:
+                        db_details = ast.literal_eval(self.configData["TARGET_DB"])
+                    except Exception:
+                        is_dict = False
+                    if is_dict == True:
+                        db_type = db_details.get('type')
+                    else:
+                        db_type = self.configData["TARGET_DB"]
+                    
+                    if db_type.lower() == 'custom':
                         self.targetCred = self.configData['TARGET_CONN']
                     else:
                         if re.search("^{.*}$", self.configData["TARGET_CONN"]):
                             self.targetCred = eval(self.configData["TARGET_CONN"])
                         else:
                             self.targetCred = dict(self.configur.items(
                                 self.configData["TARGET_CONN"]))
@@ -309,15 +346,14 @@
         try:
             file_path = download_common_file(
                 file_name, self.data.get("SUITE_VARS", None))
             file_obj = moduleImports(file_path)
             self.logger.info("Running before method")
             obj_ = file_obj
             before_obj = DvObj(
-                object=self.reporter,
                 project=self.project,
                 source_df=self.source_df,
                 target_df=self.target_df,
                 source_columns=self.source_columns,
                 target_columns=self.target_columns,
                 keys=self.keys,
                 env=self.env,
@@ -367,15 +403,14 @@
         try:
             file_path = download_common_file(
                 file_name, self.data.get("SUITE_VARS", None))
             file_obj = moduleImports(file_path)
             self.logger.info("Running After method")
             obj_ = file_obj
             after_obj = DvObj(
-                object=self.reporter,
                 project=self.project,
                 value_df=self.value_df,
                 keys_df=self.keys_df,
                 env=self.env,
                 reporter=self.reporter 
             )
             if class_name != "":
@@ -429,21 +464,24 @@
                 keep='last', inplace=True)
         dup_keys_df['Reason-of-Failure'] = f'Duplicate Key in {type}'
         if len(dup_keys_df['Reason-of-Failure']) > 0:
             self.reporter.addRow(f"Checking for Duplicates Keys in {type}",f"Found Duplicate Keys in {type}",status.FAIL)
         return dup_keys_df, dup_length
     
     def parseConfig(self,config):
-        pattern = r"ENV.\w*"
+        pattern = r"ENV.([a-zA-Z0-9_]+)"
         for key in config.keys():
             value=config.get(key)
             if(type(value)!=logging.Logger):
-                match=re.search(pattern, value)
-                if("ENV." in value and match and os.environ.get(match.group().replace("ENV.",""))):
-                    config[key]=re.sub(pattern,os.environ.get(match.group().replace("ENV.","")), value)
+                if re.search("mysql.connector.connect",value) or re.search("^{",value):
+                    config[key] = re.sub(pattern, lambda match: f"'{os.environ.get(match.group(1), '')}'", value)
+                else:
+                    if("ENV." in value):
+                        config[key]=os.environ.get(value.replace("ENV.",""))
+        print(config)
         return config
     
     def parseConfigDict(self,conf):
         for key in conf.keys():
             if("ENV." in conf.get(key) and os.environ.get(conf.get(key).replace("ENV.",""))):
                 conf[key]=os.environ.get(conf.get(key).replace("ENV.",""))
         return conf
```

### Comparing `gempyp-1.0.60b2/gempyp/engine/baseTemplate.py` & `gempyp-1.0.70b0/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/engine/dataUpload.py` & `gempyp-1.0.70b0/gempyp/engine/dataUpload.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 import logging
 from gempyp.config import DefaultSettings
 from gempyp.libs.enums.status import status
 import logging
 import re
 import json
+import sys
 
 not_uploaded = []
 suite_data = []
 flag = False
 suite_uploaded = False
 list_of_testcase = []
 respon = {}
@@ -50,61 +51,75 @@
     """
 
     try:
         if len(respon) != 0:
             payload = dataAlter(payload)
         payload = noneRemover(payload)
         response = _sendData(payload, DefaultSettings.getUrls("suite-exe-api"), bridge_token, user_name, mode)
-
         if response and response.status_code in [201, 200]:
             global suite_uploaded
             logging.info("Suite data uploaded successfully")
             suite_uploaded = True
             try:
                 DefaultSettings.project_id = json.loads(response.text)["data"]["p_id"]
             except Exception as e:
                 logging.info(traceback.format_exc())
             if payload in suite_data:
                 suite_data.remove(payload)
         elif response and response.status_code == 200:
             logging.info("Suite Data updated Successfully")
-        else:
+        elif re.search('50[0-9]',str(response.status_code)):
             logging.info("Suite data is not uploaded")
             if payload not in suite_data:
                 suite_data.append(payload)
+        else:
+            logging.info("Some Error From the Client Side, Terminating Execution")
+            sys.exit()
+        # else:
+        #     logging.info("Suite data is not uploaded")
+        #     if payload not in suite_data:
+        #         suite_data.append(payload)
                 
     except Exception as e:
         logging.error(traceback.format_exc())
 
 def sendTestcaseData(payload, bridge_token, user_name):
     """
     for checking the sendTestCaseData api response
     """
-
     try:
         method = "POST"
         payload = json.loads(payload)
         tc_run_id = payload["tc_run_id"]
         if tc_run_id[:-37] in list_of_testcase:
         #checking whether testcase present in previous run 
             payload, method = getTestcase(payload, method, bridge_token, user_name)
         payload = json.dumps(payload)
         response = _sendData(payload, DefaultSettings.getUrls("test-exe-api"), bridge_token, user_name, method)
         ### Applying regex to the response
-
         x = re.search("already present",response.text,re.IGNORECASE)
         if response.status_code == 201:
             logging.info("data uploaded successfully")
             if payload in not_uploaded:
                 not_uploaded.remove(payload)
         elif response.status_code == 200:
             logging.info("data updated successfully")
             if payload in not_uploaded:
                 not_uploaded.remove(payload)
     ### code for adding unuploaded testcases
+        # elif re.search('50[0-9]',str(response.status_code)):
+        #     if payload not in not_uploaded:
+        #         not_uploaded.append(payload)
+        #         logging.info("Testcase data is not uploaded")
+        #         if x != None:
+        #             global flag
+        #             flag = True
+        # else:
+        #     logging.info("Some Error From the Client Side, Terminating Execution")
+        #     sys.exit()
         else:
             if payload not in not_uploaded:
                 not_uploaded.append(payload)
                 logging.info("Testcase data is not uploaded")
                 if x != None:
                     global flag
                     flag = True
@@ -160,15 +175,15 @@
     payload['testcase_info'] = sorted_dict
 
     tc_count = 0
     try:
         # tc_count = sum(list(set(payload.get('testcase_info', {}).values()) - set(['TOTAL'])))
         tc_count = sum(payload.get('testcase_info', {}).values()) - payload.get('testcase_info', {}).get("TOTAL", 0)
     except Exception as e:
-        print(e)
+        traceback.print_exc()
 
     if tc_count > 0:
         payload['expected_testcases'] = tc_count
     for s in status:
         if sorted_dict.get(s.name, 0) > 0:
             payload['status'] = s.name
             break
```

### Comparing `gempyp-1.0.60b2/gempyp/engine/engine.py` & `gempyp-1.0.70b0/gempyp/engine/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from gempyp.pyprest.pypRest import PypRest
 import smtplib
 from gempyp.dv.dvRunner import DvRunner
 from gempyp.jira.jiraIntegration import jiraIntegration
 from multiprocessing import Process, Pipe
 from gempyp.libs.gem_s3_common import upload_to_s3, create_s3_link
 from gempyp.libs.common import *
+import re
 
 
 
 def executorFactory(data: Dict,conn= None, custom_logger=None ) -> Tuple[List, Dict]:
     
     """
     calls the differnt executors method based on testcase type e.g. gempyp,pyprest,dvm
@@ -130,23 +131,23 @@
         #         if dataUpload.suite_uploaded == False:
         #             logging.info("------Retrying to Upload Suite Data------")
         #             dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"])
             
         self.makeOutputFolder()
         self.start()
 
-        if(self.jewel_user):
+        if(self.jewel_user and DefaultSettings.apiSuccess):
             self.DATA.retryUploadSuiteData(self.bridgetoken,self.username)
             ### Trying to reupload suite data
             # if dataUpload.suite_uploaded == False:
             #     logging.info("------Retrying to Upload Suite Data------")
             #     dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"])
 
         ### checking if suite data is uploaded if true than retrying to upload testcase otherwise storing them in json file
-        jewel,failed_Utestcases,unuploaded_path=self.DATA.retryUploadTestcases(self.s_run_id,self.bridgetoken,self.username,self.ouput_folder)
+        jewel,failed_Utestcases=self.DATA.retryUploadTestcases(self.s_run_id,self.bridgetoken,self.username,self.ouput_folder)
         # if dataUpload.suite_uploaded == True:
         #     jewelLink = DefaultSettings.getUrls('jewel-url')
         #     self.jewel = f'{jewelLink}/#/autolytics/execution-report?s_run_id={self.s_run_id}&p_id={DefaultSettings.project_id}'
         #     if len(dataUpload.not_uploaded) != 0:
         #         logging.info("------Trying again to Upload Testcase------")
         #         for testcase in dataUpload.not_uploaded:
         #             dataUpload.sendTestcaseData(testcase, self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"])
@@ -178,15 +179,16 @@
         #     pass
 
     
 
         
         # ### checking if suite post/get request is successful to call put request otherwise writing suite data in a file
         # if dataUpload.suite_uploaded == True:
-        if dataUpload.suite_uploaded:
+        unuploaded_path = None
+        if dataUpload.suite_uploaded and DefaultSettings.apiSuccess:
             dataUpload.sendSuiteData(self.DATA.toSuiteJson(), self.bridgetoken, self.username, mode="PUT")
 
             if self.skip_jira == 0:
                 jira_id = jiraIntegration(self.s_run_id, self.jira_email, self.jira_access_token, self.jira_project_id, self.project_env, self.jira_workflow, self.jira_title, self.bridgetoken, self.username, self.report_name)  # adding title  ######################### post 1.0.4
                 if jira_id is not None:
                     self.DATA.suite_detail.at[0, "meta_data"].append({"Jira_id": jira_id})
             # # dataUpload.sendSuiteData(self.DATA.toSuiteJson(), self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"], mode="PUT")
@@ -195,21 +197,21 @@
             #     logging.warning("Maybe username or bridgetoken is missing or wrong thus data is not uploaded in db.")
             # dataUpload.suite_data.append(self.DATA.toSuiteJson())
             # listToStr = ',\n'.join(map(str, dataUpload.suite_data))
             # unuploaded_path = os.path.join(self.ouput_folder, "Unuploaded_suiteData.json")
             # with open(unuploaded_path,'w') as w:
             #     w.write(listToStr)
             #     w.write(listToStr)
-            unuploaded_path=self.DATA.WriteSuiteFile(self.base_url,self.ouput_folder)
+            unuploaded_path=self.DATA.WriteSuiteFile(self.base_url,self.ouput_folder,self.username,self.bridgetoken)
             
         if("EMAIL_TO" in self.PARAMS.keys()):
             sendMail(self.s_run_id,self.mail,self.bridgetoken, self.username)
 
-        self.repJson, output_file_path = TemplateData().makeSuiteReport(self.DATA.getJSONData(), self.testcase_data, self.ouput_folder,self.jewel_user)
-        TemplateData().repSummary(self.repJson, output_file_path, jewel, failed_Utestcases, unuploaded_path,self.bridgetoken,self.username,self.jewel_user)
+        self.repJson = TemplateData().makeSuiteReport(self.DATA.getJSONData(), self.testcase_data, self.ouput_folder,self.jewel_user)
+        TemplateData().repSummary(self.repJson, jewel, unuploaded_path)
 
     def makeOutputFolder(self):
         """
         make outputFolder for report named as gempyp_reports in user home directory if not given by the user and makes log fplder for log files
         if given by user than set user given path for reports file   
         """
 
@@ -327,14 +329,16 @@
         if "S_RUN_ID" in self.PARAMS:
             self.s_run_id = self.PARAMS["S_RUN_ID"]
         else:
             if not self.unique_id:
                 self.unique_id = uuid.uuid4()
             self.s_run_id = f"{self.project_name}_{self.project_env}_{self.unique_id}"
             self.s_run_id = self.s_run_id.upper()
+        self.s_run_id = re.sub(r'[^\w\s]', '',self.s_run_id)
+        self.s_run_id=re.sub(r'\s+', '_',self.s_run_id)
         logging.info("S_RUN_ID: {}".format(self.s_run_id))
         suite_details = {
             "s_run_id": self.s_run_id,
             "s_start_time": self.start_time,
             "s_end_time": None,
             "s_id": self.PARAMS.get("S_ID", "test_id"),
             "status": status.EXE.name,
@@ -370,15 +374,18 @@
             logging.error(traceback.format_exc())
             try:
                 self.DATA.suite_detail.at[0, "meta_data"].append({"REASON OF FAILURE": str(e)})
                 self.updateSuiteData()
             except Exception as err:
                 logging.error(traceback.format_exc())
                 logging.info(err)
-            dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.bridgetoken, self.username)
+            if DefaultSettings.apiSuccess:
+                dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.bridgetoken, self.username)
+            else:
+                dataUpload.suite_data.append(self.DATA.toSuiteJson())
             # need to add reason of failure of the suite in misc
 
 
     def updateSuiteData(self):
         """
         updates the suiteData after all the runs have been executed
         """
@@ -540,15 +547,15 @@
                 )
                 output = [output]
             if 'json_data' in output[0]:
                 unsorted_dict = output[0]['json_data']['meta_data'][2]
                 sorted_dict = self.totalOrder(unsorted_dict)
                 output[0]['json_data']['meta_data'][2] = sorted_dict
 
-            output[0]['testcase_dict']['run_type'], output[0]['testcase_dict']['run_mode'] = self.set_run_type_mode()
+            output[0]['testcase_dict']['run_type'], output[0]['testcase_dict']['run_mode'],output[0]['testcase_dict']['job_name'],output[0]['testcase_dict']['job_runid'] = self.set_run_type_mode()
             for i in output:
                 if 'json_data' in i:
                     i["testcase_dict"]["steps"] = i["json_data"]["steps"]
                 else:
                     i["testcase_dict"]["steps"] = self.build_err_step_case()
                 
                 testcase_dict = i["testcase_dict"]
@@ -563,36 +570,82 @@
                 self.DATA.testcase_details = self.DATA.testcase_details.append(
                     testcase_dict, ignore_index=True
                 )
                 self.updateTestcaseMiscData(
                     i["misc"], tc_run_id=testcase_dict.get("tc_run_id")
                 )
         
-                if(self.jewel_user):
+                if(self.jewel_user and dataUpload.suite_uploaded):
                     dataUpload.sendTestcaseData((self.DATA.totestcaseJson(testcase_dict.get("tc_run_id").upper(), self.s_run_id)), self.bridgetoken, self.username)
+                else:
+                    dataUpload.not_uploaded.append((self.DATA.totestcaseJson(testcase_dict.get("tc_run_id").upper(), self.s_run_id)))
         except Exception as e:
             traceback.print_exc()
             logging.error("in update_df: {e}".format(e=e))
     
     def build_err_step_case(self):
         step = [{'Step Name': 'Starting Test', 'Step Description': 'Either the testcase is inappropriate or some error occured while executing the test. Please recheck', 'status': 'ERR'}]
          
         return step
+    
+    def raise_exception(self,name):
+        raise ValueError("{} does not exist".format(name))
 
     def set_run_type_mode(self):
-        type, mode = None, None
         try:
-            if self.PARAMS.get('RUN_TYPE', RunTypes.ON_DEMAND.value) in [i.value for i in RunTypes]:
-                type = self.PARAMS.get('RUN_TYPE', RunTypes.ON_DEMAND.value)
-
-            operating_system = "cli-" + platform.uname().system
-            mode = self.PARAMS.get('RUN_MODE', operating_system.upper())
-        except Exception as e:
-            traceback.print_exc()
-        return type, mode
+            run_type=run_mode=job_name=job_runid=None
+            mappings = {('JEWEL'): { 
+                'run_type': 'Scheduled', 
+                'run_mode': 'JEWEL',
+                'job_name': lambda: os.environ.get('JEWEL_JOB',None), 
+                'job_runid': 'NONE' 
+            },
+            ('SCHEDULER_TOOL'): { 
+            'run_type': 'Scheduled', 
+            'run_mode': lambda: os.environ.get('SCHEDULER_TOOL'), 
+            'job_name': lambda: os.environ.get('SCHEDULER_JOB') if os.environ.get('SCHEDULER_JOB',None) else self.raise_exception("Schedular job"), 
+            'job_runid': lambda: os.environ.get('SCHEDULER_RUNNUM') if os.environ.get('SCHEDULER_RUNNUM',None) else self.raise_exception("Schedular rennum")
+            }, 
+            ('CI_CD_CT_TOOL'): { 
+            'run_type': 'CI-CD-CT', 
+            'run_mode': lambda: os.environ.get('CI_CD_CT_TOOL') if os.environ.get('CI_CD_CT_TOOL',None) else self.raise_exception("CI_CD_CT_TOOL"), 
+            'job_name': lambda: os.environ.get('CI_CD_CT_JOB') if os.environ.get('CI_CD_CT_JOB',None) else self.raise_exception('CI_CD_CT_JOB'), 
+            'job_runid': lambda: os.environ.get('CI_CD_CT_RUNNUM') if os.environ.get('CI_CD_CT_RUNNUM',None) else self.raise_exception('CI_CD_CT_RUNNUM') 
+            }, 
+            ('AUTO_JOB_NAME'): { 
+            'run_type': 'Scheduled', 
+            'run_mode': 'Autosys', 
+            'job_name': lambda: os.environ.get('AUTOSERV') + '.' + os.environ.get('AUTO_JOB_NAME') if os.environ.get('AUTOSERV',None) and os.environ.get('AUTO_JOB_NAME',None) else self.raise_exception("AUTOSERV or AUTO_JOB_NAME"), 
+            'job_runid': lambda: os.environ.get('AUTO_JOBID') if os.environ.get('AUTO_JOBID',None) else self.raise_exception("AUTO_JOBID")
+            }, 
+            ('JENKINS_URL'): { 
+            'run_type': lambda: 'Scheduled' if os.environ.get('BUILD_CAUSE')=='TIMERTRIGGER' else 'CI-CD-CT' if os.environ.get('BUILD_CAUSE')=='SCMTRIGGER'  else 'On Demand', 
+            'run_mode': 'Jenkins', 
+            'job_name': lambda: os.environ.get('JOB_DISPLAY_URL') if os.environ.get('JOB_DISPLAY_URL',None) else self.raise_exception("JOB_DISPLAY_URL"), 
+            'job_runid': lambda: os.environ.get('BUILD_URL') if os.environ.get('BUILD_URL',None) else self.raise_exception("BUILD_URL")}
+            }
+            # Try to match the environment variables to one of the defined mappings 
+            for env_vars, mapping in mappings.items():
+                if (env_vars in os.environ):
+                        # Evaluate the values that require computation (i.e. lambda functions) 
+                        run_type = mapping['run_type']() if callable(mapping['run_type']) else mapping['run_type'] 
+                        run_mode = mapping['run_mode']() if callable(mapping['run_mode']) else mapping['run_mode'] 
+                        job_name = mapping['job_name']() if callable(mapping['job_name']) else mapping['job_name'] 
+                        job_runid = mapping['job_runid']() if callable(mapping['job_runid']) else mapping['job_runid'] 
+                        break 
+                else: 
+                    # If no mapping is found, set default values 
+                    run_type = 'On Demand' 
+                    # run_mode = os.name
+                    run_mode=platform.uname().system
+                    job_name = 'NONE' 
+                    job_runid = 'NONE'
+        except ValueError as e:
+            logging.error(e)
+        return run_type,run_mode,job_name,job_runid
 
     def getErrorTestcase(
         self,
         message: str,
         testcase_name: str,
         category: str = None,
         product_type: str = None,
@@ -788,8 +841,7 @@
                 unsorted_dict.pop(key)
             elif key == "PASS" or key == 'FAIL':
                 sorted_dict[key] = 0
         sorted_dict.update(unsorted_dict)
         return sorted_dict
     
      
-
```

### Comparing `gempyp-1.0.60b2/gempyp/engine/gempypHelper.py` & `gempyp-1.0.70b0/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/engine/runner.py` & `gempyp-1.0.70b0/gempyp/engine/runner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.70b0/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/engine/testData.py` & `gempyp-1.0.70b0/gempyp/engine/testData.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from gempyp.libs.common import dateTimeEncoder, findDuration
 from datetime import datetime, timezone
 import numpy as np
 from gempyp.engine import dataUpload
 import logging
 import os
 from gempyp.config import DefaultSettings
+from cryptography.fernet import Fernet
+from gempyp.config.DefaultSettings import encrypt_key, checkUrl
 
 class TestData:
     def __init__(self):
         """
         declairing some attribute the are used in testcaseDetails in report and return a object that is used to update data
         """
         self.testcaseDetailColumn = [
@@ -198,24 +200,26 @@
 
     def validateSrunidInDB(self,jewel_user,s_run_id,username,bridgetoken):
         if jewel_user:
             # if "RUN_ID" in params:
             if s_run_id:
                 logging.info("************Trying to check If s_run_id is present in DB*****************")
                 # response =  dataUpload.checkingData(s_run_id, params["BRIDGE_TOKEN"], params["USERNAME"])
-                if not dataUpload.checkingData(s_run_id,bridgetoken, username):
-                    logging.info("************s_run_id not present in DB Trying to call Post*****************")
-                    dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken,username)
-                else:
-                    print("s_run_id already present --------------")
-                    dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken, username,mode="PUT")
+                if DefaultSettings.apiSuccess:
+                    if not dataUpload.checkingData(s_run_id,bridgetoken, username):
+                        logging.info("************s_run_id not present in DB Trying to call Post*****************")
+                        dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken,username)
+                    else:
+                        logging.info("---------s_run_id already present --------------")
+                        dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken, username,mode="PUT")
             else:
-                dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken, username)
-                ### first try to rerun the data
-                self.retryUploadSuiteData(bridgetoken,username)
+                if DefaultSettings.apiSuccess:
+                    dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken, username)
+                    ### first try to rerun the data
+                    self.retryUploadSuiteData(bridgetoken,username)
 
     
     def retryUploadSuiteData(self,bridgetoken,username):
             # if dataUpload.suite_uploaded == False:
             if not dataUpload.suite_uploaded:
                         logging.info("------Retrying to Upload Suite Data------")
                         dataUpload.sendSuiteData((self.toSuiteJson()), bridgetoken, username)
@@ -225,43 +229,54 @@
         jewel = ''
         unuploaded_path = ""
         failed_Utestcases=0
         # if dataUpload.suite_uploaded == True:
         if dataUpload.suite_uploaded:
             jewelLink = DefaultSettings.getUrls('jewel-url')
             jewel = f'{jewelLink}/#/autolytics/execution-report?s_run_id={s_run_id}&p_id={DefaultSettings.project_id}'
-            if len(dataUpload.not_uploaded) != 0:
-                logging.info("------Trying again to Upload Testcase------")
-                for testcase in dataUpload.not_uploaded:
-                    dataUpload.sendTestcaseData(testcase,bridgetoken, username)
-                if dataUpload.flag:
-                    logging.warning("Testcase may be present with same tc_run_id in database")
-                unuploaded_path=self.unuploadedFile(output_folder,dataUpload.not_uploaded,"Unploaded_testCases.json")
-            failed_Utestcases = len(dataUpload.not_uploaded) 
+        if len(dataUpload.not_uploaded) != 0 and dataUpload.suite_uploaded:
+            logging.info("------Trying again to Upload Testcase------")
+            for testcase in dataUpload.not_uploaded:
+                dataUpload.sendTestcaseData(testcase,bridgetoken, username)
+            # if dataUpload.flag:
+                # logging.warning("Testcase may be present with same tc_run_id in database")
+            # unuploaded_path=self.unuploadedFile(output_folder,dataUpload.not_uploaded,"Unploaded_testCases.json")
+            # failed_Utestcases = len(dataUpload.not_uploaded) 
             ### Creating file for unuploaded testcases
             # if len(dataUpload.not_uploaded) != 0:
             #     if dataUpload.flag == True:
             #         logging.warning("Testcase may be present with same tc_run_id in database")
             #     unuploaded_path=self.unuploadedFile(output_folder,dataUpload.not_uploaded,"Unploaded_testCases.json")
-        return jewel,failed_Utestcases,unuploaded_path
+        # return jewel,failed_Utestcases,unuploaded_path
+        return jewel,failed_Utestcases
 
 
-    def WriteSuiteFile(self,base_url,output_folder):
+    def WriteSuiteFile(self,base_url,output_folder,username,bridge_token):
             if not base_url:
                 logging.warning("Maybe username or bridgetoken is missing or wrong thus data is not uploaded in db.")
             dataUpload.suite_data.append(self.toSuiteJson())
-            unuploaded_path=self.unuploadedFile(output_folder,dataUpload.suite_data,"Unuploaded_suiteData.json")
+            unuploaded_dict = {}
+            unuploaded_dict["suite_data"] = dataUpload.suite_data
+            unuploaded_dict["testcases"] = dataUpload.not_uploaded
+            # unuploaded_dict["urls"] = DefaultSettings.urls['data']
+            unuploaded_dict["base_url"] = checkUrl(base_url)
+            unuploaded_dict["user_name"] = username
+            unuploaded_dict["bridge_token"] = bridge_token
+            unuploaded_path=self.unuploadedFile(output_folder,unuploaded_dict,"Unuploaded_data.json")
             return unuploaded_path
 
 
     ### Function to create unuploadedFile
     def unuploadedFile(self,output_folder,data,fileName):
         unuploaded_path = ""
-        listToStr = ',\n'.join(map(str, data))
+        # listToStr = ',\n'.join(map(str, data))
         unuploaded_path = os.path.join(output_folder, fileName)
-        with open(unuploaded_path,'w') as w:
-            w.write(listToStr)
+        data = str(data)
+        fernet = Fernet(encrypt_key)
+        data = fernet.encrypt(data.encode())
+        with open(unuploaded_path,'wb') as w:
+            w.write(data)
         return unuploaded_path
```

### Comparing `gempyp-1.0.60b2/gempyp/final_report.html` & `gempyp-1.0.70b0/gempyp/final_report.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/gemPyp.py` & `gempyp-1.0.70b0/gempyp/gemPyp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from gempyp.config.xmlConfig import XmlConfig
 import argparse
 from gempyp.engine.engine import Engine
 from gempyp.libs.common import download_common_file
+from gempyp.data_uploader import dataUploader
+import logging
 
 class Gempyp:
     def __init__(self):
         """
         initiating some variables  
         """
         self.config = None
@@ -22,14 +24,15 @@
         self.JEWEL_USER=None
         self.S_RUN_ID = None
         self.TESTCASE_LIST = None
         self.ENTER_POINT = None
         self.S_ID = None
         self.RUN_TYPE = None
         self.RUN_MODE = None
+        self.RE_RUN = None
     
     def argParser(self):
         """Argument parser to help running through CLI"""
 
         parser = argparse.ArgumentParser()
         parser.add_argument('-config','-c',dest='config',type=str, required=False)
         parser.add_argument('-mailTo','-mailTo',dest='MAIL-TO', type=str, required=False)
@@ -46,32 +49,45 @@
         parser.add_argument('-category','-category',dest='CATEGORY',type=str, required=False)
         parser.add_argument('-run_id','-run_id',dest='S_RUN_ID',type=str, required=False)
         parser.add_argument('-tc','-testcase_list',dest='TESTCASE_LIST',type=str, required=False)
         parser.add_argument('-enter_point','-enter_point',dest='ENTER_POINT',type=str, required=False)
         parser.add_argument('-s_id','-s_id',dest='S_ID',type=str, required=False)
         parser.add_argument('-run_type','-run_type',dest='RUN_TYPE',type=str, required=False)
         parser.add_argument('-run_mode','-run_mode',dest='RUN_MODE',type=str, required=False)
+        parser.add_argument('-rerun','-rerun',dest='RE_RUN',type=str, required=False)
 
         args = parser.parse_args()
         return args
 
     def runner(self):
         """
         This function takes the config and updates the config data in case or cli run and direct(python) run
         """
         s_run_id = vars(self)["S_RUN_ID"]
-        file_path=download_common_file(self.config)
-        config=XmlConfig(file_path,s_run_id)
-        if not self.args:
-            del self.__dict__["args"]
-            config.cli_config = vars(self)
+        # if self.args != None:
+        if self.args.RE_RUN != None:
+                print("Trying to Reupload Data")
+                dataUploader(self.args.RE_RUN,self.args.JEWEL_BRIDGE_TOKEN)
+        elif self.RE_RUN != None:
+                print("Trying to Reupload Data")
+                if self.args.JEWEL_BRIDGE_TOKEN:
+                    dataUploader(self.RE_RUN, self.args.JEWEL_BRIDGE_TOKEN)
+                else:
+                    dataUploader(self.RE_RUN, self.JEWEL_BRIDGE_TOKEN)
+        # if self.args.RE_RUN
         else:
-            config.cli_config = vars(self.args)
-        config.update()
-        Engine(config)
+            file_path=download_common_file(self.config)
+            config=XmlConfig(file_path,s_run_id)
+            if not self.args:
+                del self.__dict__["args"]
+                config.cli_config = vars(self)
+            else:
+                config.cli_config = vars(self.args)
+            config.update()
+            Engine(config)
 
     def parser(self):
         """Calls the parser and handles the case of no cli args"""
         args = self.argParser()
         if args.config != None:
             self.config = args.config
         self.args = args
```

### Comparing `gempyp-1.0.60b2/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.70b0/gempyp/jira/jiraIntegration.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.70b0/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/libs/common.py` & `gempyp-1.0.70b0/gempyp/libs/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,18 +216,18 @@
     if not testcaseLength:  # in case of zero testcases, we should not insert suite data 
             logging.warning("NO TESTCASES TO RUN..... PLEASE CHECK RUN FLAGS. ABORTING.................")
             sys.exit()
             
 
 
 def runBaseUrls(jewel_user,base_url,username,bridgetoken):
-    if jewel_user:
+    
             #trying rerun of base url api in case of api failure
             if base_url and DefaultSettings.apiSuccess == False:
-                logging.info("Retrying to call Api for getting urls")
+                logging.info("Trying to call Api for getting urls")
                 DefaultSettings.getEnterPoint(base_url ,bridgetoken,username)
             if not base_url:
                 DefaultSettings.getEnterPoint(DefaultSettings.default_baseurl ,bridgetoken, username)
 
 
 def sendMail(s_run_id,mails,bridge_token,username):
     try:
```

### Comparing `gempyp-1.0.60b2/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.70b0/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/libs/logConfig.py` & `gempyp-1.0.70b0/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/libs/parsers.py` & `gempyp-1.0.70b0/gempyp/libs/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
             # we treat them as list
             else:
                 Result[element.tag.upper()] = xmlToList(element)
 
         # if the element doesnot have any children
         else:
-            Result[element.tag.upper()] = element.text
+            if(type(element.tag)==str):
+                Result[element.tag.upper()] = element.text
     return remove_none_from_dict(Result)  ##################### post 1.0.4
 
 
 def xmlToList(root) -> List:
     Result = []
 
     for element in root:
```

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.70b0/gempyp/pyprest/apiCommon.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.70b0/gempyp/pyprest/compareFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.70b0/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.70b0/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.70b0/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.70b0/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/postVariables.py` & `gempyp-1.0.70b0/gempyp/pyprest/postVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.70b0/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/preVariables.py` & `gempyp-1.0.70b0/gempyp/pyprest/preVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/pypRest.py` & `gempyp-1.0.70b0/gempyp/pyprest/pypRest.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/reporting.py` & `gempyp-1.0.70b0/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/restEngine.py` & `gempyp-1.0.70b0/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/restObj.py` & `gempyp-1.0.70b0/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/utils.py` & `gempyp-1.0.70b0/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.70b0/gempyp/pyprest/variableReplacement.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     def getVariableValues(self, var_name):
         varName = var_name.strip("$[#]")
         try:
             # if "SUITE.".casefold() or "ENV.".casefold() in varName.casefold()
             if "SUITE.".casefold() in varName.casefold():  # ############ post 1.0.4
                 varValue = self.suite_pre_variables[varName.replace(".", "_").upper()]
                 print(varValue)
-            if "ENV.".casefold() in varName.casefold() and os.environ.get(varName.strip("$[#ENV.").strip("]")):
-                varValue = os.environ.get(varName.strip("$[#ENV.").strip("]"))
             else:
                 varValue = self.local_pre_variables[varName]
                 # suite_variables
                 # varValue = self.local_pre_variables[varName]
+            if "ENV.".casefold() in varName.casefold() and os.environ.get(varName.strip("$[#ENV.").strip("]")):
+                varValue = os.environ.get(varName.strip("$[#ENV.").strip("]"))
         except:
             return "null"
         str_val = var_name.replace("$[#"+varName+"]", str(varValue))
         if "$[#" not in str_val:
             return str(str_val) 
         if "$[#" or "$" in str_val:
             return self.getVariableValues(str_val)
```

### Comparing `gempyp-1.0.60b2/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.70b0/gempyp/reporter/reportGenerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -116,52 +116,52 @@
         # self.testcaseData = json.dumps(self.testcaseData)
         reportJson = json.dumps(reportJson)
         suiteReport = suiteReport.replace("DATA_1", reportJson)
         
         # if not len(testcase_data) > 0:   ##TODO
         #     return repJson, None
         ouput_file_path=""
-        if not jewel_user:
-            ResultFile = os.path.join(ouput_folder, "Result_{}.html".format(date))
-            ouput_file_path = ResultFile
-            with open(ResultFile, "w+") as f:
-                f.write(suiteReport)
-        return repJson, ouput_file_path
+        # if not jewel_user:
+        #     ResultFile = os.path.join(ouput_folder, "Result_{}.html".format(date))
+        #     ouput_file_path = ResultFile
+        #     with open(ResultFile, "w+") as f:
+        #         f.write(suiteReport)
+        # return repJson, ouput_file_path
+        return repJson
     
     def makeTestcaseReport(self):
         index_path = os.path.dirname(__file__)
         index_path = os.path.join(os.path.split(index_path)[0], "testcase.html")
         with open(index_path, "r") as f:
             Result_data = f.read()
         json_data = self._toJSON()
         return json.loads(json_data)
 
-    def repSummary(self, repJson, output_file_path, jewel_link, failed_testcases, unuploaded_path,bridgetoken,username,jewel_user):
+    def repSummary(self, repJson,jewel_link, unuploaded_path):
         """
         logging some information
         """
         try:
             logging.info("---------- Finalised the report --------------")
             logging.info("============== Run Summary =============")
             count_info = {key.lower(): val for key, val in repJson['suits_details']['testcase_info'].items()}
             log_str = f"Total Testcases: {str(count_info.get('total', 0))} | Passed Testcases: {str(count_info.get('pass', 0))} | Failed Testcases: {str(count_info.get('fail', 0))} | "
             status_dict = {"info": "Info", "warn": "WARN", "exe": "Exe", "err":"ERR"}
             for key, val in count_info.items():
                 if key in status_dict.keys():
                     log_str += f"{status_dict[key.lower()]} Testcases: {val} | "
             logging.info(log_str.strip(" | "))
 
-            if failed_testcases != 0:
-                logging.info(f"Number of Testcases not Uploaded:{failed_testcases}")
-                logging.info(f"Unuploaded Testcase File Path:{unuploaded_path}")
+            if unuploaded_path != None:
+                logging.info(f"Unuploaded Data File Path:{unuploaded_path}")
             #  we will check if output report is None, then display report not created
             if len(jewel_link)>0:
 #                 s3_report_file_url= create_s3_link(url=upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=bridgetoken, username=username, file=output_file_path.split('/')[-1],tag="public")[0]["Url"]) 
                 logging.info('Report at Jewel: {link}'.format(link = jewel_link))
 #                 logging.info('Report at S3: {link}'.format(link = s3_report_file_url))
                 
-            if not jewel_user:
-                logging.info('-------- Report created Successfully at: {path}'.format(path=output_file_path))
+            # if not jewel_user:
+                # logging.info('-------- Report created Successfully at: {path}'.format(path=output_file_path))
 
 
         except Exception as e:
             logging.error(traceback.format_exc(e))
```

### Comparing `gempyp-1.0.60b2/gempyp/sdk/executor.py` & `gempyp-1.0.70b0/gempyp/sdk/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from asyncio.log import logger
 import getpass
 import json
 from pathlib import Path
 import sys
 import uuid
 from datetime import datetime
 from gempyp.engine.baseTemplate import TestcaseReporter
@@ -16,43 +15,46 @@
 import logging
 import tempfile
 import subprocess
 import sys
 import os
 import pandas as pd
 from gempyp.libs.enums.status import status
+from gempyp.libs.common import *
 
 
 class Executor(TestcaseReporter):
     def __init__(self, **kwargs):
         self.method = kwargs.get("tc_name", self.getMethodName())
-        self.log_file = tempfile.gettempdir() + "\logs.txt"
+        self.log_file = tempfile.gettempdir() + "\logs.log"
         # os.makedirs("testcase_log_folder")
+        print(self.log_file)
         sys.stdout = sys.stderr =  open(self.log_file, 'w')
-        logging.basicConfig(filename="logs.txt", filemode='w', format='%(name)s - %(asctime)s-%(levelname)s - %(message)s',level=logging.DEBUG)
-        # custom_logger = my_custom_logger("logs.txt")
+        logging.basicConfig(filename="logs.log", filemode='w', format='%(name)s - %(levelname)s - %(message)s',level=logging.DEBUG)
+        # custom_logger = my_custom_logger("logs.log")
         logging.info("inside constructor here--------------------")
         logging.info(f"-------Executing testcase - {self.getMethodName()}---------")
         self.data = self.getTestcaseData()
-        self.reporter = TestcaseReporter(self.data["PROJECT"], self.data["NAME"])
+        self.reporter = TestcaseReporter(self.data["PROJECT_NAME"], self.data["NAME"])
        
         
 
         path = __file__
         path = path.rsplit(os.sep, 1)[0]
         self.DATA = TestData()
         # make suite details and upload it
         self.makeSuiteDetails()
+        runBaseUrls(self.jewel_user,self.data["ENTER_POINT"],self.data["JEWEL_USER"],self.data["JEWEL_BRIDGE_TOKEN"])
         if not os.getenv("PID"):
             self.makeOutputFolder()
             os.environ["PID"] = str(os.getpid())
             subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True)
             try:
                 logging.info(f"---------------S_RUN_ID-------------{self.s_run_id}")
-                dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.data["BRIDGE_TOKEN"], self.data["USERNAME"]) # check with deamon, should insert only once
+                dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"]) # check with deamon, should insert only once
                   # logging not working
             except Exception as e:
                 print(f"Exception occured - {e}")
                 pass
 
     def __del__(self):
         self.final()
@@ -67,20 +69,17 @@
         # create testcase reporter json
         self.reporter.json_data = self.reporter.template_data.makeTestcaseReport()
         # serializing data, adding suite data
         report_dict = self.reporter.serialize()
 
         report_dict["TESTCASEMETADATA"] = self.getMetaData()
         report_dict["config_data"] = self.getConfigData()
-
         # creating output json
         output.append(getOutput(report_dict))
-        output[0]["product_type"] = "GEMPYP-SDK"
         for i in output:
-            logging.info("---------------TC_RUN_ID-----------------"+i["testcase_dict"]["tc_run_id"].upper())
             i["testcase_dict"]["steps"] = i["json_data"]["steps"]
             dict_ = {}
             dict_["testcases"] = {}
             dict_["REPORT_LOCATION"] = os.getenv("REPORT_LOCATION")
             dict_["misc_data"] = {}
             tmp_dir = os.path.join(tempfile.gettempdir(), self.s_run_id + ".txt")
             
@@ -94,70 +93,73 @@
             if isinstance(suite_data, str):
                 suite_data = json.loads(suite_data)
             if isinstance(self.DATA.toSuiteJson(), str):
                 suite_temp = json.loads(self.DATA.toSuiteJson())
             if not os.path.exists(tmp_dir):
                 with open(tmp_dir, "w") as f:
                     dict_[self.s_run_id] = self.updateSuiteData(suite_data)
-                    dict_["s_id"] = suite_temp["s_id"]
-                    dict_["misc_data"] = suite_temp["misc_data"]
                     dict_["testcases"][i["testcase_dict"].get("tc_run_id")] = i["json_data"]
                     f.write(json.dumps(dict_))
             else:
                 with open(tmp_dir, "r+") as f:
                     data = f.read()
                     data = json.loads(data)
                     data[self.s_run_id] = self.updateSuiteData(suite_data, data[self.s_run_id])
-                    data["s_id"] = suite_temp["s_id"]
-                    data["misc_data"] = suite_temp["misc_data"]
                     data["testcases"][i["testcase_dict"].get("tc_run_id")] = i["json_data"]
                     f.seek(0)
                     f.write(json.dumps(data))
-            
-            dataUpload.sendTestcaseData((self.DATA.totestcaseJson(i["testcase_dict"]["tc_run_id"].upper(), self.data["S_RUN_ID"])), self.data["BRIDGE_TOKEN"], self.data["USERNAME"])  # instead of output, I need to pass s_run id and  tc_run_id
+            logging.info("---------------TC_RUN_ID-----------------"+i["testcase_dict"]["tc_run_id"].upper())
+            dataUpload.sendTestcaseData((self.DATA.totestcaseJson(i["testcase_dict"]["tc_run_id"].upper(), self.data["S_RUN_ID"])), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"])  # instead of output, I need to pass s_run id and  tc_run_id
             
             # sys.stdout.close()
         
             # os.rename(self.log_file, tmp_dir.rsplit(".", 1)[0] + ".log")
 
             
 
     def getTestcaseData(self):
+        self.jewel_user=False
         config_file = configparser.ConfigParser()
         directory_path = os.getcwd()
 
         if not os.path.exists(directory_path + os.sep + "gempyp.conf"):
             print("Config file is missing. Aborting  gempyp report......")
             sys.exit()
         config_file.read("gempyp.conf")
         data = {}
-        self.projectName = data["PROJECT"] = config_file['ReportSetting']["project"]
+        self.projectName = data["PROJECT_NAME"] = config_file['ReportSetting']["project_name"]
         self.testcaseName = data["NAME"] = self.method
-        self.env = data["ENV"] = config_file['ReportSetting'].get("env", "PROD")
-        data["USERNAME"] = config_file['ReportSetting'].get("USERNAME", getpass.getuser())
-        data["BRIDGE_TOKEN"] = config_file['ReportSetting'].get("BRIDGE_TOKEN", None)
-        data["REPORT_LOCATION"] = config_file['ReportSetting'].get("outputfolder", None)
+        self.env = data["ENVIRONMENT"] = config_file['ReportSetting'].get("environment", "PROD")
+        data["JEWEL_USER"] = config_file['ReportSetting'].get("jewel_user", getpass.getuser())
+        data["JEWEL_BRIDGE_TOKEN"] = config_file['ReportSetting'].get("jewel_bridge_token", None)
+        data["REPORT_LOCATION"] = config_file['ReportSetting'].get("report_location", None)
         data["MACHINE"] = platform.node()
-        data["MAIL"] = config_file['ReportSetting'].get("mail", None)
-        self.report_name = data["REPORT_NAME"] = config_file['ReportSetting'].get("reportname", "SMOKE_TEST")
-        self.report_info=data["REPORT_INFO"]=config_file['ReportSetting'].get("reportinfo", "SMOKE_TEST_INFO")
+        data["MAIL_TO"] = config_file['ReportSetting'].get("mail_to", None)
+        data["MAIL_CC"] = config_file['ReportSetting'].get("mail_cc", None)
+        data["MAIL_BCC"] = config_file['ReportSetting'].get("mail_bcc", None)
+        data["ENTER_POINT"]=config_file['ReportSetting'].get("enter_point", None)
+        if data["JEWEL_USER"] and data["JEWEL_BRIDGE_TOKEN"]:
+            self.jewel_user=True
+        self.report_type = data["REPORT_NAME"] = config_file['ReportSetting'].get("report_name", "SMOKE_TEST")
         if not os.getenv("S_RUN_ID"):
-            s_run_id = data["PROJECT"] + "_" + data["ENV"] + "_" + str(uuid.uuid4())
+            s_run_id = data["PROJECT_NAME"] + "_" + data["ENVIRONMENT"] + "_" + str(uuid.uuid4())
             os.environ["S_RUN_ID"] = s_run_id.upper()
         self.s_run_id = data["S_RUN_ID"] = config_file['ReportSetting'].get("s_run_id", os.getenv("S_RUN_ID"))
         return data
 
     def getMetaData(self):
         data = {
-            'PROJECTNAME': self.data["PROJECT"], 
-            'ENV': self.data["ENV"], 
+            'PROJECT_NAME': self.data["PROJECT_NAME"], 
+            'ENVIRONMENT': self.data["ENVIRONMENT"], 
             'S_RUN_ID': self.data["S_RUN_ID"], 
-            'USER': self.data["USERNAME"], 
+            'USER': self.data["JEWEL_USER"], 
             'MACHINE': self.data["MACHINE"], 
-            'REPORT_LOCATION': self.data["REPORT_LOCATION"]}
+            'REPORT_LOCATION': self.data["REPORT_LOCATION"],
+            'SUITE_VARS': self.data.get("SUITE_VARS", {}),
+            'INVOKE_USER': os.getenv("INVOKEUSER", self.data["JEWEL_USER"])}
         return data
 
     def getMethodName(self):
         try:
             currframe = inspect.currentframe()
             callframe = inspect.getouterframes(currframe, 2)
             count = -1
@@ -177,27 +179,37 @@
         data = {'NAME': self.data["NAME"], 'CATEGORY': 'External','LOGGER': ""}
         return data
 
     def makeSuiteDetails(self):
         """
         making suite Details 
         """
-
+        
+        run_mode = "LINUX_CLI"
+        if os.name == 'nt':
+            run_mode = "WINDOWS"
         Suite_details = {
             "s_run_id": self.data["S_RUN_ID"],
             "s_start_time": datetime.now(timezone.utc),
             "s_end_time": None,
+            "s_id": self.data.get("S_ID", "test_id"),
             "status": status.EXE.name,
-            "project_name": self.data["PROJECT"],
-            "user": self.data["USERNAME"],
-            "report_name": self.data["REPORT_INFO"],
-            "framework_name": "GEMPYP",
-            "env": self.data["ENV"],
+            "project_name": self.data["PROJECT_NAME"],
+            "report_name": self.data["REPORT_NAME"],
+            "run_type": "ON DEMAND",
+            "user": self.data["JEWEL_USER"],
+            "env": self.data["ENVIRONMENT"],
             "machine": self.data["MACHINE"],
+            "initiated_by": self.data["JEWEL_USER"],
+            "run_mode": run_mode,
             "os": platform.system().upper(),
+            "meta_data": [],
+            "testcase_info": None,
+            "expected_testcases":2,
+            "framework_name": "GEMPYP",
         }
         self.DATA.suite_detail = self.DATA.suite_detail.append(
             Suite_details, ignore_index=True
         )
 
         
 
@@ -223,16 +235,16 @@
     def makeOutputFolder(self):
         """
         to make GemPyp_Report folder 
         """
 
         logging.info("---------- Making output folders -------------")
         report_folder_name = f"{self.projectName}_{self.env}"
-        if self.report_name:
-            report_folder_name = report_folder_name + f"_{self.report_name}"
+        if self.report_type:
+            report_folder_name = report_folder_name + f"_{self.report_type}"
         date = datetime.now().strftime("%Y_%b_%d_%H%M%S_%f")
         report_folder_name = report_folder_name + f"_{date}"
         if self.data.get("REPORT_LOCATION"):
             self.ouput_folder = os.path.join(
                 self.data.get("REPORT_LOCATION"), report_folder_name
             )
         else:
@@ -245,38 +257,39 @@
         os.makedirs(self.ouput_folder)
 
     def updateSuiteData(self, current_data, old_data=None):
         """
         updates the suiteData after all the runs have been executed
         """
         start_time = current_data["suits_details"]["s_start_time"]
-        end_time = current_data["suits_details"]["testcase_details"][0]["end_time"]
-        testcaseData = current_data["suits_details"]["testcase_details"]
+        end_time = current_data["suits_details"]['testcase_details'][0]["end_time"]
+        testcaseData = current_data["suits_details"]['testcase_details']
         if old_data:
-            testcaseData = (old_data["suits_details"]["testcase_details"]
-             + current_data["suits_details"]["testcase_details"])
+            testcaseData = (old_data["suits_details"]['testcase_details']
+             + current_data["suits_details"]['testcase_details'])
             start_time = old_data["suits_details"]["s_start_time"]
         statusDict = {k.name: 0 for k in status}
         for i in testcaseData:
             statusDict[i["status"]] += 1
         # get the status count of the status
         SuiteStatus = status.FAIL.name
 
         # based on the status priority
         for s in status:
             if statusDict.get(s.name, 0) > 0:
                 SuiteStatus = s.name
 
         current_data["suits_details"]["status"] = SuiteStatus
-        current_data["suits_details"]["testcase_details"] = testcaseData
+        current_data["suits_details"]['testcase_details'] = testcaseData
         current_data["suits_details"]["s_start_time"] = start_time
         current_data["suits_details"]["s_end_time"] = end_time
         count = 0
         for key in list(statusDict.keys()):
             if statusDict[key] == 0:
                 del statusDict[key]
             else:
                 count += statusDict[key]
-        statusDict["Total"] = count
-        current_data["suits_details"]["Testcase_Info"] = statusDict
+        statusDict["total"] = count
+        current_data["suits_details"]["expected_testcases"]=count
+        current_data["suits_details"]["testcase_info"] = statusDict
 
-        return current_data
+        return current_data
```

### Comparing `gempyp-1.0.60b2/gempyp/sdk/worker.py` & `gempyp-1.0.70b0/gempyp/sdk/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,45 +3,48 @@
 import json
 import configparser
 import psutil
 import sys
 from gempyp.engine import dataUpload
 from gempyp.reporter.reportGenerator import TemplateData
 import logging
+from gempyp.libs.common import *
 
 
 def pid_running(pid):
     if not pid:
         return False
     if psutil.pid_exists(int(pid)):
         return True
     else:
         return False
 
 def create_report(data, s_run_id):
-
+     # read bridgetoken
+    try:
+        jewel=False
+        config_file = configparser.ConfigParser()
+        config_file.read("gempyp.conf")
+        bridgetoken = config_file['ReportSetting'].get("jewel_bridge_token", None)
+        username=config_file['ReportSetting'].get("jewel_user", None)
+        if username and bridgetoken:
+            jewel=True
+    except Exception as e:
+        bridgetoken = None
     data = json.loads(data)
+    runBaseUrls(jewel,config_file['ReportSetting'].get("enter_point", None),username,bridgetoken)
     json_data = data[s_run_id]
     testcaseData = data["testcases"]
     output_folder = data["REPORT_LOCATION"]
-    repJson, ouput_file_path = TemplateData().makeSuiteReport(json.dumps(json_data), testcaseData, output_folder)
+    repJson, ouput_file_path = TemplateData().makeSuiteReport(json.dumps(json_data), testcaseData, output_folder,jewel)
     suite_data = json_data["suits_details"]
-    suite_data["s_id"] = data["s_id"]
     suite_data["misc_data"] = data["misc_data"]
     username = suite_data["initiated_by"]
     del suite_data["testcase_details"]
-    del suite_data["Testcase_Info"]
-
-    # read bridgetoken
-    try:
-        config_file = configparser.ConfigParser()
-        config_file.read("gempyp.conf")
-        bridgetoken = config_file['ReportSetting'].get("bridge_token", None)
-    except Exception as e:
-        bridgetoken = None
+    del suite_data["testcase_info"]
     dataUpload.sendSuiteData(json.dumps(suite_data), bridgetoken, username, mode="PUT")
     return ouput_file_path
 
 
 if __name__ == "__main__":
     while(True):
         if not pid_running(os.environ["PID"]):
@@ -51,12 +54,12 @@
                 file_path = os.path.join(tempfile.gettempdir(), s_run_id + ".txt")
                 if os.path.exists(file_path):
                     with open(file_path, "r+") as f:
                         data = str(f.read())
                         output_file_path = create_report(data, s_run_id)
                         # where to get this json data from
                         current_pid = os.getpid()
-                        logging.info(f"Find Gempyp logs at - {s_run_id + '.txt'}")  ## replacing log with txt for UI compatibility
+                        logging.info(f"Find Gempyp logs at - {s_run_id + '.log'}")
                         logging.info(f"Find Gempyp Report at - {output_file_path}")
-                        os.rename("logs.txt",f"{s_run_id}.txt")
+                        os.rename("logs.log",f"{s_run_id}.log")
                         os.kill(current_pid, 19)
-                        sys.exit()
+                        sys.exit()
```

### Comparing `gempyp-1.0.60b2/gempyp/testcase.html` & `gempyp-1.0.70b0/gempyp/testcase.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/pyproject.toml` & `gempyp-1.0.70b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.60-beta.2"
+version = "1.0.70b"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
```

### Comparing `gempyp-1.0.60b2/README.md` & `gempyp-1.0.70b0/README.md`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.60b2/PKG-INFO` & `gempyp-1.0.70b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gempyp
-Version: 1.0.60b2
+Version: 1.0.70b0
 Summary: An ecosystem of libraries useful for software development
 Home-page: https://github.com/Gemini-Solutions/gempyp
 License: MIT
 Author: Gemini Solutions-QA
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
 Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
 Requires-Dist: cffi (>=1.15.0,<2.0.0)
 Requires-Dist: charset-normalizer (>=2.0.12,<3.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: cryptography (>=38.0.1,<39.0.0)
 Requires-Dist: humanfriendly (>=10.0,<11.0)
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: gempyp Version: 1.0.60b2 Summary: An ecosystem of
+Metadata-Version: 2.1 Name: gempyp Version: 1.0.70b0 Summary: An ecosystem of
 libraries useful for software development Home-page: https://github.com/Gemini-
 Solutions/gempyp License: MIT Author: Gemini Solutions-QA Requires-Python:
 >=3.6.8,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0) Requires-Dist:
-certifi (>=2022.6.15,<2023.0.0) Requires-Dist: cffi (>=1.15.0,<2.0.0) Requires-
-Dist: charset-normalizer (>=2.0.12,<3.0.0) Requires-Dist: coloredlogs
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: XlsxWriter (>=3.0.3,<4.0.0) Requires-Dist: certifi
+(>=2022.6.15,<2023.0.0) Requires-Dist: cffi (>=1.15.0,<2.0.0) Requires-Dist:
+charset-normalizer (>=2.0.12,<3.0.0) Requires-Dist: coloredlogs
 (>=15.0.1,<16.0.0) Requires-Dist: cryptography (>=38.0.1,<39.0.0) Requires-
 Dist: humanfriendly (>=10.0,<11.0) Requires-Dist: idna (>=3.4,<4.0) Requires-
 Dist: lxml (>=4.9.0,<5.0.0) Requires-Dist: mysql-connector-python
 (>=8.0.30,<9.0.0) Requires-Dist: ntlm-auth (>=1.5.0,<2.0.0) Requires-Dist:
 numpy (>=1.19.5,<2.0.0) Requires-Dist: pandas (>=1.1.5,<2.0.0) Requires-Dist:
 pg8000 (>=1.26.0,<2.0.0) Requires-Dist: pycparser (>=2.21,<3.0) Requires-Dist:
 pyreadline (>=2.1,<3.0) Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) Requires-
```

