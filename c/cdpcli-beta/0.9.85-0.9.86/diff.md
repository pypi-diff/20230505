# Comparing `tmp/cdpcli-beta-0.9.85.tar.gz` & `tmp/cdpcli-beta-0.9.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.85.tar", last modified: Thu Apr 20 20:39:30 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.86.tar", last modified: Fri May  5 02:26:28 2023, max compression
```

## Comparing `cdpcli-beta-0.9.85.tar` & `cdpcli-beta-0.9.86.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-04-20 20:39:27.000000 cdpcli-beta-0.9.85/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    95434 2023-04-20 20:39:27.000000 cdpcli-beta-0.9.85/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   142870 2023-04-20 20:39:29.000000 cdpcli-beta-0.9.85/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   102900 2023-04-20 20:39:28.000000 cdpcli-beta-0.9.85/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31579 2023-04-20 20:39:29.000000 cdpcli-beta-0.9.85/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-04-20 20:39:28.000000 cdpcli-beta-0.9.85/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.771835 cdpcli-beta-0.9.85/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-04-20 20:39:29.000000 cdpcli-beta-0.9.85/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-04-20 20:39:28.000000 cdpcli-beta-0.9.85/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   177884 2023-04-20 20:39:27.000000 cdpcli-beta-0.9.85/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   175988 2023-04-20 20:39:26.000000 cdpcli-beta-0.9.85/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-04-20 20:39:28.000000 cdpcli-beta-0.9.85/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-04-20 20:39:27.000000 cdpcli-beta-0.9.85/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56974 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    72055 2023-04-20 20:39:29.000000 cdpcli-beta-0.9.85/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30891 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.763836 cdpcli-beta-0.9.85/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.775836 cdpcli-beta-0.9.85/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.779836 cdpcli-beta-0.9.85/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.779836 cdpcli-beta-0.9.85/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.779836 cdpcli-beta-0.9.85/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.779836 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-04-20 20:39:30.000000 cdpcli-beta-0.9.85/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.767835 cdpcli-beta-0.9.85/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:39:30.783836 cdpcli-beta-0.9.85/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-04-20 20:29:49.000000 cdpcli-beta-0.9.85/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.294208 cdpcli-beta-0.9.86/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-05-05 02:26:28.294208 cdpcli-beta-0.9.86/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-05-05 02:26:23.000000 cdpcli-beta-0.9.86/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   142870 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   102900 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31579 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193567 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   175988 2023-05-05 02:26:23.000000 cdpcli-beta-0.9.86/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    72346 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.270208 cdpcli-beta-0.9.86/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.270208 cdpcli-beta-0.9.86/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/versioneer.py
```

### Comparing `cdpcli-beta-0.9.85/LICENSE.txt` & `cdpcli-beta-0.9.86/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.86/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/PKG-INFO` & `cdpcli-beta-0.9.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.85
+Version: 0.9.86
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.85/README.md` & `cdpcli-beta-0.9.86/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/__init__.py` & `cdpcli-beta-0.9.86/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/argparser.py` & `cdpcli-beta-0.9.86/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/argprocess.py` & `cdpcli-beta-0.9.86/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/arguments.py` & `cdpcli-beta-0.9.86/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/auth.py` & `cdpcli-beta-0.9.86/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.86/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/clicommand.py` & `cdpcli-beta-0.9.86/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/clidriver.py` & `cdpcli-beta-0.9.86/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/client.py` & `cdpcli-beta-0.9.86/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/compat.py` & `cdpcli-beta-0.9.86/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/completer.py` & `cdpcli-beta-0.9.86/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/config.py` & `cdpcli-beta-0.9.86/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/configloader.py` & `cdpcli-beta-0.9.86/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/credentials.py` & `cdpcli-beta-0.9.86/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.86/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/cli.json` & `cdpcli-beta-0.9.86/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -474,15 +474,15 @@
             $ref: '#/definitions/Error'
       x-mutating: true
   /api/v1/compute/upgradeDeployment:
     post:
       summary: Upgrades a deployment to a different chart.
       description: Upgrades a deployment to a different chart.
       operationId: upgradeDeployment
-      x-entitlement: COMPUTE_API_LIFTIE_DEPLOYMENT
+      x-entitlement: COMPUTE_API_LIFTIE
       parameters:
         - name: input
           in: body
           required: true
           schema:
             $ref: '#/definitions/UpgradeDeploymentRequest'
       responses:
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/dw/dw.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -367,14 +367,58 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/UpgradeClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/dw/backupCluster:
+    post:
+      x-mutating: true
+      x-no-compatibility-guarantee: true
+      summary: Creates a backup from the cluster configuration and settings.
+      description: Creates a backup from the configuration and settings, including all the connected DbCatalogs, Virtual Warehouses and Data Visualisation Apps. The returned data may be used to restore all the entities by using the "restore-cluster" command.
+      operationId: backupCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/BackupClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/BackupClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/restoreCluster:
+    post:
+      x-mutating: true
+      x-no-compatibility-guarantee: true
+      summary: Restores the cluster from a backup data made by "backup-cluster" command.
+      description: Restores the cluster from a backup data made by "backup-cluster" command. The operation restores the default DbCatalog configuration, the Virtual Warehouses and the Data Visualisation Apps.
+      operationId: restoreCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/RestoreClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/RestoreClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/createDataVisualization:
     post:
       summary: Creates a Cloudera Data Visualization.
       description: Creates a Cloudera Data Visualization.
       operationId: createDataVisualization
       parameters:
         - name: input
@@ -666,14 +710,56 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/RestartDbcResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/dw/describeDbcConfig:
+    post:
+      x-mutating: false
+      summary: Describes the Database Catalog current configuration.
+      description: Describes the Database Catalog current configuration.
+      operationId: describeDbcConfig
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/DescribeDbcConfigRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/DescribeDbcConfigResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/updateDbcConfig:
+    post:
+      x-mutating: true
+      summary: Update a Database Catalog configuration.
+      description: Update a Database Catalog configuration.
+      operationId: updateDbcConfig
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateDbcConfigRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateDbcConfigResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/createDbcDiagnosticDataJob:
     post:
       x-mutating: true
       x-form-factors: public
       summary: Create a diagnostic job for the given database catalog.
       description: Creates a diagnostic job for the given database catalog. The diagnostic data job is useful for troubleshooting purposes. The job collects logs and metrics (see --download-options to see available options) which are going to be bundled into a single file and will be available at the desired location (see --destination). General metadata about the diagnostics will also be included as the bundle-info.json file.
       operationId: createDbcDiagnosticDataJob
@@ -842,14 +928,35 @@
           schema:
             $ref: '#/definitions/DescribeVwResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: false
+  /api/v1/dw/updateVwConfig:
+    post:
+      x-mutating: true
+      summary: Update a Virtual Warehouse configuration.
+      description: Update a Virtual Warehouse configuration.
+      operationId: updateVwConfig
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateVwConfigRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateVwConfigResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/deleteVw:
     post:
       x-no-compatibility-guarantee: true
       x-mutating: true
       summary: Delete a Virtual Warehouse.
       description: Delete a Virtual Warehouse.
       operationId: deleteVw
@@ -910,16 +1017,16 @@
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
   /api/v1/dw/startVw:
     post:
       x-mutating: true
-      summary: Starts a paused Virtual Warehouse.
-      description: Starts a paused Virtual Warehouse. Has no effect if the VW is already started.
+      summary: Starts a suspended Virtual Warehouse.
+      description: Starts a suspended Virtual Warehouse. Has no effect if the VW is already started.
       operationId: startVw
       parameters:
         - name: input
           in: body
           required: true
           schema:
             $ref: '#/definitions/StartVwRequest'
@@ -928,36 +1035,14 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/StartVwResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/dw/pauseVw:
-    post:
-      x-deprecated: true
-      x-mutating: true
-      summary: Pauses a running Virtual Warehouse.
-      description: DEPRECATED in favor of suspend-vw command. Pauses a running Virtual Warehouse. Has no effect if the VW is already paused.
-      operationId: pauseVw
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/PauseVwRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/PauseVwResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
   /api/v1/dw/suspendVw:
     post:
       x-mutating: true
       summary: Suspends a running Virtual Warehouse.
       description: Suspends a running Virtual Warehouse. Has no effect if the VW is already suspended.
       operationId: suspendVw
       parameters:
@@ -1103,14 +1188,35 @@
           description: successful operation
           schema:
             $ref: '#/definitions/ListLatestVersionsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/dw/describeVwConfig:
+    post:
+      x-mutating: false
+      summary: Describes the current configuration of a Hive or Impala Virtual Warehouse.
+      description: Describes the current configuration of a Hive or Impala Virtual Warehouse.
+      operationId: describeVwConfig
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/DescribeVwConfigRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/DescribeVwConfigResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/describeConfig:
     post:
       x-no-compatibility-guarantee: true
       x-mutating: false
       summary: Describe a service configuration.
       description: Describe a service configuration.
       operationId: describeConfig
@@ -1804,16 +1910,27 @@
         description: Using an overlay network will save IP addresses in the VPC by using a private IP address range for Pods in the cluster.
       databaseBackupRetentionPeriod:
         type: integer
         format: int32
         default: 30
         description: PostgreSQL server backup retention days.
       whitelistIpCIDRs:
+        x-form-factors: public,private
         type: string
-        description: Comma separated list of IP address CIDRs to whitelist.
+        description: This field is still available for Private Cloud deployments, however it'll be removed for Public Cloud in the next DWX release. Please use the use 'whitelistK8sClusterAccessIpCIDRs' in combination of 'whitelistWorkloadAccessIpCIDRs' on Public Cloud. Comma separated list of IP address CIDRs to whitelist.
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
       usePrivateLoadBalancer:
         type: boolean
         description: Set up load balancer with private IP address. In AWS it is created in private subnets. In Azure an internal load balancer gets created. Make sure there is connectivity between your client network and the network (VPC/VNet) where CDW environment is deployed.
       enableStorageRoles:
         type: boolean
         description: Enable Storage Roles
         default: false
@@ -1830,20 +1947,104 @@
         description: Options for activating an Azure environment.
         $ref: '#/definitions/AzureActivationOptions'
         x-form-factors: public
       privateCloudOptions:
         description: Options for activating a Private Cloud environment.
         $ref: '#/definitions/PrivateCloudActivationOptions'
         x-form-factors: private
-      customId:
-        type: string
-        description: Custom environment ID provided to the cluster
       customSubdomain:
         type: string
         description: Custom environment subdomain. Overrides the environment subdomain using a customized domain either in the old subdomain format like ENV_ID.dw or the new format like dw-ENV_NAME.
+  BackupClusterRequest:
+    type: object
+    description: Request object for the backupCluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster.
+  BackupClusterResponse:
+    type: object
+    description: Response object for the backupCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster.
+      timestamp:
+        type: string
+        format: date-time
+        description: The date of the creation.
+      data:
+        x-sensitive: true
+        type: string
+        description: The backup data.
+      md5:
+        x-sensitive: true
+        type: string
+        description: The md5 hash of the encoded data.
+  RestoreClusterRequest:
+    type: object
+    description: Request object for the restoreCluster method.
+    required:
+      - clusterId
+      - data
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster.
+      data:
+        type: string
+        description: Dump of configuration received by calling "dump-cluster" command.
+  RestoreClusterResponse:
+    type: object
+    description: Response object for the restoreCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: The the ID of the cluster.
+      operationId:
+        type: string
+        description: The the ID of the restore operation.
+      dbcRestorePlans:
+        type: array
+        description: Information about the restore-plan of the DbCatalogs.
+        items:
+          $ref: '#/definitions/RestoreClusterEntityPlan'
+      hiveRestorePlans:
+        type: array
+        description: Information about the restore-plan of the Hive Virtual Warehouses.
+        items:
+          $ref: '#/definitions/RestoreClusterEntityPlan'
+      impalaRestorePlans:
+        type: array
+        description: Information about the restore-plan of the Impala Virtual Warehouses.
+        items:
+          $ref: '#/definitions/RestoreClusterEntityPlan'
+      vizRestorePlans:
+        type: array
+        description: Information about the restore-plan of the Data Visualization Apps.
+        items:
+          $ref: '#/definitions/RestoreClusterEntityPlan'
+  RestoreClusterEntityPlan:
+    type: object
+    description: Entity status after the restore operation.
+    properties:
+      ref:
+        type: string
+        description: The reference of the entity in the backup data.
+      id:
+        type: string
+        description: The ID of the entity.
+      action:
+        type: string
+        description: 'The action associated with the plan. Possible actions: Create, Update, Skip'
+      message:
+        type: string
+        description: The description of the plan.
   CustomRegistryOptions:
     type: object
     description: Options for custom ACR, ECR, or Docker registry.
     properties:
       registryType:
         enum:
           - ACR
@@ -1874,14 +2075,24 @@
         items:
           type: string
       publicSubnetIds:
         type: array
         description: IDs of public AWS subnets where the cluster should be deployed.
         items:
           type: string
+      workerSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster worker nodes should be deployed.
+        items:
+          type: string
+      lbSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster load balancer should be deployed.
+        items:
+          type: string
       customAmiId:
         type: string
         description: Custom AMI ID.
       nodeRoleCDWManagedPolicyArn:
         type: string
         description: Managed Policy Arn to be attached to the Node Instance Role.
       enableSpotInstances:
@@ -1901,14 +2112,17 @@
         items:
           type: string
         description: Additional (fallback) instance types listed in their priority order. They will be used instead of the primary compute instance type in case it is unavailable. You cannot include any instance type that was already indicated in computeInstanceTypes. Use describe-allowed-instance-types to see currently supported values and also the default value when nothing is provided for the computeInstanceTypes.
   AzureActivationOptions:
     type: object
     description: Options for activating an Azure environment.
     properties:
+      userAssignedManagedIdentity:
+        type: string
+        description: Resource ID of the managed identity used by AKS. It is a mandatory parameter for Azure cluster creation.
       subnetId:
         type: string
         description: ID of Azure subnet where the cluster should be deployed.
       enableAZ:
         type: boolean
         description: Enables Azure Availability Zones for the cluster deployment.
       enableSpotInstances:
@@ -1919,17 +2133,14 @@
         type: array
         items:
           type: string
         description: Azure compute instance types that the environment is restricted to use. This affects the creation of virtual warehouses where this restriction will apply. Select an instance type that meets your computing, memory, networking, or storage needs. As of now, only a single instance type can be listed. Use describe-allowed-instance-types to see currently possible values and the default value used for the case it is not provided.
       logAnalyticsWorkspaceId:
         type: string
         description: Enable monitoring of Azure Kubernetes Service (AKS) cluster. Workspace ID for Azure log analytics.
-      dockerBridgeCidr:
-        type: string
-        description: Docker bridge CIDR range for deployment.
       outboundType:
         type: string
         description: Network outbound type. This setting controls the egress traffic for cluster nodes in Azure Kubernetes Service. Please refer to the following AKS documentation on the Azure portal. https://learn.microsoft.com/en-us/azure/aks/egress-outboundtype, https://learn.microsoft.com/en-us/azure/aks/nat-gateway
         enum:
           - LoadBalancer
           - UserAssignedNATGateway
           - UserDefinedRouting
@@ -1941,16 +2152,17 @@
         type: string
         description: Private DNS zone AKS resource ID.
       enablePrivateAks:
         type: boolean
         description: Enable Azure Private AKS mode.
         default: false
       enableUptimeSLA:
+        x-deprecated: true
         type: boolean
-        description: Enable uptime SLA for Kubernetes API server.
+        description: Enable uptime SLA for Kubernetes API server. This option is deprecated and will be removed upon the next release of the DWX Public Cloud. The uptime SLA for the Kubernetes API server will be always enabled.
         default: false
   PrivateCloudActivationOptions:
     type: object
     description: Options for activating a Private Cloud environment.
     required:
       - delegationUsername
       - delegationPassword
@@ -2030,18 +2242,29 @@
       clusterId:
         type: string
         description: The ID of the cluster to update.
       description:
         type: string
         description: Cluster description.
       whitelistIpCIDRs:
+        x-form-factors: public,private
         type: array
         items:
           type: string
         description: 'List of IP address CIDRs to whitelist. NOTE: CDW is in process of rolling out a new feature to whitelist IP CIDR separately for Kubernetes Clusters and Loadbalancers on CDP Public Cloud. For an existing cluster, if different IP CIDR has been already applied to LoadBalancer and the Kubernetes cluster through the DWX UI, then updating the IP CIDR of such cluster is not supported from CLI. In the upcoming release, the CLI will support this feature. Please make use of UI for the same.'
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
       awsUpdate:
         type: object
         description: Additional properties for AWS clusters.
         properties:
           externalBuckets:
             type: object
             description: External bucket definition.
@@ -2052,14 +2275,24 @@
         type: object
         description: Additional properties for Azure clusters.
         properties:
           renewCertificate:
             type: boolean
             default: false
             description: Renew Azure cluster certificate.
+      observabilityConfig:
+        type: object
+        description: Update the cluster observability configurations. You can forward logs from environments activated in Cloudera Data Warehouse (CDW) to observability and monitoring systems such as Datadog, New Relic, or Splun. Please refer to the following Cloudera documentation for more info. https://docs.cloudera.com/data-warehouse/cloud/monitoring/topics/dw-observability-log-forwarding.html
+        properties:
+          logsForwardingConfig:
+            type: string
+            description: Create the log forwarding configuration in a valid fluentd format. Then that configuration is later inserted into a larger fluentd configuration.
+          proxyCABundle:
+            type: string
+            description: Set the proxy CA certificates (PEM Bundle). If you use a TLS-terminating proxy server to inspect outbound internet traffic, you need to provide the proxy server's CA certificates bundle in PEM bundle format when you configure log forwarding.
   ExternalBucketAccessInfo:
     type: object
     description: External bucket definition.
     properties:
       accessMode:
         type: string
         description: Specifies whether the external bucket will be added in read-only or read-write mode.
@@ -3224,14 +3457,18 @@
         description: Query isolation settings for the Virtual Warehouse. For Impala this value will be considered only if Unified Analytics is enabled.
         $ref: '#/definitions/QueryIsolationOptionsRequest'
       tags:
         type: array
         description: Tags associated with the resources.
         items:
           $ref: '#/definitions/TagRequest'
+      platformJwtAuth:
+        type: boolean
+        default: false
+        description: Value of 'true' automatically configures the Virtual Warehouse to support JWTs issues by the CDP JWT token provider.  Value of 'false' does not enable JWT auth on the Virtual Warehouse.  If this field is not specified, it defaults to 'false'.
   TagRequest:
     description: A key/value pair that can be attached to some resources.
     type: object
     required:
       - key
       - value
     properties:
@@ -3301,14 +3538,55 @@
   DescribeVwResponse:
     type: object
     description: Response object for the describeVw method.
     properties:
       vw:
         description: The Virtual Warehouse.
         $ref: '#/definitions/VwSummary'
+  UpdateVwConfigRequest:
+    type: object
+    description: Request object for the updateVwConfig method.
+    required:
+      - clusterId
+      - vwId
+      - component
+    properties:
+      clusterId:
+        type: string
+        description: ID of the cluster.
+      vwId:
+        type: string
+        description: ID of the Virtual Warehouse.
+      component:
+        type: string
+        description: Configuration component to update. Hive components are [DasWebapp, Hiveserver2, QueryCoordinator, QueryExecutor, StandaloneQueryExecutor, TokenAuth, Hue]. Impala components are [Hue, ImpalaAutoscaler, ImpalaCatalogd, ImpalaCoordinator, ImpalaExecutor, ImpalaProxy, ImpalaStatestored, ImpalaTokenAuth].
+        enum:
+          - DasWebapp
+          - Hiveserver2
+          - QueryCoordinator
+          - QueryExecutor
+          - StandaloneQueryExecutor
+          - TokenAuth
+          - Hue
+          - ImpalaAutoscaler
+          - ImpalaCatalogd
+          - ImpalaCoordinator
+          - ImpalaExecutor
+          - ImpalaProxy
+          - ImpalaStatestored
+          - ImpalaTokenAuth
+      set:
+        description: Configuration files of the selected component to update.
+        type: array
+        items:
+          type: object
+          $ref: '#/definitions/ConfigBlock'
+  UpdateVwConfigResponse:
+    type: object
+    description: Response object for the updateVwConfig method.
   RebuildVwRequest:
     type: object
     description: Request object for the rebuildVw method.
     required:
       - clusterId
       - vwId
     properties:
@@ -3361,14 +3639,24 @@
     description: Response object of the cluster AWS settings.
     properties:
       subnetIds:
         type: array
         description: IDs of AWS subnets where the cluster has been deployed.
         items:
           type: string
+      workerSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster worker nodes should be deployed.
+        items:
+          type: string
+      lbSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster load balancer should be deployed.
+        items:
+          type: string
       availabilityZones:
         type: array
         items:
           type: string
         description: List of availability zones that the cluster is restricted to use.
       customAmiId:
         type: string
@@ -3880,14 +4168,51 @@
             description: Command to use impala-shell for Impala Virtual Warehouses.
           hue:
             type: string
             description: URL of Hue for both Hive and Impala Virtual Warehouses.
           das:
             type: string
             description: URL of Data Analytics Studio for Hive Virtual Warehouses.
+          hostname:
+            type: string
+            description: Hostname for clients to use when connecting to the VW.
+          port:
+            type: integer
+            format: int32
+            description: Port for clients to use when connecting to the VW.
+          jwtConnectionString:
+            type: string
+            description: Generic semi-colon delimited list of key-value pairs that contain all necessary information for clients to construct a connection to this Virtual Warehouse using JWTs as the authentication method.
+          jwtTokenGenUrl:
+            type: string
+            description: When platform JWT authentication is enabled, contains a URL where a JWT token can be generated by the CDP JWT token provider.
+      supportedAuthMethods:
+        type: object
+        description: Describes which authentication methods are supported on this Virtual Warehouse.
+        required:
+          - ldap
+          - jwt
+          - sso
+        properties:
+          ldap:
+            type: boolean
+            description: Indicates if username/password access to this Virtual Warehouse is supported.
+          jwt:
+            type: boolean
+            description: Indicates if JWT auth is supported on this Virtual Warehouse.
+          sso:
+            type: boolean
+            description: Indicates if SSO auth is supported on this Virtual Warehouse.
+      jwtAuth:
+        type: object
+        description: Details related to JWT Authentication settings on this Virtual Warehouse.
+        properties:
+          provider:
+            type: string
+            description: If JWT auth is enabled on the Virtual Warehouse, describes the type of provider.  If set to "CDP", then the CDP JWT auth provider is configured.  If set to "CUSTOM", then another JWT provider is configured.  If empty or missing, then JWT auth is not enabled on this Virtual Warehouse.
       tags:
         type: array
         description: Tags associated with the resources.
         items:
           $ref: '#/definitions/TagResponse'
       compactor:
         type: boolean
@@ -3923,14 +4248,101 @@
     properties:
       key:
         type: string
         description: The tag's name.
       value:
         type: string
         description: The associated value of the tag.
+  DescribeDbcConfigRequest:
+    type: object
+    description: Request object for the describeDbcConfig method.
+    required:
+      - clusterId
+      - dbcId
+    properties:
+      clusterId:
+        type: string
+        description: ID of the cluster.
+      dbcId:
+        type: string
+        description: ID of the Database Catalog.
+  DescribeDbcConfigResponse:
+    type: object
+    description: Response object for the describeDbcConfig method.
+    properties:
+      config:
+        description: The Database Catalog configuration.
+        $ref: '#/definitions/ServiceConfigResp'
+  UpdateDbcConfigRequest:
+    type: object
+    description: Request object for the updateDbcConfig method.
+    required:
+      - clusterId
+      - dbcId
+      - component
+    properties:
+      clusterId:
+        type: string
+        description: ID of the cluster.
+      dbcId:
+        type: string
+        description: ID of the Database Catalog.
+      component:
+        type: string
+        description: Database Catalog configuration component to update.
+        enum:
+          - DasEventProcessor
+          - DatabusProducer
+          - HueQueryProcessor
+          - Metastore
+      set:
+        description: Configuration files of the selected component to update.
+        type: array
+        items:
+          type: object
+          $ref: '#/definitions/ConfigBlock'
+  ConfigBlock:
+    type: object
+    description: Set values for a configuration file of a service.
+    properties:
+      configFile:
+        type: string
+        x-no-param-file: true
+        description: Configuration file to update.
+      keyValue:
+        type: object
+        description: Set values for key-value format configuration file e.g. ENV, PROPERTIES, FLAGFILE, HADOOP_XML typed file.
+        additionalProperties:
+          type: string
+      content:
+        description: Set values for text format configuration file e.g. TEXT, JSON, YAML, XML typed file.
+        type: string
+  UpdateDbcConfigResponse:
+    type: object
+    description: Response object for the updateDbcConfig method.
+  DescribeVwConfigRequest:
+    type: object
+    description: Request object for the describeVwConfig method.
+    required:
+      - clusterId
+      - vwId
+    properties:
+      clusterId:
+        type: string
+        description: ID of the cluster.
+      vwId:
+        type: string
+        description: ID of the Virtual Warehouse.
+  DescribeVwConfigResponse:
+    type: object
+    description: Response object for the describeVwConfig method.
+    properties:
+      config:
+        description: The Virtual Warehouse configuration.
+        $ref: '#/definitions/ServiceConfigResp'
   DescribeConfigRequest:
     type: object
     description: Request object for the describeConfig method.
     required:
       - clusterId
       - configId
     properties:
@@ -4036,14 +4448,18 @@
         $ref: '#/definitions/AutoscalingOptionsUpdateRequest'
       impalaHaSettings:
         description: High Availability settings update for the Impala Virtual Warehouse.
         $ref: '#/definitions/ImpalaHASettingsUpdateRequest'
       queryIsolationOptions:
         description: Query isolation settings for Hive Virtual Warehouses.
         $ref: '#/definitions/QueryIsolationOptionsRequest'
+      platformJwtAuth:
+        type: boolean
+        x-nullable: true
+        description: Value of 'true' automatically configures the Virtual Warehouse to support JWTs issues by the CDP JWT token provider.  Value of 'false' does not enable JWT auth on the Virtual Warehouse.  If this field is not specified, it defaults to 'false'.
   UpdateVwResponse:
     type: object
     description: Response object for the updateVw method.
   UpdateDbcRequest:
     type: object
     description: Request object for the updateDbc method.
     required:
@@ -4355,30 +4771,14 @@
         description: The ID of the Virtual Warehouse cluster.
       vwId:
         type: string
         description: The ID of the Virtual Warehouse.
   StartVwResponse:
     type: object
     description: The response object for the startVw method.
-  PauseVwRequest:
-    type: object
-    description: The request object for the pauseVw method.
-    required:
-      - clusterId
-      - vwId
-    properties:
-      clusterId:
-        type: string
-        description: The ID of the Virtual Warehouse cluster.
-      vwId:
-        type: string
-        description: The ID of the Virtual Warehouse.
-  PauseVwResponse:
-    type: object
-    description: The response object for the pauseVw method.
   SuspendVwRequest:
     type: object
     description: The request object for the suspendVw method.
     required:
       - clusterId
       - vwId
     properties:
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/ml/ml.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -917,17 +917,14 @@
     description: List of possible Outbound types.
     enum:
       - UNKNOWN
       - OUTBOUND_TYPE_UDR
   RestoreWorkspaceRequest:
     type: object
     description: Request object for RestoreWorkspace method.
-    required:
-      - newWorkspaceParameters
-      - backupCrn
     properties:
       newWorkspaceParameters:
         description: The parameters required for a new Cloudera Machine Learning workspace.
         $ref: '#/definitions/CreateWorkspaceRequest'
       backupCrn:
         type: string
         description: The CRN of the backup snapshot to used for restoring.
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -837,14 +837,17 @@
         description: The desired number of strong meta servers for this database. A positive, non-zero number is required. Use removeStrongMetaServers to remove strong meta servers entirely. Requires the COD_STRONG_META_SERVERS entitlement.
       removeStrongMetaServers:
         type: boolean
         description: Removes any strong meta servers provisioned for this database. Requires the COD_STRONG_META_SERVERS entitlement.
       catalog:
         type: string
         description: Catalog name for the image.
+      verticalScale:
+        description: Vertical Scale request for database.
+        $ref: '#/definitions/GroupType'
   AutoScalingParameters:
     type: object
     description: A Parameters to configure AutoScaling
     properties:
       targetedValueForMetric:
         type: integer
         format: int64
@@ -1698,17 +1701,14 @@
         description: Available connectors for this database
       kerberosConfiguration:
         description: Kerberos configuration information
         $ref: '#/definitions/KerberosConfiguration'
   UpgradeDatabaseRequest:
     type: object
     description: Asynchronous request to upgrade the CDP Runtime for a database.
-    required:
-      - environment
-      - database
     properties:
       environment:
         type: string
         description: The name or CRN of the environment.
       database:
         type: string
         description: The name or CRN of the database.
@@ -2198,8 +2198,14 @@
         type: string
         description: The name or CRN of the database.
       edgeNodes:
         type: array
         items:
           $ref: '#/definitions/EdgeNode'
         description: The list of edge nodes for a database.
+  GroupType:
+    type: string
+    description: "Group type for the database nodes.\n `GATEWAY` - GATEWAY value of the Group variable. `MASTER` - MASTER value of the Group variable."
+    enum:
+      - GATEWAY
+      - MASTER
 x-audit: true
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.85
+  version: 0.9.86
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -749,14 +749,15 @@
         description: Custom replication properties.
         type: object
         additionalProperties:
           type: string
       plugins:
         description: Plugins.
         type: array
+        x-default: null
         items:
           type: string
       nextRun:
         description: Next expected run of the policy.
         type: string
       target:
         description: Replication target details.
@@ -911,14 +912,15 @@
         type: string
       cloudEncryptionKey:
         description: Cloud encryption key.
         type: string
       plugins:
         description: Plugins.
         type: array
+        x-default: null
         items:
           type: string
       hiveExternalTableBaseDirectory:
         description: Hive external table base directory.
         type: string
       cmPolicySubmitUser:
         description: CM policy submit user.
@@ -967,14 +969,15 @@
           - DELETE_PERMANENTLY
       alert:
         description: Alerting behavior.
         $ref: '#/definitions/Alert'
       exclusionFilters:
         description: Exclusion filters in glob format.
         type: array
+        x-default: null
         items:
           type: string
   ErrorHandling:
     type: object
     description: Error handling behavior.
     required:
       - skipChecksumChecks
```

### Comparing `cdpcli-beta-0.9.85/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.86/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.86/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/doc/style.py` & `cdpcli-beta-0.9.86/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/docs.py` & `cdpcli-beta-0.9.86/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/endpoint.py` & `cdpcli-beta-0.9.86/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.86/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/exceptions.py` & `cdpcli-beta-0.9.86/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.86/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/formatter.py` & `cdpcli-beta-0.9.86/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/help.py` & `cdpcli-beta-0.9.86/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/loader.py` & `cdpcli-beta-0.9.86/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/main.py` & `cdpcli-beta-0.9.86/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/model.py` & `cdpcli-beta-0.9.86/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/paginate.py` & `cdpcli-beta-0.9.86/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/paramfile.py` & `cdpcli-beta-0.9.86/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.86/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/parser.py` & `cdpcli-beta-0.9.86/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.86/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/schema.py` & `cdpcli-beta-0.9.86/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/serialize.py` & `cdpcli-beta-0.9.86/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/shorthand.py` & `cdpcli-beta-0.9.86/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/signers.py` & `cdpcli-beta-0.9.86/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/table.py` & `cdpcli-beta-0.9.86/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/text.py` & `cdpcli-beta-0.9.86/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/textwriter.py` & `cdpcli-beta-0.9.86/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.86/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/translate.py` & `cdpcli-beta-0.9.86/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/utils.py` & `cdpcli-beta-0.9.86/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli/validate.py` & `cdpcli-beta-0.9.86/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.86/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.85
+Version: 0.9.86
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.85/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.86/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/setup.py` & `cdpcli-beta-0.9.86/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/setup_common.py` & `cdpcli-beta-0.9.86/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/__init__.py` & `cdpcli-beta-0.9.86/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.86/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.86/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.86/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.86/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_auth.py` & `cdpcli-beta-0.9.86/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.86/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_client.py` & `cdpcli-beta-0.9.86/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_completer.py` & `cdpcli-beta-0.9.86/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.86/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_docs.py` & `cdpcli-beta-0.9.86/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.86/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_help.py` & `cdpcli-beta-0.9.86/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.86/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_model.py` & `cdpcli-beta-0.9.86/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.86/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.86/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.86/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.86/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.86/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_signers.py` & `cdpcli-beta-0.9.86/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.86/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_utils.py` & `cdpcli-beta-0.9.86/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/tests/unit/test_validate.py` & `cdpcli-beta-0.9.86/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.85/versioneer.py` & `cdpcli-beta-0.9.86/versioneer.py`

 * *Files identical despite different names*

