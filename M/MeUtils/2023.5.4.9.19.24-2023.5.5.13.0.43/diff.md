# Comparing `tmp/MeUtils-2023.5.4.9.19.24.tar.gz` & `tmp/MeUtils-2023.5.5.13.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.5.4.9.19.24.tar", last modified: Thu May  4 01:19:24 2023, max compression
+gzip compressed data, was "MeUtils-2023.5.5.13.0.43.tar", last modified: Fri May  5 05:00:44 2023, max compression
```

## Comparing `MeUtils-2023.5.4.9.19.24.tar` & `MeUtils-2023.5.5.13.0.43.tar`

### file list

```diff
@@ -1,685 +1,685 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.899768 MeUtils-2023.5.4.9.19.24/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.794686 MeUtils-2023.5.4.9.19.24/.idea/
--rw-r--r--   0 betterme   (501) staff       (20)      182 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      742 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/MeUtils.iml
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.795016 MeUtils-2023.5.4.9.19.24/.idea/inspectionProfiles/
--rw-r--r--   0 betterme   (501) staff       (20)     3037 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 betterme   (501) staff       (20)      195 2023-04-14 01:05:27.000000 MeUtils-2023.5.4.9.19.24/.idea/misc.xml
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/modules.xml
--rw-r--r--   0 betterme   (501) staff       (20)      167 2023-04-14 01:04:23.000000 MeUtils-2023.5.4.9.19.24/.idea/vcs.xml
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.795802 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1864 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    24060 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)      949 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1864 2023-05-04 01:19:24.899541 MeUtils-2023.5.4.9.19.24/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1065 2023-04-26 01:59:34.000000 MeUtils-2023.5.4.9.19.24/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      196 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.800115 MeUtils-2023.5.4.9.19.24/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.5.4.9.19.24/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.801644 MeUtils-2023.5.4.9.19.24/meutils/annzoo/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.801911 MeUtils-2023.5.4.9.19.24/meutils/annzoo/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/annzoo/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.802033 MeUtils-2023.5.4.9.19.24/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6028 2023-04-21 04:14:28.000000 MeUtils-2023.5.4.9.19.24/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.803548 MeUtils-2023.5.4.9.19.24/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.804306 MeUtils-2023.5.4.9.19.24/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.804590 MeUtils-2023.5.4.9.19.24/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)     8275 2023-04-27 09:03:26.000000 MeUtils-2023.5.4.9.19.24/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.804832 MeUtils-2023.5.4.9.19.24/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.810377 MeUtils-2023.5.4.9.19.24/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.5.4.9.19.24/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-05-04 01:19:24.000000 MeUtils-2023.5.4.9.19.24/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.815471 MeUtils-2023.5.4.9.19.24/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.817131 MeUtils-2023.5.4.9.19.24/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1679 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6732 2023-05-04 01:19:21.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.5.4.9.19.24/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3536 2023-03-31 02:35:37.000000 MeUtils-2023.5.4.9.19.24/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.817546 MeUtils-2023.5.4.9.19.24/meutils/docarray_/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.819265 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.824982 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.825407 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.826600 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.827154 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.827527 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.828479 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.829455 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.830550 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.831375 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.832090 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.832729 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.833599 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.834394 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.835027 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.835646 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.836275 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.836936 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.842393 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.842996 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.844154 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.844443 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.844861 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.845203 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.845580 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.845872 MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.846030 MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.847180 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.847581 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.847710 MeUtils-2023.5.4.9.19.24/meutils/docarray_/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.848416 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.848668 MeUtils-2023.5.4.9.19.24/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2171 2023-04-26 12:04:06.000000 MeUtils-2023.5.4.9.19.24/meutils/easy_search/es.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.5.4.9.19.24/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.850037 MeUtils-2023.5.4.9.19.24/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.5.4.9.19.24/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      407 2023-04-27 09:18:36.000000 MeUtils-2023.5.4.9.19.24/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-04-14 02:08:05.000000 MeUtils-2023.5.4.9.19.24/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.851198 MeUtils-2023.5.4.9.19.24/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.5.4.9.19.24/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2290 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.5.4.9.19.24/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.851779 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     6921 2023-04-25 07:32:56.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.852164 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-04-25 03:45:09.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-04-25 06:23:09.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2300 2023-04-25 07:48:57.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1972 2023-04-24 02:28:40.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-04-25 07:39:01.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3206 2023-04-24 02:28:40.000000 MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.853166 MeUtils-2023.5.4.9.19.24/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     3181 2023-03-31 02:35:37.000000 MeUtils-2023.5.4.9.19.24/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.853932 MeUtils-2023.5.4.9.19.24/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.854426 MeUtils-2023.5.4.9.19.24/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.855018 MeUtils-2023.5.4.9.19.24/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/other/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.5.4.9.19.24/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.856028 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.859903 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.862612 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.862866 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.863969 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.864370 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.864600 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.865343 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.865946 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.866657 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.867324 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.868204 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.868900 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.869759 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.870730 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.871522 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.872262 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.873255 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.874254 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.877579 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.878352 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.879133 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.879432 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.879745 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.880053 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.880354 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.880521 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.880762 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.881579 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.882076 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.882232 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.4.9.19.24/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.882703 MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.5.4.9.19.24/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8419 2023-04-27 08:56:11.000000 MeUtils-2023.5.4.9.19.24/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.884423 MeUtils-2023.5.4.9.19.24/meutils/plot/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/plot/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.885478 MeUtils-2023.5.4.9.19.24/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.885907 MeUtils-2023.5.4.9.19.24/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2397 2023-04-28 05:43:39.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.886506 MeUtils-2023.5.4.9.19.24/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.887533 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      898 2023-04-28 10:41:27.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     6995 2023-04-28 10:39:20.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      131 2023-04-28 10:38:41.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.887696 MeUtils-2023.5.4.9.19.24/meutils/serving/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:48:41.000000 MeUtils-2023.5.4.9.19.24/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.888005 MeUtils-2023.5.4.9.19.24/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.888786 MeUtils-2023.5.4.9.19.24/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6417 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.889271 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-04-07 09:07:13.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.5.4.9.19.24/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.890458 MeUtils-2023.5.4.9.19.24/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.891467 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/hegui.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.891599 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.894701 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.894850 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1207 2023-04-18 10:18:45.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.896659 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.896801 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.897056 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.897313 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.897721 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/templates/合规日报模板.docx
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.898576 MeUtils-2023.5.4.9.19.24/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/typings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      529 2023-04-11 09:18:47.000000 MeUtils-2023.5.4.9.19.24/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      324 2023-04-04 15:18:39.000000 MeUtils-2023.5.4.9.19.24/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       32 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 01:19:24.899255 MeUtils-2023.5.4.9.19.24/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 01:19:24.899820 MeUtils-2023.5.4.9.19.24/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.5.4.9.19.24/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.080059 MeUtils-2023.5.5.13.0.43/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.949533 MeUtils-2023.5.5.13.0.43/.idea/
+-rw-r--r--   0 betterme   (501) staff       (20)      182 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      742 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/MeUtils.iml
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.949832 MeUtils-2023.5.5.13.0.43/.idea/inspectionProfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)     3037 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 betterme   (501) staff       (20)      195 2023-04-14 01:05:27.000000 MeUtils-2023.5.5.13.0.43/.idea/misc.xml
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/modules.xml
+-rw-r--r--   0 betterme   (501) staff       (20)      167 2023-04-14 01:04:23.000000 MeUtils-2023.5.5.13.0.43/.idea/vcs.xml
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.950554 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1866 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    24060 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      949 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1866 2023-05-05 05:00:44.079886 MeUtils-2023.5.5.13.0.43/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.5.5.13.0.43/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      196 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.954938 MeUtils-2023.5.5.13.0.43/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.5.5.13.0.43/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.956784 MeUtils-2023.5.5.13.0.43/meutils/annzoo/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.957342 MeUtils-2023.5.5.13.0.43/meutils/annzoo/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/annzoo/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.957539 MeUtils-2023.5.5.13.0.43/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6034 2023-05-05 05:00:40.000000 MeUtils-2023.5.5.13.0.43/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.958909 MeUtils-2023.5.5.13.0.43/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.959630 MeUtils-2023.5.5.13.0.43/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.959928 MeUtils-2023.5.5.13.0.43/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8275 2023-04-27 09:03:26.000000 MeUtils-2023.5.5.13.0.43/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.960239 MeUtils-2023.5.5.13.0.43/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.965845 MeUtils-2023.5.5.13.0.43/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.5.5.13.0.43/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-05-05 05:00:43.000000 MeUtils-2023.5.5.13.0.43/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.971116 MeUtils-2023.5.5.13.0.43/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.972882 MeUtils-2023.5.5.13.0.43/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1679 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6730 2023-05-04 01:22:21.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.5.5.13.0.43/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3536 2023-03-31 02:35:37.000000 MeUtils-2023.5.5.13.0.43/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.973513 MeUtils-2023.5.5.13.0.43/meutils/docarray_/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.978479 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.984198 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.984680 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.986625 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.987219 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.987556 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.988693 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.989712 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.991266 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.992760 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.994165 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.995419 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.996710 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.998023 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:43.999117 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.000337 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.001350 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.002528 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.009182 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.009980 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.011074 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.011320 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.011695 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.012012 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.012356 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.012586 MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.012831 MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.013975 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.014472 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.014595 MeUtils-2023.5.5.13.0.43/meutils/docarray_/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.015979 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.016532 MeUtils-2023.5.5.13.0.43/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2171 2023-04-26 12:04:06.000000 MeUtils-2023.5.5.13.0.43/meutils/easy_search/es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.5.5.13.0.43/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.018560 MeUtils-2023.5.5.13.0.43/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.5.5.13.0.43/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      911 2023-05-05 02:22:21.000000 MeUtils-2023.5.5.13.0.43/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-04-14 02:08:05.000000 MeUtils-2023.5.5.13.0.43/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.019859 MeUtils-2023.5.5.13.0.43/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.5.5.13.0.43/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2290 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.5.5.13.0.43/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.021132 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     6921 2023-04-25 07:32:56.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.021868 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-04-25 03:45:09.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-04-25 06:23:09.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2300 2023-04-25 07:48:57.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1972 2023-04-24 02:28:40.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-04-25 07:39:01.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3206 2023-04-24 02:28:40.000000 MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.023200 MeUtils-2023.5.5.13.0.43/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3181 2023-03-31 02:35:37.000000 MeUtils-2023.5.5.13.0.43/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.024745 MeUtils-2023.5.5.13.0.43/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.025695 MeUtils-2023.5.5.13.0.43/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.026576 MeUtils-2023.5.5.13.0.43/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/other/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.5.5.13.0.43/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.027570 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.031460 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.035191 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.035588 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.037026 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.037646 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.037911 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.038848 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.039720 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.040674 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.041757 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.042713 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.043800 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.044949 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.045810 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.046559 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.047469 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.048434 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.049668 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.053586 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.054221 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.055282 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.055559 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.055858 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.056149 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.056438 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.056592 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.056759 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.057579 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.058082 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.058221 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.5.13.0.43/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.058860 MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.5.5.13.0.43/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8419 2023-04-27 08:56:11.000000 MeUtils-2023.5.5.13.0.43/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.060409 MeUtils-2023.5.5.13.0.43/meutils/plot/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/plot/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.061970 MeUtils-2023.5.5.13.0.43/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.062700 MeUtils-2023.5.5.13.0.43/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2397 2023-04-28 05:43:39.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.063923 MeUtils-2023.5.5.13.0.43/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.065232 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      898 2023-04-28 10:41:27.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6995 2023-04-28 10:39:20.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      131 2023-04-28 10:38:41.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.065622 MeUtils-2023.5.5.13.0.43/meutils/serving/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:48:41.000000 MeUtils-2023.5.5.13.0.43/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.065877 MeUtils-2023.5.5.13.0.43/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.066681 MeUtils-2023.5.5.13.0.43/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6417 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.067451 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-04-07 09:07:13.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.5.5.13.0.43/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.068965 MeUtils-2023.5.5.13.0.43/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.070297 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/hegui.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.070495 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.073851 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.074016 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1207 2023-04-18 10:18:45.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.076046 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.076231 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.076589 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.076967 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.077703 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/templates/合规日报模板.docx
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.078963 MeUtils-2023.5.5.13.0.43/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/typings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      529 2023-04-11 09:18:47.000000 MeUtils-2023.5.5.13.0.43/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      324 2023-04-04 15:18:39.000000 MeUtils-2023.5.5.13.0.43/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       32 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 05:00:44.079604 MeUtils-2023.5.5.13.0.43/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 05:00:44.080109 MeUtils-2023.5.5.13.0.43/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.5.5.13.0.43/setup.py
```

### Comparing `MeUtils-2023.5.4.9.19.24/.idea/MeUtils.iml` & `MeUtils-2023.5.5.13.0.43/.idea/MeUtils.iml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/.idea/inspectionProfiles/Project_Default.xml` & `MeUtils-2023.5.5.13.0.43/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/LICENSE` & `MeUtils-2023.5.5.13.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.5.4.9.19.24
+Version: 2023.5.5.13.0.43
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -71,14 +71,16 @@
 
 @wecom_hook('wecom_hook_test', 'Sleeping 3s')
 def wecom_hook_test():
     time.sleep(3)
 
 ```
 
+
+
 ---
 ## TODO
 
 pyspark https://wiki.n.miui.com/pages/viewpage.action?pageId=477643956
 
 ---
 ![刷题](https://tva1.sinaimg.cn/large/008eGmZEly1gopa6fzuwwj30xj0u0ado.jpg)
```

### Comparing `MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/MeUtils.egg-info/requires.txt` & `MeUtils-2023.5.5.13.0.43/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -21,43 +21,43 @@
 schedule
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-missingno
-simplejson
-seaborn
-fastapi[all]
-pymongo
-iteration_utilities
-schedule
-thriftpy2
-redis-py-cluster
-faiss-gpu
 pandas-profiling[notebook]
-pymysql
-gensim
+uvicorn
+polars
 faiss-cpu
-thefuck
-streamlit
 pymupd
-geopy
-pretty_errors
-reportlab
-pandas_summary
-pymilvus
 jmespath
+schedule
+redis-py-cluster
 dataframe_image
+pymongo
+jinja2
+seaborn
+faiss-gpu
+simplejson
+pandas_summary
+thefuck
+pymilvus
+reportlab
+geopy
 jieba
 pyarrow
-polars
-uvicorn
-jinja2
+fastapi[all]
+gensim
+iteration_utilities
+streamlit
+missingno
+thriftpy2
+pymysql
+pretty_errors
 cachetools
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
```

### Comparing `MeUtils-2023.5.4.9.19.24/PKG-INFO` & `MeUtils-2023.5.5.13.0.43/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.5.4.9.19.24
+Version: 2023.5.5.13.0.43
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -71,14 +71,16 @@
 
 @wecom_hook('wecom_hook_test', 'Sleeping 3s')
 def wecom_hook_test():
     time.sleep(3)
 
 ```
 
+
+
 ---
 ## TODO
 
 pyspark https://wiki.n.miui.com/pages/viewpage.action?pageId=477643956
 
 ---
 ![刷题](https://tva1.sinaimg.cn/large/008eGmZEly1gopa6fzuwwj30xj0u0ado.jpg)
```

### Comparing `MeUtils-2023.5.4.9.19.24/README.md` & `MeUtils-2023.5.5.13.0.43/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 @wecom_hook('wecom_hook_test', 'Sleeping 3s')
 def wecom_hook_test():
     time.sleep(3)
 
 ```
 
+
+
 ---
 ## TODO
 
 pyspark https://wiki.n.miui.com/pages/viewpage.action?pageId=477643956
 
 ---
 ![刷题](https://tva1.sinaimg.cn/large/008eGmZEly1gopa6fzuwwj30xj0u0ado.jpg)
```

### Comparing `MeUtils-2023.5.4.9.19.24/clear_git_history.sh` & `MeUtils-2023.5.5.13.0.43/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/README.md` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/README_gensim.md` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_faiss.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_gensim.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_service.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/ann_v1.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/cli.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/examples/client.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/annzoo/shake_demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/annzoo/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/cache_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/cache_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,22 +39,17 @@
 # ME
 from meutils.decorators import decorator, singleton
 from meutils.hash_utils import md5
 
 TTLCache = lru_cache()(_TTLCache)
 
 
-def any2str(obj):
-    if hasattr(obj, 'tostring'):
-        obj = obj.tostring()
-    return md5(str(obj))
-
-
-def key_fn(*args, **kwargs):
-    return f"{args}_{kwargs}"
+def _pickle(obj, file):
+    with open(file) as f:
+        pickle.dump(obj, f)
 
 
 def map_cache():
     return cached({})
 
 
 def ttl_cache(ttl=60, maxsize=1024, key=keys.hashkey):
@@ -112,23 +107,25 @@
 def disk_cache(func, location='cachedir', maxsize=128, ttl=np.inf, *args, **kwargs):
     ttl_cache = _TTLCache(maxsize, ttl)  # 单例
 
     k = md5(f"cache_{func.__name__}_{args}_{kwargs}")
     output = Path(location) / Path(k) / '__output.pkl'
 
     if (ttl == np.inf or k in ttl_cache) and output.is_file():  # ttl=np.inf 不作key判断, 相当于maxsize无穷大
-        return joblib.load(output)
+        # return joblib.load(output)
+        return pickle.load(open(output, 'rb'))
 
     else:
         ttl_cache[k] = 0  # 更新cache
 
         logger.info(f"CacheKey: {k}")
         output.parent.mkdir(parents=True, exist_ok=True)
         _ = func(*args, **kwargs)
-        joblib.dump(_, output)
+        # joblib.dump(_, output)
+        pickle.dump(_, open(output, 'wb'))
         return _
 
 
 def mecache(location='mecache', maxsize=128, ttl=np.inf):
     ttl_cache = TTLCache(maxsize, ttl)
 
     @wrapt.decorator
```

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/cli.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/conf.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/cron.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/monitor.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/clis/nesc.py` & `MeUtils-2023.5.5.13.0.43/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/cmds/README.md` & `MeUtils-2023.5.5.13.0.43/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.5.5.13.0.43/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/coding/find132.py` & `MeUtils-2023.5.5.13.0.43/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/common.py` & `MeUtils-2023.5.5.13.0.43/meutils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.5.5.13.0.43/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/data/SimHei.ttf` & `MeUtils-2023.5.5.13.0.43/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/data/coordinate.py` & `MeUtils-2023.5.5.13.0.43/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/date_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/db/README.md` & `MeUtils-2023.5.5.13.0.43/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/db/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/db/mongo.py` & `MeUtils-2023.5.5.13.0.43/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/db/neo4j.py` & `MeUtils-2023.5.5.13.0.43/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/ai.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/catch.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/common.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         if torch.cuda.is_available():
             with torch.cuda.device(device):
                 torch.cuda.empty_cache()
                 torch.cuda.ipc_collect()
 
         elif torch.backends.mps.is_available():
             try:
-                from torch.mps import mps
-                torch.mps.empty_cache()
+                from torch.mps import empty_cache
+                empty_cache()
             except Exception as e:
                 logger.warning(f"仅支持pytorch2.x: {e}")
     return func(*args, **kwargs)
 
 
 @decorator
 def return2log(func, sink=sys.stderr, logkwargs=None, *args, **kwargs):
```

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/decorator.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/decorator_demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/feishu.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/retry.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/decorators/scheduler.py` & `MeUtils-2023.5.5.13.0.43/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/dist_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/annlite.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/base.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/chunk.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/document.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/elastic.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/match.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/memory.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/milvus.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/content.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/dataloader/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/dataloader/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/delitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/embed.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/empty.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/evaluation.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/getattr.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/getitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/group.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/binary.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/common.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/csv.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/dataframe.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/from_gen.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/json.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/pbar.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/io/pushpull.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/match.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/parallel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/plot.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/post.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/pydantic.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/reduce.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/sample.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/setitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/strawberry.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/text.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/mixins/traverse.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/opensearch.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/qdrant.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/lookup.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/queryset/parser.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/redis.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/sqlite.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/annlite/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/base/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/elastic/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/memory/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/milvus/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/opensearch/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/qdrant/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/redis/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/sqlite/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/storage/weaviate/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/array/weaviate.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/base.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/enums.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/getter.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/setter.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/dataclasses/types.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/data.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/generators.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/_property.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/attribute.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/audio.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/blob.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/content.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/convert.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/dump.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/featurehash.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/image.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/mesh.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/multimodal.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/plot.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/porting.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/property.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/protobuf.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/pydantic.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/rich_embedding.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/strawberry.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/sugar.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/text.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/mixins/video.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/pydantic_model.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/document/strawberry_type.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/numpy.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/paddle.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/tensorflow.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/distance/torch.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/evaluation.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/math/ndarray.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/io/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/io/ndarray.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb/docarray_pb2.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/proto/pb2/docarray_pb2.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/ci-vendors.json` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/resources/embedding-projector/index.html.gz` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/data.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/score/mixins/property.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_/typing/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.5.5.13.0.43/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/easy_search/es.py` & `MeUtils-2023.5.5.13.0.43/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/hash_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/import_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/init/oo.py` & `MeUtils-2023.5.5.13.0.43/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/io/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/io/image.py` & `MeUtils-2023.5.5.13.0.43/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/io/tf_io.py` & `MeUtils-2023.5.5.13.0.43/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/jinja_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/log_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/SplitSentence.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/_textsplitter/text_split.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/ner.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/textsplitter.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/nlp_utils/word_segmentation.py` & `MeUtils-2023.5.5.13.0.43/meutils/nlp_utils/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/emails.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/feishu.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/file_post.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/wechat.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/wechat_.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/wecom.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/notice/weekmeet.py` & `MeUtils-2023.5.5.13.0.43/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/np_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdf.py` & `MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdm.py` & `MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/office_automation/pdm_run.py` & `MeUtils-2023.5.5.13.0.43/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.5.5.13.0.43/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/besttable.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/crontab.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/annlite.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/base.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/chunk.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/document.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/elastic.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/match.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/memory.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/milvus.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/content.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/dataloader/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/dataloader/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/delitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/embed.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/empty.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/evaluation.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/getattr.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/getitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/group.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/binary.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/common.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/csv.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/dataframe.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/from_gen.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/json.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/pbar.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/io/pushpull.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/match.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/parallel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/plot.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/post.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/pydantic.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/reduce.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/sample.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/setitem.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/strawberry.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/text.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/mixins/traverse.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/opensearch.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/qdrant.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/lookup.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/queryset/parser.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/redis.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/sqlite.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/annlite/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/base/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/elastic/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/memory/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/milvus/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/opensearch/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/qdrant/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/redis/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/sqlite/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/backend.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/find.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/storage/weaviate/seqlike.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/array/weaviate.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/base.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/enums.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/getter.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/setter.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/dataclasses/types.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/data.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/generators.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/_property.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/attribute.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/audio.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/blob.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/content.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/convert.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/dump.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/featurehash.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/image.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/mesh.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/multimodal.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/plot.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/porting.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/property.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/protobuf.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/pydantic.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/rich_embedding.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/strawberry.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/sugar.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/text.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/mixins/video.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/pydantic_model.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/document/strawberry_type.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/numpy.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/paddle.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/tensorflow.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/distance/torch.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/evaluation.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/helper.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/math/ndarray.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/io/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/io/ndarray.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb/docarray_pb2.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/proto/pb2/docarray_pb2.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/ci-vendors.json` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/resources/embedding-projector/index.html.gz` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/data.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/score/mixins/property.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/other/docarray/typing/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/opt.py` & `MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/path_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/pd_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/pipe.py` & `MeUtils-2023.5.5.13.0.43/meutils/pipe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/plot/demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/plot/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/plot/echarts.py` & `MeUtils-2023.5.5.13.0.43/meutils/plot/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/plot/mecharts.py` & `MeUtils-2023.5.5.13.0.43/meutils/plot/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/plot/metrics.py` & `MeUtils-2023.5.5.13.0.43/meutils/plot/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/plot/plot_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/plot/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/request_utils/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/request_utils/crawler.py` & `MeUtils-2023.5.5.13.0.43/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/request_utils/download.py` & `MeUtils-2023.5.5.13.0.43/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/request_utils/results.py` & `MeUtils-2023.5.5.13.0.43/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/request_utils/公网ip.py` & `MeUtils-2023.5.5.13.0.43/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/serving/_fastapi.py` & `MeUtils-2023.5.5.13.0.43/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/serving/gui/bar.py` & `MeUtils-2023.5.5.13.0.43/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/serving/gui/demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/_test.py` & `MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/serving/st_utils/common.py` & `MeUtils-2023.5.5.13.0.43/meutils/serving/st_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/sftp.py` & `MeUtils-2023.5.5.13.0.43/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/sk_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/smooth_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/spark/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/Translator.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/__init__.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/json_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/str_utils/regular_expression.py` & `MeUtils-2023.5.5.13.0.43/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/demo.j2` & `MeUtils-2023.5.5.13.0.43/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/demo.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/demox.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/df_html.j2` & `MeUtils-2023.5.5.13.0.43/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/hegui.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.5.5.13.0.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/tpl.docx` & `MeUtils-2023.5.5.13.0.43/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/templates/合规日报模板.docx` & `MeUtils-2023.5.5.13.0.43/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/tools/cprint.py` & `MeUtils-2023.5.5.13.0.43/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/tools/machine_monitor.py` & `MeUtils-2023.5.5.13.0.43/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/tools/monitor.yml` & `MeUtils-2023.5.5.13.0.43/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/tools/seize.py` & `MeUtils-2023.5.5.13.0.43/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/tools/service_monitor.py` & `MeUtils-2023.5.5.13.0.43/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/meutils/zk_utils.py` & `MeUtils-2023.5.5.13.0.43/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/pypi.sh` & `MeUtils-2023.5.5.13.0.43/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.4.9.19.24/setup.py` & `MeUtils-2023.5.5.13.0.43/setup.py`

 * *Files identical despite different names*

