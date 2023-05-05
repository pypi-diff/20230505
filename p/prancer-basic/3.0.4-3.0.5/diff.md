# Comparing `tmp/prancer-basic-3.0.4.tar.gz` & `tmp/prancer-basic-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prancer-basic-3.0.4.tar", last modified: Thu Apr  6 10:31:50 2023, max compression
+gzip compressed data, was "prancer-basic-3.0.5.tar", last modified: Fri May  5 11:39:43 2023, max compression
```

## Comparing `prancer-basic-3.0.4.tar` & `prancer-basic-3.0.5.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.765941 prancer-basic-3.0.4/
--rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/LICENSE
--rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-06 10:31:50.765941 prancer-basic-3.0.4/PKG-INFO
--rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 10:31:50.765941 prancer-basic-3.0.4/setup.cfg
--rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.733940 prancer-basic-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/prancer_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 10:31:50.000000 prancer-basic-3.0.4/src/prancer_basic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/collection_config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/collection_config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/collection_config/config_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparison_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorLexer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorListener.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorParser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/compare_types.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/rule_interpreter.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/test_comparator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/rules/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/rules/arm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/arm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7732 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/arm/secret_azure_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/rules/cloudformation/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/cloudformation/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.745940 prancer-basic-3.0.4/src/processor/comparison/rules/common/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/common/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/common/sensitive_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.749940 prancer-basic-3.0.4/src/processor/comparison/rules/deploymentmanager/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/deploymentmanager/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.749940 prancer-basic-3.0.4/src/processor/comparison/rules/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/terraform/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/comparison/rules/terraform/secret_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/arn_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/connector/git_connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/git_connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/git_connector/git_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/git_connector/git_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10750 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    58325 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_aws.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23404 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_azure.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_azure_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_base.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_custom.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_custom_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_db.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_exception.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_fs.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33234 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_google.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_kubernetes.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/snapshot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/connector/special_compliance/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/special_compliance/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/special_compliance/compliances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/connector/special_crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/special_crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/special_crawler/azure_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/special_crawler/base_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/validation.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/connector/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23940 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/crawler/master_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/database/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/database/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     9830 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/database/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/helper/config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/config/config_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/config/remote_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/config/rundata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/helper/file/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/file/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/file/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.753940 prancer-basic-3.0.4/src/processor/helper/hcl/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/hcl/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/hcl/hcl_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/hcl/parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/hcl/transformer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/hcl/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/httpapi/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/httpapi/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/httpapi/http_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/httpapi/restapi.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/httpapi/restapi_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/jinja/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/jinja/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/jinja/jinja_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/json/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/json/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/json/commentjson.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8385 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/json/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/utils/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/cli_generate_azure_vault_key.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/cli_populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/cli_terraform_to_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/cli_validator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/compliance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/fs_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/git_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/utils/jinjatemplates/mastertest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/helper/yaml/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/yaml/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/helper/yaml/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/logging/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/logging/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/logging/dburl_kv.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/logging/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.757940 prancer-basic-3.0.4/src/processor/reporting/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/reporting/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/reporting/json_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/template_processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/ack_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/aso_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/aws_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6180 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/azure_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/template_processor/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/base/base_template_constatns.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/base/base_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/google_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/helm_chart_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/json_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/kcc_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/kubernetes_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/terraform_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/template_processor/yaml_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/aws/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/aws/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/aws/aws_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/azure/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/azure/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    17363 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/azure/azure_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/base/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/google/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/google/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/google/google_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/google/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/helm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/helm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/helm/helm_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/kubernetes/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/kubernetes/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/kubernetes/kubernetes_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/terraform/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.761941 prancer-basic-3.0.4/src/processor/templates/terraform/helper/expression/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/expression/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/expression/base_expressions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/expression/terraform_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:31:50.765941 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/collection_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/encoding_function.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/numeric_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/string_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/terraform_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/helper/module_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-04-06 10:29:27.000000 prancer-basic-3.0.4/src/processor/templates/terraform/terraform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.901557 prancer-basic-3.0.5/
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/LICENSE
+-rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/PKG-INFO
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:39:43.901557 prancer-basic-3.0.5/setup.cfg
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.881557 prancer-basic-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/prancer_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/collection_config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/collection_config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/collection_config/config_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparison_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorLexer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorListener.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorParser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/compare_types.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/rule_interpreter.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/test_comparator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/arm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/arm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7732 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/arm/secret_azure_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/common/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/common/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/common/sensitive_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/secret_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/arn_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/git_connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/git_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/git_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10831 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    58392 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_aws.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23681 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_azure.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_azure_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_base.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_custom.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_custom_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_db.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_exception.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_fs.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33285 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_google.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_kubernetes.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/special_compliance/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_compliance/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_compliance/compliances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/special_crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/azure_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/base_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/validation.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    24954 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/master_snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13961 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/database/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/database/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     9830 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/database/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/config_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/remote_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/rundata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/file/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/file/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/file/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/hcl/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/hcl_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/transformer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/httpapi/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/http_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/restapi.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/restapi_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/jinja/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/jinja/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/jinja/jinja_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/json/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/commentjson.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8248 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/utils/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_generate_azure_vault_key.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_terraform_to_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_validator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/compliance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/fs_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/git_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/mastertest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/yaml/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/yaml/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/yaml/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/logging/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/dburl_kv.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/reporting/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/reporting/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/reporting/json_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/template_processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/ack_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/aso_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/aws_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6180 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/azure_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/template_processor/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/base_template_constatns.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/base_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/google_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/helm_chart_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/json_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/kcc_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/kubernetes_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/terraform_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/yaml_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/aws/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/aws/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/aws/aws_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/azure/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/azure/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    17363 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/azure/azure_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/base/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/google/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/google_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/helm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/helm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/helm/helm_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/kubernetes/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/kubernetes/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/kubernetes/kubernetes_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/base_expressions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/terraform_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/collection_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/encoding_function.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/numeric_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/string_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/terraform_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/module_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/terraform_parser.py
```

### Comparing `prancer-basic-3.0.4/LICENSE` & `prancer-basic-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/PKG-INFO` & `prancer-basic-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.4
+Version: 3.0.5
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.4/README.md` & `prancer-basic-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/setup.py` & `prancer-basic-3.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  Prancer Basic allows to users to run cloud validation.
  The supported cloud frameworks are azure, aws and git.
 """
 
 setup(
     name='prancer-basic',
     # also update the version in processor.__init__.py file
-    version='3.0.4',
+    version='3.0.5',
     description='Prancer Basic, http://prancer.io/',
     long_description=LONG_DESCRIPTION,
     license = "BSD",
     # The project's main homepage.
     url='https://github.com/prancer-io/cloud-validation-framework',
     # Author(s) details
     author='Farshid M/Ajey Khanapuri',
```

### Comparing `prancer-basic-3.0.4/src/prancer_basic.egg-info/PKG-INFO` & `prancer-basic-3.0.5/src/prancer_basic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.4
+Version: 3.0.5
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.4/src/prancer_basic.egg-info/SOURCES.txt` & `prancer-basic-3.0.5/src/prancer_basic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 src/processor/connector/special_compliance/__init__.py
 src/processor/connector/special_compliance/compliances.py
 src/processor/connector/special_crawler/__init__.py
 src/processor/connector/special_crawler/azure_crawler.py
 src/processor/connector/special_crawler/base_crawler.py
 src/processor/crawler/__init__.py
 src/processor/crawler/master_snapshot.py
+src/processor/crawler/utils.py
 src/processor/database/__init__.py
 src/processor/database/database.py
 src/processor/helper/__init__.py
 src/processor/helper/config/__init__.py
 src/processor/helper/config/config_utils.py
 src/processor/helper/config/remote_utils.py
 src/processor/helper/config/rundata_utils.py
```

### Comparing `prancer-basic-3.0.4/src/prancer_basic.egg-info/requires.txt` & `prancer-basic-3.0.5/src/prancer_basic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/collection_config/config_handler.py` & `prancer-basic-3.0.5/src/processor/collection_config/config_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparison_functions.py` & `prancer-basic-3.0.5/src/processor/comparison/comparison_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorLexer.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorLexer.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorListener.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorListener.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/comparatorParser.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorParser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/compare_types.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/compare_types.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/rule_interpreter.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/rule_interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/comparisonantlr/test_comparator.py` & `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/test_comparator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/interpreter.py` & `prancer-basic-3.0.5/src/processor/comparison/interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/rules/arm/secret_azure_iac.py` & `prancer-basic-3.0.5/src/processor/comparison/rules/arm/secret_azure_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/rules/cloudformation/secret_aws_iac.py` & `prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/secret_aws_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/rules/common/sensitive_extension.py` & `prancer-basic-3.0.5/src/processor/comparison/rules/common/sensitive_extension.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py` & `prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/comparison/rules/terraform/secret_tf.py` & `prancer-basic-3.0.5/src/processor/comparison/rules/terraform/secret_tf.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/arn_parser.py` & `prancer-basic-3.0.5/src/processor/connector/arn_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/git_connector/git_functions.py` & `prancer-basic-3.0.5/src/processor/connector/git_connector/git_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/git_connector/git_processor.py` & `prancer-basic-3.0.5/src/processor/connector/git_connector/git_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/populate_json.py` & `prancer-basic-3.0.5/src/processor/connector/populate_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from processor.helper.json.json_utils import get_field_value_with_default, get_field_value, json_from_file
 from processor.helper.file.file_utils import exists_file, exists_dir
 from processor.helper.httpapi.restapi_azure import json_source
 from processor.connector.vault import get_vault_data
 from processor.connector.snapshot_custom import get_custom_data, git_clone_dir
 from processor.logging.log_handler import getlogger
 from subprocess import Popen, PIPE
+import copy
 import tempfile
 import re
 import os
 import urllib
 
 logger = getlogger()
 
@@ -64,14 +65,15 @@
         return False
 
     snapshots = master_snapshot_json["snapshots"]
     if not isinstance(snapshots, list):
         logger.error("Invalid json %s: 'Snapshots' field is not type list in snapshot configuration file." % file_location)
         return False
 
+    snapshot_list = []
     for snapshot in snapshots:
         if "type" not in snapshot:
             logger.error("Invalid json %s: 'type' field is not exists in snapshot configuration file." % file_location)
             validate = False
             break
 
         if "connectorUser" not in snapshot:
@@ -82,14 +84,15 @@
             found_connector_user = False
             for connector_user in connector_users:
                 if connector_user["id"] == snapshot["connectorUser"]:
                     found_connector_user = True
                     for key, value in connector_user.items():
                         if key != "id":
                             snapshot[key] = value
+                    snapshot_list.append(copy.deepcopy(snapshot))
         
             if not found_connector_user:
                 logger.error("Invalid json %s: `testUser` in snapshot configuration file is not mactch with the 'connectorUser' in remote snapshot file." % file_location)
                 validate = False
                 break
             
         if "nodes" not in snapshot:
@@ -126,15 +129,15 @@
         if not validate:
             break
 
     if validate:
         document_json.pop("connector")
         document_json.pop("remoteFile")
         document_json.pop("connectorUsers")
-        document_json["snapshots"] = master_snapshot_json["snapshots"]
+        document_json["snapshots"] = snapshot_list
     
     return validate    
 
 def validate_test_data(test_json, document_json, file_location):
     validate = True
     
     if "testSet" not in test_json:
```

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_aws.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,14 +1198,15 @@
                                         'snapshotId': '%s%s' % (node['masterSnapshotId'], str(count)),
                                         'validate': validate,
                                         'detailMethods': data['detailMethods'],
                                         'structure': 'aws',
                                         'masterSnapshotId': node['masterSnapshotId'],
                                         'collection': data['collection'],
                                         'arn' : data['arn'],
+                                        'account_id': account_id,
                                         'status' : 'active'
                                     }
                                     if node.get("boto_type"):
                                         node_data["boto_type"] = node.get("boto_type")
                                     snapshot_data[node['masterSnapshotId']].append(node_data)
                                     count += 1
             if mastercode:
```

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_azure.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             resource_group = exmatch.group(1)
          
         child_resource_type_list = node.get('type', "").split("/")   
         if len(child_resource_type_list) == 2:
             exmatch = re.search(r'/subscriptions.*/resourceGroups/.*?/', node['path'], re.I)
             if exmatch:
                 export_template_url = 'https://management.azure.com%sexportTemplate?api-version=2021-04-01' % (exmatch.group(0).lower())
-                status, data = export_template(export_template_url, hdrs, node['path'])
+                status, data = export_template(export_template_url, hdrs, node['path'], retry_count=0)
                 
         db_record['path'] = node['path']
         
         if status and isinstance(status, int) and status == 200:
             if data and data.get("resources"):
                 try:
                     temp_dir = tempfile.mkdtemp()
@@ -294,23 +294,15 @@
 
     if include_regex_list and path and any(re.match(regex, path) for regex in include_regex_list):
         include_regex = True
 
     return include_path or include_regex
 
 
-def populate_azure_snapshot(snapshot, container=None, snapshot_type='azure'):
-    """ Populates the resources from azure."""
-    dbname = config_value('MONGODB', 'dbname')
-    snapshot_source = get_field_value(snapshot, 'source')
-    snapshot_user = get_field_value(snapshot, 'testUser')
-    snapshot_nodes = get_field_value(snapshot, 'nodes')
-    snapshot_data, valid_snapshotids = validate_snapshot_nodes(snapshot_nodes)
-    client_id, client_secret, sub_name, sub_id, tenant_id = \
-        get_web_client_data(snapshot_type, snapshot_source, snapshot_user, container)
+def populate_client_secret(client_id, client_secret, snapshot_user):
     if not client_id:
         # logger.info("No client_id in the snapshot to access azure resource!...")
         raise Exception("No client id in the snapshot to access azure resource!...")
 
     # Read the client secrets from envirnment variable
     if not client_secret:
         client_secret = os.getenv(snapshot_user, None)
@@ -324,14 +316,28 @@
             logger.info('Client Secret from Vault, Secret: %s', '*' * len(client_secret))
         elif get_from_currentdata(CUSTOMER):
             logger.error("Client Secret key does not set in a vault")
             raise Exception("Client Secret key does not set in a vault")
 
     if not client_secret:
         raise Exception("No `client_secret` key in the connector file to access azure resource!...")
+    
+    return client_secret
+
+def populate_azure_snapshot(snapshot, container=None, snapshot_type='azure'):
+    """ Populates the resources from azure."""
+    dbname = config_value('MONGODB', 'dbname')
+    snapshot_source = get_field_value(snapshot, 'source')
+    snapshot_user = get_field_value(snapshot, 'testUser')
+    snapshot_nodes = get_field_value(snapshot, 'nodes')
+    snapshot_data, valid_snapshotids = validate_snapshot_nodes(snapshot_nodes)
+    client_id, client_secret, sub_name, sub_id, tenant_id = \
+        get_web_client_data(snapshot_type, snapshot_source, snapshot_user, container)
+    
+    client_secret = populate_client_secret(client_id, client_secret, snapshot_user)
 
     logger.info('\t\tSubscription: %s', sub_id)
     logger.info('\t\tTenant: %s', tenant_id)
     logger.info('\t\tclient: %s', client_id)
     put_in_currentdata('clientId', client_id)
     put_in_currentdata('clientSecret', client_secret)
     put_in_currentdata('subscriptionId', sub_id)
@@ -443,15 +449,16 @@
                             if not ignoreNode:
                                 snapshot_data[node['masterSnapshotId']].append(
                                     {
                                         'masterSnapshotId': [node['masterSnapshotId']],
                                         'snapshotId': data['snapshotId'],
                                         'path': data['path'],
                                         'validate': validate,
-                                        'status': 'active'
+                                        'status': 'active',
+                                        'subscriptionId': sub_id
                                     })
 
         for data in all_data_records:
             if get_dbtests():
                 if get_collection_size(data['collection']) == 0:
                     # Creating indexes for collection
                     create_indexes(
```

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_azure_refactor.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_azure_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_base.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_base.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_custom.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_custom.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_custom_refactor.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_custom_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_db.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_db.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_fs.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_fs.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_google.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_google.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,14 +586,15 @@
                     {
                         "masterSnapshotId" : [node['masterSnapshotId']],
                         "snapshotId": '%s%s' % (node['masterSnapshotId'], str(count)),
                         "type": resource_node_type,
                         "collection": node['collection'],
                         "path": path,
                         "status" : "active",
+                        'project_id': project_id,
                         "validate" : node['validate'] if 'validate' in node else True
                     })
     return snapshot_data
 
 def get_checksum(data):
     """ Get the checksum for the Google data fetched."""
     checksum = None
```

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_kubernetes.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_kubernetes.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/snapshot_utils.py` & `prancer-basic-3.0.5/src/processor/connector/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/special_compliance/compliances.py` & `prancer-basic-3.0.5/src/processor/connector/special_compliance/compliances.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/special_crawler/azure_crawler.py` & `prancer-basic-3.0.5/src/processor/connector/special_crawler/azure_crawler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/validation.py` & `prancer-basic-3.0.5/src/processor/connector/validation.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/connector/vault.py` & `prancer-basic-3.0.5/src/processor/connector/vault.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/crawler/master_snapshot.py` & `prancer-basic-3.0.5/src/processor/crawler/master_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from processor.connector.snapshot_custom import populate_custom_snapshot, get_custom_data
 from processor.connector.snapshot_aws import populate_aws_snapshot
 from processor.connector.snapshot_google import populate_google_snapshot
 from processor.connector.snapshot_kubernetes import populate_kubernetes_snapshot
 from processor.connector.populate_json import pull_json_data
 from processor.helper.file.file_utils import exists_file,remove_file
 from processor.template_processor.base.base_template_processor import set_processed_templates
+from processor.crawler.utils import check_container_for_all_accounts
 
 doc_id = None
 logger = getlogger()
 # Different types of snapshots supported by the validation framework.
 mastersnapshot_fns = {
     'azure': populate_azure_snapshot,
     'filesystem': populate_custom_snapshot,
@@ -56,14 +57,17 @@
     'google' : populate_google_snapshot,
     'kubernetes': populate_kubernetes_snapshot
 }
 
 REMOVE_SNAPSHOTGEN_FIELDS = [
     "exclude",
     "source",
+    "subscriptionId",
+    "account_id",
+    "project_id"
 ]
 
 def generate_snapshot(snapshot_json_data, snapshot_file_data):
     """
     Checks if the snapshot is a master snapshot file.
     """
     if snapshot_json_data:
@@ -80,16 +84,25 @@
                             if mastersnapshotId and mastersnapshotId in snapshot_file_data and \
                                     isinstance(snapshot_file_data[mastersnapshotId], list):
                                 for sid_data in snapshot_file_data[mastersnapshotId]:
                                     structure = sid_data.pop('structure', None)
                                     # if structure and structure == 'aws':
                                     #     newnode = {}
                                     # else:
+                                    snapshot_type = snapshot.get("type")
                                     if "source" in sid_data and sid_data["source"] != snapshot.get("source"):
                                         continue
+
+                                    if snapshot_type == "azure" and sid_data.get("subscriptionId") != snapshot.get("subscriptionId"):
+                                        continue
+                                    elif snapshot_type == "aws" and sid_data.get("account_id") != snapshot.get("accountId"):
+                                        continue
+                                    elif snapshot_type == "google" and sid_data.get("project_id") != snapshot.get("project-id"):
+                                        continue
+
                                     newnode = copy.deepcopy(node)
                                     newnode.update(sid_data)
                                     
                                     for field in REMOVE_SNAPSHOTGEN_FIELDS:
                                         if field in newnode:
                                             del newnode[field]
                                         # if field in sid_data:
@@ -159,25 +172,27 @@
                 if ms_id not in snapshot_data:
                     snapshot_data[ms_id] = node_list
 
     # for each snapshot_json_data, update the existing json data or add the new json data here.
     return snapshot_data
 
 
-def generate_snapshots_from_mastersnapshot_file(mastersnapshot_file):
+def generate_snapshots_from_mastersnapshot_file(mastersnapshot_file, container, file_name):
     """
     Each snapshot file from the filesystem is loaded as a json datastructue
      and generate all the nodes in this json datastructure.
     """
     mastersnapshot_file_name = '%s.json' % mastersnapshot_file if mastersnapshot_file and not \
         mastersnapshot_file.endswith('.json') else mastersnapshot_file
     mastersnapshot_json_data = json_from_file(mastersnapshot_file_name)
     if not mastersnapshot_json_data:
         logger.error("masterSnapshot file %s looks to be empty, next!...", mastersnapshot_file)
         return {}, {}
+    
+    mastersnapshot_json_data = check_container_for_all_accounts(container, mastersnapshot_json_data, file_name)
 
     if "connector" in mastersnapshot_json_data and "remoteFile" in mastersnapshot_json_data and mastersnapshot_json_data["connector"] and mastersnapshot_json_data["remoteFile"]:
         _, pull_response = pull_json_data(mastersnapshot_json_data)
         if not pull_response:
             return {}, {}
     logger.debug(json.dumps(mastersnapshot_json_data, indent=2))
     parts = mastersnapshot_file_name.rsplit('.', 1)
@@ -238,15 +253,15 @@
     populated = []
     for snapshot_file in snapshot_files:
         logger.info('\tMASTERSNAPSHOT:%s', snapshot_file)
         parts = snapshot_file.rsplit('/', 1)
         if parts[-1] in snapshots or parts[-1] == mastersnapshotfile_name_json:
             if parts[-1] not in populated:
                 # Take the snapshot and crawl for the  resource types.
-                snapshot_file_data, snapshot_json_data = generate_snapshots_from_mastersnapshot_file(snapshot_file)
+                snapshot_file_data, snapshot_json_data = generate_snapshots_from_mastersnapshot_file(snapshot_file, container, parts[-1])
                 file_name = '%s.json' % snapshot_file if snapshot_file and not snapshot_file.endswith('.json') else snapshot_file
                 # snapshot_json_data = json_from_file(file_name)
                 generate_snapshot(snapshot_json_data, snapshot_file_data)
                 parts = file_name.rsplit('.', 1)
                 new_file_name = '%s_gen.%s' % (parts[0], parts[1])
                 save_json_to_file(snapshot_json_data, new_file_name)
                 populated.append(parts[-1])
@@ -305,14 +320,15 @@
         if docs and len(docs):
             logger.info('Number of mastersnapshot Documents: %s', len(docs))
             snapshots = mastersnapshots_used_in_mastertests_database(container)
             populated = []
             for doc in docs:
                 if doc['json']:
                     snapshot = doc['name']
+                    doc['json'] = check_container_for_all_accounts(container, doc['json'], snapshot)
                     if "connector" in doc['json'] and "remoteFile" in doc['json'] and doc['json']["connector"] and doc['json']["remoteFile"]:
                         _, pull_response = pull_json_data(doc['json'])
                         if not pull_response:
                             logger.info("Failed to populate master snapshot json from the git repository")
                             break
 
                     if snapshot in snapshots or snapshot == mastersnapshotfile:
```

### Comparing `prancer-basic-3.0.4/src/processor/database/database.py` & `prancer-basic-3.0.5/src/processor/database/database.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/config/config_utils.py` & `prancer-basic-3.0.5/src/processor/helper/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/config/remote_utils.py` & `prancer-basic-3.0.5/src/processor/helper/config/remote_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/config/rundata_utils.py` & `prancer-basic-3.0.5/src/processor/helper/config/rundata_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/file/file_utils.py` & `prancer-basic-3.0.5/src/processor/helper/file/file_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/hcl/hcl_utils.py` & `prancer-basic-3.0.5/src/processor/helper/hcl/hcl_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/hcl/parser.py` & `prancer-basic-3.0.5/src/processor/helper/hcl/parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/hcl/yacc.py` & `prancer-basic-3.0.5/src/processor/helper/hcl/yacc.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/httpapi/http_utils.py` & `prancer-basic-3.0.5/src/processor/helper/httpapi/http_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/httpapi/restapi.py` & `prancer-basic-3.0.5/src/processor/helper/httpapi/restapi.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/httpapi/restapi_azure.py` & `prancer-basic-3.0.5/src/processor/helper/httpapi/restapi_azure.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/jinja/jinja_utils.py` & `prancer-basic-3.0.5/src/processor/helper/jinja/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/json/commentjson.py` & `prancer-basic-3.0.5/src/processor/helper/json/commentjson.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/json/json_utils.py` & `prancer-basic-3.0.5/src/processor/helper/json/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,16 +214,14 @@
         snapshot_files = []
     return container_dir, snapshot_files
 
 
 def get_json_files(json_dir, file_type, name=None):
     """Return list of json files based on the file type."""
     file_list = []
-    # logger.info('JSON dir:%s, filetype: %s', json_dir, file_type)
-    globalllll= glob.glob('%s/*.json' % json_dir.replace('//', '/'))
     if name:
         name = json_dir + "/" + name + ".json"
     if json_dir and file_type:
         for filename in glob.glob('%s/*.json' % json_dir.replace('//', '/')):
             if name and name != filename:
                 continue
             json_data = json_from_file(filename)
```

### Comparing `prancer-basic-3.0.4/src/processor/helper/utils/cli_generate_azure_vault_key.py` & `prancer-basic-3.0.5/src/processor/helper/utils/cli_generate_azure_vault_key.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/utils/cli_populate_json.py` & `prancer-basic-3.0.5/src/processor/helper/utils/cli_populate_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/utils/cli_terraform_to_json.py` & `prancer-basic-3.0.5/src/processor/helper/utils/cli_terraform_to_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/utils/cli_validator.py` & `prancer-basic-3.0.5/src/processor/helper/utils/cli_validator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/utils/compliance_utils.py` & `prancer-basic-3.0.5/src/processor/helper/utils/compliance_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/helper/yaml/yaml_utils.py` & `prancer-basic-3.0.5/src/processor/helper/yaml/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/logging/dburl_kv.py` & `prancer-basic-3.0.5/src/processor/logging/dburl_kv.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/logging/log_handler.py` & `prancer-basic-3.0.5/src/processor/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/reporting/json_output.py` & `prancer-basic-3.0.5/src/processor/reporting/json_output.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/ack_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/ack_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/aso_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/aso_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/aws_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/aws_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/azure_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/azure_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/base/base_template_constatns.py` & `prancer-basic-3.0.5/src/processor/template_processor/base/base_template_constatns.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/base/base_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/base/base_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/google_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/google_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/helm_chart_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/helm_chart_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/json_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/json_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/kcc_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/kcc_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/kubernetes_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/kubernetes_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/terraform_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/terraform_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/template_processor/yaml_template_processor.py` & `prancer-basic-3.0.5/src/processor/template_processor/yaml_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/aws/aws_parser.py` & `prancer-basic-3.0.5/src/processor/templates/aws/aws_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/azure/azure_parser.py` & `prancer-basic-3.0.5/src/processor/templates/azure/azure_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/base/template_parser.py` & `prancer-basic-3.0.5/src/processor/templates/base/template_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/google/google_parser.py` & `prancer-basic-3.0.5/src/processor/templates/google/google_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/google/util.py` & `prancer-basic-3.0.5/src/processor/templates/google/util.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/helm/helm_parser.py` & `prancer-basic-3.0.5/src/processor/templates/helm/helm_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/kubernetes/kubernetes_parser.py` & `prancer-basic-3.0.5/src/processor/templates/kubernetes/kubernetes_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/expression/base_expressions.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/base_expressions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/collection_functions.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/collection_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/encoding_function.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/encoding_function.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/numeric_functions.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/string_functions.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/string_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/function/terraform_functions.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/terraform_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/helper/module_parser.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/helper/module_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.4/src/processor/templates/terraform/terraform_parser.py` & `prancer-basic-3.0.5/src/processor/templates/terraform/terraform_parser.py`

 * *Files identical despite different names*

