# Comparing `tmp/aind_metadata_service-0.4.1.tar.gz` & `tmp/aind_metadata_service-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.1.tar", last modified: Wed Apr 26 17:07:51 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.2.tar", last modified: Thu May  4 23:30:28 2023, max compression
```

## Comparing `aind_metadata_service-0.4.1.tar` & `aind_metadata_service-0.4.2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 17:07:25.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.137261 aind_metadata_service-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.145261 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 23:30:12.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.161261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.165261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.145261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.165261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/test_response_handle.py
```

### Comparing `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/.github/workflows/ci.yml` & `aind_metadata_service-0.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/.github/workflows/publish.yml` & `aind_metadata_service-0.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/.gitignore` & `aind_metadata_service-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/Dockerfile` & `aind_metadata_service-0.4.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/LICENSE` & `aind_metadata_service-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/PKG-INFO` & `aind_metadata_service-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.1
+Version: 0.4.2
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.1/README.md` & `aind_metadata_service-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/doc_template/Makefile` & `aind_metadata_service-0.4.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/doc_template/make.bat` & `aind_metadata_service-0.4.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/doc_template/source/conf.py` & `aind_metadata_service-0.4.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/pyproject.toml` & `aind_metadata_service-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from aind_data_schema.procedures import Procedures
 from fastapi.responses import JSONResponse
 from office365.runtime.auth.client_credential import ClientCredential
 from office365.sharepoint.client_context import ClientContext
 
 from aind_metadata_service.response_handler import Responses
-from aind_metadata_service.sharepoint.nsb2019.mapping import NSB2019Mapping
+from aind_metadata_service.sharepoint.nsb2019.procedures import NSB2019Mapping
 from aind_metadata_service.sharepoint.nsb2023.mapping import NSB2023Mapping
 
 
 class SharePointClient:
     """This class contains the api to connect to SharePoint db."""
 
     def __init__(
```

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,33 +17,34 @@
     OphysProbe,
     ProbeName,
     Side,
     SubjectProcedure,
 )
 from office365.sharepoint.client_context import ClientContext
 
-from aind_metadata_service.sharepoint.nsb2019.models import (
+from aind_metadata_service.sharepoint.nsb2023.models import BurrHoleProcedure
+from aind_metadata_service.sharepoint.nsb2023.models import (
     CraniotomyType as NSBCraniotomyType,
 )
-from aind_metadata_service.sharepoint.nsb2019.models import (
-    HeadPostInfo,
+from aind_metadata_service.sharepoint.nsb2023.models import (
+    HeadPostInfo2023,
     Hemisphere,
     InjectionType,
-    NSBList2019,
+    NSBList2023,
 )
 
 
-class NSB2019Mapping:
+class NSB2023Mapping:
     """Provides methods to retrieve procedure information from sharepoint,
     parses the response into an intermediate data model, and maps that model
-    into AIND Procedures model."""
+    into AIND internal Procedures model."""
 
     def get_procedures_from_sharepoint(
         self, subject_id: str, client_context: ClientContext, list_title: str
-    ) -> List[SubjectProcedure]:
+    ):
         """
         Get list of Procedures from NSB 2019 database.
         Parameters
         ----------
         subject_id : str
           ID of the subject to find procedure information for
         client_context : ClientContext
@@ -52,317 +53,349 @@
           Title of the list where the 2019 procedure data is stored
 
         Returns
         -------
         List[SubjectProcedure]
 
         """
-
-        labtrack_alias = NSBList2019.__fields__.get("labtracks_id").alias
+        labtrack_alias = NSBList2023.__fields__.get("labtracks_id").alias
         filter_string = f"{labtrack_alias} eq '{subject_id}'"
         list_view = client_context.web.lists.get_by_title(
             list_title
-        ).views.get_by_title(getattr(NSBList2019, "_view_title"))
+        ).views.get_by_title(getattr(NSBList2023, "_view_title"))
         client_context.load(list_view)
         client_context.execute_query()
         list_items = list_view.get_items().filter(filter_string)
         client_context.load(list_items)
         client_context.execute_query()
         list_of_procedures = []
         for list_item in list_items:
-            parsed_nsb_model = NSBList2019.parse_obj(list_item.to_json())
+            parsed_nsb_model = NSBList2023.parse_obj(list_item.to_json())
             procedures = self.map_nsb_model(parsed_nsb_model)
             list_of_procedures.extend(procedures)
         return list_of_procedures
 
     # flake8: noqa: C901
-    def map_nsb_model(self, nsb_model: NSBList2019) -> List[SubjectProcedure]:
+    def map_nsb_model(self, nsb_model: NSBList2023) -> List[SubjectProcedure]:
         """Maps an individual list item model into List[SubjectProcedures]"""
         procedures = []
-        start_date = self._map_datetime_to_date(nsb_model.date_of_surgery)
-        end_date = start_date
         experimenter_full_name = self._map_auth_id_to_exp_name(
             nsb_model.author_id
         )
         iacuc_protocol = nsb_model.iacuc_protocol
-        animal_weight_prior = nsb_model.weight_before_surgery
-        animal_weight_post = nsb_model.weight_after_surgery
 
-        # Check if headframe type procedure in list of procedures
+        # Check if any headframe procedures
         if nsb_model.has_hp_procedure():
-            hf_kwargs = {
-                "start_date": start_date,
-                "end_date": end_date,
-                "experimenter_full_name": experimenter_full_name,
-                "iacuc_protocol": iacuc_protocol,
-                "animal_weight_prior": animal_weight_prior,
-                "animal_weight_post": animal_weight_post,
-            }
-            headpost_type = nsb_model.headpost_type
-            headpost_info = HeadPostInfo.from_headpost_type(
-                headpost_type=headpost_type
-            )
-            hf_kwargs["headframe_type"] = headpost_info.headframe_type
-            hf_kwargs[
-                "headframe_part_number"
-            ] = headpost_info.headframe_part_number
-            hf_kwargs["well_type"] = headpost_info.well_type
-            hf_kwargs["well_part_number"] = headpost_info.well_part_number
-            hp_iso_level = nsb_model.hp_iso_level
-            anaesthetic_type = "isoflurane"
+            hp_during = nsb_model.headpost_perform_during
+            hf_surgery_during_info = nsb_model.surgery_during_info(hp_during)
             anaesthetic = Anaesthetic.construct(
-                type=anaesthetic_type,
-                level=hp_iso_level,
-            )
-            hf_kwargs["anaesthesia"] = anaesthetic
-            headframe_proc = Headframe.construct(**hf_kwargs)
-            procedures.append(headframe_proc)
-
-        # Check if injection type procedure in procedure_types
-        if nsb_model.has_inj_procedure():
-            # Map first injection procedure
-            inj1_kwargs = {}
-            inj1_start_date = self._map_datetime_to_date(
-                nsb_model.date_1st_injection
-            )
-            inj1_kwargs["start_date"] = inj1_start_date
-            inj1_kwargs["end_date"] = inj1_start_date
-            inj1_kwargs[
-                "animal_weight_prior"
-            ] = nsb_model.first_injection_weight_before
-            inj1_kwargs[
-                "animal_weight_post"
-            ] = nsb_model.first_injection_weight_after
-            inj1_kwargs["injection_duration"] = self._duration_to_minutes(
-                nsb_model.inj1_length_of_time
-            )
-            # First injection anaesthetic
-            inj1_anaesthetic_type = "isoflurane"
-            inj1_anaesthetic_duration = nsb_model.first_injection_iso_duration
-            inj1_anaesthetic_level = nsb_model.round1_inj_iso_level
-            inj1_kwargs["anaesthesia"] = Anaesthetic.construct(
-                type=inj1_anaesthetic_type,
-                duration=inj1_anaesthetic_duration,
-                level=inj1_anaesthetic_level,
-            )
-            inj1_kwargs["recovery_time"] = nsb_model.first_inj_recovery
-            inj1_kwargs["workstation_id"] = nsb_model.workstation_1st_injection
-            inj1_kwargs["injection_hemisphere"] = self._map_hemisphere(
-                nsb_model.virus_hemisphere
-            )
-            inj1_kwargs["injection_coordinate_ml"] = nsb_model.virus_ml
-            inj1_kwargs["injection_coordinate_ap"] = nsb_model.virus_ap
-            inj1_kwargs[
-                "injection_coordinate_reference"
-            ] = self._map_ap_info_to_coord_reference(nsb_model.virus_ap)
-            inj1_kwargs["injection_coordinate_depth"] = nsb_model.virus_dv
-            inj1_kwargs["injection_angle"] = nsb_model.inj1_angle0
-            inj1_kwargs["bregma_to_lambda_distance"] = nsb_model.breg_2_lamb
-            # inj1_virus_strain = nsb_model.inj1_virus_strain_rt
-            inj1_kwargs[
-                "injection_materials"
-            ] = self._map_virus_strain_to_materials(
-                nsb_model.inj1_virus_strain_rt
-            )
-            if nsb_model.inj1_type == InjectionType.IONTOPHORESIS:
-                inj1_kwargs["instrument_id"] = nsb_model.ionto_number_inj1
-                inj1_kwargs["injection_current"] = nsb_model.inj1_current
-                inj1_kwargs[
-                    "alternating_current"
-                ] = nsb_model.inj1_alternating_time
-                injection1 = IontophoresisInjection.construct(**inj1_kwargs)
-            elif nsb_model.inj1_type == InjectionType.NANOJECT:
-                inj1_kwargs["instrument_id"] = nsb_model.nanoject_number_inj10
-                inj1_kwargs["injection_volume"] = nsb_model.inj1_vol
-                injection1 = NanojectInjection.construct(**inj1_kwargs)
-            else:
-                injection1 = BrainInjection.construct(**inj1_kwargs)
-            procedures.append(injection1)
-
-        # Add second injection if exists
-        if nsb_model.has_2nd_inj_procedure():
-            inj2_kwargs = {}
-            inj2_start_date = self._map_datetime_to_date(
-                nsb_model.date_2nd_injection
-            )
-            inj2_kwargs["start_date"] = inj2_start_date
-            inj2_kwargs["end_date"] = inj2_start_date
-            inj2_kwargs[
-                "animal_weight_prior"
-            ] = nsb_model.second_injection_weight_before
-            inj2_kwargs[
-                "animal_weight_post"
-            ] = nsb_model.second_injection_weight_after
-            inj2_kwargs["injection_duration"] = self._duration_to_minutes(
-                nsb_model.inj2_length_of_time
-            )
-            # First injection anaesthetic
-            inj2_anaesthetic_type = "isoflurane"
-            inj2_anaesthetic_duration = nsb_model.second_injection_iso_duration
-            inj2_anaesthetic_level = nsb_model.round2_inj_iso_level
-            inj2_kwargs["anaesthesia"] = Anaesthetic.construct(
-                type=inj2_anaesthetic_type,
-                duration=inj2_anaesthetic_duration,
-                level=inj2_anaesthetic_level,
-            )
-            inj2_kwargs["recovery_time"] = nsb_model.second_inj_recovery
-            inj2_kwargs["workstation_id"] = nsb_model.workstation_2nd_injection
-            inj2_kwargs["injection_hemisphere"] = self._map_hemisphere(
-                nsb_model.hemisphere_2nd_inj
-            )
-            inj2_kwargs["injection_coordinate_ml"] = nsb_model.ml_2nd_inj
-            inj2_kwargs["injection_coordinate_ap"] = nsb_model.ap_2nd_inj
-            inj2_kwargs[
-                "injection_coordinate_reference"
-            ] = self._map_ap_info_to_coord_reference(nsb_model.ap_2nd_inj)
-            inj2_kwargs["injection_coordinate_depth"] = nsb_model.dv_2nd_inj
-            inj2_kwargs["injection_angle"] = nsb_model.inj2_angle0
-            # Is this the same for 1st and 2nd injections?
-            inj2_kwargs["bregma_to_lambda_distance"] = nsb_model.breg_2_lamb
-            # inj2_virus_strain = nsb_model.inj2_virus_strain_rt
-            inj2_kwargs[
-                "injection_materials"
-            ] = self._map_virus_strain_to_materials(
-                nsb_model.inj2_virus_strain_rt
+                type="isoflurane",
+                duration=(
+                    hf_surgery_during_info.anaesthetic_duration_in_minutes
+                ),
+                level=hf_surgery_during_info.anaesthetic_level,
+            )
+            headpost_info = HeadPostInfo2023.from_hp_and_hp_type(
+                hp=nsb_model.headpost, hp_type=nsb_model.headpost_type
+            )
+
+            headframe_procedure = Headframe.construct(
+                start_date=self._map_datetime_to_date(
+                    hf_surgery_during_info.start_date
+                ),
+                end_date=self._map_datetime_to_date(
+                    hf_surgery_during_info.start_date
+                ),
+                experimenter_full_name=experimenter_full_name,
+                iacuc_protocol=iacuc_protocol,
+                animal_weight_prior=hf_surgery_during_info.weight_prior,
+                animal_weight_post=hf_surgery_during_info.weight_post,
+                headframe_type=headpost_info.headframe_type,
+                headframe_part_number=headpost_info.headframe_part_number,
+                well_type=headpost_info.well_type,
+                well_part_number=headpost_info.well_part_number,
+                anaesthesia=anaesthetic,
             )
-            if nsb_model.inj2_type == InjectionType.IONTOPHORESIS:
-                inj2_kwargs["instrument_id"] = nsb_model.ionto_number_inj2
-                inj2_kwargs["injection_current"] = nsb_model.inj2_current
-                inj2_kwargs[
-                    "alternating_current"
-                ] = nsb_model.inj2_alternating_time
-                injection2 = IontophoresisInjection.construct(**inj2_kwargs)
-            elif nsb_model.inj2_type == InjectionType.NANOJECT:
-                inj2_kwargs["instrument_id"] = nsb_model.nanoject_number_inj2
-                inj2_kwargs["injection_volume"] = nsb_model.inj2_vol
-                injection2 = NanojectInjection.construct(**inj2_kwargs)
-            else:
-                injection2 = BrainInjection.construct(**inj2_kwargs)
-            procedures.append(injection2)
+            procedures.append(headframe_procedure)
 
-        # Check if craniotomy procedure
+        # Check for craniotomy procedures
         if nsb_model.has_cran_procedure():
-            cran_kwargs = {
-                "start_date": start_date,
-                "end_date": end_date,
-                "experimenter_full_name": experimenter_full_name,
-                "iacuc_protocol": iacuc_protocol,
-                "animal_weight_prior": animal_weight_prior,
-                "animal_weight_post": animal_weight_post,
-            }
-            hp_iso_level = nsb_model.hp_iso_level
-            anaesthetic_type = "isoflurane"
-            anaesthetic = Anaesthetic.construct(
-                type=anaesthetic_type,
-                level=hp_iso_level,
-            )
-            cran_kwargs["anaesthesia"] = anaesthetic
             craniotomy_type = self._map_craniotomy_type(
                 nsb_model.craniotomy_type
             )
-            cran_kwargs["craniotomy_type"] = craniotomy_type
-            cran_kwargs["craniotomy_coordinates_reference"] = (
-                CoordinateReferenceLocation.LAMBDA
-                if craniotomy_type == CraniotomyType.VISCTX
-                else None
-            )
-            cran_kwargs["craniotomy_hemisphere"] = self._map_hemisphere(
-                nsb_model.hp_loc
-            )
-
-            cran_kwargs["craniotomy_coordinates_ml"] = nsb_model.hp_ml
-            cran_kwargs["craniotomy_coordinates_ap"] = nsb_model.hp_ap
-            cran_kwargs[
-                "craniotomy_size"
-            ] = self._map_nsb_craniotomy_type_to_size(
-                nsb_model.craniotomy_type
+            cran_during = nsb_model.craniotomy_perform_during
+            cran_during_info = nsb_model.surgery_during_info(cran_during)
+            anaesthetic = Anaesthetic.construct(
+                type="isoflurane",
+                duration=cran_during_info.anaesthetic_duration_in_minutes,
+                level=cran_during_info.anaesthetic_level,
             )
-            cran_kwargs["dura_removed"] = nsb_model.hp_durotomy
-            cran_kwargs["workstation_id"] = nsb_model.hp_work_station
-            cran_kwargs["bregma_to_lambda_distance"] = nsb_model.breg_2_lamb
-            craniotomy = Craniotomy.construct(**cran_kwargs)
-            procedures.append(craniotomy)
-
-        # Check if there is Fiber Implant Procedure
-        if nsb_model.has_fiber_implant_procedure():
-            ophys_probes = []
-            fiber_implant1 = nsb_model.fiber_implant1
-            fiber_implant2 = nsb_model.fiber_implant2
             bregma_to_lambda_distance = nsb_model.breg_2_lamb
-            if fiber_implant1 is not None:
-                name = ProbeName.PROBE_A.value
-                stereotactic_coordinate_ml = nsb_model.virus_ml
-                stereotactic_coordinate_ap = nsb_model.virus_ap
-                coordinate_reference = self._map_ap_info_to_coord_reference(
-                    nsb_model.virus_ap
+            if craniotomy_type == CraniotomyType.FIVE_MM:
+                craniotomy_coordinates_reference = (
+                    CoordinateReferenceLocation.LAMBDA
                 )
-                stereotactic_coordinate_dv = nsb_model.fiber_implant1_dv
-                angle = nsb_model.inj1_angle_v2
-                ophys_probe1 = OphysProbe.construct(
-                    name=name,
-                    stereotactic_coordinate_ml=stereotactic_coordinate_ml,
-                    stereotactic_coordinate_ap=stereotactic_coordinate_ap,
-                    stereotactic_coordinate_dv=stereotactic_coordinate_dv,
-                    angle=angle,
-                    bregma_to_lambda_distance=bregma_to_lambda_distance,
-                    stereotactic_coordinate_reference=coordinate_reference,
+                craniotomy_size = 5
+            elif craniotomy_type == CraniotomyType.THREE_MM:
+                craniotomy_coordinates_reference = None
+                craniotomy_size = 3
+            else:
+                craniotomy_coordinates_reference = None
+                craniotomy_size = None
+
+            cran_procedure = Craniotomy.construct(
+                start_date=self._map_datetime_to_date(
+                    cran_during_info.start_date
+                ),
+                end_date=self._map_datetime_to_date(
+                    cran_during_info.start_date
+                ),
+                experimenter_full_name=experimenter_full_name,
+                iacuc_protocol=iacuc_protocol,
+                animal_weight_prior=cran_during_info.weight_prior,
+                animal_weight_post=cran_during_info.weight_post,
+                craniotomy_type=craniotomy_type,
+                craniotomy_size=craniotomy_size,
+                anaesthesia=anaesthetic,
+                workstation_id=cran_during_info.workstation_id,
+                recovery_time=cran_during_info.recovery_time,
+                bregma_to_lambda_distance=bregma_to_lambda_distance,
+                craniotomy_coordinates_reference=(
+                    craniotomy_coordinates_reference
+                ),
+            )
+            procedures.append(cran_procedure)
+
+        # Check if there are any procedures for burr holes 1 through 4
+        for burr_hole_num in range(1, 5):
+            if nsb_model.has_burr_hole_procedure(
+                burr_hole_num=burr_hole_num,
+                burr_hole_procedure=BurrHoleProcedure.INJECTION,
+            ):
+                burr_hole_info = nsb_model.burr_hole_info(
+                    burr_hole_num=burr_hole_num
+                )
+                burr_during_info = nsb_model.surgery_during_info(
+                    during=burr_hole_info.during,
+                    inj_type=burr_hole_info.inj_type,
+                )
+                anaesthetic = Anaesthetic.construct(
+                    type="isoflurane",
+                    duration=burr_during_info.anaesthetic_duration_in_minutes,
+                    level=burr_during_info.anaesthetic_level,
+                )
+                injection_materials = (
+                    None
+                    if burr_hole_info.virus_strain is None
+                    else InjectionMaterial.construct(
+                        full_genome_name=burr_hole_info.virus_strain
+                    )
+                )
+                if burr_hole_info.inj_type == InjectionType.IONTOPHORESIS:
+                    injection_proc = IontophoresisInjection.construct(
+                        start_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        end_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        experimenter_full_name=experimenter_full_name,
+                        iacuc_protocol=iacuc_protocol,
+                        animal_weight_prior=burr_during_info.weight_prior,
+                        animal_weight_post=burr_during_info.weight_post,
+                        workstation_id=burr_during_info.workstation_id,
+                        injection_hemisphere=self._map_hemisphere(
+                            burr_hole_info.hemisphere
+                        ),
+                        injection_coordinate_ml=burr_hole_info.coordinate_ml,
+                        injection_coordinate_ap=burr_hole_info.coordinate_ap,
+                        injection_coordinate_depth=(
+                            burr_hole_info.coordinate_depth
+                        ),
+                        injection_angle=burr_hole_info.angle,
+                        injection_current=burr_hole_info.inj_current,
+                        injection_duration=self._duration_to_minutes(
+                            burr_hole_info.inj_duration
+                        ),
+                        alternating_current=burr_hole_info.alternating_current,
+                        recovery_time=burr_during_info.recovery_time,
+                        instrument_id=burr_during_info.instrument_id,
+                        anaesthesia=anaesthetic,
+                        bregma_to_lambda_distance=nsb_model.breg_2_lamb,
+                        injection_coordinate_reference=(
+                            CoordinateReferenceLocation.BREGMA
+                        ),
+                        injection_materials=injection_materials,
+                    )
+                elif burr_hole_info.inj_type == InjectionType.NANOJECT:
+                    injection_proc = NanojectInjection.construct(
+                        start_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        end_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        experimenter_full_name=experimenter_full_name,
+                        iacuc_protocol=iacuc_protocol,
+                        animal_weight_prior=burr_during_info.weight_prior,
+                        animal_weight_post=burr_during_info.weight_post,
+                        workstation_id=burr_during_info.workstation_id,
+                        injection_hemisphere=self._map_hemisphere(
+                            burr_hole_info.hemisphere
+                        ),
+                        injection_coordinate_ml=burr_hole_info.coordinate_ml,
+                        injection_coordinate_ap=burr_hole_info.coordinate_ap,
+                        injection_coordinate_depth=(
+                            burr_hole_info.coordinate_depth
+                        ),
+                        injection_angle=burr_hole_info.angle,
+                        injection_current=burr_hole_info.inj_current,
+                        injection_duration=self._duration_to_minutes(
+                            burr_hole_info.inj_duration
+                        ),
+                        injection_volume=burr_hole_info.inj_volume,
+                        alternating_current=burr_hole_info.alternating_current,
+                        recovery_time=burr_during_info.recovery_time,
+                        instrument_id=burr_during_info.instrument_id,
+                        anaesthesia=anaesthetic,
+                        bregma_to_lambda_distance=nsb_model.breg_2_lamb,
+                        injection_coordinate_reference=(
+                            CoordinateReferenceLocation.BREGMA
+                        ),
+                        injection_materials=injection_materials,
+                    )
+                else:
+                    injection_proc = BrainInjection.construct(
+                        start_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        end_date=self._map_datetime_to_date(
+                            burr_during_info.start_date
+                        ),
+                        experimenter_full_name=experimenter_full_name,
+                        iacuc_protocol=iacuc_protocol,
+                        animal_weight_prior=burr_during_info.weight_prior,
+                        animal_weight_post=burr_during_info.weight_post,
+                        workstation_id=burr_during_info.workstation_id,
+                        injection_hemisphere=self._map_hemisphere(
+                            burr_hole_info.hemisphere
+                        ),
+                        injection_coordinate_ml=burr_hole_info.coordinate_ml,
+                        injection_coordinate_ap=burr_hole_info.coordinate_ap,
+                        injection_coordinate_depth=(
+                            burr_hole_info.coordinate_depth
+                        ),
+                        injection_angle=burr_hole_info.angle,
+                        injection_duration=self._duration_to_minutes(
+                            burr_hole_info.inj_duration
+                        ),
+                        recovery_time=burr_during_info.recovery_time,
+                        instrument_id=burr_during_info.instrument_id,
+                        anaesthesia=anaesthetic,
+                        bregma_to_lambda_distance=nsb_model.breg_2_lamb,
+                        injection_coordinate_reference=(
+                            CoordinateReferenceLocation.BREGMA
+                        ),
+                        injection_materials=injection_materials,
+                    )
+                procedures.append(injection_proc)
+            if nsb_model.has_burr_hole_procedure(
+                burr_hole_num=burr_hole_num,
+                burr_hole_procedure=BurrHoleProcedure.FIBER_IMPLANT,
+            ):
+                probe_name = self._map_burr_hole_number_to_probe(burr_hole_num)
+                burr_hole_info = nsb_model.burr_hole_info(
+                    burr_hole_num=burr_hole_num
                 )
-                ophys_probes.append(ophys_probe1)
-            if fiber_implant2 is not None:
-                name = ProbeName.PROBE_B.value
-                stereotactic_coordinate_ml = nsb_model.ml_2nd_inj
-                stereotactic_coordinate_ap = nsb_model.ap_2nd_inj
-                coordinate_reference = self._map_ap_info_to_coord_reference(
-                    nsb_model.ap_2nd_inj
+                burr_during_info = nsb_model.surgery_during_info(
+                    during=burr_hole_info.during,
+                    inj_type=burr_hole_info.inj_type,
                 )
-                stereotactic_coordinate_dv = nsb_model.fiber_implant2_dv
-                angle = nsb_model.inj2_angle_v2
-                ophys_probe2 = OphysProbe.construct(
-                    name=name,
-                    stereotactic_coordinate_ml=stereotactic_coordinate_ml,
-                    stereotactic_coordinate_ap=stereotactic_coordinate_ap,
-                    stereotactic_coordinate_dv=stereotactic_coordinate_dv,
-                    angle=angle,
+                bregma_to_lambda_distance = nsb_model.breg_2_lamb
+                anaesthetic = Anaesthetic.construct(
+                    type="isoflurane",
+                    duration=burr_during_info.anaesthetic_duration_in_minutes,
+                    level=burr_during_info.anaesthetic_level,
+                )
+                ophys_probe = OphysProbe.construct(
+                    name=probe_name,
+                    stereotactic_coordinate_ml=burr_hole_info.coordinate_ml,
+                    stereotactic_coordinate_ap=burr_hole_info.coordinate_ap,
+                    stereotactic_coordinate_dv=(
+                        burr_hole_info.fiber_implant_depth
+                    ),
+                    angle=burr_hole_info.angle,
                     bregma_to_lambda_distance=bregma_to_lambda_distance,
-                    stereotactic_coordinate_reference=coordinate_reference,
+                    stereotactic_coordinate_reference=(
+                        CoordinateReferenceLocation.BREGMA
+                    ),
+                )
+                fiber_implant_proc = FiberImplant.construct(
+                    start_date=self._map_datetime_to_date(
+                        burr_during_info.start_date
+                    ),
+                    end_date=self._map_datetime_to_date(
+                        burr_during_info.start_date
+                    ),
+                    experimenter_full_name=experimenter_full_name,
+                    iacuc_protocol=iacuc_protocol,
+                    animal_weight_prior=burr_during_info.weight_prior,
+                    animal_weight_post=burr_during_info.weight_post,
+                    probes=ophys_probe,
+                    anaesthesia=anaesthetic,
                 )
-                ophys_probes.append(ophys_probe2)
-            fiber_implant = FiberImplant.construct(
-                start_date=start_date,
-                end_date=end_date,
+                procedures.append(fiber_implant_proc)
+
+        # Create generic procedure model if no specific procedures found
+        if len(procedures) == 0:
+            subject_procedure = SubjectProcedure.construct(
+                start_date=self._map_datetime_to_date(
+                    nsb_model.date_of_surgery
+                ),
+                end_date=self._map_datetime_to_date(nsb_model.date_of_surgery),
                 experimenter_full_name=experimenter_full_name,
                 iacuc_protocol=iacuc_protocol,
-                animal_weight_prior=animal_weight_prior,
-                animal_weight_post=animal_weight_post,
-                probes=ophys_probes,
+                animal_weight_prior=nsb_model.weight_before_surgery,
+                animal_weight_post=nsb_model.weight_after_surgery,
             )
-            procedures.append(fiber_implant)
-
-        # If list of procedures is blank or unknown, create a basic procedure
-        if (
-            not nsb_model.has_inj_procedure()
-            and not nsb_model.has_2nd_inj_procedure()
-            and not nsb_model.has_hp_procedure()
-            and not nsb_model.has_cran_procedure()
-            and not nsb_model.has_fiber_implant_procedure()
-        ):
-            basic_kwargs = {
-                "start_date": start_date,
-                "end_date": end_date,
-                "experimenter_full_name": experimenter_full_name,
-                "iacuc_protocol": iacuc_protocol,
-                "animal_weight_prior": animal_weight_prior,
-                "animal_weight_post": animal_weight_post,
-            }
-            subject_procedure = SubjectProcedure.construct(**basic_kwargs)
             procedures.append(subject_procedure)
 
         return procedures
 
     @staticmethod
+    def _map_craniotomy_type(
+        nsb_craniotomy: Optional[NSBCraniotomyType],
+    ) -> Optional[CraniotomyType]:
+        """Maps NSB CraniotomyType into AIND CraniotomyType"""
+        if nsb_craniotomy == NSBCraniotomyType.FIVE_MM:
+            return CraniotomyType.FIVE_MM
+        elif nsb_craniotomy == NSBCraniotomyType.THREE_MM:
+            return CraniotomyType.THREE_MM
+        elif nsb_craniotomy == NSBCraniotomyType.WHC:
+            return CraniotomyType.WHC
+        else:
+            return CraniotomyType.OTHER
+
+    @staticmethod
+    def _map_burr_hole_number_to_probe(
+        burr_hole_num: int,
+    ) -> Optional[ProbeName]:
+        """Maps NSB Burr hole number into AIND ProbeName"""
+        if burr_hole_num == 1:
+            return ProbeName.PROBE_A
+        elif burr_hole_num == 2:
+            return ProbeName.PROBE_B
+        elif burr_hole_num == 3:
+            return ProbeName.PROBE_C
+        elif burr_hole_num == 4:
+            return ProbeName.PROBE_D
+        else:
+            return None
+
+    @staticmethod
     def _map_auth_id_to_exp_name(
         nsb_author_id: Optional[str],
     ) -> Optional[str]:
         """Maps NSB Author ID to Experimenter name as "NSB" + ID"""
         return "NSB" if nsb_author_id is None else f"NSB-{nsb_author_id}"
 
     @staticmethod
@@ -374,43 +407,14 @@
             return Side.LEFT
         elif nsb_hemisphere == Hemisphere.RIGHT:
             return Side.RIGHT
         else:
             return None
 
     @staticmethod
-    def _map_craniotomy_type(
-        nsb_craniotomy: Optional[NSBCraniotomyType],
-    ) -> Optional[CraniotomyType]:
-        """Maps NSB CraniotomyType into AIND CraniotomyType"""
-        if nsb_craniotomy == NSBCraniotomyType.VISUAL_CORTEX:
-            return CraniotomyType.VISCTX
-        elif nsb_craniotomy == NSBCraniotomyType.FRONTAL_WINDOW:
-            return CraniotomyType.THREE_MM
-        elif (
-            nsb_craniotomy == NSBCraniotomyType.WHC_NP
-            or nsb_craniotomy == NSBCraniotomyType.WHC_2P
-        ):
-            return CraniotomyType.WHC
-        else:
-            return CraniotomyType.OTHER
-
-    @staticmethod
-    def _map_nsb_craniotomy_type_to_size(
-        cran_type: NSBCraniotomyType,
-    ) -> Optional[float]:
-        """Maps NSB CraniotomyType into size"""
-        if cran_type == NSBCraniotomyType.VISUAL_CORTEX:
-            return 5.0
-        elif cran_type == NSBCraniotomyType.FRONTAL_WINDOW:
-            return 3.0
-        else:
-            return None
-
-    @staticmethod
     def _map_ap_info_to_coord_reference(
         _: None,
     ) -> Optional[CoordinateReferenceLocation]:
         """Maps NSB virus ap into AIND CoordinateReferenceLocation"""
         return None
 
     @staticmethod
```

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,43 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from enum import Enum
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field, SecretStr, validator
 
-from aind_metadata_service.sharepoint.nsb2019.models import (
-    HeadPostInfo,
-    Hemisphere,
-    InjectionType,
-    NumberWithNotes,
-    Sex,
-)
+
+class Sex(Enum):
+    """Enum class for Sex Types"""
+
+    MALE = "Male"
+    FEMALE = "Female"
+
+
+@dataclass
+class NumberWithNotes:
+    """Container to hold a parsed number from a string"""
+
+    raw_input: Optional[str] = None
+    number: Optional[float] = None
+    notes: Optional[str] = None
+
+
+class InjectionType(Enum):
+    """Enum class for Injection Types"""
+
+    NANOJECT = "Nanoject (Pressure)"
+    IONTOPHORESIS = "Iontophoresis"
+
+
+class Hemisphere(Enum):
+    """Enum class for Hemisphere"""
+
+    RIGHT = "Right"
+    LEFT = "Left"
 
 
 class CraniotomyType(Enum):
     """Enum class for Craniotomy Types"""
 
     FIVE_MM = "5mm"
     THREE_MM = "3mm"
@@ -59,17 +81,23 @@
 class During(Enum):
     """Enum class for Initial/FollowUp classifiers"""
 
     INITIAL_SURGERY = "Initial Surgery"
     FOLLOW_UP_SURGERY = "Follow up Surgery"
 
 
-class HeadPostInfo2023(HeadPostInfo):
+@dataclass
+class HeadPostInfo2023:
     """Extends HeadPostInfo data container to include extra constructor"""
 
+    headframe_type: Optional[str] = None
+    headframe_part_number: Optional[str] = None
+    well_type: Optional[str] = None
+    well_part_number: Optional[str] = None
+
     # flake8: noqa: C901
     @classmethod
     def from_hp_and_hp_type(
         cls, hp: Optional[HeadPost], hp_type: Optional[HeadPostType]
     ):
         """Construct HeadPostInfo2023 from headpost and headpost_type"""
         headframe_type = hp
```

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.1
+Version: 0.4.2
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/aind_metadata_service/labtracks/client.py
 src/aind_metadata_service/labtracks/query_builder.py
 src/aind_metadata_service/sharepoint/__init__.py
 src/aind_metadata_service/sharepoint/client.py
 src/aind_metadata_service/sharepoint/nsb2019/__init__.py
 src/aind_metadata_service/sharepoint/nsb2019/mapping.py
 src/aind_metadata_service/sharepoint/nsb2019/models.py
+src/aind_metadata_service/sharepoint/nsb2019/procedures.py
 src/aind_metadata_service/sharepoint/nsb2023/__init__.py
 src/aind_metadata_service/sharepoint/nsb2023/mapping.py
 src/aind_metadata_service/sharepoint/nsb2023/models.py
 tests/__init__.py
 tests/test_client.py
 tests/test_response_handle.py
 tests/labtracks/__init__.py
```

### Comparing `aind_metadata_service-0.4.1/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.2/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.2/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.2/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4801724137931034%*

 * *Differences: {'2': "{'injection_materials': [OrderedDict([('material_id', None), ('full_genome_name', None), "*

 * *      "('plasmid_name', None), ('genome_copy', None), ('titer', None), ('titer_unit', 'gc/mL'), "*

 * *      "('prep_lot_number', None), ('prep_date', None), ('prep_type', None), ('prep_protocol', "*

 * *      "None)])], 'injection_angle': 0, 'experimenter_full_name': 'NSB-187'}",*

 * * '3': "{'injection_materials': [OrderedDict([('material_id', None), ('full_genome_name', None), "*

 * *      "('plasmid_name', None), ('genome_copy […]*

```diff
@@ -1,9 +1,53 @@
 [
     {
+        "anaesthesia": null,
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
+        "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB-187",
+        "iacuc_protocol": "2115",
+        "notes": null,
+        "probes": [
+            {
+                "angle": null,
+                "angle_unit": "degree",
+                "bregma_to_lambda_distance": 4.0,
+                "bregma_to_lambda_unit": "millimeter",
+                "core_diameter_unit": "\u03bcm",
+                "ferrule_material": null,
+                "name": "Probe A",
+                "notes": null,
+                "stereotactic_coordinate_ap": null,
+                "stereotactic_coordinate_dv": null,
+                "stereotactic_coordinate_ml": null,
+                "stereotactic_coordinate_reference": null,
+                "stereotactic_coordinate_unit": "millimeter"
+            },
+            {
+                "angle": null,
+                "angle_unit": "degree",
+                "bregma_to_lambda_distance": 4.0,
+                "bregma_to_lambda_unit": "millimeter",
+                "core_diameter_unit": "\u03bcm",
+                "ferrule_material": null,
+                "name": "Probe B",
+                "notes": null,
+                "stereotactic_coordinate_ap": null,
+                "stereotactic_coordinate_dv": null,
+                "stereotactic_coordinate_ml": null,
+                "stereotactic_coordinate_reference": null,
+                "stereotactic_coordinate_unit": "millimeter"
+            }
+        ],
+        "procedure_type": "Fiber implant",
+        "start_date": "2022-12-06",
+        "weight_unit": "gram"
+    },
+    {
         "anaesthesia": {
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
@@ -28,26 +72,40 @@
             "type": "isoflurane"
         },
         "animal_weight_post": 19.2,
         "animal_weight_prior": 19.1,
         "bregma_to_lambda_distance": 4.0,
         "bregma_to_lambda_unit": "millimeter",
         "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB-187",
         "iacuc_protocol": null,
-        "injection_angle": null,
+        "injection_angle": 0,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": null,
         "injection_coordinate_unit": "millimeter",
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Left",
-        "injection_materials": null,
+        "injection_materials": [
+            {
+                "full_genome_name": null,
+                "genome_copy": null,
+                "material_id": null,
+                "plasmid_name": null,
+                "prep_date": null,
+                "prep_lot_number": null,
+                "prep_protocol": null,
+                "prep_type": null,
+                "titer": null,
+                "titer_unit": "gc/mL"
+            }
+        ],
         "injection_volume": null,
         "injection_volume_unit": "nanoliter",
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Nanoject injection",
         "recovery_time": null,
         "start_date": "2022-12-06",
@@ -64,106 +122,45 @@
             "type": "isoflurane"
         },
         "animal_weight_post": 19.6,
         "animal_weight_prior": 19.6,
         "bregma_to_lambda_distance": 4.0,
         "bregma_to_lambda_unit": "millimeter",
         "end_date": null,
+        "experimenter_full_name": "NSB-187",
         "iacuc_protocol": null,
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": null,
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
         "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Left",
-        "injection_materials": null,
+        "injection_materials": [
+            {
+                "full_genome_name": null,
+                "genome_copy": null,
+                "material_id": null,
+                "plasmid_name": null,
+                "prep_date": null,
+                "prep_lot_number": null,
+                "prep_protocol": null,
+                "prep_type": null,
+                "titer": null,
+                "titer_unit": "gc/mL"
+            }
+        ],
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": null,
         "start_date": null,
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
-    },
-    {
-        "anaesthesia": {
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "bregma_to_lambda_distance": 4.0,
-        "bregma_to_lambda_unit": "millimeter",
-        "craniotomy_coordinates_ap": null,
-        "craniotomy_coordinates_ml": null,
-        "craniotomy_coordinates_reference": "Lambda",
-        "craniotomy_coordinates_unit": "millimeter",
-        "craniotomy_hemisphere": "Right",
-        "craniotomy_size": 5.0,
-        "craniotomy_size_unit": "millimeter",
-        "craniotomy_type": "Visual Cortex",
-        "dura_removed": true,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2115",
-        "implant_part_number": null,
-        "notes": null,
-        "procedure_type": "Craniotomy",
-        "protective_material": null,
-        "recovery_time": null,
-        "start_date": "2022-12-06",
-        "weight_unit": "gram",
-        "workstation_id": "SWS 3"
-    },
-    {
-        "anaesthesia": null,
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2115",
-        "notes": null,
-        "probes": [
-            {
-                "angle": null,
-                "angle_unit": "degree",
-                "bregma_to_lambda_distance": 4.0,
-                "bregma_to_lambda_unit": "millimeter",
-                "core_diameter_unit": "\u03bcm",
-                "ferrule_material": null,
-                "name": "Probe A",
-                "notes": null,
-                "stereotactic_coordinate_ap": null,
-                "stereotactic_coordinate_dv": null,
-                "stereotactic_coordinate_ml": null,
-                "stereotactic_coordinate_reference": null,
-                "stereotactic_coordinate_unit": "millimeter"
-            },
-            {
-                "angle": null,
-                "angle_unit": "degree",
-                "bregma_to_lambda_distance": 4.0,
-                "bregma_to_lambda_unit": "millimeter",
-                "core_diameter_unit": "\u03bcm",
-                "ferrule_material": null,
-                "name": "Probe B",
-                "notes": null,
-                "stereotactic_coordinate_ap": null,
-                "stereotactic_coordinate_dv": null,
-                "stereotactic_coordinate_ml": null,
-                "stereotactic_coordinate_reference": null,
-                "stereotactic_coordinate_unit": "millimeter"
-            }
-        ],
-        "procedure_type": "Fiber implant",
-        "start_date": "2022-12-06",
-        "weight_unit": "gram"
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6108345934139785%*

 * *Differences: {'0': "{'start_date': '2022-01-03', 'end_date': '2022-01-03', 'iacuc_protocol': '2103', "*

 * *      "'animal_weight_prior': 25.2, 'animal_weight_post': 28.2, 'anaesthesia': {'level': 2.0, "*

 * *      "'duration': 90.0}, 'headframe_type': 'WHC NP', 'headframe_part_number': '0160-100-42', "*

 * *      "'well_part_number': '0160-200-36', 'well_type': 'Neuropixel'}",*

 * * '1': "{'start_date': '2022-01-03', 'end_date': '2022-01-03', 'iacuc_protocol': '2103', "*

 * *      "'animal_weight_prior': 25.2, 'animal_weight_post': 28.2, 'anae […]*

```diff
@@ -1,125 +1,138 @@
 [
     {
         "anaesthesia": {
+            "duration": 90.0,
             "duration_unit": "minute",
-            "level": null,
+            "level": 2.0,
             "type": "isoflurane"
         },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "end_date": "2022-12-06",
+        "animal_weight_post": 28.2,
+        "animal_weight_prior": 25.2,
+        "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "headframe_material": null,
-        "headframe_part_number": "0160-100-10 Rev A",
-        "headframe_type": "CAM-style",
-        "iacuc_protocol": "2115",
+        "headframe_part_number": "0160-100-42",
+        "headframe_type": "WHC NP",
+        "iacuc_protocol": "2103",
         "notes": null,
         "procedure_type": "Headframe",
-        "start_date": "2022-12-06",
+        "start_date": "2022-01-03",
         "weight_unit": "gram",
-        "well_part_number": null,
-        "well_type": "CAM-style"
+        "well_part_number": "0160-200-36",
+        "well_type": "Neuropixel"
     },
     {
         "alternating_current": null,
         "anaesthesia": {
-            "duration": null,
+            "duration": 90.0,
             "duration_unit": "minute",
-            "level": null,
+            "level": 2.0,
             "type": "isoflurane"
         },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
+        "animal_weight_post": 28.2,
+        "animal_weight_prior": 25.2,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
-        "end_date": "2022-12-06",
-        "iacuc_protocol": null,
+        "end_date": "2022-01-03",
+        "experimenter_full_name": "NSB-187",
+        "iacuc_protocol": "2103",
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
-        "injection_coordinate_reference": null,
+        "injection_coordinate_reference": "Bregma",
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
-        "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
-        "injection_hemisphere": "Right",
+        "injection_hemisphere": null,
         "injection_materials": null,
+        "injection_volume": null,
+        "injection_volume_unit": "nanoliter",
         "instrument_id": null,
         "notes": null,
-        "procedure_type": "Iontophoresis injection",
-        "recovery_time": null,
-        "start_date": "2022-12-06",
+        "procedure_type": "Nanoject injection",
+        "recovery_time": 25.0,
+        "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": "SWS 3"
+        "workstation_id": null
     },
     {
+        "alternating_current": null,
         "anaesthesia": {
-            "duration": null,
+            "duration": 120.0,
             "duration_unit": "minute",
-            "level": null,
+            "level": 2.5,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
-        "animal_weight_prior": null,
+        "animal_weight_prior": 28.2,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
-        "end_date": "2022-12-06",
-        "iacuc_protocol": null,
+        "end_date": null,
+        "experimenter_full_name": "NSB-187",
+        "iacuc_protocol": "2103",
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
-        "injection_coordinate_reference": null,
+        "injection_coordinate_reference": "Bregma",
         "injection_coordinate_unit": "millimeter",
+        "injection_current": null,
         "injection_duration": null,
         "injection_duration_unit": "minute",
-        "injection_hemisphere": "Right",
+        "injection_hemisphere": null,
         "injection_materials": null,
         "injection_volume": null,
         "injection_volume_unit": "nanoliter",
-        "instrument_id": "NJ#4",
+        "instrument_id": null,
         "notes": null,
         "procedure_type": "Nanoject injection",
-        "recovery_time": null,
-        "start_date": "2022-12-06",
+        "recovery_time": 30,
+        "start_date": null,
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
     },
     {
+        "alternating_current": null,
         "anaesthesia": {
+            "duration": null,
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
-        "craniotomy_coordinates_ap": null,
-        "craniotomy_coordinates_ml": null,
-        "craniotomy_coordinates_reference": null,
-        "craniotomy_coordinates_unit": "millimeter",
-        "craniotomy_hemisphere": null,
-        "craniotomy_size": null,
-        "craniotomy_size_unit": "millimeter",
-        "craniotomy_type": "Whole hemisphere craniotomy",
-        "dura_removed": false,
-        "end_date": "2022-12-06",
+        "end_date": null,
         "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2115",
-        "implant_part_number": null,
+        "iacuc_protocol": "2103",
+        "injection_angle": null,
+        "injection_angle_unit": "degree",
+        "injection_coordinate_ap": null,
+        "injection_coordinate_depth": null,
+        "injection_coordinate_ml": null,
+        "injection_coordinate_reference": "Bregma",
+        "injection_coordinate_unit": "millimeter",
+        "injection_current": null,
+        "injection_duration": null,
+        "injection_duration_unit": "minute",
+        "injection_hemisphere": null,
+        "injection_materials": null,
+        "injection_volume": null,
+        "injection_volume_unit": "nanoliter",
+        "instrument_id": null,
         "notes": null,
-        "procedure_type": "Craniotomy",
-        "protective_material": null,
+        "procedure_type": "Nanoject injection",
         "recovery_time": null,
-        "start_date": "2022-12-06",
+        "start_date": null,
+        "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": "SWS 3"
+        "workstation_id": null
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.38666666666666666%*

 * *Differences: {'2': "{'injection_materials': [OrderedDict([('material_id', None), ('full_genome_name', None), "*

 * *      "('plasmid_name', None), ('genome_copy', None), ('titer', None), ('titer_unit', 'gc/mL'), "*

 * *      "('prep_lot_number', None), ('prep_date', None), ('prep_type', None), ('prep_protocol', "*

 * *      "None)])], 'injection_angle': 0, 'experimenter_full_name': 'NSB-187'}",*

 * * 'delete': '[3, 2]',*

 * * 'insert': "[(0, OrderedDict([('start_date', '2022-12-06'), ('end_date', '2022-12-06'), "*

 * *           "('experimenter_full […]*

```diff
@@ -1,9 +1,53 @@
 [
     {
+        "anaesthesia": null,
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
+        "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB-187",
+        "iacuc_protocol": "2115",
+        "notes": null,
+        "probes": [
+            {
+                "angle": null,
+                "angle_unit": "degree",
+                "bregma_to_lambda_distance": 4.0,
+                "bregma_to_lambda_unit": "millimeter",
+                "core_diameter_unit": "\u03bcm",
+                "ferrule_material": null,
+                "name": "Probe A",
+                "notes": null,
+                "stereotactic_coordinate_ap": null,
+                "stereotactic_coordinate_dv": null,
+                "stereotactic_coordinate_ml": null,
+                "stereotactic_coordinate_reference": null,
+                "stereotactic_coordinate_unit": "millimeter"
+            },
+            {
+                "angle": null,
+                "angle_unit": "degree",
+                "bregma_to_lambda_distance": 4.0,
+                "bregma_to_lambda_unit": "millimeter",
+                "core_diameter_unit": "\u03bcm",
+                "ferrule_material": null,
+                "name": "Probe B",
+                "notes": null,
+                "stereotactic_coordinate_ap": null,
+                "stereotactic_coordinate_dv": null,
+                "stereotactic_coordinate_ml": null,
+                "stereotactic_coordinate_reference": null,
+                "stereotactic_coordinate_unit": "millimeter"
+            }
+        ],
+        "procedure_type": "Fiber implant",
+        "start_date": "2022-12-06",
+        "weight_unit": "gram"
+    },
+    {
         "anaesthesia": {
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
@@ -29,106 +73,45 @@
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
         "bregma_to_lambda_distance": 4.0,
         "bregma_to_lambda_unit": "millimeter",
         "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB-187",
         "iacuc_protocol": null,
-        "injection_angle": null,
+        "injection_angle": 0,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": null,
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
         "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": null,
-        "injection_materials": null,
+        "injection_materials": [
+            {
+                "full_genome_name": null,
+                "genome_copy": null,
+                "material_id": null,
+                "plasmid_name": null,
+                "prep_date": null,
+                "prep_lot_number": null,
+                "prep_protocol": null,
+                "prep_type": null,
+                "titer": null,
+                "titer_unit": "gc/mL"
+            }
+        ],
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": null,
         "start_date": "2022-12-06",
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": "SWS 3"
-    },
-    {
-        "anaesthesia": {
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "bregma_to_lambda_distance": 4.0,
-        "bregma_to_lambda_unit": "millimeter",
-        "craniotomy_coordinates_ap": null,
-        "craniotomy_coordinates_ml": null,
-        "craniotomy_coordinates_reference": null,
-        "craniotomy_coordinates_unit": "millimeter",
-        "craniotomy_hemisphere": null,
-        "craniotomy_size": 3.0,
-        "craniotomy_size_unit": "millimeter",
-        "craniotomy_type": "3 mm",
-        "dura_removed": null,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2115",
-        "implant_part_number": null,
-        "notes": null,
-        "procedure_type": "Craniotomy",
-        "protective_material": null,
-        "recovery_time": null,
-        "start_date": "2022-12-06",
-        "weight_unit": "gram",
-        "workstation_id": "SWS 3"
-    },
-    {
-        "anaesthesia": null,
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2115",
-        "notes": null,
-        "probes": [
-            {
-                "angle": null,
-                "angle_unit": "degree",
-                "bregma_to_lambda_distance": 4.0,
-                "bregma_to_lambda_unit": "millimeter",
-                "core_diameter_unit": "\u03bcm",
-                "ferrule_material": null,
-                "name": "Probe A",
-                "notes": null,
-                "stereotactic_coordinate_ap": null,
-                "stereotactic_coordinate_dv": null,
-                "stereotactic_coordinate_ml": null,
-                "stereotactic_coordinate_reference": null,
-                "stereotactic_coordinate_unit": "millimeter"
-            },
-            {
-                "angle": null,
-                "angle_unit": "degree",
-                "bregma_to_lambda_distance": 4.0,
-                "bregma_to_lambda_unit": "millimeter",
-                "core_diameter_unit": "\u03bcm",
-                "ferrule_material": null,
-                "name": "Probe B",
-                "notes": null,
-                "stereotactic_coordinate_ap": null,
-                "stereotactic_coordinate_dv": null,
-                "stereotactic_coordinate_ml": null,
-                "stereotactic_coordinate_reference": null,
-                "stereotactic_coordinate_unit": "millimeter"
-            }
-        ],
-        "procedure_type": "Fiber implant",
-        "start_date": "2022-12-06",
-        "weight_unit": "gram"
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {'delete': '[0]',*

 * * 'insert': "[(1, OrderedDict([('start_date', '2022-12-06'), ('end_date', '2022-12-06'), "*

 * *           "('experimenter_full_name', 'NSB-187'), ('iacuc_protocol', '2115'), "*

 * *           "('animal_weight_prior', None), ('animal_weight_post', None), ('weight_unit', 'gram'), "*

 * *           "('anaesthesia', OrderedDict([('type', 'isoflurane'), ('duration_unit', 'minute'), "*

 * *           "('level', None)])), ('notes', None), ('procedure_type', 'Headframe'), "*

 * *           "('headframe_type', 'Neuropixel- […]*

```diff
@@ -3,35 +3,14 @@
         "anaesthesia": {
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB-187",
-        "headframe_material": null,
-        "headframe_part_number": "0160-100-10",
-        "headframe_type": "Neuropixel-style",
-        "iacuc_protocol": "2115",
-        "notes": null,
-        "procedure_type": "Headframe",
-        "start_date": "2022-12-06",
-        "weight_unit": "gram",
-        "well_part_number": "0160-200-36",
-        "well_type": "Neuropixel-style"
-    },
-    {
-        "anaesthesia": {
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
         "craniotomy_coordinates_ap": null,
         "craniotomy_coordinates_ml": null,
         "craniotomy_coordinates_reference": null,
         "craniotomy_coordinates_unit": "millimeter",
         "craniotomy_hemisphere": null,
@@ -46,9 +25,30 @@
         "notes": null,
         "procedure_type": "Craniotomy",
         "protective_material": null,
         "recovery_time": null,
         "start_date": "2022-12-06",
         "weight_unit": "gram",
         "workstation_id": "SWS 3"
+    },
+    {
+        "anaesthesia": {
+            "duration_unit": "minute",
+            "level": null,
+            "type": "isoflurane"
+        },
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
+        "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB-187",
+        "headframe_material": null,
+        "headframe_part_number": "0160-100-10",
+        "headframe_type": "Neuropixel-style",
+        "iacuc_protocol": "2115",
+        "notes": null,
+        "procedure_type": "Headframe",
+        "start_date": "2022-12-06",
+        "weight_unit": "gram",
+        "well_part_number": "0160-200-36",
+        "well_type": "Neuropixel-style"
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {'delete': '[0]',*

 * * 'insert': "[(1, OrderedDict([('start_date', '2022-12-06'), ('end_date', '2022-12-06'), "*

 * *           "('experimenter_full_name', 'NSB'), ('iacuc_protocol', '2115'), ('animal_weight_prior', "*

 * *           "None), ('animal_weight_post', None), ('weight_unit', 'gram'), ('anaesthesia', "*

 * *           "OrderedDict([('type', 'isoflurane'), ('duration_unit', 'minute'), ('level', None)])), "*

 * *           "('notes', None), ('procedure_type', 'Headframe'), ('headframe_type', None), "*

 * *           "('headfra […]*

```diff
@@ -3,35 +3,14 @@
         "anaesthesia": {
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
-        "end_date": "2022-12-06",
-        "experimenter_full_name": "NSB",
-        "headframe_material": null,
-        "headframe_part_number": null,
-        "headframe_type": null,
-        "iacuc_protocol": "2115",
-        "notes": null,
-        "procedure_type": "Headframe",
-        "start_date": "2022-12-06",
-        "weight_unit": "gram",
-        "well_part_number": null,
-        "well_type": null
-    },
-    {
-        "anaesthesia": {
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
         "craniotomy_coordinates_ap": null,
         "craniotomy_coordinates_ml": null,
         "craniotomy_coordinates_reference": null,
         "craniotomy_coordinates_unit": "millimeter",
         "craniotomy_hemisphere": null,
@@ -46,9 +25,30 @@
         "notes": null,
         "procedure_type": "Craniotomy",
         "protective_material": null,
         "recovery_time": null,
         "start_date": "2022-12-06",
         "weight_unit": "gram",
         "workstation_id": "SWS 3"
+    },
+    {
+        "anaesthesia": {
+            "duration_unit": "minute",
+            "level": null,
+            "type": "isoflurane"
+        },
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
+        "end_date": "2022-12-06",
+        "experimenter_full_name": "NSB",
+        "headframe_material": null,
+        "headframe_part_number": null,
+        "headframe_type": null,
+        "iacuc_protocol": "2115",
+        "notes": null,
+        "procedure_type": "Headframe",
+        "start_date": "2022-12-06",
+        "weight_unit": "gram",
+        "well_part_number": null,
+        "well_type": null
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901315789473685%*

 * *Differences: {"'Breg2Lamb'": "'4'",*

 * * "'FiberImplant2'": 'True',*

 * * "'Procedure'": "'HP+Injection+Optic Fiber Implant'"}*

```diff
@@ -1,13 +1,13 @@
 {
     "AP2ndInj": "-3.05",
     "Age_x0020_at_x0020_Injection": "44901.0000000000",
     "Attachments": false,
     "AuthorId": 187,
-    "Breg2Lamb": "4mm",
+    "Breg2Lamb": "4",
     "Cage": null,
     "ComAfter1stInj": "Select...",
     "ComAfter2ndInj": "Select...",
     "ComCoplanar": "Select...",
     "ComDamage": "Select...",
     "ComDuring1stInj": "Select...",
     "ComDuring2ndInj": "Select...",
@@ -30,15 +30,15 @@
     "EditorId": 2916,
     "End_x0020_of_x0020_Week": "2022-12-09T08:00:00Z",
     "Exudate_x0020_Severity": "Select...",
     "Eye_x0020_Affected": "Select...",
     "Eye_x0020_Issue": "Select...",
     "FiberImplant1": true,
     "FiberImplant1DV": "4.2",
-    "FiberImplant2": false,
+    "FiberImplant2": true,
     "FiberImplant2DV": "4.2",
     "FileSystemObjectType": 0,
     "FirstInjRecovery": null,
     "FirstInjectionIsoDuration": null,
     "FirstInjectionWeightAfter": "19.2",
     "FirstInjectionWeightBefor": "19.1",
     "FirstRoundIontoIssue": "Select...",
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "INJ+HP+C+Optic Fiber Implant",
+    "Procedure": "HP+Injection+Optic Fiber Implant",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": "19.6",
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638157894736842%*

 * *Differences: {"'AuthorId'": 'None',*

 * * "'CraniotomyType'": 'None',*

 * * "'Date2ndInjection'": 'None',*

 * * "'HeadpostType'": "'Select...'",*

 * * "'ImplantIDCoverslipType'": "'5mm'",*

 * * "'Inj2Round'": "'N/A'",*

 * * "'Inj2Type'": "'Iontophoresis'",*

 * * "'NanojectNumberInj2'": "'Select...'",*

 * * "'Procedure'": "'HP+C CAM'",*

 * * "'Title'": "'650102HP+C CAM'",*

 * * "'Virus_x0020_A_x002f_P'": "'-1.6'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "AP2ndInj": "-3.05",
     "Age_x0020_at_x0020_Injection": "44901.0000000000",
     "Attachments": false,
-    "AuthorId": 187,
+    "AuthorId": null,
     "Breg2Lamb": null,
     "Cage": null,
     "ComAfter1stInj": "Select...",
     "ComAfter2ndInj": "Select...",
     "ComCoplanar": "Select...",
     "ComDamage": "Select...",
     "ComDuring1stInj": "Select...",
@@ -14,19 +14,19 @@
     "ComDurotomy": "Select...",
     "ComSinusbleed": "Select...",
     "ComSwelling": "Select...",
     "ComWindow": "Select...",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x0100D7F25D3C051CD548B3304044B3DA2E96",
     "Contusion": "Select...",
-    "CraniotomyType": "WHC NP",
+    "CraniotomyType": null,
     "Created": "2022-12-02T17:04:37Z",
     "DV2ndInj": "4.3",
     "Date1stInjection": "2022-12-06T08:00:00Z",
-    "Date2ndInjection": "2022-12-06T08:00:00Z",
+    "Date2ndInjection": null,
     "DateRangeEnd": "2022-12-09T08:00:00Z",
     "DateRangeStart": "2022-12-05T08:00:00Z",
     "Date_x0020_of_x0020_Birth": null,
     "Date_x0020_of_x0020_Surgery": "2022-12-06T08:00:00Z",
     "EditorId": 2916,
     "End_x0020_of_x0020_Week": "2022-12-09T08:00:00Z",
     "Exudate_x0020_Severity": "Select...",
@@ -48,41 +48,41 @@
     "HPRecovery": null,
     "HPRequestorCommentsPlaintext": null,
     "HPSurgeonComments": null,
     "HP_x0020_A_x002f_P": "1.3",
     "HP_x0020_Diameter": "5mm",
     "HP_x0020_M_x002f_L": "2.8",
     "HP_x0020__x0026__x0020_Inj": "Yes",
-    "HeadpostType": "CAM-style headframe (0160-100-10 Rev A)",
+    "HeadpostType": "Select...",
     "Hemisphere2ndInj": "Right",
     "HpLoc": "Center",
     "HpPerf": "Select if applicable...",
     "HpPrevInject": "Select...",
     "HpWorkStation": "SWS 3",
     "IACUC_x0020_Protocol_x0020__x002": "2115",
     "ID": 5554,
     "Id": 5554,
-    "ImplantIDCoverslipType": "5mm coverslip",
+    "ImplantIDCoverslipType": "5mm",
     "Inj1AlternatingTime": "7/7",
     "Inj1Angle_v2": "0",
     "Inj1Current": "5uA",
     "Inj1LenghtofTime": "5min",
     "Inj1Round": "1st",
     "Inj1StorageLocation": "A Box",
     "Inj1Type": "Iontophoresis",
     "Inj1VirusStrain_rt": null,
     "Inj1Vol": "400",
     "Inj1angle0": "0 degrees",
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": "0",
     "Inj2Current": "5uA",
     "Inj2LenghtofTime": null,
-    "Inj2Round": "2nd",
+    "Inj2Round": "N/A",
     "Inj2StorageLocation": "A Box",
-    "Inj2Type": "Nanoject (Pressure)",
+    "Inj2Type": "Iontophoresis",
     "Inj2VirusStrain_rt": null,
     "Inj2Vol": "400",
     "Inj2angle0": "Select...",
     "IontoNumberHPINJ": null,
     "IontoNumberInj1": "Select...",
     "IontoNumberInj2": "Select...",
     "Iso_x0020_On": null,
@@ -98,21 +98,21 @@
     "Long1stRoundInjCmts": null,
     "Long2ndRndInjCmts": null,
     "LongRequestorComments": null,
     "LongSurgeonComments": null,
     "ML2ndInj": "-0.6",
     "Modified": "2022-12-02T18:15:36Z",
     "NanojectNumberInj10": "Select...",
-    "NanojectNumberInj2": "NJ#4",
+    "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "Injection+C CAM+HP",
+    "Procedure": "HP+C CAM",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
@@ -125,21 +125,21 @@
     "SurgeryStatus": "New",
     "TEST_x0020_1st_x0020_Round_x0020Id": 2916,
     "TEST_x0020_1st_x0020_Round_x0020StringId": "2916",
     "TEST_x0020_2nd_x0020_Round_x0020Id": null,
     "TEST_x0020_2nd_x0020_Round_x0020StringId": null,
     "Test1Id": 2916,
     "Test1StringId": "2916",
-    "Title": "650102Injection+C CAM+HP",
+    "Title": "650102HP+C CAM",
     "Touch_x0020_Up_x0020_Status": "Select...",
     "Touch_x0020_Up_x0020_SurgeonId": null,
     "Touch_x0020_Up_x0020_SurgeonStringId": null,
     "Touch_x0020_Up_x0020_Weight_x002": null,
     "Touch_x0020_Up_x0020__x0020_Comp": null,
-    "Virus_x0020_A_x002f_P": "-1.6, rostral to lambda",
+    "Virus_x0020_A_x002f_P": "-1.6",
     "Virus_x0020_D_x002f_V": "4.3, 2.6",
     "Virus_x0020_Hemisphere": "Right",
     "Virus_x0020_M_x002f_L": "-3.3",
     "Weight_x0020_after_x0020_Surgery": null,
     "Weight_x0020_before_x0020_Surger": null,
     "WorkStation1stInjection": "SWS 3",
     "WorkStation2ndInjection": "Select...",
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'Procedure'": "'HP+Injection+Optic Fiber Implant'",*

 * * "'Title'": "'650102HP+Injection+Optic Fiber Implant'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "HP+C+Injection+Optic Fiber Implant",
+    "Procedure": "HP+Injection+Optic Fiber Implant",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
@@ -125,15 +125,15 @@
     "SurgeryStatus": "New",
     "TEST_x0020_1st_x0020_Round_x0020Id": 2916,
     "TEST_x0020_1st_x0020_Round_x0020StringId": "2916",
     "TEST_x0020_2nd_x0020_Round_x0020Id": null,
     "TEST_x0020_2nd_x0020_Round_x0020StringId": null,
     "Test1Id": 2916,
     "Test1StringId": "2916",
-    "Title": "650102HP+Injection+Optic Fiber Implant+C",
+    "Title": "650102HP+Injection+Optic Fiber Implant",
     "Touch_x0020_Up_x0020_Status": "Select...",
     "Touch_x0020_Up_x0020_SurgeonId": null,
     "Touch_x0020_Up_x0020_SurgeonStringId": null,
     "Touch_x0020_Up_x0020_Weight_x002": null,
     "Touch_x0020_Up_x0020__x0020_Comp": null,
     "Virus_x0020_A_x002f_P": "-1.6",
     "Virus_x0020_D_x002f_V": "Anywhere",
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'Procedure'": "'HP+C Multiscope'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "HP+C",
+    "Procedure": "HP+C Multiscope",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'Procedure'": "'HP only'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "HP",
+    "Procedure": "HP only",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'Procedure'": "'HP only'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "HP",
+    "Procedure": "HP only",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671052631578947%*

 * *Differences: {"'AuthorId'": '187',*

 * * "'CraniotomyType'": "'WHC NP'",*

 * * "'Date2ndInjection'": "'2022-12-06T08:00:00Z'",*

 * * "'HeadpostType'": "'CAM-style headframe (0160-100-10 Rev A)'",*

 * * "'ImplantIDCoverslipType'": "'5mm coverslip'",*

 * * "'Inj2Round'": "'2nd'",*

 * * "'Inj2Type'": "'Nanoject (Pressure)'",*

 * * "'NanojectNumberInj2'": "'NJ#4'",*

 * * "'Title'": "'650102Injection+C CAM+HP'",*

 * * "'Virus_x0020_A_x002f_P'": "'-1.6, rostral to lambda'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "AP2ndInj": "-3.05",
     "Age_x0020_at_x0020_Injection": "44901.0000000000",
     "Attachments": false,
-    "AuthorId": null,
+    "AuthorId": 187,
     "Breg2Lamb": null,
     "Cage": null,
     "ComAfter1stInj": "Select...",
     "ComAfter2ndInj": "Select...",
     "ComCoplanar": "Select...",
     "ComDamage": "Select...",
     "ComDuring1stInj": "Select...",
@@ -14,19 +14,19 @@
     "ComDurotomy": "Select...",
     "ComSinusbleed": "Select...",
     "ComSwelling": "Select...",
     "ComWindow": "Select...",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x0100D7F25D3C051CD548B3304044B3DA2E96",
     "Contusion": "Select...",
-    "CraniotomyType": null,
+    "CraniotomyType": "WHC NP",
     "Created": "2022-12-02T17:04:37Z",
     "DV2ndInj": "4.3",
     "Date1stInjection": "2022-12-06T08:00:00Z",
-    "Date2ndInjection": null,
+    "Date2ndInjection": "2022-12-06T08:00:00Z",
     "DateRangeEnd": "2022-12-09T08:00:00Z",
     "DateRangeStart": "2022-12-05T08:00:00Z",
     "Date_x0020_of_x0020_Birth": null,
     "Date_x0020_of_x0020_Surgery": "2022-12-06T08:00:00Z",
     "EditorId": 2916,
     "End_x0020_of_x0020_Week": "2022-12-09T08:00:00Z",
     "Exudate_x0020_Severity": "Select...",
@@ -48,41 +48,41 @@
     "HPRecovery": null,
     "HPRequestorCommentsPlaintext": null,
     "HPSurgeonComments": null,
     "HP_x0020_A_x002f_P": "1.3",
     "HP_x0020_Diameter": "5mm",
     "HP_x0020_M_x002f_L": "2.8",
     "HP_x0020__x0026__x0020_Inj": "Yes",
-    "HeadpostType": "Select...",
+    "HeadpostType": "CAM-style headframe (0160-100-10 Rev A)",
     "Hemisphere2ndInj": "Right",
     "HpLoc": "Center",
     "HpPerf": "Select if applicable...",
     "HpPrevInject": "Select...",
     "HpWorkStation": "SWS 3",
     "IACUC_x0020_Protocol_x0020__x002": "2115",
     "ID": 5554,
     "Id": 5554,
-    "ImplantIDCoverslipType": "5mm",
+    "ImplantIDCoverslipType": "5mm coverslip",
     "Inj1AlternatingTime": "7/7",
     "Inj1Angle_v2": "0",
     "Inj1Current": "5uA",
     "Inj1LenghtofTime": "5min",
     "Inj1Round": "1st",
     "Inj1StorageLocation": "A Box",
     "Inj1Type": "Iontophoresis",
     "Inj1VirusStrain_rt": null,
     "Inj1Vol": "400",
     "Inj1angle0": "0 degrees",
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": "0",
     "Inj2Current": "5uA",
     "Inj2LenghtofTime": null,
-    "Inj2Round": "N/A",
+    "Inj2Round": "2nd",
     "Inj2StorageLocation": "A Box",
-    "Inj2Type": "Iontophoresis",
+    "Inj2Type": "Nanoject (Pressure)",
     "Inj2VirusStrain_rt": null,
     "Inj2Vol": "400",
     "Inj2angle0": "Select...",
     "IontoNumberHPINJ": null,
     "IontoNumberInj1": "Select...",
     "IontoNumberInj2": "Select...",
     "Iso_x0020_On": null,
@@ -98,15 +98,15 @@
     "Long1stRoundInjCmts": null,
     "Long2ndRndInjCmts": null,
     "LongRequestorComments": null,
     "LongSurgeonComments": null,
     "ML2ndInj": "-0.6",
     "Modified": "2022-12-02T18:15:36Z",
     "NanojectNumberInj10": "Select...",
-    "NanojectNumberInj2": "Select...",
+    "NanojectNumberInj2": "NJ#4",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
     "Procedure": "HP+C CAM",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
@@ -125,21 +125,21 @@
     "SurgeryStatus": "New",
     "TEST_x0020_1st_x0020_Round_x0020Id": 2916,
     "TEST_x0020_1st_x0020_Round_x0020StringId": "2916",
     "TEST_x0020_2nd_x0020_Round_x0020Id": null,
     "TEST_x0020_2nd_x0020_Round_x0020StringId": null,
     "Test1Id": 2916,
     "Test1StringId": "2916",
-    "Title": "650102HP+C CAM",
+    "Title": "650102Injection+C CAM+HP",
     "Touch_x0020_Up_x0020_Status": "Select...",
     "Touch_x0020_Up_x0020_SurgeonId": null,
     "Touch_x0020_Up_x0020_SurgeonStringId": null,
     "Touch_x0020_Up_x0020_Weight_x002": null,
     "Touch_x0020_Up_x0020__x0020_Comp": null,
-    "Virus_x0020_A_x002f_P": "-1.6",
+    "Virus_x0020_A_x002f_P": "-1.6, rostral to lambda",
     "Virus_x0020_D_x002f_V": "4.3, 2.6",
     "Virus_x0020_Hemisphere": "Right",
     "Virus_x0020_M_x002f_L": "-3.3",
     "Weight_x0020_after_x0020_Surgery": null,
     "Weight_x0020_before_x0020_Surger": null,
     "WorkStation1stInjection": "SWS 3",
     "WorkStation2ndInjection": "Select...",
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.20703125%*

 * *Differences: {'0': "{'recovery_time': None, 'instrument_id': 'Ionto #1', 'bregma_to_lambda_distance': 6.1, "*

 * *      "'injection_hemisphere': 'Right', 'procedure_type': 'Iontophoresis injection', "*

 * *      "'injection_current_unit': 'microamps', delete: ['injection_volume', "*

 * *      "'injection_volume_unit']}",*

 * * 'delete': '[3, 2, 0]'}*

```diff
@@ -1,138 +1,39 @@
 [
     {
-        "anaesthesia": {
-            "duration": 90.0,
-            "duration_unit": "minute",
-            "level": 2.0,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": 28.2,
-        "animal_weight_prior": 25.2,
-        "end_date": "2022-01-03",
-        "experimenter_full_name": "NSB-187",
-        "headframe_material": null,
-        "headframe_part_number": "0160-100-42",
-        "headframe_type": "WHC NP",
-        "iacuc_protocol": "2103",
-        "notes": null,
-        "procedure_type": "Headframe",
-        "start_date": "2022-01-03",
-        "weight_unit": "gram",
-        "well_part_number": "0160-200-36",
-        "well_type": "Neuropixel"
-    },
-    {
         "alternating_current": null,
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
         },
         "animal_weight_post": 28.2,
         "animal_weight_prior": 25.2,
-        "bregma_to_lambda_distance": null,
+        "bregma_to_lambda_distance": 6.1,
         "bregma_to_lambda_unit": "millimeter",
         "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": "Bregma",
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
+        "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
-        "injection_hemisphere": null,
+        "injection_hemisphere": "Right",
         "injection_materials": null,
-        "injection_volume": null,
-        "injection_volume_unit": "nanoliter",
-        "instrument_id": null,
+        "instrument_id": "Ionto #1",
         "notes": null,
-        "procedure_type": "Nanoject injection",
-        "recovery_time": 25.0,
-        "start_date": "2022-01-03",
-        "targeted_structure": null,
-        "weight_unit": "gram",
-        "workstation_id": null
-    },
-    {
-        "alternating_current": null,
-        "anaesthesia": {
-            "duration": 120.0,
-            "duration_unit": "minute",
-            "level": 2.5,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": 28.2,
-        "bregma_to_lambda_distance": null,
-        "bregma_to_lambda_unit": "millimeter",
-        "end_date": null,
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2103",
-        "injection_angle": null,
-        "injection_angle_unit": "degree",
-        "injection_coordinate_ap": null,
-        "injection_coordinate_depth": null,
-        "injection_coordinate_ml": null,
-        "injection_coordinate_reference": "Bregma",
-        "injection_coordinate_unit": "millimeter",
-        "injection_current": null,
-        "injection_duration": null,
-        "injection_duration_unit": "minute",
-        "injection_hemisphere": null,
-        "injection_materials": null,
-        "injection_volume": null,
-        "injection_volume_unit": "nanoliter",
-        "instrument_id": null,
-        "notes": null,
-        "procedure_type": "Nanoject injection",
-        "recovery_time": 30,
-        "start_date": null,
-        "targeted_structure": null,
-        "weight_unit": "gram",
-        "workstation_id": null
-    },
-    {
-        "alternating_current": null,
-        "anaesthesia": {
-            "duration": null,
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "bregma_to_lambda_distance": null,
-        "bregma_to_lambda_unit": "millimeter",
-        "end_date": null,
-        "experimenter_full_name": "NSB-187",
-        "iacuc_protocol": "2103",
-        "injection_angle": null,
-        "injection_angle_unit": "degree",
-        "injection_coordinate_ap": null,
-        "injection_coordinate_depth": null,
-        "injection_coordinate_ml": null,
-        "injection_coordinate_reference": "Bregma",
-        "injection_coordinate_unit": "millimeter",
-        "injection_current": null,
-        "injection_duration": null,
-        "injection_duration_unit": "minute",
-        "injection_hemisphere": null,
-        "injection_materials": null,
-        "injection_volume": null,
-        "injection_volume_unit": "nanoliter",
-        "instrument_id": null,
-        "notes": null,
-        "procedure_type": "Nanoject injection",
+        "procedure_type": "Iontophoresis injection",
         "recovery_time": null,
-        "start_date": null,
+        "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
     }
 ]
```

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-"""Tests NSB 2019 data model is parsed correctly"""
+"""Tests NSB 2023 data model is parsed correctly"""
 
 import json
 import logging
 import os
 from copy import deepcopy
-from datetime import timedelta
 from pathlib import Path
 from typing import List, Tuple
 from unittest import TestCase
 from unittest import main as unittest_main
 
-from aind_data_schema.procedures import (
-    BrainInjection,
-    CraniotomyType,
-    InjectionMaterial,
-)
+from aind_data_schema.procedures import CraniotomyType, InjectionMaterial
 
-from aind_metadata_service.sharepoint.nsb2019.mapping import NSB2019Mapping
-from aind_metadata_service.sharepoint.nsb2019.models import NSBList2019
+from aind_metadata_service.sharepoint.nsb2023.mapping import NSB2023Mapping
+from aind_metadata_service.sharepoint.nsb2023.models import NSBList2023
 
 if os.getenv("LOG_LEVEL"):  # pragma: no cover
     logging.basicConfig(level=os.getenv("LOG_LEVEL"))
 
 TEST_DIR = Path(os.path.dirname(os.path.realpath(__file__))) / ".." / ".."
-DIR_RAW = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "raw"
-DIR_MAP = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "mapped"
+DIR_RAW = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "raw"
+DIR_MAP = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "mapped"
 LIST_ITEM_FILE_NAMES = os.listdir(DIR_RAW)
 sorted(LIST_ITEM_FILE_NAMES)
 LIST_ITEM_FILE_PATHS = [DIR_RAW / str(f) for f in LIST_ITEM_FILE_NAMES]
 MAPPED_ITEM_FILE_NAMES = os.listdir(DIR_MAP)
 sorted(MAPPED_ITEM_FILE_NAMES)
 MAPPED_FILE_PATHS = [DIR_MAP / str(f) for f in MAPPED_ITEM_FILE_NAMES]
 
 
-class TestNSB2019Parsers(TestCase):
-    """Tests methods in NSB2019Mapping class"""
+class TestNSB2023Parsers(TestCase):
+    """Tests methods in NSB2023Mapping class"""
 
     @classmethod
     def setUpClass(cls):
         """Load json files before running tests."""
         cls.list_items = cls._load_json_files()
 
     @staticmethod
@@ -52,93 +47,84 @@
                 / ("mapped_" + file_path.name)
             )
             with open(file_path) as f:
                 contents = json.load(f)
             with open(mapped_file_path) as f:
                 mapped_contents = json.load(f)
             list_items.append((contents, mapped_contents, file_path.name))
-        list_items.sort(key=lambda x: x[2])
+            list_items.sort(key=lambda x: x[2])
         return list_items
 
     def test_parser(self):
         """Checks that raw data is parsed correctly"""
         for list_item in self.list_items:
             raw_data = list_item[0]
             expected_mapped_data = list(list_item[1])
             expected_mapped_data.sort(key=lambda x: str(x))
             raw_file_name = list_item[2]
             logging.debug(f"Processing file: {raw_file_name}")
-            nsb_model = NSBList2019.parse_obj(raw_data)
-            mapper = NSB2019Mapping()
+            nsb_model = NSBList2023.parse_obj(raw_data)
+            mapper = NSB2023Mapping()
             mapped_procedure = mapper.map_nsb_model(nsb_model)
             mapped_procedure_json = [
                 json.loads(p.json()) for p in mapped_procedure
             ]
             mapped_procedure_json.sort(key=lambda x: str(x))
             self.assertEqual(expected_mapped_data, mapped_procedure_json)
 
-    def test_inj_mapping_edge_cases(self):
-        """Tests the case where there is an INJ procedure, but the inj types
-        are malformed. It should create generic BrainInjection objects."""
-
-        list_item = self.list_items[0]
-        raw_data = deepcopy(list_item[0])
-        raw_data["Inj1Type"] = "Select..."
-        raw_data["Inj2Type"] = "Select..."
-        raw_data["Procedure"] = "INJ"
-        raw_data["Virus_x0020_A_x002f_P"] = "Select..."
-        raw_data["ImplantIDCoverslipType"] = "3.5"
-        nsb_model = NSBList2019.parse_obj(raw_data)
-        mapper = NSB2019Mapping()
-        mapped_procedure = mapper.map_nsb_model(nsb_model)
-        self.assertTrue(isinstance(mapped_procedure[0], BrainInjection))
-        self.assertTrue(isinstance(mapped_procedure[1], BrainInjection))
-
     def test_craniotomy_edge_case(self):
         """Tests other craniotomy cases"""
 
         # Check WHC type
-        list_item = self.list_items[2]  # Should be list_item3.json
+        list_item = self.list_items[2]
         raw_data = deepcopy(list_item[0])
-        raw_data["Procedure"] = "HP+C"
-        raw_data["CraniotomyType"] = "WHC NP"
-        nsb_model1 = NSBList2019.parse_obj(raw_data)
-        mapper = NSB2019Mapping()
+        raw_data["Procedure"] = "WHC NP"
+        raw_data["CraniotomyType"] = "WHC"
+        nsb_model1 = NSBList2023.parse_obj(raw_data)
+        mapper = NSB2023Mapping()
         mapped_procedure1 = mapper.map_nsb_model(nsb_model1)
         mapped_procedure1.sort(key=lambda x: str(x))
         cran_proc1 = mapped_procedure1[0]
         self.assertEqual(
             CraniotomyType.WHC, getattr(cran_proc1, "craniotomy_type")
         )
 
         # Check OTHER type
+        raw_data["Procedure"] = "WHC NP"
         raw_data["CraniotomyType"] = "Other"
-        nsb_model2 = NSBList2019.parse_obj(raw_data)
+        nsb_model2 = NSBList2023.parse_obj(raw_data)
         mapped_procedure2 = mapper.map_nsb_model(nsb_model2)
         mapped_procedure2.sort(key=lambda x: str(x))
         cran_proc2 = mapped_procedure2[0]
         self.assertEqual(
             CraniotomyType.OTHER, getattr(cran_proc2, "craniotomy_type")
         )
 
-    def test_map_duration_minutes(self):
-        """Tests that durations are mapped correctly"""
-        duration1 = timedelta(minutes=5)
-        mapper = NSB2019Mapping()
-        minutes1 = mapper._duration_to_minutes(duration1)
-        self.assertEqual(5, minutes1)
-        duration2 = None
-        minutes2 = mapper._duration_to_minutes(duration2)
-        self.assertIsNone(minutes2)
-
-    def test_virus_strain_mapping(self):
-        """Tests map_virus_strain_to_materials method."""
-        mapper = NSB2019Mapping()
-        inj_materials = mapper._map_virus_strain_to_materials("abc")
-        expected_inj_materials = InjectionMaterial.construct(
-            full_genome_name="abc"
+    def test_injection_edge_case(self):
+        """Tests the case where there is an INJ procedure, but the inj types
+        are malformed. It should create generic BrainInjection objects."""
+        list_item = self.list_items[3]
+        raw_data = deepcopy(list_item[0])
+        raw_data["Inj1Type"] = "Select..."
+        raw_data["ImplantIDCoverslipType"] = "3.5"
+        nsb_model = NSBList2023.parse_obj(raw_data)
+        mapper = NSB2023Mapping()
+        mapped_procedure = mapper.map_nsb_model(nsb_model)
+        mapped_virus_strain = mapper._map_virus_strain_to_materials("abc-def")
+        mapped_virus_strain_none = mapper._map_virus_strain_to_materials(None)
+        mapped_coordinate_ref = mapper._map_ap_info_to_coord_reference(None)
+        self.assertEqual(
+            InjectionMaterial.construct(full_genome_name="abc-def"),
+            mapped_virus_strain,
         )
-        self.assertEqual(expected_inj_materials, inj_materials)
+        self.assertIsNone(mapped_virus_strain_none)
+        self.assertIsNone(mapped_coordinate_ref)
+        self.assertIsNotNone(mapped_procedure)
+
+    def test_burr_hole_to_probe_edge_case(self):
+        """Tests edge case where burr hole number is 5"""
+        mapper = NSB2023Mapping()
+        self.assertIsNone(mapper._map_burr_hole_number_to_probe(5))
 
 
 if __name__ == "__main__":
     unittest_main()
```

### Comparing `aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import List, Tuple
 from unittest import TestCase
 from unittest import main as unittest_main
 
-from aind_metadata_service.sharepoint.nsb2019.models import NSBList2019, Sex
+from aind_metadata_service.sharepoint.nsb2019.models import NSBList, Sex
 
 if os.getenv("LOG_LEVEL"):  # pragma: no cover
     logging.basicConfig(level=os.getenv("LOG_LEVEL"))
 
 TEST_DIR = Path(os.path.dirname(os.path.realpath(__file__))) / ".." / ".."
 SHAREPOINT_DIR = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "raw"
 LIST_ITEM_FILE_NAMES = os.listdir(SHAREPOINT_DIR)
@@ -41,39 +41,29 @@
 
     def test_models_parsed(self):
         """Tests that the given list item files are parsed without error."""
         for index in range(len(self.list_items)):
             list_item = self.list_items[index][0]
             filename = self.list_items[index][1]
             logging.debug(f"Processing file: {filename}")
-            nsb_model = NSBList2019.parse_obj(list_item)
+            nsb_model = NSBList.parse_obj(list_item)
             self.assertEqual(nsb_model.author_id, list_item.get("AuthorId"))
 
     def test_aberrant_data_parsed(self):
         """Tests that certain edge cases get handled correctly"""
         list_item = deepcopy(self.list_items[0][0])
         # Test that numeric entries instead of strings will also get parsed
-        list_item["Age_x0020_at_x0020_Injection"] = 22
+        list_item["Age_x0020_at_x0020_Injection"] = "22"
         # Test that malformed or null types get mapped to None
-        list_item["Inj1Type"] = "Select..."
+        list_item["Inj1Type"] = "Wrong string"
         list_item["HPDurotomy"] = None
         # Check that the sex types are being mapped correctly
         list_item["Sex"] = "Female"
-        nsb_model = NSBList2019.parse_obj(list_item)
-        self.assertEqual(22, nsb_model.age_at_injection)
+        nsb_model = NSBList.parse_obj(list_item)
+        self.assertEqual("22", nsb_model.age_at_injection)
         self.assertIsNone(nsb_model.inj1_type)
         self.assertIsNone(nsb_model.hp_durotomy)
         self.assertEqual(Sex.FEMALE, nsb_model.sex)
 
-    def test_boolean_properties(self):
-        """Tests the boolean methods are correct."""
-        list_item = deepcopy(self.list_items[0][0])
-        nsb_model = NSBList2019.parse_obj(list_item)
-        self.assertTrue(nsb_model.has_cran_procedure())
-        self.assertTrue(nsb_model.has_hp_procedure())
-        self.assertTrue(nsb_model.has_inj_procedure())
-        self.assertTrue(nsb_model.has_2nd_inj_procedure())
-        self.assertTrue(nsb_model.has_fiber_implant_procedure())
-
 
 if __name__ == "__main__":
     unittest_main()
```

### Comparing `aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""Tests NSB 2023 data model is parsed correctly"""
+"""Tests NSB 2019 data model is parsed correctly"""
 
 import json
 import logging
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import List, Tuple
 from unittest import TestCase
 from unittest import main as unittest_main
 
-from aind_data_schema.procedures import CraniotomyType
+from aind_data_schema.procedures import BrainInjection
 
-from aind_metadata_service.sharepoint.nsb2023.mapping import NSB2023Mapping
-from aind_metadata_service.sharepoint.nsb2023.models import NSBList2023
+from aind_metadata_service.sharepoint.nsb2019.mapping import MappedNSBList
+from aind_metadata_service.sharepoint.nsb2019.models import NSBList
 
 if os.getenv("LOG_LEVEL"):  # pragma: no cover
     logging.basicConfig(level=os.getenv("LOG_LEVEL"))
 
 TEST_DIR = Path(os.path.dirname(os.path.realpath(__file__))) / ".." / ".."
-DIR_RAW = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "raw"
-DIR_MAP = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "mapped"
+DIR_RAW = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "raw"
+DIR_MAP = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "mapped"
 LIST_ITEM_FILE_NAMES = os.listdir(DIR_RAW)
 sorted(LIST_ITEM_FILE_NAMES)
 LIST_ITEM_FILE_PATHS = [DIR_RAW / str(f) for f in LIST_ITEM_FILE_NAMES]
 MAPPED_ITEM_FILE_NAMES = os.listdir(DIR_MAP)
 sorted(MAPPED_ITEM_FILE_NAMES)
 MAPPED_FILE_PATHS = [DIR_MAP / str(f) for f in MAPPED_ITEM_FILE_NAMES]
 
 
-class TestNSB2023Parsers(TestCase):
-    """Tests methods in NSB2023Mapping class"""
+class TestNSB2019Parsers(TestCase):
+    """Tests methods in NSB2019Mapping class"""
 
     @classmethod
     def setUpClass(cls):
         """Load json files before running tests."""
         cls.list_items = cls._load_json_files()
 
     @staticmethod
@@ -47,75 +47,70 @@
                 / ("mapped_" + file_path.name)
             )
             with open(file_path) as f:
                 contents = json.load(f)
             with open(mapped_file_path) as f:
                 mapped_contents = json.load(f)
             list_items.append((contents, mapped_contents, file_path.name))
-            list_items.sort(key=lambda x: x[2])
+        list_items.sort(key=lambda x: x[2])
         return list_items
 
     def test_parser(self):
         """Checks that raw data is parsed correctly"""
         for list_item in self.list_items:
             raw_data = list_item[0]
             expected_mapped_data = list(list_item[1])
             expected_mapped_data.sort(key=lambda x: str(x))
             raw_file_name = list_item[2]
             logging.debug(f"Processing file: {raw_file_name}")
-            nsb_model = NSBList2023.parse_obj(raw_data)
-            mapper = NSB2023Mapping()
-            mapped_procedure = mapper.map_nsb_model(nsb_model)
+            nsb_model = NSBList.parse_obj(raw_data)
+            mapped_model = MappedNSBList(nsb=nsb_model)
+            mapped_procedures = mapped_model.get_procedures()
             mapped_procedure_json = [
-                json.loads(p.json()) for p in mapped_procedure
+                json.loads(p.json()) for p in mapped_procedures
             ]
             mapped_procedure_json.sort(key=lambda x: str(x))
-            self.assertEqual(expected_mapped_data, mapped_procedure_json)
 
-    def test_craniotomy_edge_case(self):
-        """Tests other craniotomy cases"""
+            self.assertEqual(expected_mapped_data, mapped_procedure_json)
 
-        # Check WHC type
-        list_item = self.list_items[2]
+    def test_properties(self):
+        """Tests that the properties are parsed correctly."""
+        list_item = self.list_items[0]
         raw_data = deepcopy(list_item[0])
-        raw_data["Procedure"] = "WHC NP"
-        raw_data["CraniotomyType"] = "WHC"
-        nsb_model1 = NSBList2023.parse_obj(raw_data)
-        mapper = NSB2023Mapping()
-        mapped_procedure1 = mapper.map_nsb_model(nsb_model1)
-        mapped_procedure1.sort(key=lambda x: str(x))
-        cran_proc1 = mapped_procedure1[0]
-        self.assertEqual(
-            CraniotomyType.WHC, getattr(cran_proc1, "craniotomy_type")
-        )
-
-        # Check OTHER type
-        raw_data["Procedure"] = "WHC NP"
-        raw_data["CraniotomyType"] = "Other"
-        nsb_model2 = NSBList2023.parse_obj(raw_data)
-        mapped_procedure2 = mapper.map_nsb_model(nsb_model2)
-        mapped_procedure2.sort(key=lambda x: str(x))
-        cran_proc2 = mapped_procedure2[0]
-        self.assertEqual(
-            CraniotomyType.OTHER, getattr(cran_proc2, "craniotomy_type")
-        )
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapped_model = MappedNSBList(nsb=nsb_model)
+        props = []
+        for k in dir(mapped_model.__class__):
+            cls = mapped_model.__class__
+            attr = getattr(cls, k)
+            if isinstance(attr, property):
+                props.append(getattr(mapped_model, k))
+        self.assertEqual(117, len(props))
 
-    def test_injection_edge_case(self):
+    def test_inj_mapping_edge_cases(self):
         """Tests the case where there is an INJ procedure, but the inj types
         are malformed. It should create generic BrainInjection objects."""
-        list_item = self.list_items[3]
+
+        list_item = self.list_items[0]
         raw_data = deepcopy(list_item[0])
         raw_data["Inj1Type"] = "Select..."
+        raw_data["Inj2Type"] = "Nanoject (Pressure)"
+        raw_data["Procedure"] = "Stereotaxic Injection"
+        raw_data["Virus_x0020_A_x002f_P"] = "3 lambda"
+        raw_data["AP2ndInj"] = "2 lambda"
         raw_data["ImplantIDCoverslipType"] = "3.5"
-        nsb_model = NSBList2023.parse_obj(raw_data)
-        mapper = NSB2023Mapping()
-        mapped_procedure = mapper.map_nsb_model(nsb_model)
-        self.assertIsNotNone(mapped_procedure)
-
-    def test_burr_hole_to_probe_edge_case(self):
-        """Tests edge case where burr hole number is 5"""
-        mapper = NSB2023Mapping()
-        self.assertIsNone(mapper._map_burr_hole_number_to_probe(5))
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model)
+        mapped_procedure = mapper.get_procedures()
+        self.assertTrue(isinstance(mapped_procedure[0], BrainInjection))
+        self.assertTrue(isinstance(mapped_procedure[1], BrainInjection))
+        raw_data["Inj2Type"] = "Select..."
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model)
+        mapped_procedure = mapper.get_procedures()
+        self.assertTrue(isinstance(mapped_procedure[0], BrainInjection))
+        self.assertTrue(isinstance(mapped_procedure[1], BrainInjection))
+        self.assertIsNone(mapper._parse_basic_float_str("one"))
 
 
 if __name__ == "__main__":
     unittest_main()
```

### Comparing `aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.2/tests/sharepoint/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,16 @@
         )
 
         expected_subject_procedures = []
         expected_subject_procedures.extend(self.list_items_2019[0][1])
         expected_subject_procedures.extend(self.list_items_2023[0][1])
         response = client.get_procedure_info(subject_id="12345")
         contents = json.loads(response.body.decode("utf-8"))
+        expected_subject_procedures.sort(key=lambda x: str(x))
+        contents["data"]["subject_procedures"].sort(key=lambda x: str(x))
         self.assertEqual(200, response.status_code)
         self.assertEqual(
             expected_subject_procedures, contents["data"]["subject_procedures"]
         )
 
 
 if __name__ == "__main__":
```

### Comparing `aind_metadata_service-0.4.1/tests/test_client.py` & `aind_metadata_service-0.4.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.1/tests/test_response_handle.py` & `aind_metadata_service-0.4.2/tests/test_response_handle.py`

 * *Files identical despite different names*

