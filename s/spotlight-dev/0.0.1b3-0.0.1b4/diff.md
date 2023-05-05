# Comparing `tmp/spotlight-dev-0.0.1b3.tar.gz` & `tmp/spotlight-dev-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b3.tar", last modified: Thu May  4 15:38:54 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b4.tar", last modified: Fri May  5 18:15:16 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b3.tar` & `spotlight-dev-0.0.1b4.tar`

### file list

```diff
@@ -1,132 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.810874 spotlight-dev-0.0.1b3/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-04 15:38:54.809873 spotlight-dev-0.0.1b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 15:38:54.810874 spotlight-dev-0.0.1b3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.784871 spotlight-dev-0.0.1b3/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.785872 spotlight-dev-0.0.1b3/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.786872 spotlight-dev-0.0.1b3/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.787872 spotlight-dev-0.0.1b3/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.788872 spotlight-dev-0.0.1b3/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.790872 spotlight-dev-0.0.1b3/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.791872 spotlight-dev-0.0.1b3/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.792872 spotlight-dev-0.0.1b3/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.794872 spotlight-dev-0.0.1b3/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.795872 spotlight-dev-0.0.1b3/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.796872 spotlight-dev-0.0.1b3/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.796872 spotlight-dev-0.0.1b3/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.798873 spotlight-dev-0.0.1b3/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.799873 spotlight-dev-0.0.1b3/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.799873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.800873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.801873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.802873 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.804873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.805873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.806873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.807873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.808874 spotlight-dev-0.0.1b3/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2189 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.809873 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3933 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.793636 spotlight-dev-0.0.1b4/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 18:15:16.792636 spotlight-dev-0.0.1b4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:15:16.793636 spotlight-dev-0.0.1b4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.747632 spotlight-dev-0.0.1b4/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.749633 spotlight-dev-0.0.1b4/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.751633 spotlight-dev-0.0.1b4/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.754633 spotlight-dev-0.0.1b4/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.756633 spotlight-dev-0.0.1b4/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.758633 spotlight-dev-0.0.1b4/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.761633 spotlight-dev-0.0.1b4/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.763634 spotlight-dev-0.0.1b4/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.766634 spotlight-dev-0.0.1b4/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.769634 spotlight-dev-0.0.1b4/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.772634 spotlight-dev-0.0.1b4/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.772634 spotlight-dev-0.0.1b4/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.777635 spotlight-dev-0.0.1b4/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.777635 spotlight-dev-0.0.1b4/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.779635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.780635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.782635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.782635 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.783635 spotlight-dev-0.0.1b4/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.785636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.786635 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.787636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.788636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.788636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/
+-rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.789636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.790636 spotlight-dev-0.0.1b4/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.792636 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b3/PKG-INFO` & `spotlight-dev-0.0.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b3/README.md` & `spotlight-dev-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/setup.py` & `spotlight-dev-0.0.1b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b3",
+    version="0.0.1b4",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/job/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b4/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/job/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b4/spotlight/api/rule/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b4/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/tag/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/tag/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b4/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/__init__.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,156 @@
-import logging
-from typing import Optional, List, Any
+from abc import ABC, abstractmethod
+from typing import Any, Optional, List
 
 from spotlight.api.job.model import JobResponse
-from spotlight.core.common.date.function import current_timestamp
-from spotlight.core.pipeline.execution import run_pipeline
-from spotlight.core.pipeline.execution.rule import AbstractRule
+from spotlight.core.pipeline.execution.rule.abstract import AbstractRule
 from spotlight.core.pipeline.model.pipeline import PipelineResult
-
-from spotlight.core.pipeline.utils.asynchronously import (
-    async_start_job,
-    async_stop_job,
+from spotlight.core.pipeline.model.rule import RuleResult
+from spotlight.core.pipeline.runner import (
+    pipeline_runner,
+    async_pipeline_runner,
+    offline_pipeline_runner,
 )
-from spotlight.core.pipeline.utils.synchronously import start_job, stop_job
-
-logger = logging.getLogger(__name__)
 
 
-def __dq_pipeline(
-    data: Any,
-    job_name: str,
-    rules: List[AbstractRule],
-    multi_processing: bool = False,
-    processes: int = 5,
-):
-    start_time = current_timestamp()
-    logger.info(f"Starting data quality pipeline [{job_name=}, {start_time=}]")
-    rule_results = run_pipeline(
-        data, rules, multi_processing=multi_processing, processes=processes
-    )
-    end_time = current_timestamp()
-    result = PipelineResult.build_result(job_name, start_time, end_time, rule_results)
-    logger.debug(f"Data quality pipeline result: {result}")
-    logger.info(
-        f"Data quality pipeline finished [{job_name=}, {end_time=}]: {result.status}"
-    )
-    return result
-
-
-def data_quality_pipeline(
-    data: Any,
-    job_name: str,
-    *,
-    tag_names: Optional[List[str]] = None,
-    tag_ids: Optional[List[str]] = None,
-    additional_rules: Optional[List[AbstractRule]] = None,
-    metadata: Optional[dict] = None,
-    multi_processing: bool = False,
-    processes: int = 5,
-) -> JobResponse:
-    """
-    Runs data through a data quality pipeline.
-
-    NOTE: You must provide the tag names and/or the tag ids for this method to run.
-    NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-    Args:
-        data (Any): Data that is run through the pipeline
-        job_name (str): Name assigned to the job created from running this pipeline
-        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
-        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
-        additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
-        supported in the API i.e. AbstractCustomCodeRules)
-        metadata (Optional[dict]): Metadata added to the job information
-        multi_processing (bool): Optional flag to run the rules over the data concurrently
-        processes (int): Optional number of process to spin up when running the rules concurrently
-
-    Returns:
-        JobResponse: The job response with all the information from the run
-    """
-    job, rules = start_job(
-        job_name=job_name,
-        tag_names=tag_names,
-        tag_ids=tag_ids,
-        metadata=metadata,
-    )
-    rules.extend(additional_rules or [])
-    result = __dq_pipeline(data, job.name, rules, multi_processing, processes)
-
-    job = stop_job(
-        job=job,
-        pipeline_result=result,
-    )
-    return job
-
-
-async def async_data_quality_pipeline(
-    data: Any,
-    job_name: str,
-    *,
-    tag_names: Optional[List[str]] = None,
-    tag_ids: Optional[List[str]] = None,
-    additional_rules: Optional[List[AbstractRule]] = None,
-    metadata: Optional[dict] = None,
-    multi_processing: bool = False,
-    processes: int = 5,
-) -> JobResponse:
-    """
-    Asynchronously runs data through a data quality pipeline.
-
-    NOTE: You must provide the tag names and/or the tag ids for this method to run.
-    NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-    Args:
-        data (Any): Data that is run through the pipeline
-        job_name (str): Name assigned to the job created from running this pipeline
-        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
-        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
-        additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
-        supported in the API i.e. AbstractCustomCodeRules)
-        metadata (Optional[dict]): Metadata added to the job information
-        tags (Optional[List[str]]): Tags added to the job
-        multi_processing (bool): Optional flag to run the rules over the data concurrently
-        processes (int): Optional number of process to spin up when running the rules concurrently
-
-    Returns:
-        JobResponse: The job response with all the information from the run
-    """
-    job, rules = await async_start_job(
-        job_name=job_name,
-        tag_names=tag_names,
-        tag_ids=tag_ids,
-        metadata=metadata,
-    )
-    rules.extend(additional_rules or [])
-    result = __dq_pipeline(data, job.name, rules, multi_processing, processes)
-
-    job = await async_stop_job(
-        job=job,
-        pipeline_result=result,
-    )
-    return job
-
-
-def offline_data_quality_pipeline(
-    job_name: str,
-    data: Any,
-    rules: List[AbstractRule],
-    *,
-    multi_processing: bool = False,
-    processes: int = 5,
-) -> PipelineResult:
-    """
-    Runs data through a data quality pipeline.
-
-    NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results unavailable in
-    the UI
-    NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-    Args:
-        job_name (str): Name for the test job
-        data (Any): Data that is run through the pipeline
-        rules (List[RuleRequest]): A list of the rules to run on the pipeline
-        multi_processing (bool): Optional flag to run the rules over the data concurrently
-        processes (int): Optional number of process to spin up when running the rules concurrently
-
-    Returns:
-        dict: A dict containing the metadata of the test job
-    """
-    result = __dq_pipeline(data, job_name, rules, multi_processing, processes)
-    return result
+class AbstractPipeline(ABC):
+    @classmethod
+    @abstractmethod
+    def apply_rule(cls, data: Any, rule: AbstractRule) -> RuleResult:
+        """
+        This method applies a rule to the data provided
+
+        Args:
+            data (Any): The data associated with the plugin
+            rule (AbstractRule): The rule being run on the data
+
+        Returns:
+            RuleResult: The result of the rule run
+        """
+        pass
+
+    @classmethod
+    def run(
+        cls,
+        data: Any,
+        job_name: str,
+        *,
+        tag_names: Optional[List[str]] = None,
+        tag_ids: Optional[List[str]] = None,
+        additional_rules: Optional[List[AbstractRule]] = None,
+        metadata: Optional[dict] = None,
+        multi_processing: bool = False,
+        processes: int = 5,
+    ) -> JobResponse:
+        """
+        Runs data through the pipeline.
+
+        NOTE: You must provide the tag names and/or the tag ids for this method to run.
+        NOTE: The number of rules run in parallel is dependent on the number of processes.
+
+        Args:
+            data (Any): Data that is run through the pipeline
+            job_name (str): Name assigned to the job created from running this pipeline
+            tag_names (Optional[List[str]]): List of tag names to use with the pipeline
+            tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
+            additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
+            supported in the API i.e. AbstractCustomCodeRules)
+            metadata (Optional[dict]): Metadata added to the job information
+            multi_processing (bool): Optional flag to run the rules over the data concurrently
+            processes (int): Optional number of process to spin up when running the rules concurrently
+
+        Returns:
+            JobResponse: The job response with all the information from the run
+        """
+        return pipeline_runner(
+            data=data,
+            job_name=job_name,
+            apply_rule=cls.apply_rule,
+            tag_names=tag_names,
+            tag_ids=tag_ids,
+            additional_rules=additional_rules,
+            metadata=metadata,
+            multi_processing=multi_processing,
+            processes=processes,
+        )
+
+    @classmethod
+    async def async_run(
+        cls,
+        data: Any,
+        job_name: str,
+        *,
+        tag_names: Optional[List[str]] = None,
+        tag_ids: Optional[List[str]] = None,
+        additional_rules: Optional[List[AbstractRule]] = None,
+        metadata: Optional[dict] = None,
+        multi_processing: bool = False,
+        processes: int = 5,
+    ) -> JobResponse:
+        """
+        Asynchronously runs data through a pipeline.
+
+        NOTE: You must provide the tag names and/or the tag ids for this method to run.
+        NOTE: The number of rules run in parallel is dependent on the number of processes.
+
+        Args:
+            data (Any): Data that is run through the pipeline
+            job_name (str): Name assigned to the job created from running this pipeline
+            tag_names (Optional[List[str]]): List of tag names to use with the pipeline
+            tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
+            additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
+            supported in the API i.e. AbstractCustomCodeRules)
+            metadata (Optional[dict]): Metadata added to the job information
+            multi_processing (bool): Optional flag to run the rules over the data concurrently
+            processes (int): Optional number of process to spin up when running the rules concurrently
+
+        Returns:
+            JobResponse: The job response with all the information from the run
+        """
+        result = await async_pipeline_runner(
+            data=data,
+            job_name=job_name,
+            apply_rule=cls.apply_rule,
+            tag_names=tag_names,
+            tag_ids=tag_ids,
+            additional_rules=additional_rules,
+            metadata=metadata,
+            multi_processing=multi_processing,
+            processes=processes,
+        )
+        return result
+
+    @classmethod
+    def offline_run(
+        cls,
+        job_name: str,
+        data: Any,
+        rules: List[AbstractRule],
+        *,
+        multi_processing: bool = False,
+        processes: int = 5,
+    ) -> PipelineResult:
+        """
+        Runs data through the pipeline.
+
+        NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results
+        unavailable in the UI
+        NOTE: The number of rules run in parallel is dependent on the number of processes.
+
+        Args:
+            job_name (str): Name for the test job
+            data (Any): Data that is run through the pipeline
+            rules (List[RuleRequest]): A list of the rules to run on the pipeline
+            multi_processing (bool): Optional flag to run the rules over the data concurrently
+            processes (int): Optional number of process to spin up when running the rules concurrently
+
+        Returns:
+            PipelineResult: The result of the pipeline
+        """
+        return offline_pipeline_runner(
+            job_name=job_name,
+            data=data,
+            apply_rule=cls.apply_rule,
+            rules=rules,
+            multi_processing=multi_processing,
+            processes=processes,
+        )
```

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/decorator.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,37 @@
-from typing import Union, Callable, Any
-from trycast import isassignable
+from typing import Any, Type
 
-from spotlight.core.pipeline.execution.plugin.abstract import AbstractPlugin
-from spotlight.core.pipeline.execution.plugin.registry import PluginRegistry
+from spotlight.core.pipeline.abstract import AbstractPipeline
+from spotlight.core.pipeline.execution.rule import AbstractRule
+from spotlight.core.pipeline.execution.synchronous import ApplyRule
 from spotlight.core.pipeline.model.rule import RuleResult
 
 
-def plugin(
-    apply_rule: Callable[[Any, Any], RuleResult] = None,
+def pipeline(
+    apply_rule: ApplyRule = None,
     *,
     name: str = "Unnamed",
-    data_type: type = None,
-    register: bool = True
-) -> Union[Callable, Any]:
+) -> Type[AbstractPipeline]:
     """
     This is a decorator to create a plugin from the apply method
 
     Args:
         apply_rule (Callable[[Any, Any], RuleResult]): The apply rule method for a plugin
         name (str): Name of the plugin
-        data_type (type): The data type used with the plugin
-        register (bool): A flag to register a plugin in the PluginRegistry or not
     """
 
     def wrap(fxn):
-        if data_type is None:
-            raise ValueError("Missing data_type")
-
         @classmethod
-        def _apply_rule(cls, data: Any, rule: Any) -> RuleResult:
+        def _apply_rule(cls, data: Any, rule: AbstractRule) -> RuleResult:
             return fxn(data, rule)
 
-        @classmethod
-        def _use_plugin(cls, data: Any) -> bool:
-            return isassignable(data, data_type)
-
-        new_plugin = type(
+        new_pipeline = type(
             name,
-            (AbstractPlugin,),
-            {"apply_rule": _apply_rule, "use_plugin": _use_plugin},
+            (AbstractPipeline,),
+            {"apply_rule": _apply_rule},
         )
-        if register:
-            PluginRegistry.register(new_plugin)
-        return new_plugin
+        return new_pipeline
 
     if apply_rule is None:
         return wrap
 
     return wrap(apply_rule)
```

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/asynchronously.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/synchronously.py` & `spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b4/spotlight/pandas/__util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import List
 
 import pandas as pd
 
 from spotlight.api.rule.model import RuleResponse
 from spotlight.core.common.enum import Severity, Status
-from spotlight.core.pipeline import AbstractRule
+from spotlight.core.pipeline.execution.rule import AbstractRule
 from spotlight.core.pipeline.model.rule import RuleResult
 
 logger = logging.getLogger(__name__)
 
 
 def build_rule_result(
     rule: AbstractRule, start_time: int, end_time: int, result: pd.DataFrame
```

### Comparing `spotlight-dev-0.0.1b3/spotlight/pandas/plugin.py` & `spotlight-dev-0.0.1b4/spotlight/pandas/pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import pandas as pd
 
-from spotlight.core.pipeline.execution.plugin.decorator import plugin
-from spotlight.core.pipeline.execution.rule import SQLRule
-from spotlight.core.pipeline.execution.rule.abstract import (
+from spotlight.core.pipeline.decorator import pipeline
+from spotlight.core.pipeline.execution.rule import (
+    SQLRule,
     AbstractRule,
     AbstractCustomCodeRule,
 )
 from spotlight.core.pipeline.model.rule import RuleResult
 from spotlight.pandas.runners import (
     pandas_sql_rule_runner,
     pandas_custom_code_rule_runner,
 )
 
 logger = logging.getLogger(__name__)
 
 
-@plugin(name="PandasPlugin", data_type=pd.DataFrame)
-def pandas_plugin(data: pd.DataFrame, rule: AbstractRule) -> RuleResult:
+@pipeline(name="PandasPipeline")
+def pandas_pipeline(data: pd.DataFrame, rule: AbstractRule) -> RuleResult:
     """
     This is the plugin interface for running rules on pandas dataframes
 
     Args:
         data (pd.DataFrame): The data being tested
         rule (AbstractRule): The rule being applied to the data
```

### Comparing `spotlight-dev-0.0.1b3/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b4/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b3/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b4/spotlight_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b3/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b4/spotlight_dev.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -71,32 +71,31 @@
 spotlight/core/common/decorators/data/synchronous.py
 spotlight/core/common/metaclass/__init__.py
 spotlight/core/common/metaclass/singleton.py
 spotlight/core/common/requests/__init__.py
 spotlight/core/common/requests/asynchronous.py
 spotlight/core/common/requests/synchronous.py
 spotlight/core/pipeline/__init__.py
+spotlight/core/pipeline/abstract.py
+spotlight/core/pipeline/decorator.py
 spotlight/core/pipeline/execution/__init__.py
 spotlight/core/pipeline/execution/synchronous.py
-spotlight/core/pipeline/execution/plugin/__init__.py
-spotlight/core/pipeline/execution/plugin/abstract.py
-spotlight/core/pipeline/execution/plugin/decorator.py
-spotlight/core/pipeline/execution/plugin/registry.py
 spotlight/core/pipeline/execution/rule/__init__.py
 spotlight/core/pipeline/execution/rule/abstract.py
 spotlight/core/pipeline/execution/rule/enum.py
 spotlight/core/pipeline/execution/rule/sql_rule.py
 spotlight/core/pipeline/model/__init__.py
 spotlight/core/pipeline/model/pipeline.py
 spotlight/core/pipeline/model/rule.py
-spotlight/core/pipeline/utils/__init__.py
-spotlight/core/pipeline/utils/asynchronously.py
-spotlight/core/pipeline/utils/synchronously.py
+spotlight/core/pipeline/runner/__init__.py
+spotlight/core/pipeline/runner/utils/__init__.py
+spotlight/core/pipeline/runner/utils/asynchronously.py
+spotlight/core/pipeline/runner/utils/synchronously.py
 spotlight/pandas/__init__.py
 spotlight/pandas/__util.py
-spotlight/pandas/plugin.py
+spotlight/pandas/pipeline.py
 spotlight/pandas/runners.py
 spotlight_dev.egg-info/PKG-INFO
 spotlight_dev.egg-info/SOURCES.txt
 spotlight_dev.egg-info/dependency_links.txt
 spotlight_dev.egg-info/requires.txt
 spotlight_dev.egg-info/top_level.txt
```

