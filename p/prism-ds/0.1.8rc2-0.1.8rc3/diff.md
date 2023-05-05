# Comparing `tmp/prism-ds-0.1.8rc2.tar.gz` & `tmp/prism-ds-0.1.8rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-ds-0.1.8rc2.tar", last modified: Tue Apr  4 02:21:17 2023, max compression
+gzip compressed data, was "prism-ds-0.1.8rc3.tar", last modified: Fri May  5 00:40:48 2023, max compression
```

## Comparing `prism-ds-0.1.8rc2.tar` & `prism-ds-0.1.8rc3.tar`

### file list

```diff
@@ -1,402 +1,402 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.159338 prism-ds-0.1.8rc2/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5508 2023-04-04 02:21:17.159511 prism-ds-0.1.8rc2/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4595 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.077293 prism-ds-0.1.8rc2/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.1.8rc2/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.077932 prism-ds-0.1.8rc2/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4689 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19578 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.080635 prism-ds-0.1.8rc2/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9495 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4548 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-04-03 01:44:48.000000 prism-ds-0.1.8rc2/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.080973 prism-ds-0.1.8rc2/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1724 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/constants.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6480 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/decorators.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.081179 prism-ds-0.1.8rc2/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.083819 prism-ds-0.1.8rc2/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc2/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc2/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc2/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.084201 prism-ds-0.1.8rc2/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5958 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5955 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.086173 prism-ds-0.1.8rc2/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12699 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2333 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6433 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/infra/module.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    20791 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/logging.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21156 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.093668 prism-ds-0.1.8rc2/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc2/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7262 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4713 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc2/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.094485 prism-ds-0.1.8rc2/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15219 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/parsers/yml_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.096955 prism-ds-0.1.8rc2/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15322 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9016 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.097528 prism-ds-0.1.8rc2/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1180 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4676 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.097737 prism-ds-0.1.8rc2/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.1.8rc2/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.097979 prism-ds-0.1.8rc2/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/agents/docker.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.098435 prism-ds-0.1.8rc2/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc2/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/minimal_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.098560 prism-ds-0.1.8rc2/prism/templates/minimal_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/minimal_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1323 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.098691 prism-ds-0.1.8rc2/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.098876 prism-ds-0.1.8rc2/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      153 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099000 prism-ds-0.1.8rc2/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099146 prism-ds-0.1.8rc2/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099272 prism-ds-0.1.8rc2/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      483 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099405 prism-ds-0.1.8rc2/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099526 prism-ds-0.1.8rc2/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.099652 prism-ds-0.1.8rc2/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      194 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.100320 prism-ds-0.1.8rc2/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.100566 prism-ds-0.1.8rc2/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.100684 prism-ds-0.1.8rc2/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.101016 prism-ds-0.1.8rc2/prism/templates/starter_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/modules/module01.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.101165 prism-ds-0.1.8rc2/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1109 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.101706 prism-ds-0.1.8rc2/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/tasks/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/tasks/python.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.102228 prism-ds-0.1.8rc2/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.102368 prism-ds-0.1.8rc2/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.104610 prism-ds-0.1.8rc2/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14138 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10275 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4524 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4601 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.071643 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.105544 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.105928 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1117 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.106432 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.106568 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1340 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.106847 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.107363 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.107633 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.108057 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.108417 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.108857 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.109509 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.110143 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.110424 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.111026 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1264 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.111410 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.111989 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.113708 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.115126 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/txt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.115349 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.115463 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.115866 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.116196 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.116398 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.116697 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.116837 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.117104 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.117256 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.117517 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.117654 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.117898 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.118430 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.118755 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.119362 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1080 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.119725 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.120153 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.120578 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.120797 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.121430 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.121701 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.122207 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.122346 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.122744 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.122869 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.123089 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31298 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.125829 prism-ds-0.1.8rc2/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.125998 prism-ds-0.1.8rc2/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.126165 prism-ds-0.1.8rc2/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.126319 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.132279 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.139617 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.140428 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.145287 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.148646 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.149680 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5017 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_jinja.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10636 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_module_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.154305 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_modules/tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.156458 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.156993 prism-ds-0.1.8rc2/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.157119 prism-ds-0.1.8rc2/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19457 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      815 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc2/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 02:21:17.159193 prism-ds-0.1.8rc2/prism_ds.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5508 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15801 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2022-10-22 21:37:16.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-04-04 02:21:17.000000 prism-ds-0.1.8rc2/prism_ds.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.1.8rc2/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1689 2023-04-04 02:21:17.160061 prism-ds-0.1.8rc2/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       88 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc2/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.091508 prism-ds-0.1.8rc3/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5559 2023-05-05 00:40:48.091606 prism-ds-0.1.8rc3/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4595 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.980237 prism-ds-0.1.8rc3/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.1.8rc3/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.982189 prism-ds-0.1.8rc3/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4689 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19578 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.986870 prism-ds-0.1.8rc3/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9495 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4548 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5452 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.987282 prism-ds-0.1.8rc3/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1724 2023-05-04 13:24:57.000000 prism-ds-0.1.8rc3/prism/constants.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6480 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/decorators.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.987498 prism-ds-0.1.8rc3/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.993019 prism-ds-0.1.8rc3/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc3/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc3/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc3/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-ds-0.1.8rc3/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.993389 prism-ds-0.1.8rc3/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5985 2023-05-04 14:38:23.000000 prism-ds-0.1.8rc3/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5955 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.999856 prism-ds-0.1.8rc3/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12699 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2395 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6433 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/infra/module.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21159 2023-05-04 22:11:22.000000 prism-ds-0.1.8rc3/prism/logging.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21156 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.006199 prism-ds-0.1.8rc3/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc3/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7262 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4713 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.1.8rc3/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.007125 prism-ds-0.1.8rc3/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15219 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/parsers/yml_parser.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.012292 prism-ds-0.1.8rc3/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15559 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9047 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.013408 prism-ds-0.1.8rc3/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1180 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4676 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.013885 prism-ds-0.1.8rc3/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.1.8rc3/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.014447 prism-ds-0.1.8rc3/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/agents/docker.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.015317 prism-ds-0.1.8rc3/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc3/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/minimal_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.015556 prism-ds-0.1.8rc3/prism/templates/minimal_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/minimal_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1323 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.016010 prism-ds-0.1.8rc3/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.016431 prism-ds-0.1.8rc3/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      153 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.016951 prism-ds-0.1.8rc3/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.017234 prism-ds-0.1.8rc3/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.017827 prism-ds-0.1.8rc3/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      483 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.019158 prism-ds-0.1.8rc3/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.019562 prism-ds-0.1.8rc3/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.019910 prism-ds-0.1.8rc3/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      194 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.020855 prism-ds-0.1.8rc3/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.021108 prism-ds-0.1.8rc3/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.021342 prism-ds-0.1.8rc3/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.022426 prism-ds-0.1.8rc3/prism/templates/starter_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/modules/module01.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.022686 prism-ds-0.1.8rc3/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1109 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.023141 prism-ds-0.1.8rc3/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/tasks/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/tasks/python.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.023676 prism-ds-0.1.8rc3/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.023842 prism-ds-0.1.8rc3/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.029842 prism-ds-0.1.8rc3/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14137 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10275 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4524 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4601 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:47.969231 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.031118 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.031300 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1117 2023-05-04 22:22:43.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.031637 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.031917 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1340 2023-05-04 22:22:43.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.032384 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.033487 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.034030 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.034710 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.035056 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.038524 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.039775 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.041869 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.042801 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.044726 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1264 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.045238 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.046306 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.046755 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.047893 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/txt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.048093 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.048203 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.048616 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.048925 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.049261 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.049659 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.050049 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.050400 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.050766 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.051310 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.051539 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.052089 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.053073 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.054601 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.058667 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1080 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.061124 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.062663 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.063266 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.063721 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.064301 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.064514 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.064985 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.065693 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.066381 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.066557 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.066889 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31080 2023-05-04 22:20:29.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.073549 prism-ds-0.1.8rc3/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.073902 prism-ds-0.1.8rc3/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.074043 prism-ds-0.1.8rc3/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.074228 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.075630 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.079394 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.080301 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.081663 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.082674 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.083856 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5017 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_jinja.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10636 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_module_parser.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.087867 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_modules/tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.089502 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.089812 prism-ds-0.1.8rc3/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.1.8rc3/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.090000 prism-ds-0.1.8rc3/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19434 2023-05-04 14:37:27.000000 prism-ds-0.1.8rc3/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.1.8rc3/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 00:40:48.091376 prism-ds-0.1.8rc3/prism_ds.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5559 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15801 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2022-10-22 21:37:16.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-05-05 00:40:47.000000 prism-ds-0.1.8rc3/prism_ds.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.1.8rc3/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1729 2023-05-05 00:40:48.092025 prism-ds-0.1.8rc3/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.1.8rc3/setup.py
```

### Comparing `prism-ds-0.1.8rc2/LICENSE` & `prism-ds-0.1.8rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/PKG-INFO` & `prism-ds-0.1.8rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.1.8rc2
+Version: 0.1.8rc3
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -12,14 +12,15 @@
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: trino
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.1.8rc2 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-ds Version: 0.1.8rc3 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-snowflake Provides-Extra: bigquery Provides-Extra: redshift Provides-Extra:
-postgres Provides-Extra: trino Provides-Extra: pyspark Provides-Extra: dbt
-Provides-Extra: docker Provides-Extra: testing License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: snowflake Provides-
+Extra: bigquery Provides-Extra: redshift Provides-Extra: postgres Provides-
+Extra: trino Provides-Extra: pyspark Provides-Extra: dbt Provides-Extra: docker
+Provides-Extra: testing License-File: LICENSE
                                  [prism logo]
           [PyPI] [https://static.pepy.tech/personalized-badge/prism-
 ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
 [![CI Linux](https://github.com/runprism/prism/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-linux.yml)
 [![CI MacOS](https://github.com/runprism/prism/actions/workflows/ci-macos.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-macos.yml)
```

### Comparing `prism-ds-0.1.8rc2/README.md` & `prism-ds-0.1.8rc3/README.md`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/admin.py` & `prism-ds-0.1.8rc3/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/agents/base.py` & `prism-ds-0.1.8rc3/prism/agents/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/agents/docker_agent.py` & `prism-ds-0.1.8rc3/prism/agents/docker_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/agents/meta.py` & `prism-ds-0.1.8rc3/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/agent.py` & `prism-ds-0.1.8rc3/prism/cli/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/base.py` & `prism-ds-0.1.8rc3/prism/cli/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/compile.py` & `prism-ds-0.1.8rc3/prism/cli/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/connect.py` & `prism-ds-0.1.8rc3/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/create_agent.py` & `prism-ds-0.1.8rc3/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/create_task.py` & `prism-ds-0.1.8rc3/prism/cli/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/create_trigger.py` & `prism-ds-0.1.8rc3/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/graph.py` & `prism-ds-0.1.8rc3/prism/cli/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/init.py` & `prism-ds-0.1.8rc3/prism/cli/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,16 @@
  ___/_/   /_/  /_/____/_/ /_/ /_/  ___
 
 Welcome to Prism, the easiest way to create clean, modular data pipelines
 using Python!
 
 To get started, navigate to your newly created project "{project_name}" and try
 running the following commands:
-    prism compile
-    prism run
+    > $ prism compile
+    > $ prism run
 
 Consult the documentation here for more information on how to get started.
     {docs_url}
 
 Happy building!"""
 
 
@@ -171,15 +171,15 @@
                 msg=TASK_COMPLETE_MSG.format(
                     project_name=project_name,
                     docs_url='docs.runprism.com'
                 )
             ),
             event_list,
             0,
-            log_level='info'
+            log_level='agent'
         )
         event_list = fire_console_event(
             prism.logging.SeparatorEvent(),
             event_list,
             0,
             log_level='info'
         )
```

### Comparing `prism-ds-0.1.8rc2/prism/cli/run.py` & `prism-ds-0.1.8rc3/prism/cli/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/cli/spark_submit.py` & `prism-ds-0.1.8rc3/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/client/__init__.py` & `prism-ds-0.1.8rc3/prism/client/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/constants.py` & `prism-ds-0.1.8rc3/prism/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #############
 # Constants #
 #############
 
 # Version number
-VERSION = '0.1.8rc2'
+VERSION = '0.1.8rc3'
 
 # Root directory of project
 ROOT_DIR = str(Path(os.path.dirname(__file__)).parent)
 
 # Files to ignore when instantiating Prism project
 IGNORE_FILES = ["__pycache__", '*checkpoint.ipynb', '.ipynb_checkpoints']
```

### Comparing `prism-ds-0.1.8rc2/prism/decorators.py` & `prism-ds-0.1.8rc3/prism/decorators.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/311ea03002abadcdcaba.png` & `prism-ds-0.1.8rc3/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/54968a39190c43d592b9.svg` & `prism-ds-0.1.8rc3/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-ds-0.1.8rc3/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/ce188596011a8fa32931.png` & `prism-ds-0.1.8rc3/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/index.html` & `prism-ds-0.1.8rc3/prism/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/docs/build/main.js.LICENSE.txt` & `prism-ds-0.1.8rc3/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/event_managers/base.py` & `prism-ds-0.1.8rc3/prism/event_managers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def fire_running_exec_event(self,
         event_list: List[prism.logging.Event]
     ):
         """
         Create ExecutionEvent informing user of task execution
         """
         e = prism.logging.ExecutionEvent(
-            msg=f"RUNNING {EVENT_COLOR}{self.name}{RESET}",
+            msg=f"RUNNING EVENT {EVENT_COLOR}'{self.name}'{RESET}",
             num=self.idx,
             total=self.total,
             status="RUN",
             execution_time=None
         )
         event_list = fire_console_event(e, event_list, log_level='info')
         return event_list
@@ -74,15 +74,15 @@
         event_list: List[prism.logging.Event]
     ) -> List[Event]:
         """
         Create ExecutionEvent informing user of successful task execution
         """
         execution_time = time.time() - start_time
         e = prism.logging.ExecutionEvent(
-            msg=f"{GREEN}FINISHED{RESET} {EVENT_COLOR}{self.name}{RESET}",
+            msg=f"{GREEN}FINISHED{RESET} EVENT {EVENT_COLOR}'{self.name}'{RESET}",
             num=self.idx,
             total=self.total,
             status="DONE",
             execution_time=execution_time
         )
         event_list = fire_console_event(e, event_list, log_level='info')
         return event_list
@@ -92,15 +92,15 @@
         event_list: List[prism.logging.Event]
     ) -> List[Event]:
         """
         Create ExecutionEvent informing user of error in task execution
         """
         execution_time = time.time() - start_time
         e = prism.logging.ExecutionEvent(
-            msg=f"{RED}ERROR{RESET} {EVENT_COLOR}{self.name}{RESET}",
+            msg=f"{RED}ERROR{RESET} IN EVENT {EVENT_COLOR}'{self.name}'{RESET}",
             num=self.idx,
             total=self.total,
             status="ERROR",
             execution_time=execution_time
         )
 
         # Set the log-level to `info`. We'll fire the actual error using log-level
```

### Comparing `prism-ds-0.1.8rc2/prism/exceptions.py` & `prism-ds-0.1.8rc3/prism/exceptions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/compiler.py` & `prism-ds-0.1.8rc3/prism/infra/compiler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/executor.py` & `prism-ds-0.1.8rc3/prism/infra/executor.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/hooks.py` & `prism-ds-0.1.8rc3/prism/infra/hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         df = adapter_obj.execute_sql(query, return_type)
         if return_type == "pandas":
             return df
 
     def dbt_ref(self,
         adapter_name: str,
         target_1: str,
-        target_2: Optional[str] = None
+        target_2: Optional[str] = None,
+        target_version: Optional[str] = None
     ) -> pd.DataFrame:
         """
         Get dbt model as a Pandas DataFrame
 
         args:
             adapter_name: name of dbt adapter in profile YML
             target_1: dbt model (or package)
@@ -80,9 +81,9 @@
         try:
             dbt_project = self.project.adapters_object_dict[adapter_name]
         except KeyError:
             raise prism.exceptions.RuntimeException(
                 message=f'adapter `{adapter_name}` not defined'
             )
 
-        df = dbt_project.handle_ref(target_1, target_2)
+        df = dbt_project.handle_ref(target_1, target_2, target_version)
         return df
```

### Comparing `prism-ds-0.1.8rc2/prism/infra/manifest.py` & `prism-ds-0.1.8rc3/prism/infra/manifest.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/module.py` & `prism-ds-0.1.8rc3/prism/infra/module.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/pipeline.py` & `prism-ds-0.1.8rc3/prism/infra/pipeline.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/project.py` & `prism-ds-0.1.8rc3/prism/infra/project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/sys_path.py` & `prism-ds-0.1.8rc3/prism/infra/sys_path.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/infra/task_manager.py` & `prism-ds-0.1.8rc3/prism/infra/task_manager.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/logging.py` & `prism-ds-0.1.8rc3/prism/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,16 @@
                 obj.setLevel(logging.INFO)
             elif level == 'warn':
                 obj.setLevel(logging.WARN)
             elif level == 'error':
                 obj.setLevel(logging.ERROR)
             elif level == 'debug':
                 obj.setLevel(logging.DEBUG)
+            elif level == 'agent':
+                obj.setLevel(logging.AGENT)  # type: ignore
             return obj
 
         # Set the appropriate log level
         DEFAULT_LOGGER = _set_level(DEFAULT_LOGGER, args.log_level)
 
         # Stream handler
         handler = logging.StreamHandler()
@@ -424,31 +426,36 @@
     total: Optional[int]
     status: str
     execution_time: Optional[float]
 
     def __str__(self):
         """
         ExecutionEvent messages are either:
-            RUNNING {event.name}
-            FINISHED {event.name}
-            ERROR {event.name}
+            RUNNING EVENT {event.name}
+            FINISHED EVENT {event.name}
+            ERROR IN EVENT {event.name}
 
         Add name of event (after removing event status and ANSI codes) to string
         representation of event.
         """
         # Remove all ANSI codes
         msg_no_ansi = escape_ansi(self.msg)
 
         # Remove the event status
         status_regex = re.compile('(RUNNING|FINISHED|ERROR)')
         msg_no_ansi_status = status_regex.sub('', msg_no_ansi)
 
+        # Remove EVENT and quotation marks
+        event_name_str = msg_no_ansi_status \
+            .replace("IN EVENT", "") \
+            .replace("EVENT", "") \
+            .replace("'", "")
+
         # Remove all trailing / leading spaces
-        event_name_str = msg_no_ansi_status.strip()
-        return super().__str__() + " - " + event_name_str + " - " + self.status
+        return super().__str__() + " - " + event_name_str.strip() + " - " + self.status
 
     def message(self):
         message = self.msg
         if self.num is not None and self.total is not None:
             message = f'{self.num} of {self.total} {self.msg}'
 
         # Add execution time and status
@@ -595,15 +602,15 @@
 
 
 @dataclass
 class TasksHeaderEvent(HeaderEvent):
     msg: str
 
     def header_str(self):
-        return f'tasks ({GRAY_PINK}{self.msg}{HEADER_GRAY})'
+        return f"tasks {GRAY_PINK}'{self.msg}'{HEADER_GRAY}"
 
 
 @dataclass
 class TriggersHeaderEvent(HeaderEvent):
     msg: str = 'triggers'
 
 
@@ -748,14 +755,16 @@
             DEFAULT_LOGGER.info(event.message())  # type: ignore
         elif log_level == "warn":
             DEFAULT_LOGGER.warning(event.message())  # type: ignore
         elif log_level == "error":
             DEFAULT_LOGGER.error(event.message())  # type: ignore
         elif log_level == "debug":
             DEFAULT_LOGGER.debug(event.message())  # type: ignore
+        elif log_level == "agent":
+            DEFAULT_LOGGER.agent(event.message())  # type: ignore
 
     # Sleep
     time.sleep(sleep)
 
     # Return event list
     if event is not None:
         event_list.append(event)
```

### Comparing `prism-ds-0.1.8rc2/prism/main.py` & `prism-ds-0.1.8rc3/prism/main.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/agent.py` & `prism-ds-0.1.8rc3/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/base.py` & `prism-ds-0.1.8rc3/prism/mixins/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/compile.py` & `prism-ds-0.1.8rc3/prism/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/connect.py` & `prism-ds-0.1.8rc3/prism/mixins/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/create_agent.py` & `prism-ds-0.1.8rc3/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/create_task.py` & `prism-ds-0.1.8rc3/prism/mixins/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/create_trigger.py` & `prism-ds-0.1.8rc3/prism/mixins/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/graph.py` & `prism-ds-0.1.8rc3/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/run.py` & `prism-ds-0.1.8rc3/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/mixins/sys_handler.py` & `prism-ds-0.1.8rc3/prism/mixins/sys_handler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/parsers/ast_parser.py` & `prism-ds-0.1.8rc3/prism/parsers/ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/parsers/base.py` & `prism-ds-0.1.8rc3/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/parsers/yml_parser.py` & `prism-ds-0.1.8rc3/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/adapter.py` & `prism-ds-0.1.8rc3/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/bigquery.py` & `prism-ds-0.1.8rc3/prism/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/dbt.py` & `prism-ds-0.1.8rc3/prism/profiles/dbt.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,24 +102,24 @@
         self.initialize_dbt_flags(self.dbt_profiles_dir)
         config = self.get_dbt_runtime_config(
             self.dbt_project_dir,
             self.dbt_profiles_dir,
             profile_target=self.dbt_profiles_target
         )
 
-        # Initialize flags and compile task
-        self.compile_task = self.initialize_compile_task(self.dbt_profiles_dir, config)
-        dbt.tracking.initialize_tracking(self.dbt_profiles_dir)
-
-        # Manifest
-        self.manifest = self.get_dbt_manifest(config)
-
         # Get adapter
         self.adapter = self.get_dbt_adapter(config)
 
+        # Initialize flags and compile task
+        dbt.tracking.initialize_from_flags(True, self.dbt_profiles_dir)
+        self.manifest = self.get_dbt_manifest(config)
+        self.compile_task = self.initialize_compile_task(
+            self.dbt_profiles_dir, config, self.manifest
+        )
+
     def parse_adapter_dict(self,
         adapter_dict: Dict[str, Optional[str]],
         adapter_name: str,
         profile_name: str,
         return_type: str = "list"
     ) -> Tuple[str, str, Optional[str]]:
         """
@@ -220,38 +220,39 @@
             flags.set_from_args(args, user_config)
 
         # Set invocation id
         events_functions.set_invocation_id()
 
     def initialize_compile_task(self,
         profiles_dir: str,
-        dbt_config: RuntimeConfig
+        dbt_config: RuntimeConfig,
+        manifest,
     ):
         """
         Initialize the compile task and call _runtime_initialize(). This must be done
         after the flags module has been initialized.
 
         args:
             profiles_dir: directory of dbt profiles
         """
         # Initialize tracking
-        dbt.tracking.initialize_tracking(profiles_dir)
+        dbt.tracking.initialize_from_flags(True, profiles_dir)
 
         # All the arguments to the compile task can be None or empty
         selector_name = None
         select: List[str] = []
         exclude: Tuple[str, str] = tuple()  # type: ignore
         state = None
         args = InitializeDbtCompileTaskArgs(
             selector_name, select, select, exclude, state, None
         )
 
         # Initialize compile task. No need to call _runtime_initialize, because we do
         # not need to read the graph
-        compile_task = CompileTask(args, dbt_config)
+        compile_task = CompileTask(args, dbt_config, manifest)
         return compile_task
 
     def get_dbt_manifest(self,
         dbt_config: RuntimeConfig
     ) -> Manifest:
         """
         Get dbt manifest; this must be called after the dbt compile task is initialized
@@ -276,14 +277,15 @@
         dbt.adapters.factory.register_adapter(dbt_config)
         adapter: SQLAdapter = adapters_factory.get_adapter(dbt_config)
         return adapter
 
     def get_parsed_model_node(self,
         target_model_name: str,
         target_model_package: Optional[str],
+        target_model_version: Optional[str],
         project_dir: str,
         manifest: Manifest
     ) -> ResultNode:
         """
         Get the node associated with the inputted target model
 
         args:
@@ -299,14 +301,15 @@
         # be more complex projects where this is not the case. We implement the simple
         # version for now.
 
         # TODO: test target model creation where node_package != project_dir
         target_model: MaybeNonSource = manifest.resolve_ref(
             target_model_name=target_model_name,
             target_model_package=target_model_package,
+            target_model_version=target_model_version,
             current_project=project_dir,
             node_package=project_dir
         )
 
         # If model isn't found, then throw an error.
         package_str = f"'{target_model_package}'." if target_model_package is not None else ""  # noqa: E501
         model_str = f"{package_str}'{target_model_name}'"
@@ -405,15 +408,16 @@
         """
         return pd.DataFrame.from_records(
             result.table.rows, columns=result.table.column_names, coerce_float=True
         )
 
     def handle_ref(self,
         target_1: str,
-        target_2: Optional[str] = None
+        target_2: Optional[str] = None,
+        target_version: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         Download a dbt model into a Pandas DataFrame:
 
         args:
             target_1, target_2: dbt model
         returns:
@@ -426,14 +430,15 @@
             target_package_name = target_1
             target_model_name = target_2
 
         # Get target model
         target_model = self.get_parsed_model_node(
             target_model_name,
             target_package_name,
+            target_version,
             self.dbt_project_dir,
             self.manifest
         )
 
         # Get relation
         target_model_relation = self.get_target_model_relation(
             target_model,
```

### Comparing `prism-ds-0.1.8rc2/prism/profiles/meta.py` & `prism-ds-0.1.8rc3/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/postgres.py` & `prism-ds-0.1.8rc3/prism/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/profile.py` & `prism-ds-0.1.8rc3/prism/profiles/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,16 @@
                     user_defined_adapter = MetaAdapter.get_adapter(adapter_type)(
                         name, adapter_conf, self.profile_name
                     )
                     self.adapters_obj_dict[name] = user_defined_adapter
 
             # The profile YML does not contain an adapters top-level key. This is
             # checked upon profile instantiation, so this should never happen.
-            except KeyError:
-                pass
+            except KeyError as e:
+                raise e
+                # pass
 
     def get_adapters_obj_dict(self):
         """
         Get dictionary of adapter objects associated with profile
         """
         return self.adapters_obj_dict
```

### Comparing `prism-ds-0.1.8rc2/prism/profiles/pyspark.py` & `prism-ds-0.1.8rc3/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/redshift.py` & `prism-ds-0.1.8rc3/prism/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/snowflake.py` & `prism-ds-0.1.8rc3/prism/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/profiles/trino.py` & `prism-ds-0.1.8rc3/prism/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/spark/wrapper.py` & `prism-ds-0.1.8rc3/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/target.py` & `prism-ds-0.1.8rc3/prism/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/task.py` & `prism-ds-0.1.8rc3/prism/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/templates/minimal_project/modules/module01.py` & `prism-ds-0.1.8rc3/prism/templates/minimal_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/templates/minimal_project/prism_project.py` & `prism-ds-0.1.8rc3/prism/templates/minimal_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/templates/starter_project/dev/dev.ipynb` & `prism-ds-0.1.8rc3/prism/templates/starter_project/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/templates/starter_project/modules/module01.py` & `prism-ds-0.1.8rc3/prism/templates/starter_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/templates/starter_project/prism_project.py` & `prism-ds-0.1.8rc3/prism/templates/starter_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/integration_test_class.py` & `prism-ds-0.1.8rc3/prism/tests/integration/integration_test_class.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_client.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,14 @@
             Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt')
         )
         expected_output = 'Hello from module 1!'
         self.assertEqual(expected_output, module01_txt)
 
         # -------------------------------------------------------
         # Without `module` param
-
         dag5.run()
 
         # Confirm creation of outputs
         self.assertTrue(
             Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt').is_file()
         )
         self.assertTrue(
```

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_compile.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_connect.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_create.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_create.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_dbt.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_dbt.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_hooks.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_hooks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_init.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/004_simple_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/modules/parquet.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/modules/parquet.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_run.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -631,30 +631,29 @@
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / 'output' / 'trigger.txt').is_file())
         with open(Path(wkdir / 'output' / 'trigger.txt'), 'r') as f:
             trigger_txt = f.read()
         self.assertEqual('This is outputted from the trigger function!', trigger_txt)
 
     def _check_trigger_events(self,
-        trigger_type: str,
         execution_event_dict: Dict[str, str],
         circa_trigger_header_event: List[str] = ['TriggersHeaderEvent'],
         final_status: str = "DONE"
     ):
         """
         Triggers kick of a predictable set of events. Check that these exist.
         """
         expected_events = run_success_starting_events + \
             ['TasksHeaderEvent'] + \
             _execution_events_modules(execution_event_dict) + \
             ["EmptyLineEvent"] + \
             circa_trigger_header_event + \
             [
-                f"ExecutionEvent - on_{trigger_type} trigger test_trigger_function - RUN",  # noqa: E501
-                f"ExecutionEvent - on_{trigger_type} trigger test_trigger_function - {final_status}",  # noqa: E501
+                "ExecutionEvent - test_trigger_function - RUN",  # noqa: E501
+                f"ExecutionEvent - test_trigger_function - {final_status}",  # noqa: E501
             ]
         return expected_events
 
     def test_trigger_on_success(self):
         """
         Test on_success trigger
         """
@@ -670,15 +669,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run', '--modules', 'module01.py']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'success',
             {'module01.py': 'DONE'}
         ) + _run_task_end_events('TaskSuccessfulEndEvent')
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Check manifest / output
         self._check_trigger_output(wkdir)
 
@@ -704,15 +702,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run', '--modules', 'module02.py']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'failure',
             {'module02.py': 'ERROR'},
             ["ExecutionErrorEvent", "TriggersHeaderEvent"]
         ) + ["SeparatorEvent"]
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Check manifest / output
         self._check_trigger_output(wkdir)
@@ -739,15 +736,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run', '--modules', 'module01.py']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'success',
             {'module01.py': 'DONE'},
             ["TriggersHeaderEvent", "TriggersPathNotDefined"]
         ) + _run_task_end_events('TaskSuccessfulEndEvent')
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Check that manifest was created
         self._check_trigger_output(wkdir)
@@ -774,15 +770,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'success',
             {'module01.py': 'DONE'},
             ["TriggersHeaderEvent"],
             'ERROR'
         ) + ['EmptyLineEvent', 'ExecutionErrorEvent', 'SeparatorEvent']
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Remove the .compiled directory, if it exists
@@ -807,15 +802,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'success',
             {'module01.py': 'DONE'},
             ["TriggersHeaderEvent", "UnexpectedTriggersYmlKeysEvent"]
         ) + _run_task_end_events('TaskSuccessfulEndEvent')
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Check that manifest was created
         self._check_trigger_output(wkdir)
@@ -843,15 +837,14 @@
         self._remove_files_in_output(wkdir)
 
         # Run all modules downstream of module01.py
         args = ['run']
         run = self._run_prism(args)
         run_results = run.get_results()
         expected_events = self._check_trigger_events(
-            'success',
             {'module01.py': 'DONE'},
             ["TriggersHeaderEvent"],
             'ERROR'
         ) + ['EmptyLineEvent', 'ExecutionErrorEvent', 'SeparatorEvent']
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Remove the .compiled directory, if it exists
```

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_spark_submit.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/integration/test_targets.py` & `prism-ds-0.1.8rc3/prism/tests/integration/test_targets.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_adapter_profile.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_agent/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_agent/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_agents.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_agents.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_all_dag_fns.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_all_dag_fns.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_jinja.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_jinja.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_module_parser.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_module_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_project.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_trigger.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-ds-0.1.8rc3/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism/triggers/__init__.py` & `prism-ds-0.1.8rc3/prism/triggers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 
         # Execute triggers
         cb_has_error = False
         for cb in triggers_to_exec:
             cb_event_manager = BaseEventManager(
                 idx=None,
                 total=None,
-                name=f'{trigger_type} trigger {cb.name}',
+                name=f'{cb.name}',
                 full_tb=full_tb,
                 func=cb.execute_trigger
             )
             cb_event_manager_output = cb_event_manager.manage_events_during_run(
                 event_list=event_list,
                 run_context=run_context,
                 fire_empty_line_events=False
```

### Comparing `prism-ds-0.1.8rc2/prism_ds.egg-info/PKG-INFO` & `prism-ds-0.1.8rc3/prism_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.1.8rc2
+Version: 0.1.8rc3
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -12,14 +12,15 @@
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: trino
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.1.8rc2 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-ds Version: 0.1.8rc3 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-snowflake Provides-Extra: bigquery Provides-Extra: redshift Provides-Extra:
-postgres Provides-Extra: trino Provides-Extra: pyspark Provides-Extra: dbt
-Provides-Extra: docker Provides-Extra: testing License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: snowflake Provides-
+Extra: bigquery Provides-Extra: redshift Provides-Extra: postgres Provides-
+Extra: trino Provides-Extra: pyspark Provides-Extra: dbt Provides-Extra: docker
+Provides-Extra: testing License-File: LICENSE
                                  [prism logo]
           [PyPI] [https://static.pepy.tech/personalized-badge/prism-
 ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
 [![CI Linux](https://github.com/runprism/prism/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-linux.yml)
 [![CI MacOS](https://github.com/runprism/prism/actions/workflows/ci-macos.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-macos.yml)
```

### Comparing `prism-ds-0.1.8rc2/prism_ds.egg-info/SOURCES.txt` & `prism-ds-0.1.8rc3/prism_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/prism_ds.egg-info/requires.txt` & `prism-ds-0.1.8rc3/prism_ds.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/pyproject.toml` & `prism-ds-0.1.8rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-ds-0.1.8rc2/setup.cfg` & `prism-ds-0.1.8rc3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = prism-ds
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.1.8rc2
+version = 0.1.8rc3
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 project_urls = 
 	homepage = https://www.runprism.com
 	documentation = https://docs.runprism.com
 	repository = https://github.com/runprism/prism
 
 [options]
 packages = find_namespace:
```

