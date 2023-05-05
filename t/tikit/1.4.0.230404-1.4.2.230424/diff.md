# Comparing `tmp/tikit-1.4.0.230404.tar.gz` & `tmp/tikit-1.4.2.230424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikit-1.4.0.230404.tar", last modified: Thu Apr  6 07:58:57 2023, max compression
+gzip compressed data, was "tikit-1.4.2.230424.tar", last modified: Fri May  5 03:32:35 2023, max compression
```

## Comparing `tikit-1.4.0.230404.tar` & `tikit-1.4.2.230424.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.757740 tikit-1.4.0.230404/
--rw-r--r--   0 suixingmeng   (501) staff       (20)       71 2022-11-29 15:10:36.000000 tikit-1.4.0.230404/MANIFEST.in
--rw-r--r--   0 suixingmeng   (501) staff       (20)      719 2023-04-06 07:58:57.757288 tikit-1.4.0.230404/PKG-INFO
--rw-r--r--   0 suixingmeng   (501) staff       (20)      499 2022-11-29 15:08:20.000000 tikit-1.4.0.230404/README.md
--rw-r--r--   0 suixingmeng   (501) staff       (20)      413 2022-11-29 15:08:20.000000 tikit-1.4.0.230404/requirements.txt
--rw-r--r--   0 suixingmeng   (501) staff       (20)       38 2023-04-06 07:58:57.757885 tikit-1.4.0.230404/setup.cfg
--rw-r--r--   0 suixingmeng   (501) staff       (20)      858 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/setup.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.727462 tikit-1.4.0.230404/tikit/
--rw-r--r--   0 suixingmeng   (501) staff       (20)      185 2023-03-03 03:08:19.000000 tikit-1.4.0.230404/tikit/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     7896 2022-11-29 15:10:36.000000 tikit-1.4.0.230404/tikit/cli.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)   192939 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/client.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     3976 2022-05-27 07:24:46.000000 tikit-1.4.0.230404/tikit/default_client.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.733237 tikit-1.4.0.230404/tikit/display_optimize/
--rw-r--r--   0 suixingmeng   (501) staff       (20)      133 2022-05-27 07:24:46.000000 tikit-1.4.0.230404/tikit/display_optimize/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     3820 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/display_optimize/dataset.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1628 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/display_optimize/resource_group.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     3951 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/display_optimize/training_model.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     4973 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/display_optimize/training_task.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1779 2022-05-27 07:24:46.000000 tikit-1.4.0.230404/tikit/hdfs.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    35661 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/hive.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    18425 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/models.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.733646 tikit-1.4.0.230404/tikit/templates/
--rw-r--r--   0 suixingmeng   (501) staff       (20)     7622 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/templates/service_config.yaml
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.734110 tikit-1.4.0.230404/tikit/tencentcloud/
--rw-r--r--   0 suixingmeng   (501) staff       (20)      630 2022-05-27 07:24:46.000000 tikit-1.4.0.230404/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.737322 tikit-1.4.0.230404/tikit/tencentcloud/common/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-11-22 10:47:38.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    16473 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     2337 2022-11-22 10:47:38.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     2002 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    12338 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.738425 tikit-1.4.0.230404/tikit/tencentcloud/common/exception/
--rw-r--r--   0 suixingmeng   (501) staff       (20)      741 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)      760 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.739207 tikit-1.4.0.230404/tikit/tencentcloud/common/http/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-11-22 10:47:38.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     5071 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.740437 tikit-1.4.0.230404/tikit/tencentcloud/common/profile/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-11-22 10:47:38.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1657 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1857 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1574 2022-11-28 01:57:03.000000 tikit-1.4.0.230404/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.740988 tikit-1.4.0.230404/tikit/tencentcloud/emr/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.742910 tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     6015 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     3465 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    33848 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.743991 tikit-1.4.0.230404/tikit/tencentcloud/tione/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-05-27 07:24:46.000000 tikit-1.4.0.230404/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.749522 tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    12419 2023-03-03 03:07:53.000000 tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)   744538 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)   260703 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.753337 tikit-1.4.0.230404/tikit/tencentcloud/wedata/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.756589 tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 suixingmeng   (501) staff       (20)        0 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)      819 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)    19834 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)     4802 2022-09-06 04:46:01.000000 tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 suixingmeng   (501) staff       (20)      893 2023-04-06 07:57:20.000000 tikit-1.4.0.230404/tikit/util.py
-drwxr-xr-x   0 suixingmeng   (501) staff       (20)        0 2023-04-06 07:58:57.730458 tikit-1.4.0.230404/tikit.egg-info/
--rw-r--r--   0 suixingmeng   (501) staff       (20)      719 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/PKG-INFO
--rw-r--r--   0 suixingmeng   (501) staff       (20)     1883 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 suixingmeng   (501) staff       (20)        1 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 suixingmeng   (501) staff       (20)       41 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/entry_points.txt
--rw-r--r--   0 suixingmeng   (501) staff       (20)      413 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/requires.txt
--rw-r--r--   0 suixingmeng   (501) staff       (20)        6 2023-04-06 07:58:57.000000 tikit-1.4.0.230404/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.167060 tikit-1.4.2.230424/
+-rw-r--r--   0 liuliu     (501) staff       (20)       71 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/MANIFEST.in
+-rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-05 03:32:35.166245 tikit-1.4.2.230424/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)      499 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/README.md
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/requirements.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       38 2023-05-05 03:32:35.167300 tikit-1.4.2.230424/setup.cfg
+-rw-r--r--   0 liuliu     (501) staff       (20)      858 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/setup.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.115871 tikit-1.4.2.230424/tikit/
+-rw-r--r--   0 liuliu     (501) staff       (20)      185 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     7896 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/cli.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   194491 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3976 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/default_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.130488 tikit-1.4.2.230424/tikit/display_optimize/
+-rw-r--r--   0 liuliu     (501) staff       (20)      133 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3820 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/dataset.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1628 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/resource_group.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3951 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/training_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4973 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/training_task.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1779 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/hdfs.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    35661 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/hive.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    19526 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.131709 tikit-1.4.2.230424/tikit/templates/
+-rw-r--r--   0 liuliu     (501) staff       (20)     7622 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/templates/service_config.yaml
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.133098 tikit-1.4.2.230424/tikit/tencentcloud/
+-rw-r--r--   0 liuliu     (501) staff       (20)      630 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.139191 tikit-1.4.2.230424/tikit/tencentcloud/common/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    16473 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2337 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2002 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/common_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12338 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/credential.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.141706 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 liuliu     (501) staff       (20)      741 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      760 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.143927 tikit-1.4.2.230424/tikit/tencentcloud/common/http/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     5071 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/http/request.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.147151 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1657 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1857 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1574 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.148120 tikit-1.4.2.230424/tikit/tencentcloud/emr/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.151420 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     6015 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3465 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    33848 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.153323 tikit-1.4.2.230424/tikit/tencentcloud/tione/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.157770 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12419 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   747496 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   260703 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.160680 tikit-1.4.2.230424/tikit/tencentcloud/wedata/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.165030 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      819 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    19834 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4802 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      893 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/util.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.125569 tikit-1.4.2.230424/tikit.egg-info/
+-rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)     1883 2023-05-05 03:32:35.000000 tikit-1.4.2.230424/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        1 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       40 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/requires.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        6 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/top_level.txt
```

### Comparing `tikit-1.4.0.230404/PKG-INFO` & `tikit-1.4.2.230424/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.0.230404
+Version: 1.4.2.230424
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-Platform: UNKNOWN
 
 TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
 Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
 
 # 发布
 '''bash
 # 公网
@@ -21,8 +20,7 @@
 '''bash
 yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
 pip install -r requirements.txt
 '''
 # 公网
 pip install tikit -U -i https://pypi.org/simple
 '''
-
```

### Comparing `tikit-1.4.0.230404/setup.py` & `tikit-1.4.2.230424/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.4.0.230404',
+    version='1.4.2.230424',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.4.0.230404/tikit/cli.py` & `tikit-1.4.2.230424/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/client.py` & `tikit-1.4.2.230424/tikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,16 @@
                              tuning_parameters_dict={},
                              resource_group_id="",
                              remark=None,
                              log_enable=False,
                              log_logset_id=None,
                              log_topic_id=None,
                              vpc_id=None,
-                             sub_net_id=None):
+                             sub_net_id=None,
+                             enable_rdma=False):
         """创建训练任务
 
         :param name:        任务名称
         :type name:         str
         :param framework:   运行的框架环境
         :type framework:    :class:`tikit.models.FrameworkInfo`
         :param cos_output:          输出的cos信息
@@ -687,14 +688,16 @@
         :type log_logset_id:        str
         :param log_topic_id:        日志的topic id
         :type log_topic_id:         str
         :param vpc_id:              vpc的id
         :type vpc_id:               str
         :param sub_net_id:          子网id
         :type sub_net_id:           str
+        :param enable_rdma:         是否使用 RMDA 网卡，只有机型支持该参数才可生效
+        :type enable_rdma:          bool
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateTrainingTaskResponse`
         """
         try:
             req = models.CreateTrainingTaskRequest()
             req.Name = name
 
@@ -728,25 +731,33 @@
             worker_info.Role = "WORKER"
             worker_info.InstanceNum = worker_resource.InstanceNum
             worker_info.Cpu = worker_resource.Cpu
             worker_info.Memory = worker_resource.Memory
             worker_info.GpuType = worker_resource.GpuType
             worker_info.Gpu = worker_resource.Gpu
             worker_info.InstanceType = worker_resource.InstanceType
+            if enable_rdma:
+                rdma_config = models.RDMAConfig()
+                rdma_config.Enable = enable_rdma
+                worker_info.RDMAConfig = rdma_config
             req.ResourceConfigInfos = [worker_info]
 
             if ps_resource:
                 ps_info = models.ResourceConfigInfo()
                 ps_info.Role = "PS"
                 ps_info.InstanceNum = ps_resource.InstanceNum
                 ps_info.Cpu = ps_resource.Cpu
                 ps_info.Memory = ps_resource.Memory
                 ps_info.GpuType = ps_resource.GpuType
                 ps_info.Gpu = ps_resource.Gpu
                 ps_info.InstanceType = ps_resource.InstanceType
+                if enable_rdma:
+                    rdma_config = models.RDMAConfig()
+                    rdma_config.Enable = enable_rdma
+                    ps_info.RDMAConfig = rdma_config
                 req.ResourceConfigInfos.append(ps_info)
 
             req.Output = self.parse_cos_info(cos_output)
             req.Tags = tags
             req.CodePackagePath = self.parse_cos_info(code_package_path) if code_package_path else None
             req.StartCmdInfo = models.StartCmdInfo()
             req.StartCmdInfo.WorkerStartCmd = worker_start_cmd
@@ -786,14 +797,21 @@
             if input_data_config.DataSource == "COS":
                 for cos_str in input_data_config.DataConfigDict:
                     data_config = models.DataConfig()
                     data_config.DataSourceType = input_data_config.DataSource
                     data_config.MappingPath = input_data_config.DataConfigDict[cos_str]
                     data_config.COSSource = self.parse_cos_info(cos_str)
                     data_configs.append(data_config)
+            if input_data_config.DataSource == "GooseFS":
+                data_config = models.DataConfig()
+                data_config.DataSourceType = input_data_config.DataSource
+                data_config.MappingPath = input_data_config.TargetPath
+                data_config.GooseFSSource = models.GooseFSSource()
+                data_config.GooseFSSource.Id = input_data_config.GooseFSId
+                data_configs.append(data_config)
             return data_configs, input_data_config.DataSource
 
         for input_data_item in input_data_config:
             data_config = models.DataConfig()
             data_config.DataSourceType = input_data_item.DataSource
             data_config.MappingPath = input_data_item.TargetPath
             if input_data_item.DataSource == "COS":
@@ -809,16 +827,25 @@
                 data_config.HDFSSource = models.HDFSConfig()
                 data_config.HDFSSource.Id = input_data_item.HdfsId
                 data_config.HDFSSource.Path = input_data_item.HdfsPath
             elif input_data_item.DataSource == "WEDATA_HDFS":
                 data_config.WeDataHDFSSource = models.WeDataHDFSConfig()
                 data_config.WeDataHDFSSource.Id = input_data_item.WedataId
                 data_config.WeDataHDFSSource.Path = input_data_item.HdfsPath
+            elif input_data_item.DataSource == "AIMarket_Algo_PreModel":
+                data_config.AIMarketAlgoPreModelSource = models.AIMarketAlgoPreModelSource()
+                data_config.AIMarketAlgoPreModelSource.Id = input_data_item.AIMarketAlgoId
+            elif input_data_item.DataSource == "GooseFS":
+                data_config.GooseFSSource = models.GooseFSSource()
+                data_config.GooseFSSource.Id = input_data_item.GooseFSId
+
             data_configs.append(data_config)
             data_type = input_data_item.DataSource
+            if data_type == "AIMarket_Algo_PreModel":
+                data_type = "COS"
         return data_configs, data_type
 
     def stop_training_task(self, task_id):
         """停止某个训练任务
 
         :param task_id: 训练任务ID
         :type task_id: str
```

### Comparing `tikit-1.4.0.230404/tikit/default_client.py` & `tikit-1.4.2.230424/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/display_optimize/dataset.py` & `tikit-1.4.2.230424/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/display_optimize/resource_group.py` & `tikit-1.4.2.230424/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/display_optimize/training_model.py` & `tikit-1.4.2.230424/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/display_optimize/training_task.py` & `tikit-1.4.2.230424/tikit/display_optimize/training_task.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/hdfs.py` & `tikit-1.4.2.230424/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/hive.py` & `tikit-1.4.2.230424/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/models.py` & `tikit-1.4.2.230424/tikit/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,14 +228,16 @@
         self.CosStr = None
         self.DatasetId = None
         self.CfsId = None
         self.CfsPath = None
         self.HdfsId = None
         self.HdfsPath = None
         self.WedataId = None
+        self.AIMarketAlgoId = None
+        self.GooseFSId = None
 
     @staticmethod
     def new_mount_cos(cos_str, target_path):
         """一个cos类型的训练数据
 
         :param cos_str:      cos存储，格式： <bucket>/<cos path>/
         :type cos_str: str
@@ -351,14 +353,48 @@
         :rtype:
         """
         ret = TrainingDataConfig()
         ret.DataSource = "COS"
         ret.DataConfigDict = cos_str_target_dict
         return ret
 
+    @staticmethod
+    def new_ai_market_algo(ai_market_algo_id, target_path):
+        """新建一个wedata hdfs类型的训练数据集配置
+
+        :param ai_market_algo_id: ai市场算法id
+        :type ai_market_algo_id: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = TrainingDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "AIMarket_Algo_PreModel"
+        ret.AIMarketAlgoId = ai_market_algo_id
+        return ret
+
+    @staticmethod
+    def new_mount_goosefs(goosefs_id, target_path):
+        """新建一个goosefs类型的训练数据集配置
+
+        :param goosefs_id: goosefs实例id
+        :type goosefs_id: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = TrainingDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "GooseFS"
+        ret.GooseFSId = goosefs_id
+        return ret
+
 
 class ReasoningEnvironment:
     def __init__(self, source, image_key=None, image_type=None, image_url=None, registry_region=None, registry_id=None):
         self.Source = source
         self.ImageKey = image_key
         self.ImageType = image_type
         self.ImageUrl = image_url
```

### Comparing `tikit-1.4.0.230404/tikit/templates/service_config.yaml` & `tikit-1.4.2.230424/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/__init__.py` & `tikit-1.4.2.230424/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/common_client.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/credential.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/http/request.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/common/sign.py` & `tikit-1.4.2.230424/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3694,22 +3694,30 @@
         :type CFSSource: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
         :param HDFSSource: 来自HDFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type HDFSSource: :class:`tencentcloud.tione.v20211111.models.HDFSConfig`
         :param WeDataHDFSSource: 来自WEDATA_HDFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type WeDataHDFSSource: :class:`tencentcloud.tione.v20211111.models.WeDataHDFSConfig`
+        :param AIMarketAlgoPreModelSource: 来自AIMarket 算法的数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AIMarketAlgoPreModelSource: :class:`tencentcloud.tione.v20211111.models.AIMarketAlgoPreModelSource`
+        :param GooseFSSource: 来自GooseFS的数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GooseFSSource: :class:`tencentcloud.tione.v20211111.models.GooseFSSource`
         """
         self.MappingPath = None
         self.DataSourceType = None
         self.DataSetSource = None
         self.COSSource = None
         self.CFSSource = None
         self.HDFSSource = None
         self.WeDataHDFSSource = None
+        self.AIMarketAlgoPreModelSource = None
+        self.GooseFSSource = None
 
 
     def _deserialize(self, params):
         self.MappingPath = params.get("MappingPath")
         self.DataSourceType = params.get("DataSourceType")
         if params.get("DataSetSource") is not None:
             self.DataSetSource = DataSetConfig()
@@ -3722,14 +3730,20 @@
             self.CFSSource._deserialize(params.get("CFSSource"))
         if params.get("HDFSSource") is not None:
             self.HDFSSource = HDFSConfig()
             self.HDFSSource._deserialize(params.get("HDFSSource"))
         if params.get("WeDataHDFSSource") is not None:
             self.WeDataHDFSSource = WeDataHDFSConfig()
             self.WeDataHDFSSource._deserialize(params.get("WeDataHDFSSource"))
+        if params.get("AIMarketAlgoPreModelSource") is not None:
+            self.AIMarketAlgoPreModelSource = AIMarketAlgoPreModelSource()
+            self.AIMarketAlgoPreModelSource._deserialize(params.get("AIMarketAlgoPreModelSource"))
+        if params.get("GooseFSSource") is not None:
+            self.GooseFSSource = GooseFSSource()
+            self.GooseFSSource._deserialize(params.get("GooseFSSource"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17524,42 +17538,68 @@
 8C80G V100*2 
 32C160G V100*4
 72C320G V100*8
 32C128G T4*1 
 40C160G T4*2 
 80C32
         :type InstanceTypeAlias: str
+        :param RDMAConfig: RDMA配置
+        :type RDMAConfig: class:`tencentcloud.tione.v20211111.models.RDMAConfig`
         """
         self.Role = None
         self.Cpu = None
         self.Memory = None
         self.GpuType = None
         self.Gpu = None
         self.InstanceType = None
         self.InstanceNum = None
         self.InstanceTypeAlias = None
+        self.RDMAConfig = None
 
 
     def _deserialize(self, params):
         self.Role = params.get("Role")
         self.Cpu = params.get("Cpu")
         self.Memory = params.get("Memory")
         self.GpuType = params.get("GpuType")
         self.Gpu = params.get("Gpu")
         self.InstanceType = params.get("InstanceType")
         self.InstanceNum = params.get("InstanceNum")
         self.InstanceTypeAlias = params.get("InstanceTypeAlias")
+        if params.get("RDMAConfig") is not None:
+            self.RDMAConfig = RDMAConfig()
+            self.RDMAConfig._deserialize(params.get("RDMAConfig"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
+class RDMAConfig(AbstractModel):
+    """RDMA配置
+    """
+    
+    def __init__(self):
+        r"""
+        :param Enable: 是否使用 RMDA 网卡
+        :type Enable: bool
+        """
+        self.Enable = None
+
+    def _deserialize(self, params):
+        self.Enable = params.get("Enable")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 class ResourceGroup(AbstractModel):
     """资源组
 
     """
 
     def __init__(self):
@@ -21044,15 +21084,60 @@
         self.Path = params.get("Path")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+
+
+class AIMarketAlgoPreModelSource(AbstractModel):
+    """AIMarketAlgo的配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: AIMarketAlgo的ID
+        :type Id: string
+        """
+        self.Id = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
+class GooseFSSource(AbstractModel):
+    """GooseFS的配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: GooseFS实例的ID
+        :type Id: string
+        """
+        self.Id = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
 
 class WeightEntry(AbstractModel):
     """服务版本的权重
 
     """
```

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit/util.py` & `tikit-1.4.2.230424/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.0.230404/tikit.egg-info/PKG-INFO` & `tikit-1.4.2.230424/tikit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.0.230404
+Version: 1.4.2.230424
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-Platform: UNKNOWN
 
 TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
 Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
 
 # 发布
 '''bash
 # 公网
@@ -21,8 +20,7 @@
 '''bash
 yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
 pip install -r requirements.txt
 '''
 # 公网
 pip install tikit -U -i https://pypi.org/simple
 '''
-
```

### Comparing `tikit-1.4.0.230404/tikit.egg-info/SOURCES.txt` & `tikit-1.4.2.230424/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

