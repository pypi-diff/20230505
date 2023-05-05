# Comparing `tmp/INGInious-0.8.6.tar.gz` & `tmp/INGInious-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "INGInious-0.8.6.tar", last modified: Wed Apr 26 10:06:31 2023, max compression
+gzip compressed data, was "INGInious-0.8.7.tar", last modified: Fri May  5 06:41:51 2023, max compression
```

## Comparing `INGInious-0.8.6.tar` & `INGInious-0.8.7.tar`

### file list

```diff
@@ -1,1018 +1,1018 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.164087 INGInious-0.8.6/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.030087 INGInious-0.8.6/.github/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.042086 INGInious-0.8.6/.github/workflows/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1850 2023-04-26 09:42:50.000000 INGInious-0.8.6/.github/workflows/ci.yml
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      422 2022-02-09 10:08:57.000000 INGInious-0.8.6/.gitignore
--rw-r--r--   0 anthony   (1000) anthony   (1000)       22 2018-11-16 12:58:08.000000 INGInious-0.8.6/.landscape.yml
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10147 2018-11-16 12:58:08.000000 INGInious-0.8.6/.pylintrc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      156 2021-06-10 10:07:01.000000 INGInious-0.8.6/.readthedocs.yaml
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1581 2018-11-16 12:58:08.000000 INGInious-0.8.6/.travis.yml
--rw-r--r--   0 anthony   (1000) anthony   (1000)      622 2023-03-14 08:45:50.000000 INGInious-0.8.6/COPYRIGHTS
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.043087 INGInious-0.8.6/INGInious.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)    40029 2023-04-26 10:06:31.000000 INGInious-0.8.6/INGInious.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)      658 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34764 2018-11-16 12:58:08.000000 INGInious-0.8.6/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      440 2018-11-16 12:58:08.000000 INGInious-0.8.6/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-04-26 10:06:31.163087 INGInious-0.8.6/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2688 2023-04-26 09:42:50.000000 INGInious-0.8.6/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.030087 INGInious-0.8.6/base-containers/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.043087 INGInious-0.8.6/base-containers/base/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1927 2022-07-12 07:33:48.000000 INGInious-0.8.6/base-containers/base/Dockerfile
--rw-r--r--   0 anthony   (1000) anthony   (1000)      610 2018-11-16 12:58:08.000000 INGInious-0.8.6/base-containers/base/README.md
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.045086 INGInious-0.8.6/base-containers/base/bin/
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    19095 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/bin/INGInious
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     5040 2022-03-18 07:57:30.000000 INGInious-0.8.6/base-containers/base/bin/_run_student_intern
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1418 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/archive
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2830 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1088 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-custom
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      549 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-grade
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1306 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-msg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1533 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-msg-tpl
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      812 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-result
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-state
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1180 2021-06-10 10:07:01.000000 INGInious-0.8.6/base-containers/base/bin/getinput
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1090 2022-02-08 16:02:58.000000 INGInious-0.8.6/base-containers/base/bin/inginious-ipython
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1066 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/parsetemplate
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1064 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-code
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      737 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-image
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1277 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-indent
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1223 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-msgblock
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2752 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/bin/run_student
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2953 2022-02-09 08:29:26.000000 INGInious-0.8.6/base-containers/base/bin/ssh_student
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)      491 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/tag
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)      623 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/tag-set
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.047087 INGInious-0.8.6/base-containers/base/inginious_container_api/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       30 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6616 2022-02-09 10:08:57.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/feedback.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3400 2021-06-10 10:07:01.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/input.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      789 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/lang.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1704 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/rst.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16470 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/run_student.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      466 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/run_types.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3065 2022-02-09 08:57:05.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/ssh_student.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    13519 2022-03-30 06:18:20.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/utils.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.047087 INGInious-0.8.6/base-containers/default/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      210 2021-02-12 07:54:48.000000 INGInious-0.8.6/base-containers/default/Dockerfile
--rw-r--r--   0 anthony   (1000) anthony   (1000)      378 2018-11-16 12:58:08.000000 INGInious-0.8.6/base-containers/default/README.md
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2068 2021-06-10 10:07:01.000000 INGInious-0.8.6/configuration.example.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.049087 INGInious-0.8.6/doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6910 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/Makefile
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/doc/admin_doc/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.050087 INGInious-0.8.6/doc/admin_doc/commands_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2703 2022-02-09 10:08:57.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-docker.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      824 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-mcq.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1192 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-autotest.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      881 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-backend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      336 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-container-update.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      407 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-database-update.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-install.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1297 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-synchronize.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webapp.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webdav.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.051087 INGInious-0.8.6/doc/admin_doc/install_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    18632 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/config_reference.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9220 2023-03-28 13:39:50.000000 INGInious-0.8.6/doc/admin_doc/install_doc/create_container.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    21186 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/admin_doc/install_doc/installation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2094 2022-02-09 08:57:05.000000 INGInious-0.8.6/doc/admin_doc/install_doc/other_oci_runtimes_support.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1350 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/static_pages.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3847 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/troubleshooting.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1342 2022-02-09 08:22:39.000000 INGInious-0.8.6/doc/admin_doc/install_doc/updating.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1172 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/admin_documentation.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.054087 INGInious-0.8.6/doc/api_doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      506 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.agent.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      336 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.backend.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      715 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.client.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      414 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/api_doc/inginious.common.filesystems.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1495 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/api_doc/inginious.common.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      692 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.common.task_file_readers.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      570 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.common.tests.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1286 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.api.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2429 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.course_admin.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1474 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      664 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.auth.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1146 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      212 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.scoreboard.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3200 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1483 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.tests.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      324 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10661 2023-03-14 08:45:50.000000 INGInious-0.8.6/doc/conf.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/doc/dev_doc/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.054087 INGInious-0.8.6/doc/dev_doc/extensions_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1902 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/how_to_extend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      753 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/i18n.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16600 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/plugins.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.057087 INGInious-0.8.6/doc/dev_doc/internals_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2083 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/architectures.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2309 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/exercises.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1217 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/frontend.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       37 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/groupes_audiences.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    71784 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    97918 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_docker.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)   119437 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_full.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    20901 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submission_evaluation_docker.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    51028 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submission_workflow.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5607 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submissions.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3834 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/understand_inginious.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      618 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/developer_documentation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      297 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/index.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11703 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/logo_rtd.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6707 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/make.bat
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/doc/teacher_doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4806 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/best_practices.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      952 2021-04-26 06:37:40.000000 INGInious-0.8.6/doc/teacher_doc/common.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11047 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/teacher_doc/course_admin.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4106 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/course_description.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1093 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/course_tuto.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      921 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/courses.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1168 2022-02-08 16:02:58.000000 INGInious-0.8.6/doc/teacher_doc/inginious_container_api.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3025 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/teacher_doc/lti.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1856 2021-04-26 06:37:40.000000 INGInious-0.8.6/doc/teacher_doc/random.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5807 2022-08-11 06:40:58.000000 INGInious-0.8.6/doc/teacher_doc/rst.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34270 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/teacher_doc/run_file.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      764 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/share_files.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      975 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/system_files.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9474 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/task_file.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5397 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/task_tuto.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/tasks.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1676 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/testing.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3060 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/translating.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      197 2022-02-09 08:22:39.000000 INGInious-0.8.6/doc/teacher_documentation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5111 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/what_is_inginious.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/inginious/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      709 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/inginious/agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11964 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/agent/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/docker_agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    50851 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/agent/docker_agent/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13345 2023-03-28 13:39:50.000000 INGInious-0.8.6/inginious/agent/docker_agent/_docker_interface.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      858 2023-03-28 13:39:50.000000 INGInious-0.8.6/inginious/agent/docker_agent/_docker_runtime.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4597 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/agent/docker_agent/_timeout_watcher.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6721 2022-08-30 07:08:17.000000 INGInious-0.8.6/inginious/agent/mcq_agent/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       42 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/agent/mcq_agent/babel.cfg
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1037 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1505 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1051 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1525 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1059 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1530 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1109 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/messages.pot
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/backend/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/backend/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22389 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/backend/backend.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1894 2022-02-09 08:29:26.000000 INGInious-0.8.6/inginious/backend/topic_priority_queue.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.063087 INGInious-0.8.6/inginious/client/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/client/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9874 2023-02-23 07:55:28.000000 INGInious-0.8.6/inginious/client/_zeromq_client.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    16216 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/client/client.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2541 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/client/client_buffer.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1271 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/client/client_sync.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.065087 INGInious-0.8.6/inginious/common/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      242 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2607 2023-02-23 07:55:28.000000 INGInious-0.8.6/inginious/common/asyncio_utils.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2458 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/babel.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4805 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/common/base.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3124 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/common/custom_yaml.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4275 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/entrypoints.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      701 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/common/exceptions.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.065087 INGInious-0.8.6/inginious/common/filesystems/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5291 2022-03-18 07:57:30.000000 INGInious-0.8.6/inginious/common/filesystems/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6096 2022-12-14 10:14:50.000000 INGInious-0.8.6/inginious/common/filesystems/local.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2131 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/common/log.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14490 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/common/messages.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2672 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/common/tags.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.066087 INGInious-0.8.6/inginious/common/task_file_readers/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      224 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      755 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/abstract_reader.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      650 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/yaml_reader.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14652 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tasks_problems.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.066087 INGInious-0.8.6/inginious/common/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5009 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tests/TestBase.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2823 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tests/TestCustomYaml.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      206 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/tests/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    12982 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/common/tests/test_filesystem_local.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.069087 INGInious-0.8.6/inginious/frontend/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2022-03-18 08:08:05.000000 INGInious-0.8.6/inginious/frontend/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5943 2022-02-09 08:22:39.000000 INGInious-0.8.6/inginious/frontend/accessible_time.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15300 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/app.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4770 2023-04-20 07:54:08.000000 INGInious-0.8.6/inginious/frontend/arch_helper.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      138 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/babel.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10782 2022-03-18 08:08:05.000000 INGInious-0.8.6/inginious/frontend/course_factory.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11693 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/courses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.070087 INGInious-0.8.6/inginious/frontend/environment_types/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1022 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      447 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/docker.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      920 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/environment_types/env_type.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2067 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/generic_docker_oci_runtime.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      395 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/kata.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      408 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/environment_types/mcq.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      393 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/nvidia.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/flask/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      157 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/flask/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/flask/mail.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11759 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/flask/mapping.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5564 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/flask/mongo_sessions.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/de/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25694 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   110889 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/el/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    29887 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   119743 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/es/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    47593 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   132063 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/fr/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    60340 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   127508 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/he/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    68397 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   130391 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.po
--rw-r--r--   0 anthony   (1000) anthony   (1000)    99891 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/messages.pot
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/nl/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4937 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   102119 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/pt/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24190 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   119920 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      530 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/vi/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.074087 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34450 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   118219 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/wa/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.074087 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2170 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   100743 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po
--rw-r--r--   0 anthony   (1000) anthony   (1000)    27989 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/installer.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      639 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/l10n_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4924 2021-02-19 11:28:54.000000 INGInious-0.8.6/inginious/frontend/lti_outcome_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2061 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/lti_request_validator.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      777 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/lti_tool_provider.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3385 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/marketplace_courses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.076087 INGInious-0.8.6/inginious/frontend/pages/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      196 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.077087 INGInious-0.8.6/inginious/frontend/pages/admin/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      199 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/admin/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2944 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/admin/admin.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.078087 INGInious-0.8.6/inginious/frontend/pages/api/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      191 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/api/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6726 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/_api_page.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1476 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/auth_methods.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1615 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/authentication.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2946 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/courses.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8534 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/api/submissions.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4517 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/api/tasks.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4502 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.080087 INGInious-0.8.6/inginious/frontend/pages/course_admin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      189 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5328 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/audience_edit.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10305 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/danger_zone.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1425 2023-03-23 10:48:36.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/search_user.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5138 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/settings.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13926 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/statistics.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2690 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/student_info.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18777 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/student_list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3489 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/submission.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12967 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/submissions.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2377 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/tags.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13627 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11817 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit_file.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5408 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16859 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/utils.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1811 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_register.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1240 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/courselist.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4503 2022-03-18 07:57:30.000000 INGInious-0.8.6/inginious/frontend/pages/group.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      813 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/index.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    12033 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/pages/lti.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      571 2021-07-15 06:35:04.000000 INGInious-0.8.6/inginious/frontend/pages/maintenance.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3957 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/marketplace.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2326 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/marketplace_course.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3020 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/mycourses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.081086 INGInious-0.8.6/inginious/frontend/pages/preferences/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      179 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2090 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/bindings.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1950 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/delete.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6131 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/profile.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1396 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/utils.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      981 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/queue.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9157 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/register.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3533 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/social.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22133 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/tasks.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    14567 2022-08-03 10:55:31.000000 INGInious-0.8.6/inginious/frontend/pages/utils.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13757 2022-12-14 10:19:50.000000 INGInious-0.8.6/inginious/frontend/parsable_text.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4724 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugin_manager.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.081086 INGInious-0.8.6/inginious/frontend/plugins/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      203 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/plugins/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.082087 INGInious-0.8.6/inginious/frontend/plugins/auth/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      180 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.085087 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      210 2022-01-01 20:58:44.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      200 2021-02-26 16:21:15.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      204 2021-02-26 10:55:03.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-04-21 06:41:19.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-02-26 10:50:17.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3416 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3372 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3442 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3426 2021-06-18 12:47:24.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6216 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6129 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6096 2021-03-01 12:53:51.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6226 2023-02-28 09:14:23.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6232 2021-10-25 13:22:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6434 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6394 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6389 2021-03-01 13:00:13.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6466 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6464 2021-06-18 12:47:24.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1691 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/custom_auth_form.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4075 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/facebook_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2665 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/github_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2979 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/google_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7358 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/ldap_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3082 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/linkedin_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7053 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/saml2_auth.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4317 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/twitter_auth.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.086087 INGInious-0.8.6/inginious/frontend/plugins/contests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11265 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7900 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7995 2021-03-01 12:53:52.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7976 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7930 2021-04-29 09:45:18.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5410 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/admin.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1671 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/course_menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4223 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/scoreboard.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/demo/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      583 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/demo/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/git_repo/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4807 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/git_repo/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3438 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.088087 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9753 2022-07-12 06:51:08.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6649 2022-03-30 09:15:04.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6798 2021-03-01 12:53:52.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6738 2021-04-21 06:41:19.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6731 2021-04-29 09:45:18.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      354 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/course_menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1220 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/main.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1418 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/scoreboard.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      425 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/task_menu.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/simple_grader/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6106 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/simple_grader/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1363 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      816 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      212 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      976 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/json_reader.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6301 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4945 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      198 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/main_menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      358 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2803 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.039086 INGInious-0.8.6/inginious/frontend/static/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.091087 INGInious-0.8.6/inginious/frontend/static/css/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11071 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/INGInious.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3518 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/INGInious.less
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9063 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/css/bootstrap-datetimepicker.min.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)   134084 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8217 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/css/codemirror.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9044 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/static/css/common.less
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31000 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/css/font-awesome.min.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7996 2021-06-18 12:47:19.000000 INGInious-0.8.6/inginious/frontend/static/css/lti.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      254 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/css/lti.less
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11150 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/css/selectize.css
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.096087 INGInious-0.8.6/inginious/frontend/static/fonts/
--rw-r--r--   0 anthony   (1000) anthony   (1000)   134808 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/FontAwesome.otf
--rw-r--r--   0 anthony   (1000) anthony   (1000)   165742 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 anthony   (1000) anthony   (1000)   444379 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)   165548 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 anthony   (1000) anthony   (1000)    98024 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 anthony   (1000) anthony   (1000)    77160 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 anthony   (1000) anthony   (1000)    20127 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 anthony   (1000) anthony   (1000)   108738 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)    45404 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 anthony   (1000) anthony   (1000)    23424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18028 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.100087 INGInious-0.8.6/inginious/frontend/static/icons/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1856 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1844 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2259 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1020 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1101 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1241 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1294 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2810 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      371 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/browserconfig.xml
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3475 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-160x160.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      535 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-16x16.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2870 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-196x196.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      928 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-32x32.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2226 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-96x96.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15086 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon.ico
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4358 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/google-icon.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3186 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-144x144.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2135 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-150x150.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1829 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x150.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3819 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x310.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1970 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-70x70.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2531 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/wb.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1573 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/wb.svg
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.101087 INGInious-0.8.6/inginious/frontend/static/images/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5244 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/header.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6681 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_full.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6531 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_full_logo_only.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4730 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_horiz.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4728 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_vert.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14493 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/logo.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13380 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/logo_maintenance.png
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.103087 INGInious-0.8.6/inginious/frontend/static/js/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2445 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/static/js/admin.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)   638597 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/all-minified.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3828 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/static/js/audiences.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2838 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/checked-list-group.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.103087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1107 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)   205623 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/codemirror.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4736 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/apl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2179 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2378 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1289 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7735 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2222 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7437 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4591 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3338 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.106087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31062 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/clike.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10105 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    28518 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/scala.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16005 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2550 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2600 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4152 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10288 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8084 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9884 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22402 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4569 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6691 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12818 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2605 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    37613 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/css.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2780 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      460 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1911 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4066 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1871 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2742 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss_test.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6362 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1908 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/d.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6332 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5124 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/dart.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1627 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1138 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/diff.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4409 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11791 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/django.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2077 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2221 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2267 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4814 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3337 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10112 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13032 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.113087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6085 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2450 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.114087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8843 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1409 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.114087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3744 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13198 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5552 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/elm.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1640 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18887 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2168 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3565 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/factor.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2024 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4703 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3091 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5230 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/forth.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1783 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8686 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2492 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8886 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/gas.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5103 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2583 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13257 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6030 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/go.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7904 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2177 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5353 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/haml.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2071 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2172 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2196 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8109 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2194 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1390 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9381 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17563 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1417 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2086 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5611 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3434 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2795 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/http.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1393 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.121087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14889 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/idl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1633 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8286 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.121087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4193 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2150 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1557 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1755 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4279 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2410 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5195 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2375 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12089 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/julia.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9843 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7668 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2073 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/lua.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10957 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25671 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2254 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5612 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1293 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3649 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/meta.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5798 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10077 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.125087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4436 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5097 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.125087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2007 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6930 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4310 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6820 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3795 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3255 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4006 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2608 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5354 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5239 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10164 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7642 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1357 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6643 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1805 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4522 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/octave.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1389 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6665 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/oz.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1440 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3055 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1890 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1542 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    56135 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/perl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.129087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1999 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18224 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/php.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.129087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1475 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5810 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/pig.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7372 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12896 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1555 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/properties.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1680 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2113 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2489 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16046 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/pug.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3260 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7568 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12479 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/python.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8961 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6593 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/q.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2518 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6396 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/r.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2180 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4623 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3775 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17769 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17547 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/rst.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5749 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10516 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1532 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3025 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/rust.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1854 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/index.html
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    15424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/sas.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11509 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/sass.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2554 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13437 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4002 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/shell.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2335 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4284 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2920 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18026 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/slim.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1904 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4543 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3973 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6828 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1365 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2672 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/solr.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1939 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12239 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/soy.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1773 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6335 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1392 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3139 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2991 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    37351 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/sql.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4132 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6932 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/stex.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2472 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    42256 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2085 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7168 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/swift.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6297 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4920 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4347 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13835 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/textile.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      220 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8510 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      439 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8462 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2897 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/toml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1803 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4465 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2392 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/troff.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3490 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10155 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3605 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7857 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1470 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4849 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1370 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4565 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/twig.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1500 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8734 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/vb.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1517 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13793 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3300 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2619 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24588 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2486 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6704 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2064 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2544 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/vue.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5784 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12570 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8609 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14470 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2176 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.146087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3693 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.146087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3072 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2292 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.147087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1406 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/z80.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6370 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/common.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7286 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/groups.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.149087 INGInious-0.8.6/inginious/frontend/static/js/libs/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    42997 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/Sortable.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    56581 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    51039 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)   158741 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/chart.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15252 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.form.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    86926 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6542 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    51679 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/moment.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    20535 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/popper.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    41501 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/selectize.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    50945 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/sentry-io-bundle.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24394 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/studio.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    30954 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/task.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16389 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/task_dispensers.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      727 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/webapp.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.039086 INGInious-0.8.6/inginious/frontend/static/plugins/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.150087 INGInious-0.8.6/inginious/frontend/static/plugins/contests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1413 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/contests.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/jquery.countdown.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)      996 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/scoreboard.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)    36374 2023-04-26 09:57:12.000000 INGInious-0.8.6/inginious/frontend/submission_manager.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.150087 INGInious-0.8.6/inginious/frontend/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3324 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/combinatory_test.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2957 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/toc.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7041 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/util.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13648 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_factory.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9078 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_problems.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11846 2023-04-26 09:54:11.000000 INGInious-0.8.6/inginious/frontend/tasks.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6972 2022-02-09 08:21:51.000000 INGInious-0.8.6/inginious/frontend/template_helper.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.154087 INGInious-0.8.6/inginious/frontend/templates/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.154087 INGInious-0.8.6/inginious/frontend/templates/admin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12064 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/admin/admin_users.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2986 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/auth.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7753 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9319 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/audience_edit.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10121 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/danger_zone.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14096 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/basic.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3102 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1846 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/environment.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1776 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3675 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/files.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1085 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      913 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18882 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/settings.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    14180 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/stats.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6499 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_info.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    28812 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5905 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list_table.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7590 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submission.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12969 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17267 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions_query.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2032 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/code.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1332 2023-02-27 12:38:00.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/file.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1050 2023-03-23 10:48:36.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/match.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2826 2022-02-09 08:22:39.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2174 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5141 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/tags.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.157087 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1698 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1225 2023-01-11 09:03:30.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1795 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      894 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_config.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1352 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1249 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2322 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1003 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/toc.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4564 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2481 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9608 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_edit.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5346 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_list.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      476 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/user_selection_box.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2034 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_register.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1573 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_unavailable.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4040 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/courselist.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      493 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/forbidden.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8084 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/group.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      667 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/internalerror.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13580 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/layout.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2128 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/lti_bind.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1462 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/lti_login.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      572 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/maintenance.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4826 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/marketplace.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2796 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/marketplace_course.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5383 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/mycourses.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      492 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/notfound.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.158087 INGInious-0.8.6/inginious/frontend/templates/preferences/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3987 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/bindings.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2872 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/delete.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      469 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4723 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/profile.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4845 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/queue.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5245 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/register.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      539 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/signin_button.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      271 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/static.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25388 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.158087 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3268 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/task_list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1819 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/toc.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      513 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/task_unavailable.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.159087 INGInious-0.8.6/inginious/frontend/templates/tasks/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      528 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/code.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1039 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/file.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      307 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/match.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      644 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/multiple_choice.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      640 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/single_line_code.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1430 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/unregister_modal.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16896 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/SeleniumFormatter.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6346 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/SeleniumTest.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4326 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestCourse.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3383 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestLogin.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2639 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestParsableText.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      972 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestPluginManager.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7381 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTask.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1841 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTaskDisplay.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1975 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTaskSubmission.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/tests/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.040087 INGInious-0.8.6/inginious/frontend/tests/tasks/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/invalid_course/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       72 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/invalid_course/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       73 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/run
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      573 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task2/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/run
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      363 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task4/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task4/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task1/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task1/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      339 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task2/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      559 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task4/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task4/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      122 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/course.json
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/invalid_task/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       34 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/invalid_task/task.yaml
--rw-r--r--   0 anthony   (1000) anthony   (1000)    44783 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/user_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9056 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/webdav.py
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     6462 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious-agent-docker
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3404 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-agent-mcq
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    12793 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious-autotest
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2162 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious-backend
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)      649 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious-install
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3981 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-webapp
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3038 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-webdav
--rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-04-26 10:06:31.164087 INGInious-0.8.6/setup.cfg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2441 2023-04-26 09:42:50.000000 INGInious-0.8.6/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.040087 INGInious-0.8.6/utils/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/utils/container_update/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3199 2022-02-09 10:08:57.000000 INGInious-0.8.6/utils/container_update/inginious-container-update
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/utils/database_updater/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     4682 2022-02-09 10:08:57.000000 INGInious-0.8.6/utils/database_updater/inginious-database-update
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.163087 INGInious-0.8.6/utils/minify/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2728 2023-04-26 09:42:50.000000 INGInious-0.8.6/utils/minify/Gruntfile.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)      452 2023-04-26 09:42:50.000000 INGInious-0.8.6/utils/minify/package.json
--rw-r--r--   0 anthony   (1000) anthony   (1000)      936 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/minify/watchers.xml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.163087 INGInious-0.8.6/utils/sync/
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3220 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/sync/inginious-synchronize
--rw-r--r--   0 anthony   (1000) anthony   (1000)      349 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/sync/synchronize.json.example
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.124490 INGInious-0.8.7/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.011489 INGInious-0.8.7/.github/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.026490 INGInious-0.8.7/.github/workflows/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1850 2023-05-05 06:37:55.000000 INGInious-0.8.7/.github/workflows/ci.yml
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      422 2022-02-09 10:08:57.000000 INGInious-0.8.7/.gitignore
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       22 2018-11-16 12:58:08.000000 INGInious-0.8.7/.landscape.yml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10147 2018-11-16 12:58:08.000000 INGInious-0.8.7/.pylintrc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      156 2021-06-10 10:07:01.000000 INGInious-0.8.7/.readthedocs.yaml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1581 2018-11-16 12:58:08.000000 INGInious-0.8.7/.travis.yml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      622 2023-03-14 08:45:50.000000 INGInious-0.8.7/COPYRIGHTS
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.027490 INGInious-0.8.7/INGInious.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-05-05 06:41:50.000000 INGInious-0.8.7/INGInious.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    40029 2023-05-05 06:41:50.000000 INGInious-0.8.7/INGInious.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-05-05 06:41:50.000000 INGInious-0.8.7/INGInious.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      674 2023-05-05 06:41:50.000000 INGInious-0.8.7/INGInious.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2023-05-05 06:41:50.000000 INGInious-0.8.7/INGInious.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34764 2018-11-16 12:58:08.000000 INGInious-0.8.7/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      440 2018-11-16 12:58:08.000000 INGInious-0.8.7/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-05-05 06:41:51.124490 INGInious-0.8.7/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2688 2023-05-05 06:37:55.000000 INGInious-0.8.7/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.011489 INGInious-0.8.7/base-containers/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.027490 INGInious-0.8.7/base-containers/base/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1927 2022-07-12 07:33:48.000000 INGInious-0.8.7/base-containers/base/Dockerfile
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      610 2018-11-16 12:58:08.000000 INGInious-0.8.7/base-containers/base/README.md
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.030490 INGInious-0.8.7/base-containers/base/bin/
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    19095 2023-02-28 09:27:21.000000 INGInious-0.8.7/base-containers/base/bin/INGInious
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     5040 2022-03-18 07:57:30.000000 INGInious-0.8.7/base-containers/base/bin/_run_student_intern
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1418 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/archive
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2830 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1088 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-custom
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      549 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-grade
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1306 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-msg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1533 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-msg-tpl
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      812 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-result
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/feedback-state
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1180 2021-06-10 10:07:01.000000 INGInious-0.8.7/base-containers/base/bin/getinput
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1090 2022-02-08 16:02:58.000000 INGInious-0.8.7/base-containers/base/bin/inginious-ipython
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1066 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/parsetemplate
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1064 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/rst-code
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      737 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/rst-image
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1277 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/rst-indent
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1223 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/rst-msgblock
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2752 2023-02-28 09:27:21.000000 INGInious-0.8.7/base-containers/base/bin/run_student
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2953 2022-02-09 08:29:26.000000 INGInious-0.8.7/base-containers/base/bin/ssh_student
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)      491 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/tag
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)      623 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/bin/tag-set
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.032490 INGInious-0.8.7/base-containers/base/inginious_container_api/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       30 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6616 2022-02-09 10:08:57.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/feedback.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3400 2021-06-10 10:07:01.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/input.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      789 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/lang.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1704 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/rst.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16470 2023-02-28 09:27:21.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/run_student.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      466 2021-04-26 06:37:40.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/run_types.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3065 2022-02-09 08:57:05.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/ssh_student.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    13519 2022-03-30 06:18:20.000000 INGInious-0.8.7/base-containers/base/inginious_container_api/utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.032490 INGInious-0.8.7/base-containers/default/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      210 2021-02-12 07:54:48.000000 INGInious-0.8.7/base-containers/default/Dockerfile
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      378 2018-11-16 12:58:08.000000 INGInious-0.8.7/base-containers/default/README.md
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2068 2021-06-10 10:07:01.000000 INGInious-0.8.7/configuration.example.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.034489 INGInious-0.8.7/doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6910 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/Makefile
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.012489 INGInious-0.8.7/doc/admin_doc/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.035489 INGInious-0.8.7/doc/admin_doc/commands_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2703 2022-02-09 10:08:57.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-agent-docker.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      824 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-agent-mcq.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1192 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-autotest.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      881 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-backend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      336 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-container-update.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      407 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-database-update.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-install.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1297 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-synchronize.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-webapp.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-webdav.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.037490 INGInious-0.8.7/doc/admin_doc/install_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    18632 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/install_doc/config_reference.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9220 2023-03-28 13:39:50.000000 INGInious-0.8.7/doc/admin_doc/install_doc/create_container.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    21186 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/admin_doc/install_doc/installation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2094 2022-02-09 08:57:05.000000 INGInious-0.8.7/doc/admin_doc/install_doc/other_oci_runtimes_support.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1350 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/install_doc/static_pages.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3847 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/admin_doc/install_doc/troubleshooting.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1342 2022-02-09 08:22:39.000000 INGInious-0.8.7/doc/admin_doc/install_doc/updating.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1172 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/admin_documentation.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.040490 INGInious-0.8.7/doc/api_doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      506 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.agent.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      336 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.backend.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      715 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.client.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      414 2022-03-18 07:57:30.000000 INGInious-0.8.7/doc/api_doc/inginious.common.filesystems.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1495 2022-03-18 07:57:30.000000 INGInious-0.8.7/doc/api_doc/inginious.common.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      692 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.common.task_file_readers.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      570 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.common.tests.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1286 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.api.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2429 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.course_admin.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1474 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      664 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.plugins.auth.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1146 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.plugins.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      212 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.plugins.scoreboard.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3200 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1483 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.frontend.tests.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      324 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/api_doc/inginious.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10661 2023-03-14 08:45:50.000000 INGInious-0.8.7/doc/conf.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.012489 INGInious-0.8.7/doc/dev_doc/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.040490 INGInious-0.8.7/doc/dev_doc/extensions_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1902 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/extensions_doc/how_to_extend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      753 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/extensions_doc/i18n.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16600 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/dev_doc/extensions_doc/plugins.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.043490 INGInious-0.8.7/doc/dev_doc/internals_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2083 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/architectures.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2309 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/exercises.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1217 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/frontend.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       37 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/groupes_audiences.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    71784 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    97918 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch_docker.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)   119437 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch_full.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    20901 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/submission_evaluation_docker.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    51028 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/submission_workflow.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5607 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/submissions.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3834 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/dev_doc/internals_doc/understand_inginious.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      618 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/developer_documentation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      297 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/index.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11703 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/logo_rtd.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6707 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/make.bat
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.046490 INGInious-0.8.7/doc/teacher_doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4806 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/teacher_doc/best_practices.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      952 2021-04-26 06:37:40.000000 INGInious-0.8.7/doc/teacher_doc/common.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11047 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/teacher_doc/course_admin.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4106 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/course_description.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1093 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/course_tuto.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      921 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/courses.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1168 2022-02-08 16:02:58.000000 INGInious-0.8.7/doc/teacher_doc/inginious_container_api.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3025 2022-03-18 07:57:30.000000 INGInious-0.8.7/doc/teacher_doc/lti.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1856 2021-04-26 06:37:40.000000 INGInious-0.8.7/doc/teacher_doc/random.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5807 2022-08-11 06:40:58.000000 INGInious-0.8.7/doc/teacher_doc/rst.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34270 2023-05-05 06:37:55.000000 INGInious-0.8.7/doc/teacher_doc/run_file.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      764 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/teacher_doc/share_files.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      975 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/teacher_doc/system_files.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9474 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/task_file.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5397 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/task_tuto.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/tasks.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1676 2018-11-16 12:58:08.000000 INGInious-0.8.7/doc/teacher_doc/testing.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3060 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/teacher_doc/translating.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      197 2022-02-09 08:22:39.000000 INGInious-0.8.7/doc/teacher_documentation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5111 2021-06-10 10:07:01.000000 INGInious-0.8.7/doc/what_is_inginious.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.046490 INGInious-0.8.7/inginious/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      709 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.047490 INGInious-0.8.7/inginious/agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11964 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/agent/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.047490 INGInious-0.8.7/inginious/agent/docker_agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    50851 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/agent/docker_agent/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13345 2023-03-28 13:39:50.000000 INGInious-0.8.7/inginious/agent/docker_agent/_docker_interface.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      858 2023-03-28 13:39:50.000000 INGInious-0.8.7/inginious/agent/docker_agent/_docker_runtime.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4597 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/agent/docker_agent/_timeout_watcher.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.047490 INGInious-0.8.7/inginious/agent/mcq_agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6721 2022-08-30 07:08:17.000000 INGInious-0.8.7/inginious/agent/mcq_agent/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       42 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/agent/mcq_agent/babel.cfg
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.047490 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.012489 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.048489 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1037 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1505 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.012489 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.048489 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1051 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1525 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.013490 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.048489 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1059 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1530 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1109 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/agent/mcq_agent/i18n/messages.pot
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.048489 INGInious-0.8.7/inginious/backend/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/backend/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22389 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/backend/backend.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1894 2022-02-09 08:29:26.000000 INGInious-0.8.7/inginious/backend/topic_priority_queue.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.049490 INGInious-0.8.7/inginious/client/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/client/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9874 2023-02-23 07:55:28.000000 INGInious-0.8.7/inginious/client/_zeromq_client.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    16216 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/client/client.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2541 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/client/client_buffer.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1271 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/client/client_sync.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.050490 INGInious-0.8.7/inginious/common/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      242 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/common/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2607 2023-02-23 07:55:28.000000 INGInious-0.8.7/inginious/common/asyncio_utils.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2458 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/common/babel.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4805 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/common/base.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3124 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/common/custom_yaml.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4275 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/common/entrypoints.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      701 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/common/exceptions.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.050490 INGInious-0.8.7/inginious/common/filesystems/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5291 2022-03-18 07:57:30.000000 INGInious-0.8.7/inginious/common/filesystems/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6096 2022-12-14 10:14:50.000000 INGInious-0.8.7/inginious/common/filesystems/local.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2131 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/common/log.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14490 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/common/messages.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2672 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/common/tags.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.051489 INGInious-0.8.7/inginious/common/task_file_readers/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      224 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/common/task_file_readers/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      755 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/common/task_file_readers/abstract_reader.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      650 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/common/task_file_readers/yaml_reader.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14652 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/common/tasks_problems.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.051489 INGInious-0.8.7/inginious/common/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5009 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/common/tests/TestBase.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2823 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/common/tests/TestCustomYaml.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      206 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/common/tests/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    12982 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/common/tests/test_filesystem_local.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.054489 INGInious-0.8.7/inginious/frontend/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2022-03-18 08:08:05.000000 INGInious-0.8.7/inginious/frontend/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5943 2022-02-09 08:22:39.000000 INGInious-0.8.7/inginious/frontend/accessible_time.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15300 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/app.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4770 2023-04-20 07:54:08.000000 INGInious-0.8.7/inginious/frontend/arch_helper.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      138 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/babel.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10782 2022-03-18 08:08:05.000000 INGInious-0.8.7/inginious/frontend/course_factory.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11693 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/courses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.055490 INGInious-0.8.7/inginious/frontend/environment_types/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1022 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/environment_types/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      447 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/environment_types/docker.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      920 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/environment_types/env_type.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2067 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/environment_types/generic_docker_oci_runtime.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      395 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/environment_types/kata.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      408 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/environment_types/mcq.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      393 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/environment_types/nvidia.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.055490 INGInious-0.8.7/inginious/frontend/flask/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      157 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/flask/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/flask/mail.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11759 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/flask/mapping.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5531 2023-05-05 06:38:05.000000 INGInious-0.8.7/inginious/frontend/flask/mongo_sessions.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.055490 INGInious-0.8.7/inginious/frontend/i18n/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.013490 INGInious-0.8.7/inginious/frontend/i18n/de/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.056490 INGInious-0.8.7/inginious/frontend/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25694 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   110889 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.013490 INGInious-0.8.7/inginious/frontend/i18n/el/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.056490 INGInious-0.8.7/inginious/frontend/i18n/el/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    29887 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   119743 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.013490 INGInious-0.8.7/inginious/frontend/i18n/es/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.056490 INGInious-0.8.7/inginious/frontend/i18n/es/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    47593 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   132063 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/fr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.057489 INGInious-0.8.7/inginious/frontend/i18n/fr/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    60340 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   127508 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/he/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.057489 INGInious-0.8.7/inginious/frontend/i18n/he/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    68397 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   130391 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/he/LC_MESSAGES/messages.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    99891 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/messages.pot
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/nl/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.057489 INGInious-0.8.7/inginious/frontend/i18n/nl/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4937 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   102119 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/pt/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.058490 INGInious-0.8.7/inginious/frontend/i18n/pt/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24190 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   119920 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/pt_BR/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.058490 INGInious-0.8.7/inginious/frontend/i18n/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      530 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/vi/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.058490 INGInious-0.8.7/inginious/frontend/i18n/vi/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34450 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   118219 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.014490 INGInious-0.8.7/inginious/frontend/i18n/wa/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.058490 INGInious-0.8.7/inginious/frontend/i18n/wa/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2170 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   100743 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    27989 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/installer.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      639 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/l10n_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4924 2021-02-19 11:28:54.000000 INGInious-0.8.7/inginious/frontend/lti_outcome_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2061 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/lti_request_validator.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      777 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/lti_tool_provider.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3385 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/marketplace_courses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.060490 INGInious-0.8.7/inginious/frontend/pages/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      196 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/pages/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.060490 INGInious-0.8.7/inginious/frontend/pages/admin/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      199 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/admin/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2944 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/pages/admin/admin.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.061490 INGInious-0.8.7/inginious/frontend/pages/api/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      191 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/pages/api/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6726 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/api/_api_page.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1476 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/api/auth_methods.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1615 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/api/authentication.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2946 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/api/courses.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8534 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/api/submissions.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4517 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/api/tasks.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4502 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.063490 INGInious-0.8.7/inginious/frontend/pages/course_admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      189 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5328 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/audience_edit.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10305 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/danger_zone.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1425 2023-03-23 10:48:36.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/search_user.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5138 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/settings.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13926 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/statistics.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2690 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/student_info.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18777 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/student_list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3489 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/submission.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12967 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/submissions.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2377 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/tags.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13627 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/task_edit.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11817 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/task_edit_file.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5408 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/task_list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16859 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/course_admin/utils.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1811 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/course_register.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1240 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/courselist.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4503 2022-03-18 07:57:30.000000 INGInious-0.8.7/inginious/frontend/pages/group.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      813 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/index.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    12033 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/frontend/pages/lti.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      571 2021-07-15 06:35:04.000000 INGInious-0.8.7/inginious/frontend/pages/maintenance.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3957 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/marketplace.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2326 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/marketplace_course.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3020 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/mycourses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.064489 INGInious-0.8.7/inginious/frontend/pages/preferences/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      179 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/pages/preferences/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2090 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/preferences/bindings.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1950 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/preferences/delete.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6131 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/preferences/profile.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1396 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/preferences/utils.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      981 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/pages/queue.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9157 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/pages/register.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3533 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/social.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22133 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/pages/tasks.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    14567 2022-08-03 10:55:31.000000 INGInious-0.8.7/inginious/frontend/pages/utils.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13757 2022-12-14 10:19:50.000000 INGInious-0.8.7/inginious/frontend/parsable_text.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4724 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugin_manager.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.064489 INGInious-0.8.7/inginious/frontend/plugins/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      203 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/plugins/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.065490 INGInious-0.8.7/inginious/frontend/plugins/auth/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      180 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.067489 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      210 2022-01-01 20:58:44.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      200 2021-02-26 16:21:15.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      204 2021-02-26 10:55:03.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-04-21 06:41:19.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-02-26 10:50:17.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3010 2023-04-27 10:00:27.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3372 2021-12-16 14:52:36.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3442 2023-02-28 09:13:57.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3426 2021-06-18 12:47:24.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5914 2023-04-27 10:00:27.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6129 2021-12-16 14:52:36.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6096 2021-03-01 12:53:51.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6226 2023-02-28 09:14:23.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6232 2021-10-25 13:22:36.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6137 2023-04-27 10:00:27.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6394 2021-12-16 14:52:36.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6389 2021-03-01 13:00:13.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6466 2023-02-28 09:13:57.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6464 2021-06-18 12:47:24.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1691 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/custom_auth_form.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4075 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/facebook_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2665 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/github_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2979 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/google_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7358 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/ldap_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3082 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/linkedin_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7053 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/saml2_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4317 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/auth/twitter_auth.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.067489 INGInious-0.8.7/inginious/frontend/plugins/contests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11265 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.068490 INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9636 2023-04-27 10:00:27.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7995 2021-03-01 12:53:52.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7976 2023-02-28 09:13:57.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7930 2021-04-29 09:45:18.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5410 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/admin.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1671 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/course_menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4223 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/contests/scoreboard.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.068490 INGInious-0.8.7/inginious/frontend/plugins/demo/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      583 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/demo/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.068490 INGInious-0.8.7/inginious/frontend/plugins/git_repo/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4807 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/frontend/plugins/git_repo/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.068490 INGInious-0.8.7/inginious/frontend/plugins/ltibestsubmission/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3438 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/ltibestsubmission/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.068490 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9753 2022-07-12 06:51:08.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.069490 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6649 2022-03-30 09:15:04.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6798 2021-03-01 12:53:52.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6738 2021-04-21 06:41:19.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6731 2021-04-29 09:45:18.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      354 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/course_menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1220 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/main.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1418 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/scoreboard.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      425 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/scoreboard/task_menu.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.069490 INGInious-0.8.7/inginious/frontend/plugins/simple_grader/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6106 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/simple_grader/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.069490 INGInious-0.8.7/inginious/frontend/plugins/task_editor_hook_example/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1363 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/task_editor_hook_example/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      816 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.069490 INGInious-0.8.7/inginious/frontend/plugins/task_file_readers/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      212 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/frontend/plugins/task_file_readers/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      976 2020-08-25 08:18:47.000000 INGInious-0.8.7/inginious/frontend/plugins/task_file_readers/json_reader.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.070490 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6301 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.070490 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4945 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      198 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/main_menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      358 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/upcoming.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2803 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.023490 INGInious-0.8.7/inginious/frontend/static/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.072490 INGInious-0.8.7/inginious/frontend/static/css/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11071 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/css/INGInious.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3518 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/css/INGInious.less
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9063 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/css/bootstrap-datetimepicker.min.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   134084 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8217 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/css/codemirror.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9044 2022-03-30 06:18:20.000000 INGInious-0.8.7/inginious/frontend/static/css/common.less
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31000 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/css/font-awesome.min.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7996 2021-06-18 12:47:19.000000 INGInious-0.8.7/inginious/frontend/static/css/lti.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      254 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/css/lti.less
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11150 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/css/selectize.css
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.074490 INGInious-0.8.7/inginious/frontend/static/fonts/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   134808 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/FontAwesome.otf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165742 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   444379 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165548 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    98024 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    77160 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    20127 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   108738 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    45404 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    23424 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18028 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.077489 INGInious-0.8.7/inginious/frontend/static/icons/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1856 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1844 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2259 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1020 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1101 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1241 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1294 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2810 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      371 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/browserconfig.xml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3475 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon-160x160.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      535 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon-16x16.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2870 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon-196x196.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      928 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon-32x32.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2226 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon-96x96.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15086 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/favicon.ico
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4358 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/google-icon.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3186 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/mstile-144x144.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2135 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/mstile-150x150.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1829 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/mstile-310x150.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3819 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/mstile-310x310.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1970 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/mstile-70x70.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2531 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/wb.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1573 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/icons/wb.svg
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.078490 INGInious-0.8.7/inginious/frontend/static/images/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5244 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/header.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6681 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/inginious_full.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6531 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/inginious_full_logo_only.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4730 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/inginious_horiz.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4728 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/inginious_vert.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14493 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/logo.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13380 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/images/logo_maintenance.png
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.079490 INGInious-0.8.7/inginious/frontend/static/js/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2445 2022-03-30 09:10:41.000000 INGInious-0.8.7/inginious/frontend/static/js/admin.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   638597 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/js/all-minified.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3828 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/frontend/static/js/audiences.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2838 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/checked-list-group.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.080489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1107 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   205623 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/codemirror.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.080489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.080489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/apl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4736 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/apl/apl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2179 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/apl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.080489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asciiarmor/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2378 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1289 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.081490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asn.1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7735 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2222 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asn.1/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.081490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asterisk/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7437 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4591 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asterisk/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.081490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/brainfuck/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3338 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.081490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31062 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/clike.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10105 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    28518 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/scala.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.082490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clojure/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16005 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2550 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clojure/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.082490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cmake/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2600 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4152 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cmake/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.082490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cobol/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10288 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8084 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cobol/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.082490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/coffeescript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9884 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22402 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.083490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/commonlisp/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4569 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6691 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.083490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/crystal/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12818 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2605 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/crystal/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.084490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    37613 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/css.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2780 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/gss.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      460 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/gss_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1911 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4066 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/less.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1871 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/less_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2742 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/scss.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/scss_test.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.084490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cypher/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6362 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1908 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cypher/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.084490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/d/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7566 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/d/d.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6332 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/d/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.084490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dart/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5124 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dart/dart.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1627 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dart/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.085490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/diff/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1138 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/diff/diff.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4409 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/diff/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.085490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/django/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11791 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/django/django.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2077 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/django/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.085490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dockerfile/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2221 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2267 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.085490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dtd/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4814 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3337 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dtd/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.086490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dylan/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10112 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13032 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dylan/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.086490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ebnf/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6085 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2450 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ebnf/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.086490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ecl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8843 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1409 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ecl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.086490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/eiffel/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3744 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13198 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/eiffel/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.086490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/elm/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5552 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/elm/elm.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1640 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/elm/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.087490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/erlang/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18887 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2168 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/erlang/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.087490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/factor/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3565 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/factor/factor.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2024 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/factor/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.087490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fcl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4703 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3091 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fcl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.088490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/forth/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5230 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/forth/forth.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1783 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/forth/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.088490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fortran/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8686 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2492 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fortran/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.088490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8886 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gas/gas.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gas/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.088490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gfm/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5103 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2583 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gfm/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.089490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gherkin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13257 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1566 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gherkin/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.089490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/go/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6030 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/go/go.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/go/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.089490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/groovy/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7904 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2177 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/groovy/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.089490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5353 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haml/haml.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2071 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haml/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.089490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/handlebars/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2172 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2196 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/handlebars/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.090489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8109 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2194 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.090489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell-literate/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1390 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9381 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.090489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haxe/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17563 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2577 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haxe/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.090489 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlembedded/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1417 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2086 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.091490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlmixed/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5611 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3434 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.091490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/http/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2795 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/http/http.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1393 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/http/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.091490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/idl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14889 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/idl/idl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1633 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/idl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8286 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.092490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4193 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31566 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2150 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1557 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.092490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jinja2/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1755 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jinja2/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4279 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.092490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jsx/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2410 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jsx/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5195 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.092490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/julia/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2375 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/julia/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12089 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/julia/julia.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.092490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/livescript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9843 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/livescript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7668 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.093490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/lua/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2073 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/lua/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/lua/lua.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.093490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/markdown/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10957 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/markdown/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25671 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.093490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mathematica/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2254 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mathematica/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5612 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.093490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mbox/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1293 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mbox/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3649 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15098 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/meta.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.094490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mirc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5798 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mirc/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10077 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.094490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mllike/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4436 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mllike/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5097 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.094490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/modelica/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2007 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/modelica/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6930 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.095490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4310 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6820 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3795 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3255 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4006 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.095490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mumps/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2608 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mumps/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5354 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.095490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nginx/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5239 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nginx/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10164 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.095490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nsis/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nsis/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7642 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.095490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ntriples/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1357 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ntriples/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6643 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.096490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/octave/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1805 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/octave/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4522 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/octave/octave.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.096490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/oz/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1389 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/oz/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6665 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/oz/oz.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.096490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pascal/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1440 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pascal/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3055 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.096490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pegjs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1890 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pegjs/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.096490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/perl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1542 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/perl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    56135 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/perl/perl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.097490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/php/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1999 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/php/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18224 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/php/php.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.097490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pig/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1475 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pig/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5810 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pig/pig.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.097490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/powershell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7372 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/powershell/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12896 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.097490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/properties/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1555 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/properties/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/properties/properties.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.098490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/protobuf/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1680 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/protobuf/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2113 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.098490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pug/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2489 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pug/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16046 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pug/pug.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.098490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/puppet/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3260 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/puppet/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7568 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.098490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/python/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/python/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12479 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/python/python.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.099490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/q/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8961 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/q/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6593 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/q/q.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.099490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/r/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2518 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/r/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6396 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/r/r.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.099490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.099490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/changes/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2180 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4623 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3775 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.099490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rst/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17769 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rst/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17547 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rst/rst.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.100490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ruby/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5749 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ruby/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10516 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.100490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rust/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1532 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rust/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3025 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rust/rust.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.100490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1854 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sas/index.html
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    15424 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sas/sas.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.100490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sass/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sass/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11509 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sass/sass.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.101490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/scheme/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2554 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/scheme/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13437 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.101490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/shell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/shell/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4002 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/shell/shell.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.101490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sieve/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2335 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sieve/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4284 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.101490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/slim/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2920 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/slim/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18026 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/slim/slim.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.102490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smalltalk/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1904 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4543 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.102490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smarty/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3973 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smarty/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6828 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.102490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/solr/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1365 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/solr/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2672 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/solr/solr.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.102490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/soy/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1939 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/soy/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12239 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/soy/soy.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.102490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sparql/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1773 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sparql/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6335 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.103490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/spreadsheet/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1392 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3139 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.103490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sql/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2991 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sql/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    37351 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sql/sql.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.103490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stex/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4132 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stex/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6932 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stex/stex.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.103490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stylus/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2472 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stylus/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    42256 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.104490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/swift/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2085 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/swift/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7168 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/swift/swift.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.104490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tcl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6297 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tcl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4920 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.105490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/textile/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4347 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/textile/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13835 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/textile/textile.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.105490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      220 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8510 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.105490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      439 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/tiki.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8462 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.106490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/toml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/toml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2897 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/toml/toml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.106490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tornado/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1803 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tornado/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.106490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/troff/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4465 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/troff/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2392 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/troff/troff.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.106490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3490 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10155 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.107490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3605 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7857 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.107490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/turtle/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1470 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/turtle/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4849 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.107490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/twig/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1370 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/twig/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4565 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/twig/twig.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.107490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vb/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1500 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vb/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8734 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vb/vb.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.107490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vbscript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1517 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vbscript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13793 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.108490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/velocity/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3300 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/velocity/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7098 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.108490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/verilog/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2619 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/verilog/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24588 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.108490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vhdl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2486 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vhdl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6704 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.108490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vue/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2064 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vue/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2544 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vue/vue.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.109490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/webidl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/webidl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5784 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.109490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12570 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.109490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xquery/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8609 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xquery/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14470 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.109490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yacas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2176 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yacas/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5424 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.110490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2098 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3693 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.110490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3072 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2292 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.110490 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/z80/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1406 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/z80/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/z80/z80.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6370 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/common.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7286 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/groups.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.112490 INGInious-0.8.7/inginious/frontend/static/js/libs/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    42997 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/Sortable.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    56581 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    51039 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/bootstrap.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)   158741 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/chart.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15252 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.form.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    86926 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6542 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    51679 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/moment.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    20535 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/popper.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    41501 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/selectize.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    50945 2021-04-26 06:37:40.000000 INGInious-0.8.7/inginious/frontend/static/js/libs/sentry-io-bundle.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24394 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/js/studio.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    30954 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/js/task.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16389 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/js/task_dispensers.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      727 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/static/js/webapp.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.023490 INGInious-0.8.7/inginious/frontend/static/plugins/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.112490 INGInious-0.8.7/inginious/frontend/static/plugins/contests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1413 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/static/plugins/contests/contests.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4566 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/plugins/contests/jquery.countdown.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      996 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/static/plugins/contests/scoreboard.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    36374 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/submission_manager.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.112490 INGInious-0.8.7/inginious/frontend/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_dispensers/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3324 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_dispensers/combinatory_test.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2957 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_dispensers/toc.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7041 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_dispensers/util.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13648 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_factory.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9078 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/task_problems.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11846 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tasks.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6972 2022-02-09 08:21:51.000000 INGInious-0.8.7/inginious/frontend/template_helper.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.115490 INGInious-0.8.7/inginious/frontend/templates/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.115490 INGInious-0.8.7/inginious/frontend/templates/admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12064 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/admin/admin_users.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2986 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/auth.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7753 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.117490 INGInious-0.8.7/inginious/frontend/templates/course_admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9319 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/audience_edit.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10121 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/danger_zone.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.117490 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14096 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/basic.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3102 2023-05-05 06:15:19.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1846 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/environment.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1776 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3675 2022-03-30 06:18:20.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/files.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1085 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      913 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18882 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/settings.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    14180 2022-03-30 06:18:20.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/stats.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6499 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/student_info.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    28812 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/student_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5905 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/student_list_table.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7590 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/submission.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12969 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/submissions.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17267 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/submissions_query.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.118490 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2032 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/code.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1332 2023-02-27 12:38:00.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/file.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1050 2023-03-23 10:48:36.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/match.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2826 2022-02-09 08:22:39.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2174 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5141 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/tags.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.119490 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1698 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1225 2023-01-11 09:03:30.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1795 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      894 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section_config.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1352 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1249 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2322 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/task_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1003 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/toc.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4564 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/util.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2481 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9608 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_edit.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5346 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/task_list.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      476 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_admin/user_selection_box.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2034 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_register.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1573 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/course_unavailable.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4040 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/courselist.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      493 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/forbidden.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8084 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/group.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      667 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/internalerror.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13580 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/layout.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2128 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/lti_bind.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1462 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/lti_login.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      572 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/maintenance.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4826 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/marketplace.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2796 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/marketplace_course.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5383 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/mycourses.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      492 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/notfound.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.119490 INGInious-0.8.7/inginious/frontend/templates/preferences/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3987 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/preferences/bindings.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2872 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/preferences/delete.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      469 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/preferences/menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4723 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/preferences/profile.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4845 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/queue.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5245 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/register.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      539 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/signin_button.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      271 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/static.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25388 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/task.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.119490 INGInious-0.8.7/inginious/frontend/templates/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3268 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/task_dispensers/task_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1819 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/task_dispensers/toc.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      513 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/task_unavailable.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.120490 INGInious-0.8.7/inginious/frontend/templates/tasks/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      528 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/tasks/code.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1039 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/tasks/file.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      307 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/tasks/match.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      644 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/tasks/multiple_choice.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      640 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/templates/tasks/single_line_code.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1430 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/templates/unregister_modal.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.121490 INGInious-0.8.7/inginious/frontend/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16896 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/SeleniumFormatter.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6346 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/SeleniumTest.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4326 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestCourse.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3383 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestLogin.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2639 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestParsableText.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      972 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestPluginManager.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7381 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestTask.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1841 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestTaskDisplay.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1975 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/TestTaskSubmission.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious/frontend/tests/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.024489 INGInious-0.8.7/inginious/frontend/tests/tasks/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/invalid_course/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       72 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/invalid_course/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       73 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task1/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task1/run
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      573 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task1/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task2/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task3/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task3/run
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      363 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task3/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task4/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test/task4/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.122490 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task1/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task1/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      339 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task2/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task3/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      559 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task3/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task4/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task4/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test3/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      122 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test3/course.json
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/inginious/frontend/tests/tasks/test3/invalid_task/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       34 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/tests/tasks/test3/invalid_task/task.yaml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    44783 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious/frontend/user_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9056 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious/frontend/webdav.py
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     6462 2022-02-09 10:08:57.000000 INGInious-0.8.7/inginious-agent-docker
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3404 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious-agent-mcq
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    12793 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious-autotest
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2162 2018-11-16 12:58:08.000000 INGInious-0.8.7/inginious-backend
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)      649 2023-05-05 06:37:55.000000 INGInious-0.8.7/inginious-install
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3981 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious-webapp
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3038 2021-06-10 10:07:01.000000 INGInious-0.8.7/inginious-webdav
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-05-05 06:41:51.124490 INGInious-0.8.7/setup.cfg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2546 2023-05-05 06:38:14.000000 INGInious-0.8.7/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.024489 INGInious-0.8.7/utils/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/utils/container_update/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3199 2022-02-09 10:08:57.000000 INGInious-0.8.7/utils/container_update/inginious-container-update
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.123490 INGInious-0.8.7/utils/database_updater/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     4682 2022-02-09 10:08:57.000000 INGInious-0.8.7/utils/database_updater/inginious-database-update
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.124490 INGInious-0.8.7/utils/minify/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2728 2023-05-05 06:37:55.000000 INGInious-0.8.7/utils/minify/Gruntfile.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      452 2023-05-05 06:37:55.000000 INGInious-0.8.7/utils/minify/package.json
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      936 2018-11-16 12:58:08.000000 INGInious-0.8.7/utils/minify/watchers.xml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-05 06:41:51.124490 INGInious-0.8.7/utils/sync/
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3220 2018-11-16 12:58:08.000000 INGInious-0.8.7/utils/sync/inginious-synchronize
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      349 2018-11-16 12:58:08.000000 INGInious-0.8.7/utils/sync/synchronize.json.example
```

### Comparing `INGInious-0.8.6/.github/workflows/ci.yml` & `INGInious-0.8.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/.pylintrc` & `INGInious-0.8.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/.travis.yml` & `INGInious-0.8.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/COPYRIGHTS` & `INGInious-0.8.7/COPYRIGHTS`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/INGInious.egg-info/PKG-INFO` & `INGInious-0.8.7/INGInious.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: INGInious
-Version: 0.8.6
+Version: 0.8.7
 Summary: An intelligent grader that allows secured and automated testing of code made by students.
 Home-page: https://github.com/UCL-INGI/INGInious
 Author: INGInious contributors
 Author-email: inginious@info.ucl.ac.be
 License: AGPL 3
 Provides-Extra: cgi
 Provides-Extra: ldap
```

### Comparing `INGInious-0.8.6/INGInious.egg-info/SOURCES.txt` & `INGInious-0.8.7/INGInious.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/INGInious.egg-info/requires.txt` & `INGInious-0.8.7/INGInious.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 docker>=3.0
+requests<2.29.0
 docutils>=0.14
 pymongo>=3.2.2
 PyYAML>=3.11
 Jinja2>=2.10
 lti>=0.9.0
 oauth2>=1.9.0.post1
 httplib2>=0.9
@@ -11,15 +12,15 @@
 pyzmq>=15.3.0
 natsort>=5.0.1
 psutil>=4.4.2
 zipstream>=1.1.4
 WsgiDAV>=3.0.0
 Werkzeug>=1.0.0
 itsdangerous>=1.1.0
-Flask>=1.1.0
+Flask>=2.0.0
 Flask-Mail>=0.9.1
 importlib_metadata>=3.7.0
 pytidylib>=0.2.4
 sphinx-autodoc-typehints>=1.12.0
 sh>=1.11
 
 [:python_version < "3.7.0"]
```

### Comparing `INGInious-0.8.6/LICENSE` & `INGInious-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/PKG-INFO` & `INGInious-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: INGInious
-Version: 0.8.6
+Version: 0.8.7
 Summary: An intelligent grader that allows secured and automated testing of code made by students.
 Home-page: https://github.com/UCL-INGI/INGInious
 Author: INGInious contributors
 Author-email: inginious@info.ucl.ac.be
 License: AGPL 3
 Provides-Extra: cgi
 Provides-Extra: ldap
```

### Comparing `INGInious-0.8.6/README.rst` & `INGInious-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/Dockerfile` & `INGInious-0.8.7/base-containers/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/README.md` & `INGInious-0.8.7/base-containers/base/README.md`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/INGInious` & `INGInious-0.8.7/base-containers/base/bin/INGInious`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/_run_student_intern` & `INGInious-0.8.7/base-containers/base/bin/_run_student_intern`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/archive` & `INGInious-0.8.7/base-containers/base/bin/archive`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback` & `INGInious-0.8.7/base-containers/base/bin/feedback`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-custom` & `INGInious-0.8.7/base-containers/base/bin/feedback-custom`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-grade` & `INGInious-0.8.7/base-containers/base/bin/feedback-grade`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-msg` & `INGInious-0.8.7/base-containers/base/bin/feedback-msg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-msg-tpl` & `INGInious-0.8.7/base-containers/base/bin/feedback-msg-tpl`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-result` & `INGInious-0.8.7/base-containers/base/bin/feedback-result`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/feedback-state` & `INGInious-0.8.7/base-containers/base/bin/feedback-state`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/getinput` & `INGInious-0.8.7/base-containers/base/bin/getinput`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/inginious-ipython` & `INGInious-0.8.7/base-containers/base/bin/inginious-ipython`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/parsetemplate` & `INGInious-0.8.7/base-containers/base/bin/parsetemplate`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/rst-code` & `INGInious-0.8.7/base-containers/base/bin/rst-code`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/rst-image` & `INGInious-0.8.7/base-containers/base/bin/rst-image`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/rst-indent` & `INGInious-0.8.7/base-containers/base/bin/rst-indent`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/rst-msgblock` & `INGInious-0.8.7/base-containers/base/bin/rst-msgblock`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/run_student` & `INGInious-0.8.7/base-containers/base/bin/run_student`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/ssh_student` & `INGInious-0.8.7/base-containers/base/bin/ssh_student`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/bin/tag-set` & `INGInious-0.8.7/base-containers/base/bin/tag-set`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/feedback.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/feedback.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/input.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/input.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/lang.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/lang.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/rst.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/rst.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/run_student.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/run_student.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/ssh_student.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/ssh_student.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/base-containers/base/inginious_container_api/utils.py` & `INGInious-0.8.7/base-containers/base/inginious_container_api/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/configuration.example.yaml` & `INGInious-0.8.7/configuration.example.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/Makefile` & `INGInious-0.8.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-docker.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-agent-docker.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-mcq.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-agent-mcq.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-autotest.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-autotest.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-backend.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-backend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-install.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-install.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-synchronize.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-synchronize.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webapp.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-webapp.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webdav.rst` & `INGInious-0.8.7/doc/admin_doc/commands_doc/inginious-webdav.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/config_reference.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/config_reference.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/create_container.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/create_container.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/installation.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/installation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/other_oci_runtimes_support.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/other_oci_runtimes_support.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/static_pages.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/static_pages.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/troubleshooting.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_doc/install_doc/updating.rst` & `INGInious-0.8.7/doc/admin_doc/install_doc/updating.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/admin_documentation.rst` & `INGInious-0.8.7/doc/admin_documentation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.client.rst` & `INGInious-0.8.7/doc/api_doc/inginious.client.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.common.rst` & `INGInious-0.8.7/doc/api_doc/inginious.common.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.common.task_file_readers.rst` & `INGInious-0.8.7/doc/api_doc/inginious.common.task_file_readers.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.common.tests.rst` & `INGInious-0.8.7/doc/api_doc/inginious.common.tests.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.api.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.api.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.course_admin.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.course_admin.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.pages.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.auth.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.plugins.auth.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.plugins.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/api_doc/inginious.frontend.tests.rst` & `INGInious-0.8.7/doc/api_doc/inginious.frontend.tests.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/conf.py` & `INGInious-0.8.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/extensions_doc/how_to_extend.rst` & `INGInious-0.8.7/doc/dev_doc/extensions_doc/how_to_extend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/extensions_doc/i18n.rst` & `INGInious-0.8.7/doc/dev_doc/extensions_doc/i18n.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/extensions_doc/plugins.rst` & `INGInious-0.8.7/doc/dev_doc/extensions_doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/architectures.rst` & `INGInious-0.8.7/doc/dev_doc/internals_doc/architectures.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/exercises.rst` & `INGInious-0.8.7/doc/dev_doc/internals_doc/exercises.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/frontend.rst` & `INGInious-0.8.7/doc/dev_doc/internals_doc/frontend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch.png` & `INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_docker.png` & `INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch_docker.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_full.png` & `INGInious-0.8.7/doc/dev_doc/internals_doc/inginious_arch_full.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/submission_evaluation_docker.png` & `INGInious-0.8.7/doc/dev_doc/internals_doc/submission_evaluation_docker.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/submission_workflow.png` & `INGInious-0.8.7/doc/dev_doc/internals_doc/submission_workflow.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/submissions.rst` & `INGInious-0.8.7/doc/dev_doc/internals_doc/submissions.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/dev_doc/internals_doc/understand_inginious.rst` & `INGInious-0.8.7/doc/dev_doc/internals_doc/understand_inginious.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/developer_documentation.rst` & `INGInious-0.8.7/doc/developer_documentation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/logo_rtd.svg` & `INGInious-0.8.7/doc/logo_rtd.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/make.bat` & `INGInious-0.8.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/best_practices.rst` & `INGInious-0.8.7/doc/teacher_doc/best_practices.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/common.rst` & `INGInious-0.8.7/doc/teacher_doc/common.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/course_admin.rst` & `INGInious-0.8.7/doc/teacher_doc/course_admin.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/course_description.rst` & `INGInious-0.8.7/doc/teacher_doc/course_description.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/course_tuto.rst` & `INGInious-0.8.7/doc/teacher_doc/course_tuto.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/courses.rst` & `INGInious-0.8.7/doc/teacher_doc/courses.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/inginious_container_api.rst` & `INGInious-0.8.7/doc/teacher_doc/inginious_container_api.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/lti.rst` & `INGInious-0.8.7/doc/teacher_doc/lti.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/random.rst` & `INGInious-0.8.7/doc/teacher_doc/random.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/rst.rst` & `INGInious-0.8.7/doc/teacher_doc/rst.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/run_file.rst` & `INGInious-0.8.7/doc/teacher_doc/run_file.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/share_files.rst` & `INGInious-0.8.7/doc/teacher_doc/share_files.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/system_files.rst` & `INGInious-0.8.7/doc/teacher_doc/system_files.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/task_file.rst` & `INGInious-0.8.7/doc/teacher_doc/task_file.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/task_tuto.rst` & `INGInious-0.8.7/doc/teacher_doc/task_tuto.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/testing.rst` & `INGInious-0.8.7/doc/teacher_doc/testing.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/teacher_doc/translating.rst` & `INGInious-0.8.7/doc/teacher_doc/translating.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/doc/what_is_inginious.rst` & `INGInious-0.8.7/doc/what_is_inginious.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/__init__.py` & `INGInious-0.8.7/inginious/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/__init__.py` & `INGInious-0.8.7/inginious/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/docker_agent/__init__.py` & `INGInious-0.8.7/inginious/agent/docker_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/docker_agent/_docker_interface.py` & `INGInious-0.8.7/inginious/agent/docker_agent/_docker_interface.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/docker_agent/_docker_runtime.py` & `INGInious-0.8.7/inginious/agent/docker_agent/_docker_runtime.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/docker_agent/_timeout_watcher.py` & `INGInious-0.8.7/inginious/agent/docker_agent/_timeout_watcher.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/__init__.py` & `INGInious-0.8.7/inginious/agent/mcq_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/messages.pot` & `INGInious-0.8.7/inginious/agent/mcq_agent/i18n/messages.pot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/backend/backend.py` & `INGInious-0.8.7/inginious/backend/backend.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/backend/topic_priority_queue.py` & `INGInious-0.8.7/inginious/backend/topic_priority_queue.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/client/_zeromq_client.py` & `INGInious-0.8.7/inginious/client/_zeromq_client.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/client/client.py` & `INGInious-0.8.7/inginious/client/client.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/client/client_buffer.py` & `INGInious-0.8.7/inginious/client/client_buffer.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/client/client_sync.py` & `INGInious-0.8.7/inginious/client/client_sync.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/asyncio_utils.py` & `INGInious-0.8.7/inginious/common/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/babel.py` & `INGInious-0.8.7/inginious/common/babel.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/base.py` & `INGInious-0.8.7/inginious/common/base.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/custom_yaml.py` & `INGInious-0.8.7/inginious/common/custom_yaml.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/entrypoints.py` & `INGInious-0.8.7/inginious/common/entrypoints.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/exceptions.py` & `INGInious-0.8.7/inginious/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/filesystems/__init__.py` & `INGInious-0.8.7/inginious/common/filesystems/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/filesystems/local.py` & `INGInious-0.8.7/inginious/common/filesystems/local.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/log.py` & `INGInious-0.8.7/inginious/common/log.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/messages.py` & `INGInious-0.8.7/inginious/common/messages.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/tags.py` & `INGInious-0.8.7/inginious/common/tags.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/task_file_readers/abstract_reader.py` & `INGInious-0.8.7/inginious/common/task_file_readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/task_file_readers/yaml_reader.py` & `INGInious-0.8.7/inginious/common/task_file_readers/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/tasks_problems.py` & `INGInious-0.8.7/inginious/common/tasks_problems.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/tests/TestBase.py` & `INGInious-0.8.7/inginious/common/tests/TestBase.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/tests/TestCustomYaml.py` & `INGInious-0.8.7/inginious/common/tests/TestCustomYaml.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/common/tests/test_filesystem_local.py` & `INGInious-0.8.7/inginious/common/tests/test_filesystem_local.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/accessible_time.py` & `INGInious-0.8.7/inginious/frontend/accessible_time.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/app.py` & `INGInious-0.8.7/inginious/frontend/app.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/arch_helper.py` & `INGInious-0.8.7/inginious/frontend/arch_helper.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/course_factory.py` & `INGInious-0.8.7/inginious/frontend/course_factory.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/courses.py` & `INGInious-0.8.7/inginious/frontend/courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/environment_types/__init__.py` & `INGInious-0.8.7/inginious/frontend/environment_types/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/environment_types/env_type.py` & `INGInious-0.8.7/inginious/frontend/environment_types/env_type.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/environment_types/generic_docker_oci_runtime.py` & `INGInious-0.8.7/inginious/frontend/environment_types/generic_docker_oci_runtime.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/flask/mapping.py` & `INGInious-0.8.7/inginious/frontend/flask/mapping.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/flask/mongo_sessions.py` & `INGInious-0.8.7/inginious/frontend/flask/mongo_sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             cookieless = True
             sid = path_session.group(2)
         elif is_lti_launch:
             cookieless = True
             sid = None
         else:
             cookieless = False
-            sid = request.cookies.get(app.session_cookie_name)
+            sid = request.cookies.get(self.get_cookie_name(app))
 
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent, cookieless=cookieless)
         if not path_session and self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
@@ -120,16 +120,15 @@
     def save_session(self, app, session, response):
         domain = self.get_cookie_domain(app)
         path = self.get_cookie_path(app)
         store_id = session.sid
         if not session:
             if session.modified:
                 self.store.delete_one({'_id': store_id})
-                response.delete_cookie(app.session_cookie_name,
-                                       domain=domain, path=path)
+                response.delete_cookie(self.get_cookie_name(app), domain=domain, path=path)
             return
 
         httponly = self.get_cookie_httponly(app)
         secure = self.get_cookie_secure(app)
         expires = self.get_expiration_time(app, session)
         cookieless = session.cookieless
         val = self.serializer.dumps(dict(session))
@@ -137,10 +136,10 @@
                               {"$set": {'data': val, 'expiration': expires, 'cookieless': cookieless}},
                               upsert=True)
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
         if not cookieless:
-            response.set_cookie(app.session_cookie_name, session_id,
+            response.set_cookie(self.get_cookie_name(app), session_id,
                                 expires=expires, httponly=httponly,
                                 domain=domain, path=path, secure=secure)
```

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/he/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/messages.pot` & `INGInious-0.8.7/inginious/frontend/i18n/messages.pot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo` & `INGInious-0.8.7/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po` & `INGInious-0.8.7/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/installer.py` & `INGInious-0.8.7/inginious/frontend/installer.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/l10n_manager.py` & `INGInious-0.8.7/inginious/frontend/l10n_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/lti_outcome_manager.py` & `INGInious-0.8.7/inginious/frontend/lti_outcome_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/lti_request_validator.py` & `INGInious-0.8.7/inginious/frontend/lti_request_validator.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/lti_tool_provider.py` & `INGInious-0.8.7/inginious/frontend/lti_tool_provider.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/marketplace_courses.py` & `INGInious-0.8.7/inginious/frontend/marketplace_courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/admin/admin.py` & `INGInious-0.8.7/inginious/frontend/pages/admin/admin.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/_api_page.py` & `INGInious-0.8.7/inginious/frontend/pages/api/_api_page.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/auth_methods.py` & `INGInious-0.8.7/inginious/frontend/pages/api/auth_methods.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/authentication.py` & `INGInious-0.8.7/inginious/frontend/pages/api/authentication.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/courses.py` & `INGInious-0.8.7/inginious/frontend/pages/api/courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/submissions.py` & `INGInious-0.8.7/inginious/frontend/pages/api/submissions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/api/tasks.py` & `INGInious-0.8.7/inginious/frontend/pages/api/tasks.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course.py` & `INGInious-0.8.7/inginious/frontend/pages/course.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/audience_edit.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/audience_edit.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/danger_zone.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/danger_zone.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/search_user.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/search_user.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/settings.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/settings.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/statistics.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/statistics.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/student_info.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/student_info.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/student_list.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/student_list.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/submission.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/submission.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/submissions.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/submissions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/tags.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/tags.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/task_edit.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit_file.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/task_edit_file.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_list.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/task_list.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_admin/utils.py` & `INGInious-0.8.7/inginious/frontend/pages/course_admin/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/course_register.py` & `INGInious-0.8.7/inginious/frontend/pages/course_register.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/courselist.py` & `INGInious-0.8.7/inginious/frontend/pages/courselist.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/group.py` & `INGInious-0.8.7/inginious/frontend/pages/group.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/index.py` & `INGInious-0.8.7/inginious/frontend/pages/index.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/lti.py` & `INGInious-0.8.7/inginious/frontend/pages/lti.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/maintenance.py` & `INGInious-0.8.7/inginious/frontend/pages/maintenance.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/marketplace.py` & `INGInious-0.8.7/inginious/frontend/pages/marketplace.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/marketplace_course.py` & `INGInious-0.8.7/inginious/frontend/pages/marketplace_course.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/mycourses.py` & `INGInious-0.8.7/inginious/frontend/pages/mycourses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/preferences/bindings.py` & `INGInious-0.8.7/inginious/frontend/pages/preferences/bindings.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/preferences/delete.py` & `INGInious-0.8.7/inginious/frontend/pages/preferences/delete.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/preferences/profile.py` & `INGInious-0.8.7/inginious/frontend/pages/preferences/profile.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/preferences/utils.py` & `INGInious-0.8.7/inginious/frontend/pages/preferences/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/queue.py` & `INGInious-0.8.7/inginious/frontend/pages/queue.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/register.py` & `INGInious-0.8.7/inginious/frontend/pages/register.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/social.py` & `INGInious-0.8.7/inginious/frontend/pages/social.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/tasks.py` & `INGInious-0.8.7/inginious/frontend/pages/tasks.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/pages/utils.py` & `INGInious-0.8.7/inginious/frontend/pages/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/parsable_text.py` & `INGInious-0.8.7/inginious/frontend/parsable_text.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugin_manager.py` & `INGInious-0.8.7/inginious/frontend/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 09:42:50 2023 UTC, .py size: 2979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1af2 4864 a30b 0000  o.........Hd....
+00000000: 610d 0d0a 0000 0000 45e4 c160 a30b 0000  a.......E..`....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000070: 5a09 6407 5a0a 6700 6408 a201 5a0b 4700  Z.d.Z.g.d...Z.G.
@@ -57,52 +57,52 @@
 00000380: 5e2f 686f 6d65 2f61 6e74 686f 6e79 2f44  ^/home/anthony/D
 00000390: 6f63 756d 656e 7473 2f69 6e67 696e 696f  ocuments/inginio
 000003a0: 7573 2d64 6576 2f49 4e47 496e 696f 7573  us-dev/INGInious
 000003b0: 2f69 6e67 696e 696f 7573 2f66 726f 6e74  /inginious/front
 000003c0: 656e 642f 706c 7567 696e 732f 6175 7468  end/plugins/auth
 000003d0: 2f67 6f6f 676c 655f 6175 7468 2e70 79da  /google_auth.py.
 000003e0: 0d67 6574 5f61 7574 685f 6c69 6e6b 1e00  .get_auth_link..
-000003f0: 0000 7308 0000 001a 0114 0108 0104 017a  ..s............z
+000003f0: 0000 7308 0000 0000 011a 0114 0108 017a  ..s............z
 00000400: 1e47 6f6f 676c 6541 7574 684d 6574 686f  .GoogleAuthMetho
 00000410: 642e 6765 745f 6175 7468 5f6c 696e 6b63  d.get_auth_linkc
 00000420: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00000430: 0a00 0000 4300 0000 7398 0000 0074 007c  ....C...s....t.|
+00000430: 0a00 0000 4300 0000 739c 0000 0074 007c  ....C...s....t.|
 00000440: 006a 017c 0164 0119 0074 026a 036a 047c  .j.|.d...t.j.j.|
-00000450: 006a 0517 0074 0664 028d 047d 027a 287c  .j...t.d...}.z(|
+00000450: 006a 0517 0074 0664 028d 047d 027a 507c  .j...t.d...}.zP|
 00000460: 026a 0774 087c 006a 0974 026a 036a 0a64  .j.t.|.j.t.j.j.d
 00000470: 038d 0301 007c 02a0 0b64 04a1 017d 0374  .....|...d...}.t
 00000480: 0ca0 0d7c 036a 0ea0 0f64 05a1 01a1 017d  ...|.j...d.....}
 00000490: 0474 107c 0464 0619 0083 017c 0464 0719  .t.|.d.....|.d..
 000004a0: 007c 0464 0819 0069 0066 0457 0053 0004  .|.d...i.f.W.S..
-000004b0: 0074 1179 4b01 007d 0501 007a 0757 0059  .t.yK..}...z.W.Y
+000004b0: 0074 1179 9601 007d 0501 007a 0e57 0059  .t.y...}...z.W.Y
 000004c0: 0064 007d 057e 0564 0053 0064 007d 057e  .d.}.~.d.S.d.}.~
-000004d0: 0577 0177 0029 094e 7209 0000 0029 0372  .w.w.).Nr....).r
-000004e0: 1600 0000 7208 0000 0072 0700 0000 2902  ....r....r....).
-000004f0: da0d 636c 6965 6e74 5f73 6563 7265 74da  ..client_secret.
-00000500: 1661 7574 686f 7269 7a61 7469 6f6e 5f72  .authorization_r
-00000510: 6573 706f 6e73 657a 2d68 7474 7073 3a2f  esponsez-https:/
-00000520: 2f77 7777 2e67 6f6f 676c 6561 7069 732e  /www.googleapis.
-00000530: 636f 6d2f 6f61 7574 6832 2f76 332f 7573  com/oauth2/v3/us
-00000540: 6572 696e 666f 7a05 7574 662d 38da 0373  erinfoz.utf-8..s
-00000550: 7562 da04 6e61 6d65 da05 656d 6169 6c29  ub..name..email)
-00000560: 1272 0300 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000570: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000580: 0700 0000 da0b 6665 7463 685f 746f 6b65  ......fetch_toke
-00000590: 6eda 0974 6f6b 656e 5f75 726c da0e 5f63  n..token_url.._c
-000005a0: 6c69 656e 745f 7365 6372 6574 da03 7572  lient_secret..ur
-000005b0: 6cda 0367 6574 da04 6a73 6f6e da05 6c6f  l..get..json..lo
-000005c0: 6164 73da 0763 6f6e 7465 6e74 da06 6465  ads..content..de
-000005d0: 636f 6465 da03 7374 72da 0945 7863 6570  code..str..Excep
-000005e0: 7469 6f6e 2906 7212 0000 0072 1300 0000  tion).r....r....
-000005f0: 7215 0000 00da 0872 6573 706f 6e73 65da  r......response.
-00000600: 0770 726f 6669 6c65 da01 6572 1700 0000  .profile..er....
-00000610: 7217 0000 0072 1800 0000 da08 6361 6c6c  r....r......call
-00000620: 6261 636b 2400 0000 731c 0000 000c 010e  back$...s.......
-00000630: 0106 ff02 030a 0106 0106 ff0a 0312 011e  ................
-00000640: 010e 010e 0108 8002 ff7a 1947 6f6f 676c  .........z.Googl
+000004d0: 0530 0030 0064 0053 0029 094e 7209 0000  .0.0.d.S.).Nr...
+000004e0: 0029 0372 1600 0000 7208 0000 0072 0700  .).r....r....r..
+000004f0: 0000 2902 da0d 636c 6965 6e74 5f73 6563  ..)...client_sec
+00000500: 7265 74da 1661 7574 686f 7269 7a61 7469  ret..authorizati
+00000510: 6f6e 5f72 6573 706f 6e73 657a 2d68 7474  on_responsez-htt
+00000520: 7073 3a2f 2f77 7777 2e67 6f6f 676c 6561  ps://www.googlea
+00000530: 7069 732e 636f 6d2f 6f61 7574 6832 2f76  pis.com/oauth2/v
+00000540: 332f 7573 6572 696e 666f 7a05 7574 662d  3/userinfoz.utf-
+00000550: 38da 0373 7562 da04 6e61 6d65 da05 656d  8..sub..name..em
+00000560: 6169 6c29 1272 0300 0000 720a 0000 0072  ail).r....r....r
+00000570: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00000580: 0000 0072 0700 0000 da0b 6665 7463 685f  ...r......fetch_
+00000590: 746f 6b65 6eda 0974 6f6b 656e 5f75 726c  token..token_url
+000005a0: da0e 5f63 6c69 656e 745f 7365 6372 6574  .._client_secret
+000005b0: da03 7572 6cda 0367 6574 da04 6a73 6f6e  ..url..get..json
+000005c0: da05 6c6f 6164 73da 0763 6f6e 7465 6e74  ..loads..content
+000005d0: da06 6465 636f 6465 da03 7374 72da 0945  ..decode..str..E
+000005e0: 7863 6570 7469 6f6e 2906 7212 0000 0072  xception).r....r
+000005f0: 1300 0000 7215 0000 00da 0872 6573 706f  ....r......respo
+00000600: 6e73 65da 0770 726f 6669 6c65 da01 6572  nse..profile..er
+00000610: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
+00000620: 6361 6c6c 6261 636b 2400 0000 7318 0000  callback$...s...
+00000630: 0000 010c 010e ff06 0302 010a 0106 ff06  ................
+00000640: 030a 0112 011e 010e 017a 1947 6f6f 676c  .........z.Googl
 00000650: 6541 7574 684d 6574 686f 642e 6361 6c6c  eAuthMethod.call
 00000660: 6261 636b 6306 0000 0000 0000 0000 0000  backc...........
 00000670: 0006 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
 00000680: 0000 7400 6401 7401 6a02 6a03 1700 6402  ..t.d.t.j.j...d.
 00000690: 1700 7c02 a004 a100 1700 6403 1700 7c03  ..|.......d...|.
 000006a0: a004 a100 1700 8301 5300 2904 4e7a 2268  ........S.).Nz"h
 000006b0: 7474 7073 3a2f 2f70 6c75 732e 676f 6f67  ttps://plus.goog
@@ -110,105 +110,106 @@
 000006d0: 3d7a 082f 636f 7572 7365 2ffa 012f 2905  =z./course/../).
 000006e0: 7202 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
 000006f0: 0d00 0000 da06 6765 745f 6964 2906 7212  ......get_id).r.
 00000700: 0000 0072 1300 0000 da06 636f 7572 7365  ...r......course
 00000710: da04 7461 736b da0a 7375 626d 6973 7369  ..task..submissi
 00000720: 6f6e da08 6c61 6e67 7561 6765 7217 0000  on..languager...
 00000730: 0072 1700 0000 7218 0000 0072 1400 0000  .r....r....r....
-00000740: 3200 0000 7302 0000 0028 017a 1647 6f6f  2...s....(.z.Goo
+00000740: 3200 0000 7302 0000 0000 017a 1647 6f6f  2...s......z.Goo
 00000750: 676c 6541 7574 684d 6574 686f 642e 7368  gleAuthMethod.sh
 00000760: 6172 6563 0100 0000 0000 0000 0000 0000  arec............
-00000770: 0100 0000 0100 0000 4300 0000 f304 0000  ........C.......
+00000770: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
 00000780: 0064 0153 0029 024e 5472 1700 0000 a901  .d.S.).NTr......
 00000790: 7212 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
 000007a0: 1800 0000 da0b 616c 6c6f 775f 7368 6172  ......allow_shar
-000007b0: 6535 0000 00f3 0200 0000 0401 7a1c 476f  e5..........z.Go
+000007b0: 6535 0000 0073 0200 0000 0001 7a1c 476f  e5...s......z.Go
 000007c0: 6f67 6c65 4175 7468 4d65 7468 6f64 2e61  ogleAuthMethod.a
 000007d0: 6c6c 6f77 5f73 6861 7265 6301 0000 0000  llow_sharec.....
 000007e0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000007f0: 0000 00f3 0600 0000 7c00 6a00 5300 a901  ........|.j.S...
-00000800: 4e29 01da 035f 6964 7235 0000 0072 1700  N)..._idr5...r..
+000007f0: 0000 0073 0600 0000 7c00 6a00 5300 a901  ...s....|.j.S...
+00000800: 4e29 01da 035f 6964 7234 0000 0072 1700  N)..._idr4...r..
 00000810: 0000 7217 0000 0072 1800 0000 722f 0000  ..r....r....r/..
-00000820: 0038 0000 00f3 0200 0000 0601 7a17 476f  .8..........z.Go
+00000820: 0038 0000 0073 0200 0000 0001 7a17 476f  .8...s......z.Go
 00000830: 6f67 6c65 4175 7468 4d65 7468 6f64 2e67  ogleAuthMethod.g
 00000840: 6574 5f69 6463 0600 0000 0000 0000 0000  et_idc..........
 00000850: 0000 0600 0000 0200 0000 4300 0000 732e  ..........C...s.
 00000860: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
 00000870: 037c 005f 027c 047c 005f 0364 017c 006a  .|._.|.|._.d.|.j
 00000880: 0017 007c 005f 047c 057c 005f 0564 0053  ...|._.|.|._.d.S
 00000890: 0029 024e 7a0e 6175 7468 2f63 616c 6c62  .).Nz.auth/callb
-000008a0: 6163 6b2f 2906 723a 0000 00da 055f 6e61  ack/).r:....._na
+000008a0: 6163 6b2f 2906 7237 0000 00da 055f 6e61  ack/).r7....._na
 000008b0: 6d65 720a 0000 0072 2100 0000 720e 0000  mer....r!...r...
 000008c0: 0072 1100 0000 2906 7212 0000 00da 0269  .r....).r......i
 000008d0: 6472 1d00 0000 da09 636c 6965 6e74 5f69  dr......client_i
 000008e0: 6472 1a00 0000 da06 646f 6d61 696e 7217  dr......domainr.
 000008f0: 0000 0072 1700 0000 7218 0000 00da 085f  ...r....r......_
 00000900: 5f69 6e69 745f 5f3b 0000 0073 0c00 0000  _init__;...s....
-00000910: 0601 0601 0601 0601 0c01 0a01 7a19 476f  ............z.Go
+00000910: 0001 0601 0601 0601 0601 0c01 7a19 476f  ............z.Go
 00000920: 6f67 6c65 4175 7468 4d65 7468 6f64 2e5f  ogleAuthMethod._
 00000930: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
 00000940: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000950: 7238 0000 0072 3900 0000 2901 723c 0000  r8...r9...).r<..
-00000960: 0072 3500 0000 7217 0000 0072 1700 0000  .r5...r....r....
-00000970: 7218 0000 00da 0867 6574 5f6e 616d 6543  r......get_nameC
-00000980: 0000 0072 3b00 0000 7a19 476f 6f67 6c65  ...r;...z.Google
-00000990: 4175 7468 4d65 7468 6f64 2e67 6574 5f6e  AuthMethod.get_n
-000009a0: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-000009b0: 0100 0000 0100 0000 4300 0000 7234 0000  ........C...r4..
-000009c0: 0029 024e 7a91 3c69 6d67 2073 7263 3d22  .).Nz.<img src="
-000009d0: 2f73 7461 7469 632f 6963 6f6e 732f 676f  /static/icons/go
-000009e0: 6f67 6c65 2d69 636f 6e2e 7376 6722 2073  ogle-icon.svg" s
-000009f0: 7479 6c65 3d22 2d6d 6f7a 2d75 7365 722d  tyle="-moz-user-
-00000a00: 7365 6c65 6374 3a20 6e6f 6e65 3b20 2d77  select: none; -w
-00000a10: 6562 6b69 742d 7573 6572 2d73 656c 6563  ebkit-user-selec
-00000a20: 743a 206e 6f6e 653b 7573 6572 2d73 656c  t: none;user-sel
-00000a30: 6563 743a 206e 6f6e 653b 2077 6964 7468  ect: none; width
-00000a40: 3a20 3530 7078 3b20 6865 6967 6874 3a35  : 50px; height:5
-00000a50: 3070 783b 2220 3e72 1700 0000 7235 0000  0px;" >r....r5..
-00000a60: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000a70: da0a 6765 745f 696d 6c69 6e6b 4600 0000  ..get_imlinkF...
-00000a80: 7237 0000 007a 1b47 6f6f 676c 6541 7574  r7...z.GoogleAut
-00000a90: 684d 6574 686f 642e 6765 745f 696d 6c69  hMethod.get_imli
-00000aa0: 6e6b 4e29 0146 290c da08 5f5f 6e61 6d65  nkN).F)...__name
-00000ab0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000ac0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00000ad0: 646f 635f 5f72 1900 0000 722d 0000 0072  doc__r....r-...r
-00000ae0: 1400 0000 7236 0000 0072 2f00 0000 7240  ....r6...r/...r@
-00000af0: 0000 0072 4100 0000 7242 0000 0072 1700  ...rA...rB...r..
-00000b00: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000b10: 0072 0600 0000 1900 0000 7314 0000 0008  .r........s.....
-00000b20: 0004 010a 0408 0608 0e08 0308 0308 0308  ................
-00000b30: 080c 0372 0600 0000 6304 0000 0000 0000  ...r....c.......
-00000b40: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
-00000b50: 0073 6200 0000 7c03 a000 6401 6402 a102  .sb...|...d.d...
-00000b60: 720b 6403 7401 6a02 6404 3c00 7c03 a000  r.d.t.j.d.<.|...
-00000b70: 6405 6406 a102 7d04 7c03 a000 6407 6406  d.d...}.|...d.d.
-00000b80: a102 7d05 7c03 a000 6408 6406 a102 7d06  ..}.|...d.d...}.
-00000b90: 7c00 a003 7404 7c03 a000 6409 a101 7c03  |...t.|...d...|.
-00000ba0: a000 640a 640b a102 7c04 7c05 7c06 8305  ..d.d...|.|.|...
-00000bb0: a101 0100 6400 5300 290c 4eda 0564 6562  ....d.S.).N..deb
-00000bc0: 7567 46da 0131 da1b 4f41 5554 484c 4942  ugF..1..OAUTHLIB
-00000bd0: 5f49 4e53 4543 5552 455f 5452 414e 5350  _INSECURE_TRANSP
-00000be0: 4f52 5472 3e00 0000 da00 721a 0000 0072  ORTr>.....r....r
-00000bf0: 3f00 0000 723d 0000 0072 1d00 0000 5a06  ?...r=...r....Z.
-00000c00: 476f 6f67 6c65 2905 7223 0000 00da 026f  Google).r#.....o
-00000c10: 73da 0765 6e76 6972 6f6e da14 7265 6769  s..environ..regi
-00000c20: 7374 6572 5f61 7574 685f 6d65 7468 6f64  ster_auth_method
-00000c30: 7206 0000 0029 07da 0e70 6c75 6769 6e5f  r....)...plugin_
-00000c40: 6d61 6e61 6765 72da 0e63 6f75 7273 655f  manager..course_
-00000c50: 6661 6374 6f72 79da 0663 6c69 656e 74da  factory..client.
-00000c60: 0463 6f6e 6672 3e00 0000 721a 0000 0072  .confr>...r....r
-00000c70: 3f00 0000 7217 0000 0072 1700 0000 7218  ?...r....r....r.
-00000c80: 0000 00da 0469 6e69 744c 0000 0073 1000  .....initL...s..
-00000c90: 0000 0c01 0a01 0c02 0c01 0c01 0e02 1001  ................
-00000ca0: 0aff 7252 0000 0029 0e72 4600 0000 7224  ..rR...).rF...r$
-00000cb0: 0000 0072 4b00 0000 720b 0000 0072 0200  ...rK...r....r..
-00000cc0: 0000 da11 7265 7175 6573 7473 5f6f 6175  ....requests_oau
-00000cd0: 7468 6c69 6272 0300 0000 da1f 696e 6769  thlibr......ingi
-00000ce0: 6e69 6f75 732e 6672 6f6e 7465 6e64 2e75  nious.frontend.u
-00000cf0: 7365 725f 6d61 6e61 6765 7272 0400 0000  ser_managerr....
-00000d00: 7210 0000 0072 2000 0000 7207 0000 0072  r....r ...r....r
-00000d10: 0600 0000 7252 0000 0072 1700 0000 7217  ....rR...r....r.
-00000d20: 0000 0072 1700 0000 7218 0000 00da 083c  ...r....r......<
-00000d30: 6d6f 6475 6c65 3e01 0000 0073 1800 0000  module>....s....
-00000d40: 0405 0802 0801 0802 0c01 0c01 0c02 0402  ................
-00000d50: 0401 0801 1006 0c33                      .......3
+00000950: 7306 0000 007c 006a 0053 0072 3600 0000  s....|.j.S.r6...
+00000960: 2901 7238 0000 0072 3400 0000 7217 0000  ).r8...r4...r...
+00000970: 0072 1700 0000 7218 0000 00da 0867 6574  .r....r......get
+00000980: 5f6e 616d 6543 0000 0073 0200 0000 0001  _nameC...s......
+00000990: 7a19 476f 6f67 6c65 4175 7468 4d65 7468  z.GoogleAuthMeth
+000009a0: 6f64 2e67 6574 5f6e 616d 6563 0100 0000  od.get_namec....
+000009b0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000009c0: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
+000009d0: 7a91 3c69 6d67 2073 7263 3d22 2f73 7461  z.<img src="/sta
+000009e0: 7469 632f 6963 6f6e 732f 676f 6f67 6c65  tic/icons/google
+000009f0: 2d69 636f 6e2e 7376 6722 2073 7479 6c65  -icon.svg" style
+00000a00: 3d22 2d6d 6f7a 2d75 7365 722d 7365 6c65  ="-moz-user-sele
+00000a10: 6374 3a20 6e6f 6e65 3b20 2d77 6562 6b69  ct: none; -webki
+00000a20: 742d 7573 6572 2d73 656c 6563 743a 206e  t-user-select: n
+00000a30: 6f6e 653b 7573 6572 2d73 656c 6563 743a  one;user-select:
+00000a40: 206e 6f6e 653b 2077 6964 7468 3a20 3530   none; width: 50
+00000a50: 7078 3b20 6865 6967 6874 3a35 3070 783b  px; height:50px;
+00000a60: 2220 3e72 1700 0000 7234 0000 0072 1700  " >r....r4...r..
+00000a70: 0000 7217 0000 0072 1800 0000 da0a 6765  ..r....r......ge
+00000a80: 745f 696d 6c69 6e6b 4600 0000 7302 0000  t_imlinkF...s...
+00000a90: 0000 017a 1b47 6f6f 676c 6541 7574 684d  ...z.GoogleAuthM
+00000aa0: 6574 686f 642e 6765 745f 696d 6c69 6e6b  ethod.get_imlink
+00000ab0: 4e29 0146 290c da08 5f5f 6e61 6d65 5f5f  N).F)...__name__
+00000ac0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000ad0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000ae0: 635f 5f72 1900 0000 722d 0000 0072 1400  c__r....r-...r..
+00000af0: 0000 7235 0000 0072 2f00 0000 723c 0000  ..r5...r/...r<..
+00000b00: 0072 3d00 0000 723e 0000 0072 1700 0000  .r=...r>...r....
+00000b10: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000b20: 0600 0000 1900 0000 7312 0000 0008 0104  ........s.......
+00000b30: 040a 0608 0e08 0308 0308 0308 0808 0372  ...............r
+00000b40: 0600 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00000b50: 0007 0000 0008 0000 0043 0000 0073 6200  .........C...sb.
+00000b60: 0000 7c03 a000 6401 6402 a102 7216 6403  ..|...d.d...r.d.
+00000b70: 7401 6a02 6404 3c00 7c03 a000 6405 6406  t.j.d.<.|...d.d.
+00000b80: a102 7d04 7c03 a000 6407 6406 a102 7d05  ..}.|...d.d...}.
+00000b90: 7c03 a000 6408 6406 a102 7d06 7c00 a003  |...d.d...}.|...
+00000ba0: 7404 7c03 a000 6409 a101 7c03 a000 640a  t.|...d...|...d.
+00000bb0: 640b a102 7c04 7c05 7c06 8305 a101 0100  d...|.|.|.......
+00000bc0: 6400 5300 290c 4eda 0564 6562 7567 46da  d.S.).N..debugF.
+00000bd0: 0131 da1b 4f41 5554 484c 4942 5f49 4e53  .1..OAUTHLIB_INS
+00000be0: 4543 5552 455f 5452 414e 5350 4f52 5472  ECURE_TRANSPORTr
+00000bf0: 3a00 0000 da00 721a 0000 0072 3b00 0000  :.....r....r;...
+00000c00: 7239 0000 0072 1d00 0000 5a06 476f 6f67  r9...r....Z.Goog
+00000c10: 6c65 2905 7223 0000 00da 026f 73da 0765  le).r#.....os..e
+00000c20: 6e76 6972 6f6e da14 7265 6769 7374 6572  nviron..register
+00000c30: 5f61 7574 685f 6d65 7468 6f64 7206 0000  _auth_methodr...
+00000c40: 0029 07da 0e70 6c75 6769 6e5f 6d61 6e61  .)...plugin_mana
+00000c50: 6765 72da 0e63 6f75 7273 655f 6661 6374  ger..course_fact
+00000c60: 6f72 79da 0663 6c69 656e 74da 0463 6f6e  ory..client..con
+00000c70: 6672 3a00 0000 721a 0000 0072 3b00 0000  fr:...r....r;...
+00000c80: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00000c90: 0469 6e69 744c 0000 0073 1000 0000 0001  .initL...s......
+00000ca0: 0c01 0a02 0c01 0c01 0c02 0e01 10ff 724e  ..............rN
+00000cb0: 0000 0029 0e72 4200 0000 7224 0000 0072  ...).rB...r$...r
+00000cc0: 4700 0000 720b 0000 0072 0200 0000 da11  G...r....r......
+00000cd0: 7265 7175 6573 7473 5f6f 6175 7468 6c69  requests_oauthli
+00000ce0: 6272 0300 0000 da1f 696e 6769 6e69 6f75  br......inginiou
+00000cf0: 732e 6672 6f6e 7465 6e64 2e75 7365 725f  s.frontend.user_
+00000d00: 6d61 6e61 6765 7272 0400 0000 7210 0000  managerr....r...
+00000d10: 0072 2000 0000 7207 0000 0072 0600 0000  .r ...r....r....
+00000d20: 724e 0000 0072 1700 0000 7217 0000 0072  rN...r....r....r
+00000d30: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
+00000d40: 6c65 3e06 0000 0073 1600 0000 0402 0801  le>....s........
+00000d50: 0802 0801 0c01 0c02 0c02 0401 0401 0806  ................
+00000d60: 1033                                     .3
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 10 10:07:01 2021 UTC, .py size: 2979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 45e4 c160 a30b 0000  a.......E..`....
+00000000: 6f0d 0d0a 0000 0000 8247 4a64 920a 0000  o........GJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000070: 5a09 6407 5a0a 6700 6408 a201 5a0b 4700  Z.d.Z.g.d...Z.G.
@@ -21,195 +21,169 @@
 00000140: 2e68 7474 7073 3a2f 2f77 7777 2e67 6f6f  .https://www.goo
 00000150: 676c 6561 7069 732e 636f 6d2f 6175 7468  gleapis.com/auth
 00000160: 2f75 7365 7269 6e66 6f2e 656d 6169 6c7a  /userinfo.emailz
 00000170: 3068 7474 7073 3a2f 2f77 7777 2e67 6f6f  0https://www.goo
 00000180: 676c 6561 7069 732e 636f 6d2f 6175 7468  gleapis.com/auth
 00000190: 2f75 7365 7269 6e66 6f2e 7072 6f66 696c  /userinfo.profil
 000001a0: 65da 066f 7065 6e69 6463 0000 0000 0000  e..openidc......
-000001b0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000001c0: 0000 7352 0000 0065 005a 0164 005a 0264  ..sR...e.Z.d.Z.d
-000001d0: 015a 0364 1464 0364 0484 015a 0464 0564  .Z.d.d.d...Z.d.d
-000001e0: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-000001f0: 0a84 005a 0764 0b64 0c84 005a 0864 0d64  ...Z.d.d...Z.d.d
-00000200: 0e84 005a 0964 0f64 1084 005a 0a64 1164  ...Z.d.d...Z.d.d
-00000210: 1284 005a 0b64 1353 0029 15da 1047 6f6f  ...Z.d.S.)...Goo
-00000220: 676c 6541 7574 684d 6574 686f 647a 1c0a  gleAuthMethodz..
-00000230: 2020 2020 476f 6f67 6c65 2061 7574 6820      Google auth 
-00000240: 6d65 7468 6f64 0a20 2020 2046 6303 0000  method.    Fc...
-00000250: 0000 0000 0000 0000 0006 0000 0005 0000  ................
-00000260: 0043 0000 0073 3a00 0000 7400 7c00 6a01  .C...s:...t.|.j.
-00000270: 7402 7403 6a04 6a05 7c00 6a06 1700 6401  t.t.j.j.|.j...d.
-00000280: 8d03 7d03 7c03 6a07 7408 7c00 6a09 6402  ..}.|.j.t.|.j.d.
-00000290: 8d02 5c02 7d04 7d05 7c05 7c01 6403 3c00  ..\.}.}.|.|.d.<.
-000002a0: 7c04 5300 2904 4e29 02da 0573 636f 7065  |.S.).N)...scope
-000002b0: da0c 7265 6469 7265 6374 5f75 7269 2901  ..redirect_uri).
-000002c0: 5a02 6864 da0b 6f61 7574 685f 7374 6174  Z.hd..oauth_stat
-000002d0: 6529 0a72 0300 0000 da0a 5f63 6c69 656e  e).r......_clien
-000002e0: 745f 6964 7207 0000 00da 0566 6c61 736b  t_idr......flask
-000002f0: da07 7265 7175 6573 74da 0875 726c 5f72  ..request..url_r
-00000300: 6f6f 74da 0e5f 6361 6c6c 6261 636b 5f70  oot.._callback_p
-00000310: 6167 65da 1161 7574 686f 7269 7a61 7469  age..authorizati
-00000320: 6f6e 5f75 726c da16 6175 7468 6f72 697a  on_url..authoriz
-00000330: 6174 696f 6e5f 6261 7365 5f75 726c da07  ation_base_url..
-00000340: 5f64 6f6d 6169 6e29 06da 0473 656c 66da  _domain)...self.
-00000350: 0c61 7574 685f 7374 6f72 6167 65da 0573  .auth_storage..s
-00000360: 6861 7265 da06 676f 6f67 6c65 720f 0000  hare..googler...
-00000370: 00da 0573 7461 7465 a900 7217 0000 00fa  ...state..r.....
-00000380: 5e2f 686f 6d65 2f61 6e74 686f 6e79 2f44  ^/home/anthony/D
-00000390: 6f63 756d 656e 7473 2f69 6e67 696e 696f  ocuments/inginio
-000003a0: 7573 2d64 6576 2f49 4e47 496e 696f 7573  us-dev/INGInious
-000003b0: 2f69 6e67 696e 696f 7573 2f66 726f 6e74  /inginious/front
-000003c0: 656e 642f 706c 7567 696e 732f 6175 7468  end/plugins/auth
-000003d0: 2f67 6f6f 676c 655f 6175 7468 2e70 79da  /google_auth.py.
-000003e0: 0d67 6574 5f61 7574 685f 6c69 6e6b 1e00  .get_auth_link..
-000003f0: 0000 7308 0000 0000 011a 0114 0108 017a  ..s............z
-00000400: 1e47 6f6f 676c 6541 7574 684d 6574 686f  .GoogleAuthMetho
-00000410: 642e 6765 745f 6175 7468 5f6c 696e 6b63  d.get_auth_linkc
-00000420: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00000430: 0a00 0000 4300 0000 739c 0000 0074 007c  ....C...s....t.|
-00000440: 006a 017c 0164 0119 0074 026a 036a 047c  .j.|.d...t.j.j.|
-00000450: 006a 0517 0074 0664 028d 047d 027a 507c  .j...t.d...}.zP|
-00000460: 026a 0774 087c 006a 0974 026a 036a 0a64  .j.t.|.j.t.j.j.d
-00000470: 038d 0301 007c 02a0 0b64 04a1 017d 0374  .....|...d...}.t
-00000480: 0ca0 0d7c 036a 0ea0 0f64 05a1 01a1 017d  ...|.j...d.....}
-00000490: 0474 107c 0464 0619 0083 017c 0464 0719  .t.|.d.....|.d..
-000004a0: 007c 0464 0819 0069 0066 0457 0053 0004  .|.d...i.f.W.S..
-000004b0: 0074 1179 9601 007d 0501 007a 0e57 0059  .t.y...}...z.W.Y
-000004c0: 0064 007d 057e 0564 0053 0064 007d 057e  .d.}.~.d.S.d.}.~
-000004d0: 0530 0030 0064 0053 0029 094e 7209 0000  .0.0.d.S.).Nr...
-000004e0: 0029 0372 1600 0000 7208 0000 0072 0700  .).r....r....r..
-000004f0: 0000 2902 da0d 636c 6965 6e74 5f73 6563  ..)...client_sec
-00000500: 7265 74da 1661 7574 686f 7269 7a61 7469  ret..authorizati
-00000510: 6f6e 5f72 6573 706f 6e73 657a 2d68 7474  on_responsez-htt
-00000520: 7073 3a2f 2f77 7777 2e67 6f6f 676c 6561  ps://www.googlea
-00000530: 7069 732e 636f 6d2f 6f61 7574 6832 2f76  pis.com/oauth2/v
-00000540: 332f 7573 6572 696e 666f 7a05 7574 662d  3/userinfoz.utf-
-00000550: 38da 0373 7562 da04 6e61 6d65 da05 656d  8..sub..name..em
-00000560: 6169 6c29 1272 0300 0000 720a 0000 0072  ail).r....r....r
-00000570: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-00000580: 0000 0072 0700 0000 da0b 6665 7463 685f  ...r......fetch_
-00000590: 746f 6b65 6eda 0974 6f6b 656e 5f75 726c  token..token_url
-000005a0: da0e 5f63 6c69 656e 745f 7365 6372 6574  .._client_secret
-000005b0: da03 7572 6cda 0367 6574 da04 6a73 6f6e  ..url..get..json
-000005c0: da05 6c6f 6164 73da 0763 6f6e 7465 6e74  ..loads..content
-000005d0: da06 6465 636f 6465 da03 7374 72da 0945  ..decode..str..E
-000005e0: 7863 6570 7469 6f6e 2906 7212 0000 0072  xception).r....r
-000005f0: 1300 0000 7215 0000 00da 0872 6573 706f  ....r......respo
-00000600: 6e73 65da 0770 726f 6669 6c65 da01 6572  nse..profile..er
-00000610: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-00000620: 6361 6c6c 6261 636b 2400 0000 7318 0000  callback$...s...
-00000630: 0000 010c 010e ff06 0302 010a 0106 ff06  ................
-00000640: 030a 0112 011e 010e 017a 1947 6f6f 676c  .........z.Googl
-00000650: 6541 7574 684d 6574 686f 642e 6361 6c6c  eAuthMethod.call
-00000660: 6261 636b 6306 0000 0000 0000 0000 0000  backc...........
-00000670: 0006 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
-00000680: 0000 7400 6401 7401 6a02 6a03 1700 6402  ..t.d.t.j.j...d.
-00000690: 1700 7c02 a004 a100 1700 6403 1700 7c03  ..|.......d...|.
-000006a0: a004 a100 1700 8301 5300 2904 4e7a 2268  ........S.).Nz"h
-000006b0: 7474 7073 3a2f 2f70 6c75 732e 676f 6f67  ttps://plus.goog
-000006c0: 6c65 2e63 6f6d 2f73 6861 7265 3f75 726c  le.com/share?url
-000006d0: 3d7a 082f 636f 7572 7365 2ffa 012f 2905  =z./course/../).
-000006e0: 7202 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-000006f0: 0d00 0000 da06 6765 745f 6964 2906 7212  ......get_id).r.
-00000700: 0000 0072 1300 0000 da06 636f 7572 7365  ...r......course
-00000710: da04 7461 736b da0a 7375 626d 6973 7369  ..task..submissi
-00000720: 6f6e da08 6c61 6e67 7561 6765 7217 0000  on..languager...
-00000730: 0072 1700 0000 7218 0000 0072 1400 0000  .r....r....r....
-00000740: 3200 0000 7302 0000 0000 017a 1647 6f6f  2...s......z.Goo
-00000750: 676c 6541 7574 684d 6574 686f 642e 7368  gleAuthMethod.sh
-00000760: 6172 6563 0100 0000 0000 0000 0000 0000  arec............
-00000770: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-00000780: 0064 0153 0029 024e 5472 1700 0000 a901  .d.S.).NTr......
-00000790: 7212 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000007a0: 1800 0000 da0b 616c 6c6f 775f 7368 6172  ......allow_shar
-000007b0: 6535 0000 0073 0200 0000 0001 7a1c 476f  e5...s......z.Go
-000007c0: 6f67 6c65 4175 7468 4d65 7468 6f64 2e61  ogleAuthMethod.a
-000007d0: 6c6c 6f77 5f73 6861 7265 6301 0000 0000  llow_sharec.....
-000007e0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000007f0: 0000 0073 0600 0000 7c00 6a00 5300 a901  ...s....|.j.S...
-00000800: 4e29 01da 035f 6964 7234 0000 0072 1700  N)..._idr4...r..
-00000810: 0000 7217 0000 0072 1800 0000 722f 0000  ..r....r....r/..
-00000820: 0038 0000 0073 0200 0000 0001 7a17 476f  .8...s......z.Go
-00000830: 6f67 6c65 4175 7468 4d65 7468 6f64 2e67  ogleAuthMethod.g
-00000840: 6574 5f69 6463 0600 0000 0000 0000 0000  et_idc..........
-00000850: 0000 0600 0000 0200 0000 4300 0000 732e  ..........C...s.
-00000860: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
-00000870: 037c 005f 027c 047c 005f 0364 017c 006a  .|._.|.|._.d.|.j
-00000880: 0017 007c 005f 047c 057c 005f 0564 0053  ...|._.|.|._.d.S
-00000890: 0029 024e 7a0e 6175 7468 2f63 616c 6c62  .).Nz.auth/callb
-000008a0: 6163 6b2f 2906 7237 0000 00da 055f 6e61  ack/).r7....._na
-000008b0: 6d65 720a 0000 0072 2100 0000 720e 0000  mer....r!...r...
-000008c0: 0072 1100 0000 2906 7212 0000 00da 0269  .r....).r......i
-000008d0: 6472 1d00 0000 da09 636c 6965 6e74 5f69  dr......client_i
-000008e0: 6472 1a00 0000 da06 646f 6d61 696e 7217  dr......domainr.
-000008f0: 0000 0072 1700 0000 7218 0000 00da 085f  ...r....r......_
-00000900: 5f69 6e69 745f 5f3b 0000 0073 0c00 0000  _init__;...s....
-00000910: 0001 0601 0601 0601 0601 0c01 7a19 476f  ............z.Go
-00000920: 6f67 6c65 4175 7468 4d65 7468 6f64 2e5f  ogleAuthMethod._
-00000930: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000940: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000950: 7306 0000 007c 006a 0053 0072 3600 0000  s....|.j.S.r6...
-00000960: 2901 7238 0000 0072 3400 0000 7217 0000  ).r8...r4...r...
-00000970: 0072 1700 0000 7218 0000 00da 0867 6574  .r....r......get
-00000980: 5f6e 616d 6543 0000 0073 0200 0000 0001  _nameC...s......
-00000990: 7a19 476f 6f67 6c65 4175 7468 4d65 7468  z.GoogleAuthMeth
-000009a0: 6f64 2e67 6574 5f6e 616d 6563 0100 0000  od.get_namec....
-000009b0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-000009c0: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
-000009d0: 7a91 3c69 6d67 2073 7263 3d22 2f73 7461  z.<img src="/sta
-000009e0: 7469 632f 6963 6f6e 732f 676f 6f67 6c65  tic/icons/google
-000009f0: 2d69 636f 6e2e 7376 6722 2073 7479 6c65  -icon.svg" style
-00000a00: 3d22 2d6d 6f7a 2d75 7365 722d 7365 6c65  ="-moz-user-sele
-00000a10: 6374 3a20 6e6f 6e65 3b20 2d77 6562 6b69  ct: none; -webki
-00000a20: 742d 7573 6572 2d73 656c 6563 743a 206e  t-user-select: n
-00000a30: 6f6e 653b 7573 6572 2d73 656c 6563 743a  one;user-select:
-00000a40: 206e 6f6e 653b 2077 6964 7468 3a20 3530   none; width: 50
-00000a50: 7078 3b20 6865 6967 6874 3a35 3070 783b  px; height:50px;
-00000a60: 2220 3e72 1700 0000 7234 0000 0072 1700  " >r....r4...r..
-00000a70: 0000 7217 0000 0072 1800 0000 da0a 6765  ..r....r......ge
-00000a80: 745f 696d 6c69 6e6b 4600 0000 7302 0000  t_imlinkF...s...
-00000a90: 0000 017a 1b47 6f6f 676c 6541 7574 684d  ...z.GoogleAuthM
-00000aa0: 6574 686f 642e 6765 745f 696d 6c69 6e6b  ethod.get_imlink
-00000ab0: 4e29 0146 290c da08 5f5f 6e61 6d65 5f5f  N).F)...__name__
-00000ac0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000ad0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000ae0: 635f 5f72 1900 0000 722d 0000 0072 1400  c__r....r-...r..
-00000af0: 0000 7235 0000 0072 2f00 0000 723c 0000  ..r5...r/...r<..
-00000b00: 0072 3d00 0000 723e 0000 0072 1700 0000  .r=...r>...r....
-00000b10: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000b20: 0600 0000 1900 0000 7312 0000 0008 0104  ........s.......
-00000b30: 040a 0608 0e08 0308 0308 0308 0808 0372  ...............r
-00000b40: 0600 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00000b50: 0007 0000 0008 0000 0043 0000 0073 6200  .........C...sb.
-00000b60: 0000 7c03 a000 6401 6402 a102 7216 6403  ..|...d.d...r.d.
-00000b70: 7401 6a02 6404 3c00 7c03 a000 6405 6406  t.j.d.<.|...d.d.
-00000b80: a102 7d04 7c03 a000 6407 6406 a102 7d05  ..}.|...d.d...}.
-00000b90: 7c03 a000 6408 6406 a102 7d06 7c00 a003  |...d.d...}.|...
-00000ba0: 7404 7c03 a000 6409 a101 7c03 a000 640a  t.|...d...|...d.
-00000bb0: 640b a102 7c04 7c05 7c06 8305 a101 0100  d...|.|.|.......
-00000bc0: 6400 5300 290c 4eda 0564 6562 7567 46da  d.S.).N..debugF.
-00000bd0: 0131 da1b 4f41 5554 484c 4942 5f49 4e53  .1..OAUTHLIB_INS
-00000be0: 4543 5552 455f 5452 414e 5350 4f52 5472  ECURE_TRANSPORTr
-00000bf0: 3a00 0000 da00 721a 0000 0072 3b00 0000  :.....r....r;...
-00000c00: 7239 0000 0072 1d00 0000 5a06 476f 6f67  r9...r....Z.Goog
-00000c10: 6c65 2905 7223 0000 00da 026f 73da 0765  le).r#.....os..e
-00000c20: 6e76 6972 6f6e da14 7265 6769 7374 6572  nviron..register
-00000c30: 5f61 7574 685f 6d65 7468 6f64 7206 0000  _auth_methodr...
-00000c40: 0029 07da 0e70 6c75 6769 6e5f 6d61 6e61  .)...plugin_mana
-00000c50: 6765 72da 0e63 6f75 7273 655f 6661 6374  ger..course_fact
-00000c60: 6f72 79da 0663 6c69 656e 74da 0463 6f6e  ory..client..con
-00000c70: 6672 3a00 0000 721a 0000 0072 3b00 0000  fr:...r....r;...
-00000c80: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00000c90: 0469 6e69 744c 0000 0073 1000 0000 0001  .initL...s......
-00000ca0: 0c01 0a02 0c01 0c01 0c02 0e01 10ff 724e  ..............rN
-00000cb0: 0000 0029 0e72 4200 0000 7224 0000 0072  ...).rB...r$...r
-00000cc0: 4700 0000 720b 0000 0072 0200 0000 da11  G...r....r......
-00000cd0: 7265 7175 6573 7473 5f6f 6175 7468 6c69  requests_oauthli
-00000ce0: 6272 0300 0000 da1f 696e 6769 6e69 6f75  br......inginiou
-00000cf0: 732e 6672 6f6e 7465 6e64 2e75 7365 725f  s.frontend.user_
-00000d00: 6d61 6e61 6765 7272 0400 0000 7210 0000  managerr....r...
-00000d10: 0072 2000 0000 7207 0000 0072 0600 0000  .r ...r....r....
-00000d20: 724e 0000 0072 1700 0000 7217 0000 0072  rN...r....r....r
-00000d30: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
-00000d40: 6c65 3e06 0000 0073 1600 0000 0402 0801  le>....s........
-00000d50: 0802 0801 0c01 0c02 0c02 0401 0401 0806  ................
-00000d60: 1033                                     .3
+000001b0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+000001c0: 0000 7340 0000 0065 005a 0164 005a 0264  ..s@...e.Z.d.Z.d
+000001d0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+000001e0: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
+000001f0: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
+00000200: 005a 0964 0e53 0029 0fda 1047 6f6f 676c  .Z.d.S.)...Googl
+00000210: 6541 7574 684d 6574 686f 647a 1c0a 2020  eAuthMethodz..  
+00000220: 2020 476f 6f67 6c65 2061 7574 6820 6d65    Google auth me
+00000230: 7468 6f64 0a20 2020 2063 0200 0000 0000  thod.    c......
+00000240: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00000250: 0000 733a 0000 0074 007c 006a 0174 0274  ..s:...t.|.j.t.t
+00000260: 036a 046a 057c 006a 0617 0064 018d 037d  .j.j.|.j...d...}
+00000270: 027c 026a 0774 087c 006a 0964 028d 025c  .|.j.t.|.j.d...\
+00000280: 027d 037d 047c 047c 0164 033c 007c 0353  .}.}.|.|.d.<.|.S
+00000290: 0029 044e 2902 da05 7363 6f70 65da 0c72  .).N)...scope..r
+000002a0: 6564 6972 6563 745f 7572 6929 015a 0268  edirect_uri).Z.h
+000002b0: 64da 0b6f 6175 7468 5f73 7461 7465 290a  d..oauth_state).
+000002c0: 7203 0000 00da 0a5f 636c 6965 6e74 5f69  r......_client_i
+000002d0: 6472 0700 0000 da05 666c 6173 6bda 0772  dr......flask..r
+000002e0: 6571 7565 7374 da08 7572 6c5f 726f 6f74  equest..url_root
+000002f0: da0e 5f63 616c 6c62 6163 6b5f 7061 6765  .._callback_page
+00000300: da11 6175 7468 6f72 697a 6174 696f 6e5f  ..authorization_
+00000310: 7572 6cda 1661 7574 686f 7269 7a61 7469  url..authorizati
+00000320: 6f6e 5f62 6173 655f 7572 6cda 075f 646f  on_base_url.._do
+00000330: 6d61 696e 2905 da04 7365 6c66 da0c 6175  main)...self..au
+00000340: 7468 5f73 746f 7261 6765 da06 676f 6f67  th_storage..goog
+00000350: 6c65 720f 0000 00da 0573 7461 7465 a900  ler......state..
+00000360: 7216 0000 00fa 5e2f 686f 6d65 2f61 6e74  r.....^/home/ant
+00000370: 686f 6e79 2f44 6f63 756d 656e 7473 2f69  hony/Documents/i
+00000380: 6e67 696e 696f 7573 2d64 6576 2f49 4e47  nginious-dev/ING
+00000390: 496e 696f 7573 2f69 6e67 696e 696f 7573  Inious/inginious
+000003a0: 2f66 726f 6e74 656e 642f 706c 7567 696e  /frontend/plugin
+000003b0: 732f 6175 7468 2f67 6f6f 676c 655f 6175  s/auth/google_au
+000003c0: 7468 2e70 79da 0d67 6574 5f61 7574 685f  th.py..get_auth_
+000003d0: 6c69 6e6b 1e00 0000 7308 0000 001a 0114  link....s.......
+000003e0: 0108 0104 017a 1e47 6f6f 676c 6541 7574  .....z.GoogleAut
+000003f0: 684d 6574 686f 642e 6765 745f 6175 7468  hMethod.get_auth
+00000400: 5f6c 696e 6b63 0200 0000 0000 0000 0000  _linkc..........
+00000410: 0000 0600 0000 0a00 0000 4300 0000 7398  ..........C...s.
+00000420: 0000 0074 007c 006a 017c 0164 0119 0074  ...t.|.j.|.d...t
+00000430: 026a 036a 047c 006a 0517 0074 0664 028d  .j.j.|.j...t.d..
+00000440: 047d 027a 287c 026a 0774 087c 006a 0974  .}.z(|.j.t.|.j.t
+00000450: 026a 036a 0a64 038d 0301 007c 02a0 0b64  .j.j.d.....|...d
+00000460: 04a1 017d 0374 0ca0 0d7c 036a 0ea0 0f64  ...}.t...|.j...d
+00000470: 05a1 01a1 017d 0474 107c 0464 0619 0083  .....}.t.|.d....
+00000480: 017c 0464 0719 007c 0464 0819 0069 0066  .|.d...|.d...i.f
+00000490: 0457 0053 0004 0074 1179 4b01 007d 0501  .W.S...t.yK..}..
+000004a0: 007a 0757 0059 0064 007d 057e 0564 0053  .z.W.Y.d.}.~.d.S
+000004b0: 0064 007d 057e 0577 0177 0029 094e 7209  .d.}.~.w.w.).Nr.
+000004c0: 0000 0029 0372 1500 0000 7208 0000 0072  ...).r....r....r
+000004d0: 0700 0000 2902 da0d 636c 6965 6e74 5f73  ....)...client_s
+000004e0: 6563 7265 74da 1661 7574 686f 7269 7a61  ecret..authoriza
+000004f0: 7469 6f6e 5f72 6573 706f 6e73 657a 2d68  tion_responsez-h
+00000500: 7474 7073 3a2f 2f77 7777 2e67 6f6f 676c  ttps://www.googl
+00000510: 6561 7069 732e 636f 6d2f 6f61 7574 6832  eapis.com/oauth2
+00000520: 2f76 332f 7573 6572 696e 666f 7a05 7574  /v3/userinfoz.ut
+00000530: 662d 38da 0373 7562 da04 6e61 6d65 da05  f-8..sub..name..
+00000540: 656d 6169 6c29 1272 0300 0000 720a 0000  email).r....r...
+00000550: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000560: 720e 0000 0072 0700 0000 da0b 6665 7463  r....r......fetc
+00000570: 685f 746f 6b65 6eda 0974 6f6b 656e 5f75  h_token..token_u
+00000580: 726c da0e 5f63 6c69 656e 745f 7365 6372  rl.._client_secr
+00000590: 6574 da03 7572 6cda 0367 6574 da04 6a73  et..url..get..js
+000005a0: 6f6e da05 6c6f 6164 73da 0763 6f6e 7465  on..loads..conte
+000005b0: 6e74 da06 6465 636f 6465 da03 7374 72da  nt..decode..str.
+000005c0: 0945 7863 6570 7469 6f6e 2906 7212 0000  .Exception).r...
+000005d0: 0072 1300 0000 7214 0000 00da 0872 6573  .r....r......res
+000005e0: 706f 6e73 65da 0770 726f 6669 6c65 da01  ponse..profile..
+000005f0: 6572 1600 0000 7216 0000 0072 1700 0000  er....r....r....
+00000600: da08 6361 6c6c 6261 636b 2400 0000 731c  ..callback$...s.
+00000610: 0000 000c 010e 0106 ff02 030a 0106 0106  ................
+00000620: ff0a 0312 011e 010e 010e 0108 8002 ff7a  ...............z
+00000630: 1947 6f6f 676c 6541 7574 684d 6574 686f  .GoogleAuthMetho
+00000640: 642e 6361 6c6c 6261 636b 6301 0000 0000  d.callbackc.....
+00000650: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000660: 0000 00f3 0600 0000 7c00 6a00 5300 a901  ........|.j.S...
+00000670: 4e29 01da 035f 6964 a901 7212 0000 0072  N)..._id..r....r
+00000680: 1600 0000 7216 0000 0072 1700 0000 da06  ....r....r......
+00000690: 6765 745f 6964 3200 0000 f302 0000 0006  get_id2.........
+000006a0: 017a 1747 6f6f 676c 6541 7574 684d 6574  .z.GoogleAuthMet
+000006b0: 686f 642e 6765 745f 6964 6306 0000 0000  hod.get_idc.....
+000006c0: 0000 0000 0000 0006 0000 0002 0000 0043  ...............C
+000006d0: 0000 0073 2e00 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+000006e0: 7c00 5f01 7c03 7c00 5f02 7c04 7c00 5f03  |._.|.|._.|.|._.
+000006f0: 6401 7c00 6a00 1700 7c00 5f04 7c05 7c00  d.|.j...|._.|.|.
+00000700: 5f05 6400 5300 2902 4e7a 0e61 7574 682f  _.d.S.).Nz.auth/
+00000710: 6361 6c6c 6261 636b 2f29 0672 2f00 0000  callback/).r/...
+00000720: da05 5f6e 616d 6572 0a00 0000 7220 0000  .._namer....r ..
+00000730: 0072 0e00 0000 7211 0000 0029 0672 1200  .r....r....).r..
+00000740: 0000 da02 6964 721c 0000 00da 0963 6c69  ....idr......cli
+00000750: 656e 745f 6964 7219 0000 00da 0664 6f6d  ent_idr......dom
+00000760: 6169 6e72 1600 0000 7216 0000 0072 1700  ainr....r....r..
+00000770: 0000 da08 5f5f 696e 6974 5f5f 3500 0000  ....__init__5...
+00000780: 730c 0000 0006 0106 0106 0106 010c 010a  s...............
+00000790: 017a 1947 6f6f 676c 6541 7574 684d 6574  .z.GoogleAuthMet
+000007a0: 686f 642e 5f5f 696e 6974 5f5f 6301 0000  hod.__init__c...
+000007b0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+000007c0: 0043 0000 0072 2d00 0000 722e 0000 0029  .C...r-...r....)
+000007d0: 0172 3300 0000 7230 0000 0072 1600 0000  .r3...r0...r....
+000007e0: 7216 0000 0072 1700 0000 da08 6765 745f  r....r......get_
+000007f0: 6e61 6d65 3d00 0000 7232 0000 007a 1947  name=...r2...z.G
+00000800: 6f6f 676c 6541 7574 684d 6574 686f 642e  oogleAuthMethod.
+00000810: 6765 745f 6e61 6d65 6301 0000 0000 0000  get_namec.......
+00000820: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000830: 0073 0400 0000 6401 5300 2902 4e7a 913c  .s....d.S.).Nz.<
+00000840: 696d 6720 7372 633d 222f 7374 6174 6963  img src="/static
+00000850: 2f69 636f 6e73 2f67 6f6f 676c 652d 6963  /icons/google-ic
+00000860: 6f6e 2e73 7667 2220 7374 796c 653d 222d  on.svg" style="-
+00000870: 6d6f 7a2d 7573 6572 2d73 656c 6563 743a  moz-user-select:
+00000880: 206e 6f6e 653b 202d 7765 626b 6974 2d75   none; -webkit-u
+00000890: 7365 722d 7365 6c65 6374 3a20 6e6f 6e65  ser-select: none
+000008a0: 3b75 7365 722d 7365 6c65 6374 3a20 6e6f  ;user-select: no
+000008b0: 6e65 3b20 7769 6474 683a 2035 3070 783b  ne; width: 50px;
+000008c0: 2068 6569 6768 743a 3530 7078 3b22 203e   height:50px;" >
+000008d0: 7216 0000 0072 3000 0000 7216 0000 0072  r....r0...r....r
+000008e0: 1600 0000 7217 0000 00da 0a67 6574 5f69  ....r......get_i
+000008f0: 6d6c 696e 6b40 0000 0073 0200 0000 0401  mlink@...s......
+00000900: 7a1b 476f 6f67 6c65 4175 7468 4d65 7468  z.GoogleAuthMeth
+00000910: 6f64 2e67 6574 5f69 6d6c 696e 6b4e 290a  od.get_imlinkN).
+00000920: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000930: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000940: 6d65 5f5f da07 5f5f 646f 635f 5f72 1800  me__..__doc__r..
+00000950: 0000 722c 0000 0072 3100 0000 7237 0000  ..r,...r1...r7..
+00000960: 0072 3800 0000 7239 0000 0072 1600 0000  .r8...r9...r....
+00000970: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000980: 0600 0000 1900 0000 7310 0000 0008 0004  ........s.......
+00000990: 0108 0408 0608 0e08 0308 080c 0372 0600  .............r..
+000009a0: 0000 6304 0000 0000 0000 0000 0000 0007  ..c.............
+000009b0: 0000 0008 0000 0043 0000 0073 6200 0000  .......C...sb...
+000009c0: 7c03 a000 6401 6402 a102 720b 6403 7401  |...d.d...r.d.t.
+000009d0: 6a02 6404 3c00 7c03 a000 6405 6406 a102  j.d.<.|...d.d...
+000009e0: 7d04 7c03 a000 6407 6406 a102 7d05 7c03  }.|...d.d...}.|.
+000009f0: a000 6408 6406 a102 7d06 7c00 a003 7404  ..d.d...}.|...t.
+00000a00: 7c03 a000 6409 a101 7c03 a000 640a 640b  |...d...|...d.d.
+00000a10: a102 7c04 7c05 7c06 8305 a101 0100 6400  ..|.|.|.......d.
+00000a20: 5300 290c 4eda 0564 6562 7567 46da 0131  S.).N..debugF..1
+00000a30: da1b 4f41 5554 484c 4942 5f49 4e53 4543  ..OAUTHLIB_INSEC
+00000a40: 5552 455f 5452 414e 5350 4f52 5472 3500  URE_TRANSPORTr5.
+00000a50: 0000 da00 7219 0000 0072 3600 0000 7234  ....r....r6...r4
+00000a60: 0000 0072 1c00 0000 5a06 476f 6f67 6c65  ...r....Z.Google
+00000a70: 2905 7222 0000 00da 026f 73da 0765 6e76  ).r".....os..env
+00000a80: 6972 6f6e da14 7265 6769 7374 6572 5f61  iron..register_a
+00000a90: 7574 685f 6d65 7468 6f64 7206 0000 0029  uth_methodr....)
+00000aa0: 07da 0e70 6c75 6769 6e5f 6d61 6e61 6765  ...plugin_manage
+00000ab0: 72da 0e63 6f75 7273 655f 6661 6374 6f72  r..course_factor
+00000ac0: 79da 0663 6c69 656e 74da 0463 6f6e 6672  y..client..confr
+00000ad0: 3500 0000 7219 0000 0072 3600 0000 7216  5...r....r6...r.
+00000ae0: 0000 0072 1600 0000 7217 0000 00da 0469  ...r....r......i
+00000af0: 6e69 7446 0000 0073 1000 0000 0c01 0a01  nitF...s........
+00000b00: 0c02 0c01 0c01 0e02 1001 0aff 7249 0000  ............rI..
+00000b10: 0029 0e72 3d00 0000 7223 0000 0072 4200  .).r=...r#...rB.
+00000b20: 0000 720b 0000 0072 0200 0000 da11 7265  ..r....r......re
+00000b30: 7175 6573 7473 5f6f 6175 7468 6c69 6272  quests_oauthlibr
+00000b40: 0300 0000 da1f 696e 6769 6e69 6f75 732e  ......inginious.
+00000b50: 6672 6f6e 7465 6e64 2e75 7365 725f 6d61  frontend.user_ma
+00000b60: 6e61 6765 7272 0400 0000 7210 0000 0072  nagerr....r....r
+00000b70: 1f00 0000 7207 0000 0072 0600 0000 7249  ....r....r....rI
+00000b80: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
+00000b90: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000ba0: 3e01 0000 0073 1800 0000 0405 0802 0801  >....s..........
+00000bb0: 0802 0c01 0c01 0c02 0402 0401 0801 1006  ................
+00000bc0: 0c2d                                     .-
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 09:42:50 2023 UTC, .py size: 7358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1af2 4864 be1c 0000  o.........Hd....
+00000000: 6f0d 0d0a 0000 0000 8247 4a64 231c 0000  o........GJd#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6401 6407 6c0b  d.l.m.Z...d.d.l.
@@ -15,375 +15,356 @@
 000000e0: 01da 0d4c 4441 5045 7863 6570 7469 6f6e  ...LDAPException
 000000f0: 2901 da13 6573 6361 7065 5f66 696c 7465  )...escape_filte
 00000100: 725f 6368 6172 7329 01da 1241 7574 6865  r_chars)...Authe
 00000110: 6e74 6963 6174 696f 6e50 6167 6529 01da  nticationPage)..
 00000120: 0a41 7574 684d 6574 686f 647a 2169 6e67  .AuthMethodz!ing
 00000130: 696e 696f 7573 2e77 6562 6170 702e 706c  inious.webapp.pl
 00000140: 7567 696e 2e61 7574 682e 6c64 6170 6300  ugin.auth.ldapc.
-00000150: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000160: 0000 0040 0000 0073 5a00 0000 6500 5a01  ...@...sZ...e.Z.
+00000150: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000160: 0000 0040 0000 0073 4800 0000 6500 5a01  ...@...sH...e.Z.
 00000170: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
 00000180: 6404 6405 8400 5a05 6406 6407 8400 5a06  d.d...Z.d.d...Z.
-00000190: 6408 6409 8400 5a07 6416 640b 640c 8401  d.d...Z.d.d.d...
-000001a0: 5a08 640d 640e 8400 5a09 640f 6410 8400  Z.d.d...Z.d.d...
-000001b0: 5a0a 6411 6412 8400 5a0b 6413 6414 8400  Z.d.d...Z.d.d...
-000001c0: 5a0c 6415 5300 2917 da0e 4c64 6170 4175  Z.d.S.)...LdapAu
-000001d0: 7468 4d65 7468 6f64 7a1a 0a20 2020 204c  thMethodz..    L
-000001e0: 4441 5020 6175 7468 206d 6574 686f 640a  DAP auth method.
-000001f0: 2020 2020 6305 0000 0000 0000 0000 0000      c...........
-00000200: 0005 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
-00000210: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
-00000220: 7c00 5f02 7c04 7c00 5f03 6400 5300 a901  |._.|.|._.d.S...
-00000230: 4e29 04da 035f 6964 da05 5f6e 616d 65da  N)..._id.._name.
-00000240: 075f 696d 6c69 6e6b da09 5f73 6574 7469  ._imlink.._setti
-00000250: 6e67 7329 05da 0473 656c 66da 0269 64da  ngs)...self..id.
-00000260: 046e 616d 65da 0669 6d6c 696e 6bda 0873  .name..imlink..s
-00000270: 6574 7469 6e67 73a9 0072 1200 0000 fa5c  ettings..r.....\
-00000280: 2f68 6f6d 652f 616e 7468 6f6e 792f 446f  /home/anthony/Do
-00000290: 6375 6d65 6e74 732f 696e 6769 6e69 6f75  cuments/inginiou
-000002a0: 732d 6465 762f 494e 4749 6e69 6f75 732f  s-dev/INGInious/
-000002b0: 696e 6769 6e69 6f75 732f 6672 6f6e 7465  inginious/fronte
-000002c0: 6e64 2f70 6c75 6769 6e73 2f61 7574 682f  nd/plugins/auth/
-000002d0: 6c64 6170 5f61 7574 682e 7079 da08 5f5f  ldap_auth.py..__
-000002e0: 696e 6974 5f5f 1a00 0000 7308 0000 0006  init__....s.....
-000002f0: 0106 0106 010a 017a 174c 6461 7041 7574  .......z.LdapAut
-00000300: 684d 6574 686f 642e 5f5f 696e 6974 5f5f  hMethod.__init__
-00000310: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000320: 0001 0000 0043 0000 00f3 0600 0000 7c00  .....C........|.
-00000330: 6a00 5300 7208 0000 00a9 0172 0900 0000  j.S.r......r....
-00000340: a901 720d 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00000350: 0072 1300 0000 da06 6765 745f 6964 2000  .r......get_id .
-00000360: 0000 f302 0000 0006 017a 154c 6461 7041  .........z.LdapA
-00000370: 7574 684d 6574 686f 642e 6765 745f 6964  uthMethod.get_id
-00000380: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000390: 0001 0000 0043 0000 0072 1500 0000 7208  .....C...r....r.
-000003a0: 0000 0029 0172 0a00 0000 7217 0000 0072  ...).r....r....r
-000003b0: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-000003c0: 6765 745f 6e61 6d65 2300 0000 7219 0000  get_name#...r...
-000003d0: 007a 174c 6461 7041 7574 684d 6574 686f  .z.LdapAuthMetho
-000003e0: 642e 6765 745f 6e61 6d65 6301 0000 0000  d.get_namec.....
-000003f0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000400: 0000 0073 1800 0000 7c00 6a00 720a 6401  ...s....|.j.r.d.
-00000410: 7c00 6a00 1700 6402 1700 5300 6403 5300  |.j...d...S.d.S.
-00000420: 2904 4e7a 0a3c 696d 6720 7372 633d 227a  ).Nz.<img src="z
-00000430: 6322 2073 7479 6c65 3d22 2d6d 6f7a 2d75  c" style="-moz-u
-00000440: 7365 722d 7365 6c65 6374 3a20 6e6f 6e65  ser-select: none
-00000450: 3b20 2d77 6562 6b69 742d 7573 6572 2d73  ; -webkit-user-s
-00000460: 656c 6563 743a 206e 6f6e 653b 2075 7365  elect: none; use
-00000470: 722d 7365 6c65 6374 3a20 6e6f 6e65 3b20  r-select: none; 
-00000480: 6d61 782d 6865 6967 6874 3a35 3070 783b  max-height:50px;
-00000490: 2220 2f3e 7a49 3c69 2063 6c61 7373 3d22  " />zI<i class="
-000004a0: 6661 2066 612d 6164 6472 6573 732d 626f  fa fa-address-bo
-000004b0: 6f6b 2220 7374 796c 653d 2266 6f6e 742d  ok" style="font-
-000004c0: 7369 7a65 3a35 3070 783b 2063 6f6c 6f72  size:50px; color
-000004d0: 3a23 3030 3030 3030 3b22 3e3c 2f69 3e29  :#000000;"></i>)
-000004e0: 0172 0b00 0000 7217 0000 0072 1200 0000  .r....r....r....
-000004f0: 7212 0000 0072 1300 0000 da0a 6765 745f  r....r......get_
-00000500: 696d 6c69 6e6b 2600 0000 730a 0000 0006  imlink&...s.....
-00000510: 0108 0102 0104 ff04 047a 194c 6461 7041  .........z.LdapA
-00000520: 7574 684d 6574 686f 642e 6765 745f 696d  uthMethod.get_im
-00000530: 6c69 6e6b 4663 0300 0000 0000 0000 0000  linkFc..........
-00000540: 0000 0300 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000550: 0000 0064 017c 006a 0017 0053 0029 024e  ...d.|.j...S.).N
-00000560: 7a0b 2f61 7574 682f 7061 6765 2f72 1600  z./auth/page/r..
-00000570: 0000 2903 720d 0000 00da 0c61 7574 685f  ..).r......auth_
-00000580: 7374 6f72 6167 65da 0573 6861 7265 7212  storage..sharer.
-00000590: 0000 0072 1200 0000 7213 0000 00da 0d67  ...r....r......g
-000005a0: 6574 5f61 7574 685f 6c69 6e6b 2e00 0000  et_auth_link....
-000005b0: 7302 0000 000a 017a 1c4c 6461 7041 7574  s......z.LdapAut
-000005c0: 684d 6574 686f 642e 6765 745f 6175 7468  hMethod.get_auth
-000005d0: 5f6c 696e 6b63 0200 0000 0000 0000 0000  _linkc..........
-000005e0: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-000005f0: 0000 0064 0053 0072 0800 0000 7212 0000  ...d.S.r....r...
-00000600: 0029 0272 0d00 0000 721c 0000 0072 1200  .).r....r....r..
-00000610: 0000 7212 0000 0072 1300 0000 da08 6361  ..r....r......ca
-00000620: 6c6c 6261 636b 3100 0000 f302 0000 0004  llback1.........
-00000630: 017a 174c 6461 7041 7574 684d 6574 686f  .z.LdapAuthMetho
-00000640: 642e 6361 6c6c 6261 636b 6306 0000 0000  d.callbackc.....
-00000650: 0000 0000 0000 0006 0000 0001 0000 0043  ...............C
-00000660: 0000 00f3 0400 0000 6401 5300 a902 4e46  ........d.S...NF
-00000670: 7212 0000 0029 0672 0d00 0000 721c 0000  r....).r....r...
-00000680: 00da 0663 6f75 7273 65da 0474 6173 6bda  ...course..task.
-00000690: 0a73 7562 6d69 7373 696f 6eda 086c 616e  .submission..lan
-000006a0: 6775 6167 6572 1200 0000 7212 0000 0072  guager....r....r
-000006b0: 1300 0000 721d 0000 0034 0000 0072 2000  ....r....4...r .
-000006c0: 0000 7a14 4c64 6170 4175 7468 4d65 7468  ..z.LdapAuthMeth
-000006d0: 6f64 2e73 6861 7265 6301 0000 0000 0000  od.sharec.......
-000006e0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000006f0: 0072 2100 0000 7222 0000 0072 1200 0000  .r!...r"...r....
-00000700: 7217 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000710: 1300 0000 da0b 616c 6c6f 775f 7368 6172  ......allow_shar
-00000720: 6537 0000 0072 2000 0000 7a1a 4c64 6170  e7...r ...z.Ldap
-00000730: 4175 7468 4d65 7468 6f64 2e61 6c6c 6f77  AuthMethod.allow
-00000740: 5f73 6861 7265 6301 0000 0000 0000 0000  _sharec.........
-00000750: 0000 0001 0000 0001 0000 0043 0000 0072  ...........C...r
-00000760: 1500 0000 7208 0000 0029 0172 0c00 0000  ....r....).r....
-00000770: 7217 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000780: 1300 0000 da0c 6765 745f 7365 7474 696e  ......get_settin
-00000790: 6773 3a00 0000 7219 0000 007a 1b4c 6461  gs:...r....z.Lda
-000007a0: 7041 7574 684d 6574 686f 642e 6765 745f  pAuthMethod.get_
-000007b0: 7365 7474 696e 6773 4e29 0146 290d da08  settingsN).F)...
-000007c0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000007d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000007e0: 5f5f da07 5f5f 646f 635f 5f72 1400 0000  __..__doc__r....
-000007f0: 7218 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000800: 1e00 0000 721f 0000 0072 1d00 0000 7227  ....r....r....r'
-00000810: 0000 0072 2800 0000 7212 0000 0072 1200  ...r(...r....r..
-00000820: 0000 7212 0000 0072 1300 0000 7207 0000  ..r....r....r...
-00000830: 0015 0000 0073 1600 0000 0800 0401 0804  .....s..........
-00000840: 0806 0803 0803 0a08 0803 0803 0803 0c03  ................
-00000850: 7207 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000860: 0000 0000 0000 0200 0000 4000 0000 731c  ..........@...s.
-00000870: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00000880: 005a 0364 0364 0484 005a 0464 0553 0029  .Z.d.d...Z.d.S.)
-00000890: 06da 164c 4441 5041 7574 6865 6e74 6963  ...LDAPAuthentic
-000008a0: 6174 696f 6e50 6167 6563 0200 0000 0000  ationPagec......
-000008b0: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
-000008c0: 0000 7324 0000 007c 006a 00a0 017c 01a1  ..s$...|.j...|..
-000008d0: 01a0 02a1 007d 027c 006a 036a 0464 0164  .....}.|.j.j.d.d
-000008e0: 027c 0264 0364 048d 0453 0029 054e fa15  .|.d.d...S.).N..
-000008f0: 6375 7374 6f6d 5f61 7574 685f 666f 726d  custom_auth_form
-00000900: 2e68 746d 6cfa 1566 726f 6e74 656e 642f  .html..frontend/
-00000910: 706c 7567 696e 732f 6175 7468 46a9 03da  plugins/authF...
-00000920: 0f74 656d 706c 6174 655f 666f 6c64 6572  .template_folder
-00000930: 7211 0000 00da 0565 7272 6f72 2905 da0c  r......error)...
-00000940: 7573 6572 5f6d 616e 6167 6572 da0f 6765  user_manager..ge
-00000950: 745f 6175 7468 5f6d 6574 686f 6472 2800  t_auth_methodr(.
-00000960: 0000 da0f 7465 6d70 6c61 7465 5f68 656c  ....template_hel
-00000970: 7065 72da 0672 656e 6465 7229 0372 0d00  per..render).r..
-00000980: 0000 720e 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000990: 0072 1200 0000 7213 0000 00da 0347 4554  .r....r......GET
-000009a0: 3f00 0000 7308 0000 0010 010a 0104 0106  ?...s...........
-000009b0: ff7a 1a4c 4441 5041 7574 6865 6e74 6963  .z.LDAPAuthentic
-000009c0: 6174 696f 6e50 6167 652e 4745 5463 0200  ationPage.GETc..
-000009d0: 0000 0000 0000 0000 0000 1300 0000 0b00  ................
-000009e0: 0000 4300 0000 73a4 0300 007c 006a 00a0  ..C...s....|.j..
-000009f0: 017c 01a1 01a0 02a1 007d 0274 036a 046a  .|.......}.t.j.j
-00000a00: 057d 037c 0364 0119 00a0 06a1 00a0 07a1  .}.|.d..........
-00000a10: 007d 047c 0364 0219 007d 057c 05a0 08a1  .}.|.d...}.|....
-00000a20: 0064 036b 0272 2a7c 006a 096a 0a64 0464  .d.k.r*|.j.j.d.d
-00000a30: 057c 0274 0b64 0683 0164 078d 0453 007a  .|.t.d...d...S.z
-00000a40: 5674 0ca0 0d64 087c 0264 0919 0017 0064  Vt...d.|.d.....d
-00000a50: 0a17 0074 0e7c 0264 0b19 0083 0117 00a1  ...t.|.d........
-00000a60: 0101 0064 0c7c 0276 0072 4b7c 0264 0c19  ...d.|.v.rK|.d..
-00000a70: 00a0 0f7c 04a1 017c 0564 0d9c 027d 066e  ...|...|.d...}.n
-00000a80: 0269 007d 067c 02a0 1064 0e64 0fa1 027d  .i.}.|...d.d...}
-00000a90: 0774 116a 1274 116a 137c 0264 0919 007c  .t.j.t.j.|.d...|
-00000aa0: 0264 0b19 007c 0264 1019 0064 116b 0274  .d...|.d...d.k.t
-00000ab0: 116a 1464 128d 0466 0164 0e7c 0769 017c  .j.d...f.d.|.i.|
-00000ac0: 06a4 018e 017d 0874 0ca0 0d64 137c 0264  .....}.t...d.|.d
-00000ad0: 0919 0017 0064 0a17 0074 0e7c 0264 0b19  .....d...t.|.d..
-00000ae0: 0083 0117 00a1 0101 0057 006e 2d04 0074  .........W.n-..t
-00000af0: 1579 ad01 007d 0901 007a 2174 0ca0 1664  .y...}...z!t...d
-00000b00: 147c 0264 0919 0017 0064 1517 0074 0e7c  .|.d.....d...t.|
-00000b10: 0983 0117 00a1 0101 007c 006a 096a 0a64  .........|.j.j.d
-00000b20: 0464 057c 0274 0b64 1683 0164 078d 0457  .d.|.t.d...d...W
-00000b30: 0006 0059 0064 007d 097e 0953 0064 007d  ...Y.d.}.~.S.d.}
-00000b40: 097e 0977 0177 007c 02a0 1064 1764 17a1  .~.w.w.|...d.d..
-00000b50: 027d 0a7c 02a0 1064 1864 18a1 027d 0b7a  .}.|...d.d...}.z
-00000b60: 1c7c 0264 1919 00a0 0f74 177c 0483 01a1  .|.d.....t.|....
-00000b70: 017d 0c7c 086a 187c 0264 1a19 007c 0c7c  .}.|.j.|.d...|.|
-00000b80: 0a7c 0b67 0264 1b8d 0301 007c 086a 1964  .|.g.d.....|.j.d
-00000b90: 1c19 007d 0d57 006e 2e04 0074 1574 1a66  ...}.W.n...t.t.f
-00000ba0: 0290 0179 0401 007d 0e01 007a 1f74 0ca0  ...y...}...z.t..
-00000bb0: 1664 1d74 0e7c 0e83 0117 00a1 0101 007c  .d.t.|.........|
-00000bc0: 08a0 1ba1 0001 007c 006a 096a 0a64 0464  .......|.j.j.d.d
-00000bd0: 057c 0274 0b64 1e83 0164 078d 0457 0006  .|.t.d...d...W..
-00000be0: 0059 0064 007d 0e7e 0e53 0064 007d 0e7e  .Y.d.}.~.S.d.}.~
-00000bf0: 0e77 0177 007c 086a 1c7c 0d64 1f19 007c  .w.w.|.j.|.d...|
-00000c00: 0564 208d 0290 0172 bd7a 877a 247c 0d64  .d ....r.z.z$|.d
-00000c10: 2119 007c 0b19 007d 0f74 1d7c 0f74 1e83  !..|...}.t.|.t..
-00000c20: 0290 0172 217c 0f64 1c19 007d 0f7c 047d  ...r!|.d...}.|.}
-00000c30: 107c 0d64 2119 007c 0a19 007d 1174 1d7c  .|.d!..|...}.t.|
-00000c40: 1174 1e83 0290 0172 337c 1164 1c19 007d  .t.....r3|.d...}
-00000c50: 1157 006e 5c04 0074 1f90 0179 6801 007d  .W.n\..t...yh..}
-00000c60: 0901 007a 2774 0ca0 1664 2274 0e7c 0983  ...z't...d"t.|..
-00000c70: 0117 0064 2317 00a1 0101 007c 006a 096a  ...d#......|.j.j
-00000c80: 0a64 0464 057c 0274 0b64 2483 01a0 0f74  .d.d.|.t.d$....t
-00000c90: 0e7c 0983 01a1 0164 078d 0457 0006 0059  .|.....d...W...Y
-00000ca0: 0064 007d 097e 0957 007c 08a0 1ba1 0001  .d.}.~.W.|......
-00000cb0: 0053 0064 007d 097e 0977 0104 0074 1590  .S.d.}.~.w...t..
-00000cc0: 0179 9001 007d 0901 007a 1c74 0ca0 1664  .y...}...z.t...d
-00000cd0: 25a1 0101 007c 006a 096a 0a64 0464 057c  %....|.j.j.d.d.|
-00000ce0: 0274 0b64 2583 0164 078d 0457 0006 0059  .t.d%..d...W...Y
-00000cf0: 0064 007d 097e 0957 007c 08a0 1ba1 0001  .d.}.~.W.|......
-00000d00: 0053 0064 007d 097e 0977 0177 0057 007c  .S.d.}.~.w.w.W.|
-00000d10: 08a0 1ba1 0001 006e 057c 08a0 1ba1 0001  .......n.|......
-00000d20: 0077 007c 006a 00a0 207c 017c 107c 117c  .w.|.j.. |.|.|.|
-00000d30: 0f69 0066 04a1 0290 0173 ac74 2164 2683  .i.f.....s.t!d&.
-00000d40: 0153 007c 006a 00a0 22a1 00a0 237c 0169  .S.|.j.."...#|.i
-00000d50: 00a1 027d 1274 217c 12a0 1064 2764 28a1  ...}.t!|...d'd(.
-00000d60: 0283 0153 0074 0ca0 0d64 29a1 0101 007c  ...S.t...d)....|
-00000d70: 08a0 1ba1 0001 007c 006a 096a 0a64 0464  .......|.j.j.d.d
-00000d80: 057c 0274 0b64 2a83 0164 078d 0453 0029  .|.t.d*..d...S.)
-00000d90: 2b4e da05 6c6f 6769 6eda 0870 6173 7377  +N..login..passw
-00000da0: 6f72 64da 0072 2e00 0000 722f 0000 007a  ord..r....r/...z
-00000db0: 0e45 6d70 7479 2070 6173 7377 6f72 6472  .Empty passwordr
-00000dc0: 3000 0000 7a0e 436f 6e6e 6563 7469 6e67  0...z.Connecting
-00000dd0: 2074 6f20 da04 686f 7374 7a07 2c20 706f   to ..hostz., po
-00000de0: 7274 20da 0470 6f72 74da 0762 696e 645f  rt ..port..bind_
-00000df0: 646e 2902 da04 7573 6572 7239 0000 00da  dn)...userr9....
-00000e00: 0961 7574 6f5f 6269 6e64 54da 0a65 6e63  .auto_bindT..enc
-00000e10: 7279 7074 696f 6eda 0373 736c 2903 723c  ryption..ssl).r<
-00000e20: 0000 00da 0775 7365 5f73 736c da08 6765  .....use_ssl..ge
-00000e30: 745f 696e 666f 7a0d 436f 6e6e 6563 7465  t_infoz.Connecte
-00000e40: 6420 746f 207a 1e43 616e 2774 2069 6e69  d to z.Can't ini
-00000e50: 7469 616c 7a65 2063 6f6e 6e65 6374 696f  tialze connectio
-00000e60: 6e20 746f 207a 023a 207a 1343 616e 6e6f  n to z.: z.Canno
-00000e70: 7420 636f 6e74 6163 7420 686f 7374 da02  t contact host..
-00000e80: 636e da04 6d61 696c da07 7265 7175 6573  cn..mail..reques
-00000e90: 745a 0762 6173 655f 646e 2901 da0a 6174  tZ.base_dn)...at
-00000ea0: 7472 6962 7574 6573 7201 0000 007a 1643  tributesr....z.C
-00000eb0: 616e 2774 2067 6574 2075 7365 7220 6461  an't get user da
-00000ec0: 7461 203a 207a 0c55 6e6b 6e6f 776e 2075  ta : z.Unknown u
-00000ed0: 7365 72da 0264 6e29 0172 3900 0000 7247  ser..dn).r9...rG
-00000ee0: 0000 007a 1043 616e 2774 2067 6574 2066  ...z.Can't get f
-00000ef0: 6965 6c64 207a 1620 6672 6f6d 2079 6f75  ield z. from you
-00000f00: 7220 4c44 4150 2073 6572 7665 727a 2843  r LDAP serverz(C
-00000f10: 616e 2774 2067 6574 2066 6965 6c64 207b  an't get field {
-00000f20: 7d20 6672 6f6d 2079 6f75 7220 4c44 4150  } from your LDAP
-00000f30: 2073 6572 7665 727a 1a43 616e 2774 2067   serverz.Can't g
-00000f40: 6574 2073 6f6d 6520 7573 6572 2066 6965  et some user fie
-00000f50: 6c64 737a 112f 7369 676e 696e 3f62 696e  ldsz./signin?bin
-00000f60: 6465 7272 6f72 da09 7265 6469 725f 7572  derror..redir_ur
-00000f70: 6cfa 012f 7a0b 4175 7468 2046 6169 6c65  l../z.Auth Faile
-00000f80: 647a 1249 6e63 6f72 7265 6374 2070 6173  dz.Incorrect pas
-00000f90: 7377 6f72 6429 2472 3300 0000 7234 0000  sword)$r3...r4..
-00000fa0: 0072 2800 0000 da05 666c 6173 6b72 4600  .r(.....flaskrF.
-00000fb0: 0000 da04 666f 726d da05 7374 7269 70da  ....form..strip.
-00000fc0: 056c 6f77 6572 da06 7273 7472 6970 7235  .lower..rstripr5
-00000fd0: 0000 0072 3600 0000 da01 5fda 066c 6f67  ...r6....._..log
-00000fe0: 6765 72da 0564 6562 7567 da03 7374 72da  ger..debug..str.
-00000ff0: 0666 6f72 6d61 74da 0367 6574 da05 6c64  .format..get..ld
-00001000: 6170 33da 0a43 6f6e 6e65 6374 696f 6eda  ap3..Connection.
-00001010: 0653 6572 7665 72da 0341 4c4c 7203 0000  .Server..ALLr...
-00001020: 00da 0965 7863 6570 7469 6f6e 7204 0000  ...exceptionr...
-00001030: 00da 0673 6561 7263 68da 0872 6573 706f  ...search..respo
-00001040: 6e73 65da 0a49 6e64 6578 4572 726f 72da  nse..IndexError.
-00001050: 0675 6e62 696e 64da 0672 6562 696e 64da  .unbind..rebind.
-00001060: 0a69 7369 6e73 7461 6e63 65da 046c 6973  .isinstance..lis
-00001070: 74da 084b 6579 4572 726f 72da 0962 696e  t..KeyError..bin
-00001080: 645f 7573 6572 7202 0000 00da 1473 6573  d_userr......ses
-00001090: 7369 6f6e 5f61 7574 685f 7374 6f72 6167  sion_auth_storag
-000010a0: 65da 0a73 6574 6465 6661 756c 7429 1372  e..setdefault).r
-000010b0: 0d00 0000 720e 0000 0072 1100 0000 5a0a  ....r....r....Z.
-000010c0: 6c6f 6769 6e5f 6461 7461 7238 0000 0072  login_datar8...r
-000010d0: 3900 0000 723d 0000 0072 3f00 0000 da04  9...r=...r?.....
-000010e0: 636f 6e6e da01 655a 0761 7474 725f 636e  conn..eZ.attr_cn
-000010f0: 5a09 6174 7472 5f6d 6169 6c5a 0c6c 6461  Z.attr_mailZ.lda
-00001100: 705f 7265 7175 6573 74da 0975 7365 725f  p_request..user_
-00001110: 6461 7461 da02 6578 da05 656d 6169 6cda  data..ex..email.
-00001120: 0875 7365 726e 616d 65da 0872 6561 6c6e  .username..realn
-00001130: 616d 6572 1c00 0000 7212 0000 0072 1200  amer....r....r..
-00001140: 0000 7213 0000 00da 0450 4f53 5444 0000  ..r......POSTD..
-00001150: 0073 a400 0000 1002 0801 1001 0801 0c03  .s..............
-00001160: 0a01 0801 06ff 0203 2202 0801 1601 0402  ........".......
-00001170: 0c02 0401 1a01 0401 04ff 04ff 0202 02fe  ................
-00001180: 0202 06fe 2603 0e01 1e01 0a01 0801 12ff  ....&...........
-00001190: 0880 02fe 0c05 0c01 0201 1201 1801 0e01  ................
-000011a0: 1401 1201 0801 0a01 0801 12ff 0880 02fd  ................
-000011b0: 1406 0401 0c01 0c01 0801 0401 0c01 0c01  ................
-000011c0: 0801 0480 1002 1601 0801 0401 1001 12fe  ................
-000011d0: 0a08 0880 10fb 0a01 0a01 0801 12ff 0a03  ................
-000011e0: 0880 02fb 0280 1405 1802 0801 1202 1001  ................
-000011f0: 0a02 0801 0a01 0801 06ff 7a1b 4c44 4150  ..........z.LDAP
-00001200: 4175 7468 656e 7469 6361 7469 6f6e 5061  AuthenticationPa
-00001210: 6765 2e50 4f53 544e 2905 7229 0000 0072  ge.POSTN).r)...r
-00001220: 2a00 0000 722b 0000 0072 3700 0000 726d  *...r+...r7...rm
-00001230: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00001240: 0000 7213 0000 0072 2d00 0000 3e00 0000  ..r....r-...>...
-00001250: 7306 0000 0008 0008 010c 0572 2d00 0000  s..........r-...
-00001260: 6304 0000 0000 0000 0000 0000 0006 0000  c...............
-00001270: 0007 0000 0043 0000 0073 8e00 0000 7c03  .....C...s....|.
-00001280: a000 6401 6402 a102 7d04 7c04 6403 7601  ..d.d...}.|.d.v.
-00001290: 7211 7401 6404 a002 7c04 a101 8301 8201  r.t.d...|.......
-000012a0: 7c04 6402 6b02 7219 6405 7c03 6401 3c00  |.d.k.r.d.|.d.<.
-000012b0: 7c03 a000 6406 6407 a102 6407 6b02 7225  |...d.d...d.k.r%
-000012c0: 6405 7c03 6406 3c00 7403 7c03 a000 6408  d.|.d.<.t.|...d.
-000012d0: a101 7c03 a000 6409 640a a102 7c03 a000  ..|...d.d...|...
-000012e0: 640b 640c a102 7c03 8304 7d05 7c00 a004  d.d...|...}.|...
-000012f0: 640d 7405 a006 640e a101 a102 0100 7c00  d.t...d.......|.
-00001300: a007 7c05 a101 0100 6405 5300 290f 61fc  ..|.....d.S.).a.
-00001310: 0200 000a 2020 2020 2020 2020 416c 6c6f  ....        Allo
-00001320: 7720 746f 2063 6f6e 6e65 6374 2074 6872  w to connect thr
-00001330: 6f75 6768 2061 204c 4441 5020 7365 7276  ough a LDAP serv
-00001340: 6963 650a 0a20 2020 2020 2020 2041 7661  ice..        Ava
-00001350: 696c 6162 6c65 2063 6f6e 6669 6775 7261  ilable configura
-00001360: 7469 6f6e 3a0a 2020 2020 2020 2020 3a3a  tion:.        ::
-00001370: 0a0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
-00001380: 7567 696e 733a 0a20 2020 2020 2020 2020  ugins:.         
-00001390: 2020 2020 2020 202d 2070 6c75 6769 6e5f         - plugin_
-000013a0: 6d6f 6475 6c65 223a 2022 696e 6769 6e69  module": "ingini
-000013b0: 6f75 732e 6672 6f6e 7465 6e64 2e70 6c75  ous.frontend.plu
-000013c0: 6769 6e73 2e61 7574 682e 6c64 6170 5f61  gins.auth.ldap_a
-000013d0: 7574 6822 2c0a 0a20 2020 2020 2020 2020  uth",..         
-000013e0: 2020 2020 2020 2020 2068 6f73 743a 2022           host: "
-000013f0: 6c64 6170 2e74 6573 742e 6265 222c 0a20  ldap.test.be",. 
-00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001410: 2070 6f72 743a 2030 2c0a 2020 2020 2020   port: 0,.      
-00001420: 2020 2020 2020 2020 2020 2020 656e 6372              encr
-00001430: 7970 7469 6f6e 3a20 2273 736c 222c 0a20  yption: "ssl",. 
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2062 6173 655f 646e 3a20 226f 3d74 6573   base_dn: "o=tes
-00001460: 742c 633d 6265 222c 0a20 2020 2020 2020  t,c=be",.       
-00001470: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-00001480: 7374 3a20 2228 7569 643d 7b7d 2922 2c0a  st: "(uid={})",.
-00001490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014a0: 2020 6e61 6d65 3a20 224c 4441 5020 4c6f    name: "LDAP Lo
-000014b0: 6769 6e22 0a0a 2020 2020 2020 2020 2a68  gin"..        *h
-000014c0: 6f73 742a 0a20 2020 2020 2020 2020 2020  ost*.           
-000014d0: 2054 6865 2068 6f73 7420 6f66 2074 6865   The host of the
-000014e0: 206c 6461 7020 7365 7276 6572 0a20 2020   ldap server.   
-000014f0: 2020 2020 202a 656e 6372 7970 7469 6f6e       *encryption
-00001500: 2a0a 2020 2020 2020 2020 2020 2020 456e  *.            En
-00001510: 6372 7970 7469 6f6e 206d 6574 686f 6420  cryption method 
-00001520: 7573 6564 2074 6f20 636f 6e6e 6563 7420  used to connect 
-00001530: 746f 2074 6865 204c 4441 5020 7365 7276  to the LDAP serv
-00001540: 6572 0a20 2020 2020 2020 2020 2020 2043  er.            C
-00001550: 616e 2062 6520 6569 7468 6572 2022 6e6f  an be either "no
-00001560: 6e65 222c 2022 7373 6c22 206f 7220 2274  ne", "ssl" or "t
-00001570: 6c73 220a 2020 2020 2020 2020 2a72 6571  ls".        *req
-00001580: 7565 7374 2a0a 2020 2020 2020 2020 2020  uest*.          
-00001590: 2020 5265 7175 6573 7420 6d61 6465 2074    Request made t
-000015a0: 6f20 7468 6520 7365 7276 6572 2069 6e20  o the server in 
-000015b0: 6f72 6465 7220 746f 2066 696e 6420 7468  order to find th
-000015c0: 6520 646e 206f 6620 7468 6520 7573 6572  e dn of the user
-000015d0: 2e20 5468 6520 6368 6172 6163 7465 7273  . The characters
-000015e0: 2022 7b7d 2220 7769 6c6c 2062 6520 7265   "{}" will be re
-000015f0: 706c 6163 6564 2062 7920 7468 6520 6c6f  placed by the lo
-00001600: 6769 6e20 6e61 6d65 2e0a 0a20 2020 2072  gin name...    r
-00001610: 4000 0000 da04 6e6f 6e65 2903 726e 0000  @.....none).rn..
-00001620: 0072 4100 0000 da03 746c 737a 1c55 6e6b  .rA.....tlsz.Unk
-00001630: 6e6f 776e 2065 6e63 7279 7074 696f 6e20  nown encryption 
-00001640: 6d65 7468 6f64 207b 7d4e 723c 0000 0072  method {}Nr<...r
-00001650: 0100 0000 720e 0000 0072 0f00 0000 5a04  ....r....r....Z.
-00001660: 4c44 4150 7210 0000 0072 3a00 0000 7a0f  LDAPr....r:...z.
-00001670: 2f61 7574 682f 7061 6765 2f3c 6964 3e5a  /auth/page/<id>Z
-00001680: 166c 6461 7061 7574 6865 6e74 6963 6174  .ldapauthenticat
-00001690: 696f 6e70 6167 6529 0872 5500 0000 da09  ionpage).rU.....
-000016a0: 4578 6365 7074 696f 6e72 5400 0000 7207  ExceptionrT...r.
-000016b0: 0000 00da 0861 6464 5f70 6167 6572 2d00  .....add_pager-.
-000016c0: 0000 da07 6173 5f76 6965 77da 1472 6567  ....as_view..reg
-000016d0: 6973 7465 725f 6175 7468 5f6d 6574 686f  ister_auth_metho
-000016e0: 6429 06da 0e70 6c75 6769 6e5f 6d61 6e61  d)...plugin_mana
-000016f0: 6765 7272 5000 0000 da02 5f32 da04 636f  gerrP....._2..co
-00001700: 6e66 7240 0000 005a 0a74 6865 5f6d 6574  nfr@...Z.the_met
-00001710: 686f 6472 1200 0000 7212 0000 0072 1300  hodr....r....r..
-00001720: 0000 da04 696e 6974 9000 0000 7314 0000  ....init....s...
-00001730: 000c 1b08 010e 0108 0108 0110 0208 0124  ...............$
-00001740: 0212 010e 0172 7700 0000 2912 722c 0000  .....rw...).r,..
-00001750: 00da 076c 6f67 6769 6e67 7256 0000 0072  ...loggingrV...r
-00001760: 4b00 0000 7202 0000 005a 156c 6461 7033  K...r....Z.ldap3
-00001770: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
-00001780: 7203 0000 005a 106c 6461 7033 2e75 7469  r....Z.ldap3.uti
-00001790: 6c73 2e63 6f6e 7672 0400 0000 da1f 696e  ls.convr......in
-000017a0: 6769 6e69 6f75 732e 6672 6f6e 7465 6e64  ginious.frontend
-000017b0: 2e70 6167 6573 2e73 6f63 6961 6c72 0500  .pages.socialr..
-000017c0: 0000 da1f 696e 6769 6e69 6f75 732e 6672  ....inginious.fr
-000017d0: 6f6e 7465 6e64 2e75 7365 725f 6d61 6e61  ontend.user_mana
-000017e0: 6765 7272 0600 0000 da09 6765 744c 6f67  gerr......getLog
-000017f0: 6765 7272 5100 0000 7207 0000 0072 2d00  gerrQ...r....r-.
-00001800: 0000 7277 0000 0072 1200 0000 7212 0000  ..rw...r....r...
-00001810: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
-00001820: 6475 6c65 3e01 0000 0073 1a00 0000 0405  dule>....s......
-00001830: 0802 0801 0801 0c02 0c01 0c01 0c02 0c01  ................
-00001840: 0a02 1002 1029 0c52                      .....).R
+00000190: 6408 6409 8400 5a07 640a 640b 8400 5a08  d.d...Z.d.d...Z.
+000001a0: 640c 640d 8400 5a09 640e 640f 8400 5a0a  d.d...Z.d.d...Z.
+000001b0: 6410 5300 2911 da0e 4c64 6170 4175 7468  d.S.)...LdapAuth
+000001c0: 4d65 7468 6f64 7a1a 0a20 2020 204c 4441  Methodz..    LDA
+000001d0: 5020 6175 7468 206d 6574 686f 640a 2020  P auth method.  
+000001e0: 2020 6305 0000 0000 0000 0000 0000 0005    c.............
+000001f0: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
+00000200: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
+00000210: 5f02 7c04 7c00 5f03 6400 5300 a901 4e29  _.|.|._.d.S...N)
+00000220: 04da 035f 6964 da05 5f6e 616d 65da 075f  ..._id.._name.._
+00000230: 696d 6c69 6e6b da09 5f73 6574 7469 6e67  imlink.._setting
+00000240: 7329 05da 0473 656c 66da 0269 64da 046e  s)...self..id..n
+00000250: 616d 65da 0669 6d6c 696e 6bda 0873 6574  ame..imlink..set
+00000260: 7469 6e67 73a9 0072 1200 0000 fa5c 2f68  tings..r.....\/h
+00000270: 6f6d 652f 616e 7468 6f6e 792f 446f 6375  ome/anthony/Docu
+00000280: 6d65 6e74 732f 696e 6769 6e69 6f75 732d  ments/inginious-
+00000290: 6465 762f 494e 4749 6e69 6f75 732f 696e  dev/INGInious/in
+000002a0: 6769 6e69 6f75 732f 6672 6f6e 7465 6e64  ginious/frontend
+000002b0: 2f70 6c75 6769 6e73 2f61 7574 682f 6c64  /plugins/auth/ld
+000002c0: 6170 5f61 7574 682e 7079 da08 5f5f 696e  ap_auth.py..__in
+000002d0: 6974 5f5f 1a00 0000 7308 0000 0006 0106  it__....s.......
+000002e0: 0106 010a 017a 174c 6461 7041 7574 684d  .....z.LdapAuthM
+000002f0: 6574 686f 642e 5f5f 696e 6974 5f5f 6301  ethod.__init__c.
+00000300: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000310: 0000 0043 0000 00f3 0600 0000 7c00 6a00  ...C........|.j.
+00000320: 5300 7208 0000 00a9 0172 0900 0000 a901  S.r......r......
+00000330: 720d 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000340: 1300 0000 da06 6765 745f 6964 2000 0000  ......get_id ...
+00000350: f302 0000 0006 017a 154c 6461 7041 7574  .......z.LdapAut
+00000360: 684d 6574 686f 642e 6765 745f 6964 6301  hMethod.get_idc.
+00000370: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000380: 0000 0043 0000 0072 1500 0000 7208 0000  ...C...r....r...
+00000390: 0029 0172 0a00 0000 7217 0000 0072 1200  .).r....r....r..
+000003a0: 0000 7212 0000 0072 1300 0000 da08 6765  ..r....r......ge
+000003b0: 745f 6e61 6d65 2300 0000 7219 0000 007a  t_name#...r....z
+000003c0: 174c 6461 7041 7574 684d 6574 686f 642e  .LdapAuthMethod.
+000003d0: 6765 745f 6e61 6d65 6301 0000 0000 0000  get_namec.......
+000003e0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+000003f0: 0073 1800 0000 7c00 6a00 720a 6401 7c00  .s....|.j.r.d.|.
+00000400: 6a00 1700 6402 1700 5300 6403 5300 2904  j...d...S.d.S.).
+00000410: 4e7a 0a3c 696d 6720 7372 633d 227a 6322  Nz.<img src="zc"
+00000420: 2073 7479 6c65 3d22 2d6d 6f7a 2d75 7365   style="-moz-use
+00000430: 722d 7365 6c65 6374 3a20 6e6f 6e65 3b20  r-select: none; 
+00000440: 2d77 6562 6b69 742d 7573 6572 2d73 656c  -webkit-user-sel
+00000450: 6563 743a 206e 6f6e 653b 2075 7365 722d  ect: none; user-
+00000460: 7365 6c65 6374 3a20 6e6f 6e65 3b20 6d61  select: none; ma
+00000470: 782d 6865 6967 6874 3a35 3070 783b 2220  x-height:50px;" 
+00000480: 2f3e 7a49 3c69 2063 6c61 7373 3d22 6661  />zI<i class="fa
+00000490: 2066 612d 6164 6472 6573 732d 626f 6f6b   fa-address-book
+000004a0: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
+000004b0: 7a65 3a35 3070 783b 2063 6f6c 6f72 3a23  ze:50px; color:#
+000004c0: 3030 3030 3030 3b22 3e3c 2f69 3e29 0172  000000;"></i>).r
+000004d0: 0b00 0000 7217 0000 0072 1200 0000 7212  ....r....r....r.
+000004e0: 0000 0072 1300 0000 da0a 6765 745f 696d  ...r......get_im
+000004f0: 6c69 6e6b 2600 0000 730a 0000 0006 0108  link&...s.......
+00000500: 0102 0104 ff04 047a 194c 6461 7041 7574  .......z.LdapAut
+00000510: 684d 6574 686f 642e 6765 745f 696d 6c69  hMethod.get_imli
+00000520: 6e6b 6302 0000 0000 0000 0000 0000 0002  nkc.............
+00000530: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000540: 6401 7c00 6a00 1700 5300 2902 4e7a 0b2f  d.|.j...S.).Nz./
+00000550: 6175 7468 2f70 6167 652f 7216 0000 00a9  auth/page/r.....
+00000560: 0272 0d00 0000 da0c 6175 7468 5f73 746f  .r......auth_sto
+00000570: 7261 6765 7212 0000 0072 1200 0000 7213  rager....r....r.
+00000580: 0000 00da 0d67 6574 5f61 7574 685f 6c69  .....get_auth_li
+00000590: 6e6b 2e00 0000 7302 0000 000a 017a 1c4c  nk....s......z.L
+000005a0: 6461 7041 7574 684d 6574 686f 642e 6765  dapAuthMethod.ge
+000005b0: 745f 6175 7468 5f6c 696e 6b63 0200 0000  t_auth_linkc....
+000005c0: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+000005d0: 4300 0000 7304 0000 0064 0053 0072 0800  C...s....d.S.r..
+000005e0: 0000 7212 0000 0072 1c00 0000 7212 0000  ..r....r....r...
+000005f0: 0072 1200 0000 7213 0000 00da 0863 616c  .r....r......cal
+00000600: 6c62 6163 6b31 0000 0073 0200 0000 0401  lback1...s......
+00000610: 7a17 4c64 6170 4175 7468 4d65 7468 6f64  z.LdapAuthMethod
+00000620: 2e63 616c 6c62 6163 6b63 0100 0000 0000  .callbackc......
+00000630: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000640: 0000 7215 0000 0072 0800 0000 2901 720c  ..r....r....).r.
+00000650: 0000 0072 1700 0000 7212 0000 0072 1200  ...r....r....r..
+00000660: 0000 7213 0000 00da 0c67 6574 5f73 6574  ..r......get_set
+00000670: 7469 6e67 7334 0000 0072 1900 0000 7a1b  tings4...r....z.
+00000680: 4c64 6170 4175 7468 4d65 7468 6f64 2e67  LdapAuthMethod.g
+00000690: 6574 5f73 6574 7469 6e67 734e 290b da08  et_settingsN)...
+000006a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000006b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000006c0: 5f5f da07 5f5f 646f 635f 5f72 1400 0000  __..__doc__r....
+000006d0: 7218 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000006e0: 1e00 0000 721f 0000 0072 2000 0000 7212  ....r....r ...r.
+000006f0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000700: 0000 7207 0000 0015 0000 0073 1200 0000  ..r........s....
+00000710: 0800 0401 0804 0806 0803 0803 0808 0803  ................
+00000720: 0c03 7207 0000 0063 0000 0000 0000 0000  ..r....c........
+00000730: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00000740: 731c 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+00000750: 0284 005a 0364 0364 0484 005a 0464 0553  ...Z.d.d...Z.d.S
+00000760: 0029 06da 164c 4441 5041 7574 6865 6e74  .)...LDAPAuthent
+00000770: 6963 6174 696f 6e50 6167 6563 0200 0000  icationPagec....
+00000780: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+00000790: 4300 0000 7324 0000 007c 006a 00a0 017c  C...s$...|.j...|
+000007a0: 01a1 01a0 02a1 007d 027c 006a 036a 0464  .......}.|.j.j.d
+000007b0: 0164 027c 0264 0364 048d 0453 0029 054e  .d.|.d.d...S.).N
+000007c0: fa15 6375 7374 6f6d 5f61 7574 685f 666f  ..custom_auth_fo
+000007d0: 726d 2e68 746d 6cfa 1566 726f 6e74 656e  rm.html..fronten
+000007e0: 642f 706c 7567 696e 732f 6175 7468 46a9  d/plugins/authF.
+000007f0: 03da 0f74 656d 706c 6174 655f 666f 6c64  ...template_fold
+00000800: 6572 7211 0000 00da 0565 7272 6f72 2905  err......error).
+00000810: da0c 7573 6572 5f6d 616e 6167 6572 da0f  ..user_manager..
+00000820: 6765 745f 6175 7468 5f6d 6574 686f 6472  get_auth_methodr
+00000830: 2000 0000 da0f 7465 6d70 6c61 7465 5f68   .....template_h
+00000840: 656c 7065 72da 0672 656e 6465 7229 0372  elper..render).r
+00000850: 0d00 0000 720e 0000 0072 1100 0000 7212  ....r....r....r.
+00000860: 0000 0072 1200 0000 7213 0000 00da 0347  ...r....r......G
+00000870: 4554 3900 0000 7308 0000 0010 010a 0104  ET9...s.........
+00000880: 0106 ff7a 1a4c 4441 5041 7574 6865 6e74  ...z.LDAPAuthent
+00000890: 6963 6174 696f 6e50 6167 652e 4745 5463  icationPage.GETc
+000008a0: 0200 0000 0000 0000 0000 0000 1300 0000  ................
+000008b0: 0b00 0000 4300 0000 73a4 0300 007c 006a  ....C...s....|.j
+000008c0: 00a0 017c 01a1 01a0 02a1 007d 0274 036a  ...|.......}.t.j
+000008d0: 046a 057d 037c 0364 0119 00a0 06a1 00a0  .j.}.|.d........
+000008e0: 07a1 007d 047c 0364 0219 007d 057c 05a0  ...}.|.d...}.|..
+000008f0: 08a1 0064 036b 0272 2a7c 006a 096a 0a64  ...d.k.r*|.j.j.d
+00000900: 0464 057c 0274 0b64 0683 0164 078d 0453  .d.|.t.d...d...S
+00000910: 007a 5674 0ca0 0d64 087c 0264 0919 0017  .zVt...d.|.d....
+00000920: 0064 0a17 0074 0e7c 0264 0b19 0083 0117  .d...t.|.d......
+00000930: 00a1 0101 0064 0c7c 0276 0072 4b7c 0264  .....d.|.v.rK|.d
+00000940: 0c19 00a0 0f7c 04a1 017c 0564 0d9c 027d  .....|...|.d...}
+00000950: 066e 0269 007d 067c 02a0 1064 0e64 0fa1  .n.i.}.|...d.d..
+00000960: 027d 0774 116a 1274 116a 137c 0264 0919  .}.t.j.t.j.|.d..
+00000970: 007c 0264 0b19 007c 0264 1019 0064 116b  .|.d...|.d...d.k
+00000980: 0274 116a 1464 128d 0466 0164 0e7c 0769  .t.j.d...f.d.|.i
+00000990: 017c 06a4 018e 017d 0874 0ca0 0d64 137c  .|.....}.t...d.|
+000009a0: 0264 0919 0017 0064 0a17 0074 0e7c 0264  .d.....d...t.|.d
+000009b0: 0b19 0083 0117 00a1 0101 0057 006e 2d04  ...........W.n-.
+000009c0: 0074 1579 ad01 007d 0901 007a 2174 0ca0  .t.y...}...z!t..
+000009d0: 1664 147c 0264 0919 0017 0064 1517 0074  .d.|.d.....d...t
+000009e0: 0e7c 0983 0117 00a1 0101 007c 006a 096a  .|.........|.j.j
+000009f0: 0a64 0464 057c 0274 0b64 1683 0164 078d  .d.d.|.t.d...d..
+00000a00: 0457 0006 0059 0064 007d 097e 0953 0064  .W...Y.d.}.~.S.d
+00000a10: 007d 097e 0977 0177 007c 02a0 1064 1764  .}.~.w.w.|...d.d
+00000a20: 17a1 027d 0a7c 02a0 1064 1864 18a1 027d  ...}.|...d.d...}
+00000a30: 0b7a 1c7c 0264 1919 00a0 0f74 177c 0483  .z.|.d.....t.|..
+00000a40: 01a1 017d 0c7c 086a 187c 0264 1a19 007c  ...}.|.j.|.d...|
+00000a50: 0c7c 0a7c 0b67 0264 1b8d 0301 007c 086a  .|.|.g.d.....|.j
+00000a60: 1964 1c19 007d 0d57 006e 2e04 0074 1574  .d...}.W.n...t.t
+00000a70: 1a66 0290 0179 0401 007d 0e01 007a 1f74  .f...y...}...z.t
+00000a80: 0ca0 1664 1d74 0e7c 0e83 0117 00a1 0101  ...d.t.|........
+00000a90: 007c 08a0 1ba1 0001 007c 006a 096a 0a64  .|.......|.j.j.d
+00000aa0: 0464 057c 0274 0b64 1e83 0164 078d 0457  .d.|.t.d...d...W
+00000ab0: 0006 0059 0064 007d 0e7e 0e53 0064 007d  ...Y.d.}.~.S.d.}
+00000ac0: 0e7e 0e77 0177 007c 086a 1c7c 0d64 1f19  .~.w.w.|.j.|.d..
+00000ad0: 007c 0564 208d 0290 0172 bd7a 877a 247c  .|.d ....r.z.z$|
+00000ae0: 0d64 2119 007c 0b19 007d 0f74 1d7c 0f74  .d!..|...}.t.|.t
+00000af0: 1e83 0290 0172 217c 0f64 1c19 007d 0f7c  .....r!|.d...}.|
+00000b00: 047d 107c 0d64 2119 007c 0a19 007d 1174  .}.|.d!..|...}.t
+00000b10: 1d7c 1174 1e83 0290 0172 337c 1164 1c19  .|.t.....r3|.d..
+00000b20: 007d 1157 006e 5c04 0074 1f90 0179 6801  .}.W.n\..t...yh.
+00000b30: 007d 0901 007a 2774 0ca0 1664 2274 0e7c  .}...z't...d"t.|
+00000b40: 0983 0117 0064 2317 00a1 0101 007c 006a  .....d#......|.j
+00000b50: 096a 0a64 0464 057c 0274 0b64 2483 01a0  .j.d.d.|.t.d$...
+00000b60: 0f74 0e7c 0983 01a1 0164 078d 0457 0006  .t.|.....d...W..
+00000b70: 0059 0064 007d 097e 0957 007c 08a0 1ba1  .Y.d.}.~.W.|....
+00000b80: 0001 0053 0064 007d 097e 0977 0104 0074  ...S.d.}.~.w...t
+00000b90: 1590 0179 9001 007d 0901 007a 1c74 0ca0  ...y...}...z.t..
+00000ba0: 1664 25a1 0101 007c 006a 096a 0a64 0464  .d%....|.j.j.d.d
+00000bb0: 057c 0274 0b64 2583 0164 078d 0457 0006  .|.t.d%..d...W..
+00000bc0: 0059 0064 007d 097e 0957 007c 08a0 1ba1  .Y.d.}.~.W.|....
+00000bd0: 0001 0053 0064 007d 097e 0977 0177 0057  ...S.d.}.~.w.w.W
+00000be0: 007c 08a0 1ba1 0001 006e 057c 08a0 1ba1  .|.......n.|....
+00000bf0: 0001 0077 007c 006a 00a0 207c 017c 107c  ...w.|.j.. |.|.|
+00000c00: 117c 0f69 0066 04a1 0290 0173 ac74 2164  .|.i.f.....s.t!d
+00000c10: 2683 0153 007c 006a 00a0 22a1 00a0 237c  &..S.|.j.."...#|
+00000c20: 0169 00a1 027d 1274 217c 12a0 1064 2764  .i...}.t!|...d'd
+00000c30: 28a1 0283 0153 0074 0ca0 0d64 29a1 0101  (....S.t...d)...
+00000c40: 007c 08a0 1ba1 0001 007c 006a 096a 0a64  .|.......|.j.j.d
+00000c50: 0464 057c 0274 0b64 2a83 0164 078d 0453  .d.|.t.d*..d...S
+00000c60: 0029 2b4e da05 6c6f 6769 6eda 0870 6173  .)+N..login..pas
+00000c70: 7377 6f72 64da 0072 2600 0000 7227 0000  sword..r&...r'..
+00000c80: 007a 0e45 6d70 7479 2070 6173 7377 6f72  .z.Empty passwor
+00000c90: 6472 2800 0000 7a0e 436f 6e6e 6563 7469  dr(...z.Connecti
+00000ca0: 6e67 2074 6f20 da04 686f 7374 7a07 2c20  ng to ..hostz., 
+00000cb0: 706f 7274 20da 0470 6f72 74da 0762 696e  port ..port..bin
+00000cc0: 645f 646e 2902 da04 7573 6572 7231 0000  d_dn)...userr1..
+00000cd0: 00da 0961 7574 6f5f 6269 6e64 54da 0a65  ...auto_bindT..e
+00000ce0: 6e63 7279 7074 696f 6eda 0373 736c 2903  ncryption..ssl).
+00000cf0: 7234 0000 00da 0775 7365 5f73 736c da08  r4.....use_ssl..
+00000d00: 6765 745f 696e 666f 7a0d 436f 6e6e 6563  get_infoz.Connec
+00000d10: 7465 6420 746f 207a 1e43 616e 2774 2069  ted to z.Can't i
+00000d20: 6e69 7469 616c 7a65 2063 6f6e 6e65 6374  nitialze connect
+00000d30: 696f 6e20 746f 207a 023a 207a 1343 616e  ion to z.: z.Can
+00000d40: 6e6f 7420 636f 6e74 6163 7420 686f 7374  not contact host
+00000d50: da02 636e da04 6d61 696c da07 7265 7175  ..cn..mail..requ
+00000d60: 6573 745a 0762 6173 655f 646e 2901 da0a  estZ.base_dn)...
+00000d70: 6174 7472 6962 7574 6573 7201 0000 007a  attributesr....z
+00000d80: 1643 616e 2774 2067 6574 2075 7365 7220  .Can't get user 
+00000d90: 6461 7461 203a 207a 0c55 6e6b 6e6f 776e  data : z.Unknown
+00000da0: 2075 7365 72da 0264 6e29 0172 3100 0000   user..dn).r1...
+00000db0: 723f 0000 007a 1043 616e 2774 2067 6574  r?...z.Can't get
+00000dc0: 2066 6965 6c64 207a 1620 6672 6f6d 2079   field z. from y
+00000dd0: 6f75 7220 4c44 4150 2073 6572 7665 727a  our LDAP serverz
+00000de0: 2843 616e 2774 2067 6574 2066 6965 6c64  (Can't get field
+00000df0: 207b 7d20 6672 6f6d 2079 6f75 7220 4c44   {} from your LD
+00000e00: 4150 2073 6572 7665 727a 1a43 616e 2774  AP serverz.Can't
+00000e10: 2067 6574 2073 6f6d 6520 7573 6572 2066   get some user f
+00000e20: 6965 6c64 737a 112f 7369 676e 696e 3f62  ieldsz./signin?b
+00000e30: 696e 6465 7272 6f72 da09 7265 6469 725f  inderror..redir_
+00000e40: 7572 6cfa 012f 7a0b 4175 7468 2046 6169  url../z.Auth Fai
+00000e50: 6c65 647a 1249 6e63 6f72 7265 6374 2070  ledz.Incorrect p
+00000e60: 6173 7377 6f72 6429 2472 2b00 0000 722c  assword)$r+...r,
+00000e70: 0000 0072 2000 0000 da05 666c 6173 6b72  ...r .....flaskr
+00000e80: 3e00 0000 da04 666f 726d da05 7374 7269  >.....form..stri
+00000e90: 70da 056c 6f77 6572 da06 7273 7472 6970  p..lower..rstrip
+00000ea0: 722d 0000 0072 2e00 0000 da01 5fda 066c  r-...r......_..l
+00000eb0: 6f67 6765 72da 0564 6562 7567 da03 7374  ogger..debug..st
+00000ec0: 72da 0666 6f72 6d61 74da 0367 6574 da05  r..format..get..
+00000ed0: 6c64 6170 33da 0a43 6f6e 6e65 6374 696f  ldap3..Connectio
+00000ee0: 6eda 0653 6572 7665 72da 0341 4c4c 7203  n..Server..ALLr.
+00000ef0: 0000 00da 0965 7863 6570 7469 6f6e 7204  .....exceptionr.
+00000f00: 0000 00da 0673 6561 7263 68da 0872 6573  .....search..res
+00000f10: 706f 6e73 65da 0a49 6e64 6578 4572 726f  ponse..IndexErro
+00000f20: 72da 0675 6e62 696e 64da 0672 6562 696e  r..unbind..rebin
+00000f30: 64da 0a69 7369 6e73 7461 6e63 65da 046c  d..isinstance..l
+00000f40: 6973 74da 084b 6579 4572 726f 72da 0962  ist..KeyError..b
+00000f50: 696e 645f 7573 6572 7202 0000 00da 1473  ind_userr......s
+00000f60: 6573 7369 6f6e 5f61 7574 685f 7374 6f72  ession_auth_stor
+00000f70: 6167 65da 0a73 6574 6465 6661 756c 7429  age..setdefault)
+00000f80: 1372 0d00 0000 720e 0000 0072 1100 0000  .r....r....r....
+00000f90: 5a0a 6c6f 6769 6e5f 6461 7461 7230 0000  Z.login_datar0..
+00000fa0: 0072 3100 0000 7235 0000 0072 3700 0000  .r1...r5...r7...
+00000fb0: da04 636f 6e6e da01 655a 0761 7474 725f  ..conn..eZ.attr_
+00000fc0: 636e 5a09 6174 7472 5f6d 6169 6c5a 0c6c  cnZ.attr_mailZ.l
+00000fd0: 6461 705f 7265 7175 6573 74da 0975 7365  dap_request..use
+00000fe0: 725f 6461 7461 da02 6578 da05 656d 6169  r_data..ex..emai
+00000ff0: 6cda 0875 7365 726e 616d 65da 0872 6561  l..username..rea
+00001000: 6c6e 616d 6572 1d00 0000 7212 0000 0072  lnamer....r....r
+00001010: 1200 0000 7213 0000 00da 0450 4f53 543e  ....r......POST>
+00001020: 0000 0073 a400 0000 1002 0801 1001 0801  ...s............
+00001030: 0c03 0a01 0801 06ff 0203 2202 0801 1601  ..........".....
+00001040: 0402 0c02 0401 1a01 0401 04ff 04ff 0202  ................
+00001050: 02fe 0202 06fe 2603 0e01 1e01 0a01 0801  ......&.........
+00001060: 12ff 0880 02fe 0c05 0c01 0201 1201 1801  ................
+00001070: 0e01 1401 1201 0801 0a01 0801 12ff 0880  ................
+00001080: 02fd 1406 0401 0c01 0c01 0801 0401 0c01  ................
+00001090: 0c01 0801 0480 1002 1601 0801 0401 1001  ................
+000010a0: 12fe 0a08 0880 10fb 0a01 0a01 0801 12ff  ................
+000010b0: 0a03 0880 02fb 0280 1405 1802 0801 1202  ................
+000010c0: 1001 0a02 0801 0a01 0801 06ff 7a1b 4c44  ............z.LD
+000010d0: 4150 4175 7468 656e 7469 6361 7469 6f6e  APAuthentication
+000010e0: 5061 6765 2e50 4f53 544e 2905 7221 0000  Page.POSTN).r!..
+000010f0: 0072 2200 0000 7223 0000 0072 2f00 0000  .r"...r#...r/...
+00001100: 7265 0000 0072 1200 0000 7212 0000 0072  re...r....r....r
+00001110: 1200 0000 7213 0000 0072 2500 0000 3800  ....r....r%...8.
+00001120: 0000 7306 0000 0008 0008 010c 0572 2500  ..s..........r%.
+00001130: 0000 6304 0000 0000 0000 0000 0000 0006  ..c.............
+00001140: 0000 0007 0000 0043 0000 0073 8e00 0000  .......C...s....
+00001150: 7c03 a000 6401 6402 a102 7d04 7c04 6403  |...d.d...}.|.d.
+00001160: 7601 7211 7401 6404 a002 7c04 a101 8301  v.r.t.d...|.....
+00001170: 8201 7c04 6402 6b02 7219 6405 7c03 6401  ..|.d.k.r.d.|.d.
+00001180: 3c00 7c03 a000 6406 6407 a102 6407 6b02  <.|...d.d...d.k.
+00001190: 7225 6405 7c03 6406 3c00 7403 7c03 a000  r%d.|.d.<.t.|...
+000011a0: 6408 a101 7c03 a000 6409 640a a102 7c03  d...|...d.d...|.
+000011b0: a000 640b 640c a102 7c03 8304 7d05 7c00  ..d.d...|...}.|.
+000011c0: a004 640d 7405 a006 640e a101 a102 0100  ..d.t...d.......
+000011d0: 7c00 a007 7c05 a101 0100 6405 5300 290f  |...|.....d.S.).
+000011e0: 61fc 0200 000a 2020 2020 2020 2020 416c  a.....        Al
+000011f0: 6c6f 7720 746f 2063 6f6e 6e65 6374 2074  low to connect t
+00001200: 6872 6f75 6768 2061 204c 4441 5020 7365  hrough a LDAP se
+00001210: 7276 6963 650a 0a20 2020 2020 2020 2041  rvice..        A
+00001220: 7661 696c 6162 6c65 2063 6f6e 6669 6775  vailable configu
+00001230: 7261 7469 6f6e 3a0a 2020 2020 2020 2020  ration:.        
+00001240: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
+00001250: 706c 7567 696e 733a 0a20 2020 2020 2020  plugins:.       
+00001260: 2020 2020 2020 2020 202d 2070 6c75 6769           - plugi
+00001270: 6e5f 6d6f 6475 6c65 223a 2022 696e 6769  n_module": "ingi
+00001280: 6e69 6f75 732e 6672 6f6e 7465 6e64 2e70  nious.frontend.p
+00001290: 6c75 6769 6e73 2e61 7574 682e 6c64 6170  lugins.auth.ldap
+000012a0: 5f61 7574 6822 2c0a 0a20 2020 2020 2020  _auth",..       
+000012b0: 2020 2020 2020 2020 2020 2068 6f73 743a             host:
+000012c0: 2022 6c64 6170 2e74 6573 742e 6265 222c   "ldap.test.be",
+000012d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012e0: 2020 2070 6f72 743a 2030 2c0a 2020 2020     port: 0,.    
+000012f0: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00001300: 6372 7970 7469 6f6e 3a20 2273 736c 222c  cryption: "ssl",
+00001310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001320: 2020 2062 6173 655f 646e 3a20 226f 3d74     base_dn: "o=t
+00001330: 6573 742c 633d 6265 222c 0a20 2020 2020  est,c=be",.     
+00001340: 2020 2020 2020 2020 2020 2020 2072 6571               req
+00001350: 7565 7374 3a20 2228 7569 643d 7b7d 2922  uest: "(uid={})"
+00001360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001370: 2020 2020 6e61 6d65 3a20 224c 4441 5020      name: "LDAP 
+00001380: 4c6f 6769 6e22 0a0a 2020 2020 2020 2020  Login"..        
+00001390: 2a68 6f73 742a 0a20 2020 2020 2020 2020  *host*.         
+000013a0: 2020 2054 6865 2068 6f73 7420 6f66 2074     The host of t
+000013b0: 6865 206c 6461 7020 7365 7276 6572 0a20  he ldap server. 
+000013c0: 2020 2020 2020 202a 656e 6372 7970 7469         *encrypti
+000013d0: 6f6e 2a0a 2020 2020 2020 2020 2020 2020  on*.            
+000013e0: 456e 6372 7970 7469 6f6e 206d 6574 686f  Encryption metho
+000013f0: 6420 7573 6564 2074 6f20 636f 6e6e 6563  d used to connec
+00001400: 7420 746f 2074 6865 204c 4441 5020 7365  t to the LDAP se
+00001410: 7276 6572 0a20 2020 2020 2020 2020 2020  rver.           
+00001420: 2043 616e 2062 6520 6569 7468 6572 2022   Can be either "
+00001430: 6e6f 6e65 222c 2022 7373 6c22 206f 7220  none", "ssl" or 
+00001440: 2274 6c73 220a 2020 2020 2020 2020 2a72  "tls".        *r
+00001450: 6571 7565 7374 2a0a 2020 2020 2020 2020  equest*.        
+00001460: 2020 2020 5265 7175 6573 7420 6d61 6465      Request made
+00001470: 2074 6f20 7468 6520 7365 7276 6572 2069   to the server i
+00001480: 6e20 6f72 6465 7220 746f 2066 696e 6420  n order to find 
+00001490: 7468 6520 646e 206f 6620 7468 6520 7573  the dn of the us
+000014a0: 6572 2e20 5468 6520 6368 6172 6163 7465  er. The characte
+000014b0: 7273 2022 7b7d 2220 7769 6c6c 2062 6520  rs "{}" will be 
+000014c0: 7265 706c 6163 6564 2062 7920 7468 6520  replaced by the 
+000014d0: 6c6f 6769 6e20 6e61 6d65 2e0a 0a20 2020  login name...   
+000014e0: 2072 3800 0000 da04 6e6f 6e65 2903 7266   r8.....none).rf
+000014f0: 0000 0072 3900 0000 da03 746c 737a 1c55  ...r9.....tlsz.U
+00001500: 6e6b 6e6f 776e 2065 6e63 7279 7074 696f  nknown encryptio
+00001510: 6e20 6d65 7468 6f64 207b 7d4e 7234 0000  n method {}Nr4..
+00001520: 0072 0100 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00001530: 5a04 4c44 4150 7210 0000 0072 3200 0000  Z.LDAPr....r2...
+00001540: 7a0f 2f61 7574 682f 7061 6765 2f3c 6964  z./auth/page/<id
+00001550: 3e5a 166c 6461 7061 7574 6865 6e74 6963  >Z.ldapauthentic
+00001560: 6174 696f 6e70 6167 6529 0872 4d00 0000  ationpage).rM...
+00001570: da09 4578 6365 7074 696f 6e72 4c00 0000  ..ExceptionrL...
+00001580: 7207 0000 00da 0861 6464 5f70 6167 6572  r......add_pager
+00001590: 2500 0000 da07 6173 5f76 6965 77da 1472  %.....as_view..r
+000015a0: 6567 6973 7465 725f 6175 7468 5f6d 6574  egister_auth_met
+000015b0: 686f 6429 06da 0e70 6c75 6769 6e5f 6d61  hod)...plugin_ma
+000015c0: 6e61 6765 7272 4800 0000 da02 5f32 da04  nagerrH....._2..
+000015d0: 636f 6e66 7238 0000 005a 0a74 6865 5f6d  confr8...Z.the_m
+000015e0: 6574 686f 6472 1200 0000 7212 0000 0072  ethodr....r....r
+000015f0: 1300 0000 da04 696e 6974 8a00 0000 7314  ......init....s.
+00001600: 0000 000c 1b08 010e 0108 0108 0110 0208  ................
+00001610: 0124 0212 010e 0172 6f00 0000 2912 7224  .$.....ro...).r$
+00001620: 0000 00da 076c 6f67 6769 6e67 724e 0000  .....loggingrN..
+00001630: 0072 4300 0000 7202 0000 005a 156c 6461  .rC...r....Z.lda
+00001640: 7033 2e63 6f72 652e 6578 6365 7074 696f  p3.core.exceptio
+00001650: 6e73 7203 0000 005a 106c 6461 7033 2e75  nsr....Z.ldap3.u
+00001660: 7469 6c73 2e63 6f6e 7672 0400 0000 da1f  tils.convr......
+00001670: 696e 6769 6e69 6f75 732e 6672 6f6e 7465  inginious.fronte
+00001680: 6e64 2e70 6167 6573 2e73 6f63 6961 6c72  nd.pages.socialr
+00001690: 0500 0000 da1f 696e 6769 6e69 6f75 732e  ......inginious.
+000016a0: 6672 6f6e 7465 6e64 2e75 7365 725f 6d61  frontend.user_ma
+000016b0: 6e61 6765 7272 0600 0000 da09 6765 744c  nagerr......getL
+000016c0: 6f67 6765 7272 4900 0000 7207 0000 0072  oggerrI...r....r
+000016d0: 2500 0000 726f 0000 0072 1200 0000 7212  %...ro...r....r.
+000016e0: 0000 0072 1200 0000 7213 0000 00da 083c  ...r....r......<
+000016f0: 6d6f 6475 6c65 3e01 0000 0073 1a00 0000  module>....s....
+00001700: 0405 0802 0801 0801 0c02 0c01 0c01 0c02  ................
+00001710: 0c01 0a02 1002 1023 0c52                 .......#.R
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 09:42:50 2023 UTC, .py size: 7053 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1af2 4864 8d1b 0000  o.........Hd....
+00000000: 6f0d 0d0a 0000 0000 8247 4a64 f21a 0000  o........GJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c05 6d08 5a08  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
@@ -19,385 +19,366 @@
 00000120: 0561 626f 7274 da13 496e 7465 726e 616c  .abort..Internal
 00000130: 5365 7276 6572 4572 726f 7229 01da 134f  ServerError)...O
 00000140: 6e65 4c6f 6769 6e5f 5361 6d6c 325f 4175  neLogin_Saml2_Au
 00000150: 7468 2901 da14 4f6e 654c 6f67 696e 5f53  th)...OneLogin_S
 00000160: 616d 6c32 5f55 7469 6c73 2901 da0d 494e  aml2_Utils)...IN
 00000170: 4749 6e69 6f75 7350 6167 6529 01da 0a41  GIniousPage)...A
 00000180: 7574 684d 6574 686f 6463 0000 0000 0000  uthMethodc......
-00000190: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000001a0: 0000 735a 0000 0065 005a 0164 005a 0264  ..sZ...e.Z.d.Z.d
+00000190: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+000001a0: 0000 7348 0000 0065 005a 0164 005a 0264  ..sH...e.Z.d.Z.d
 000001b0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
 000001c0: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-000001d0: 005a 0764 1664 0b64 0c84 015a 0864 0d64  .Z.d.d.d...Z.d.d
-000001e0: 0e84 005a 0964 0f64 1084 005a 0a64 1164  ...Z.d.d...Z.d.d
-000001f0: 1284 005a 0b64 1364 1484 005a 0c64 1553  ...Z.d.d...Z.d.S
-00000200: 0029 17da 0e53 414d 4c41 7574 684d 6574  .)...SAMLAuthMet
-00000210: 686f 647a 1e0a 2020 2020 5341 4d4c 2053  hodz..    SAML S
-00000220: 534f 2061 7574 6820 6d65 7468 6f64 0a20  SO auth method. 
-00000230: 2020 2063 0500 0000 0000 0000 0000 0000     c............
-00000240: 0500 0000 0200 0000 4300 0000 731c 0000  ........C...s...
-00000250: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
-00000260: 005f 027c 047c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
-00000270: 2904 da03 5f69 64da 055f 6e61 6d65 da07  )..._id.._name..
-00000280: 5f69 6d6c 696e 6bda 095f 7365 7474 696e  _imlink.._settin
-00000290: 6773 2905 da04 7365 6c66 da02 6964 da04  gs)...self..id..
-000002a0: 6e61 6d65 da06 696d 6c69 6e6b da08 7365  name..imlink..se
-000002b0: 7474 696e 6773 a900 7215 0000 00fa 5d2f  ttings..r.....]/
-000002c0: 686f 6d65 2f61 6e74 686f 6e79 2f44 6f63  home/anthony/Doc
-000002d0: 756d 656e 7473 2f69 6e67 696e 696f 7573  uments/inginious
-000002e0: 2d64 6576 2f49 4e47 496e 696f 7573 2f69  -dev/INGInious/i
-000002f0: 6e67 696e 696f 7573 2f66 726f 6e74 656e  nginious/fronten
-00000300: 642f 706c 7567 696e 732f 6175 7468 2f73  d/plugins/auth/s
-00000310: 616d 6c32 5f61 7574 682e 7079 da08 5f5f  aml2_auth.py..__
-00000320: 696e 6974 5f5f 1f00 0000 7308 0000 0006  init__....s.....
-00000330: 0106 0106 010a 017a 1753 414d 4c41 7574  .......z.SAMLAut
-00000340: 684d 6574 686f 642e 5f5f 696e 6974 5f5f  hMethod.__init__
-00000350: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000360: 0001 0000 0043 0000 00f3 0600 0000 7c00  .....C........|.
-00000370: 6a00 5300 720b 0000 0029 0172 0c00 0000  j.S.r....).r....
-00000380: a901 7210 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000390: 0072 1600 0000 da06 6765 745f 6964 2500  .r......get_id%.
-000003a0: 0000 f302 0000 0006 017a 1553 414d 4c41  .........z.SAMLA
-000003b0: 7574 684d 6574 686f 642e 6765 745f 6964  uthMethod.get_id
-000003c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000003d0: 0001 0000 0043 0000 0072 1800 0000 720b  .....C...r....r.
-000003e0: 0000 0029 0172 0d00 0000 7219 0000 0072  ...).r....r....r
-000003f0: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
-00000400: 6765 745f 6e61 6d65 2800 0000 721b 0000  get_name(...r...
-00000410: 007a 1753 414d 4c41 7574 684d 6574 686f  .z.SAMLAuthMetho
-00000420: 642e 6765 745f 6e61 6d65 6301 0000 0000  d.get_namec.....
-00000430: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000440: 0000 0073 1800 0000 7c00 6a00 720a 6401  ...s....|.j.r.d.
-00000450: 7c00 6a00 1700 6402 1700 5300 6403 5300  |.j...d...S.d.S.
-00000460: 2904 4e7a 0a3c 696d 6720 7372 633d 227a  ).Nz.<img src="z
-00000470: 6322 2073 7479 6c65 3d22 2d6d 6f7a 2d75  c" style="-moz-u
-00000480: 7365 722d 7365 6c65 6374 3a20 6e6f 6e65  ser-select: none
-00000490: 3b20 2d77 6562 6b69 742d 7573 6572 2d73  ; -webkit-user-s
-000004a0: 656c 6563 743a 206e 6f6e 653b 2075 7365  elect: none; use
-000004b0: 722d 7365 6c65 6374 3a20 6e6f 6e65 3b20  r-select: none; 
-000004c0: 6d61 782d 6865 6967 6874 3a35 3070 783b  max-height:50px;
-000004d0: 2220 2f3e 7a44 3c69 2063 6c61 7373 3d22  " />zD<i class="
-000004e0: 6661 2066 612d 6964 2d63 6172 6422 2073  fa fa-id-card" s
-000004f0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00000500: 3530 7078 3b20 636f 6c6f 723a 2330 3030  50px; color:#000
-00000510: 3030 303b 223e 3c2f 693e 2901 720e 0000  000;"></i>).r...
-00000520: 0072 1900 0000 7215 0000 0072 1500 0000  .r....r....r....
-00000530: 7216 0000 00da 0a67 6574 5f69 6d6c 696e  r......get_imlin
-00000540: 6b2b 0000 0073 0a00 0000 0601 0801 0201  k+...s..........
-00000550: 04ff 0404 7a19 5341 4d4c 4175 7468 4d65  ....z.SAMLAuthMe
-00000560: 7468 6f64 2e67 6574 5f69 6d6c 696e 6b46  thod.get_imlinkF
-00000570: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00000580: 0005 0000 0043 0000 0073 2200 0000 7400  .....C...s"...t.
-00000590: 7401 7c00 6a02 8301 7c00 6a02 8302 7d03  t.|.j...|.j...}.
-000005a0: 7c03 a003 7404 a005 7c01 a101 a101 5300  |...t...|.....S.
-000005b0: 720b 0000 0029 0672 0600 0000 da0f 7072  r....).r......pr
-000005c0: 6570 6172 655f 7265 7175 6573 7472 0f00  epare_requestr..
-000005d0: 0000 da05 6c6f 6769 6eda 046a 736f 6eda  ....login..json.
-000005e0: 0564 756d 7073 2904 7210 0000 00da 0c61  .dumps).r......a
-000005f0: 7574 685f 7374 6f72 6167 65da 0573 6861  uth_storage..sha
-00000600: 7265 da04 6175 7468 7215 0000 0072 1500  re..authr....r..
-00000610: 0000 7216 0000 00da 0d67 6574 5f61 7574  ..r......get_aut
-00000620: 685f 6c69 6e6b 3300 0000 7304 0000 0012  h_link3...s.....
-00000630: 0110 017a 1c53 414d 4c41 7574 684d 6574  ...z.SAMLAuthMet
-00000640: 686f 642e 6765 745f 6175 7468 5f6c 696e  hod.get_auth_lin
-00000650: 6b63 0200 0000 0000 0000 0000 0000 1000  kc..............
-00000660: 0000 0900 0000 4300 0000 73ce 0100 0074  ......C...s....t
-00000670: 007c 006a 0183 017d 0274 026a 036a 047d  .|.j...}.t.j.j.}
-00000680: 0364 017c 0376 0172 2474 0574 0664 0264  .d.|.v.r$t.t.d.d
-00000690: 036a 0774 08a0 097c 0364 0419 00a1 0174  .j.t...|.d.....t
-000006a0: 08a0 097c 0364 0519 00a1 0164 068d 0264  ...|.d.....d...d
-000006b0: 078d 0283 0182 0174 0a7c 027c 006a 0183  .......t.|.|.j..
-000006c0: 027d 047c 04a0 0ba1 0001 007c 04a0 0ca1  .}.|.......|....
-000006d0: 007d 057c 006a 0164 0819 00a0 0d64 0967  .}.|.j.d.....d.g
-000006e0: 00a1 0244 005d 297d 067c 04a0 0ea1 0064  ...D.])}.|.....d
-000006f0: 0a6b 0272 6474 0fa0 1064 0ba1 01a0 1164  .k.rdt...d.....d
-00000700: 0ca1 0101 0074 12a0 137c 006a 01a1 017d  .....t...|.j...}
-00000710: 077c 067c 0764 0819 0064 0d3c 0074 0a7c  .|.|.d...d.<.t.|
-00000720: 027c 0783 027d 047c 04a0 0ba1 0001 007c  .|...}.|.......|
-00000730: 04a0 0ca1 007d 0571 3b74 147c 0583 0164  .....}.q;t.|...d
-00000740: 0e6b 0272 d864 0f7c 006a 0176 0072 d87c  .k.r.d.|.j.v.r.|
-00000750: 04a0 15a1 007d 087c 087c 006a 0164 0f19  .....}.|.|.j.d..
-00000760: 0064 1019 0019 0064 0e19 007d 097c 087c  .d.....d...}.|.|
-00000770: 006a 0164 0f19 0064 1119 0019 0064 0e19  .j.d...d.....d..
-00000780: 007d 0a7c 087c 006a 0164 0f19 0064 1219  .}.|.|.j.d...d..
-00000790: 0019 0064 0e19 007d 0b69 007d 0c7c 006a  ...d...}.i.}.|.j
-000007a0: 01a0 0d64 1369 00a1 02a0 16a1 0044 005d  ...d.i.......D.]
-000007b0: 125c 027d 0d7d 0e7c 0e7c 0876 0072 ae7c  .\.}.}.|.|.v.r.|
-000007c0: 087c 0e19 0064 0e19 006e 0164 147c 0c7c  .|...d...n.d.|.|
-000007d0: 0d3c 0071 a074 17a0 187c 02a1 017d 0f64  .<.q.t...|...}.d
-000007e0: 047c 0376 0072 d47c 0f7c 0364 0419 006b  .|.v.r.|.|.d...k
-000007f0: 0372 d67c 01a0 1974 1aa0 1b7c 0364 0419  .r.|...t...|.d..
-00000800: 00a1 01a1 0101 0074 1c7c 0983 017c 0a7c  .......t.|...|.|
-00000810: 0b7c 0c66 0453 0064 0053 0064 0053 0074  .|.f.S.d.S.d.S.t
-00000820: 0fa0 1064 0ba1 01a0 1d64 1564 16a0 1e7c  ...d.....d.d...|
-00000830: 05a1 0117 00a1 0101 0064 0053 0029 174e  .........d.S.).N
-00000840: 5a11 616c 7265 6164 7952 6564 6972 6563  Z.alreadyRedirec
-00000850: 7465 64e9 c800 0000 61f8 0400 000a 2020  ted.....a.....  
-00000860: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00000870: 444f 4354 5950 4520 6874 6d6c 3e0a 2020  DOCTYPE html>.  
-00000880: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-00000890: 746d 6c3e 0a20 2020 2020 2020 2020 2020  tml>.           
-000008a0: 2020 2020 2020 2020 203c 6865 6164 3e0a           <head>.
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 2020 2020 2020 3c6d 6574 6120 6368          <meta ch
-000008d0: 6172 7365 743d 2275 7466 2d38 2220 2f3e  arset="utf-8" />
-000008e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008f0: 2020 2020 203c 2f68 6561 643e 0a20 2020       </head>.   
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 203c 626f 6479 206f 6e6c 6f61 643d 2264   <body onload="d
-00000920: 6f63 756d 656e 742e 666f 726d 735b 305d  ocument.forms[0]
-00000930: 2e73 7562 6d69 7428 2922 3e0a 2020 2020  .submit()">.    
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 2020 3c6e 6f73 6372 6970 743e 0a20      <noscript>. 
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 2020 2020 2020 2020 203c 703e 0a20             <p>. 
-00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000990: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000009a0: 7374 726f 6e67 3e4e 6f74 653a 3c2f 7374  strong>Note:</st
-000009b0: 726f 6e67 3e20 5369 6e63 6520 796f 7572  rong> Since your
-000009c0: 2062 726f 7773 6572 2064 6f65 7320 6e6f   browser does no
-000009d0: 7420 7375 7070 6f72 7420 4a61 7661 5363  t support JavaSc
-000009e0: 7269 7074 2c0a 2020 2020 2020 2020 2020  ript,.          
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 2020 796f 7520 6d75 7374 2070        you must p
-00000a10: 7265 7373 2074 6865 2043 6f6e 7469 6e75  ress the Continu
-00000a20: 6520 6275 7474 6f6e 206f 6e63 6520 746f  e button once to
-00000a30: 2070 726f 6365 6564 2e0a 2020 2020 2020   proceed..      
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 2020 3c2f 703e 0a20 2020 2020        </p>.     
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2020 203c 2f6e 6f73 6372 6970 743e 0a20     </noscript>. 
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2020 2020 2020 203c 666f 726d 206d 6574         <form met
-00000aa0: 686f 643d 2270 6f73 7422 3e0a 2020 2020  hod="post">.    
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 2020 2020 2020 2020 3c64 6976 3e0a 2020          <div>.  
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000af0: 6e70 7574 2074 7970 653d 2268 6964 6465  nput type="hidde
-00000b00: 6e22 206e 616d 653d 2252 656c 6179 5374  n" name="RelaySt
-00000b10: 6174 6522 2076 616c 7565 3d22 7b52 656c  ate" value="{Rel
-00000b20: 6179 5374 6174 657d 222f 3e0a 2020 2020  ayState}"/>.    
-00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b40: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00000b50: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
-00000b60: 206e 616d 653d 2253 414d 4c52 6573 706f   name="SAMLRespo
-00000b70: 6e73 6522 2076 616c 7565 3d22 7b53 414d  nse" value="{SAM
-00000b80: 4c52 6573 706f 6e73 657d 222f 3e0a 2020  LResponse}"/>.  
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000bb0: 6e70 7574 2074 7970 653d 2268 6964 6465  nput type="hidde
-00000bc0: 6e22 206e 616d 653d 2261 6c72 6561 6479  n" name="already
-00000bd0: 5265 6469 7265 6374 6564 2220 7661 6c75  Redirected" valu
-00000be0: 653d 2279 6573 222f 3e0a 2020 2020 2020  e="yes"/>.      
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2020 2020 2020 2020 203c 6e6f 7363 7269           <noscri
-00000c30: 7074 3e0a 2020 2020 2020 2020 2020 2020  pt>.            
+000001d0: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
+000001e0: 005a 0964 0e64 0f84 005a 0a64 1053 0029  .Z.d.d...Z.d.S.)
+000001f0: 11da 0e53 414d 4c41 7574 684d 6574 686f  ...SAMLAuthMetho
+00000200: 647a 1e0a 2020 2020 5341 4d4c 2053 534f  dz..    SAML SSO
+00000210: 2061 7574 6820 6d65 7468 6f64 0a20 2020   auth method.   
+00000220: 2063 0500 0000 0000 0000 0000 0000 0500   c..............
+00000230: 0000 0200 0000 4300 0000 731c 0000 007c  ......C...s....|
+00000240: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
+00000250: 027c 047c 005f 0364 0053 00a9 014e 2904  .|.|._.d.S...N).
+00000260: da03 5f69 64da 055f 6e61 6d65 da07 5f69  .._id.._name.._i
+00000270: 6d6c 696e 6bda 095f 7365 7474 696e 6773  mlink.._settings
+00000280: 2905 da04 7365 6c66 da02 6964 da04 6e61  )...self..id..na
+00000290: 6d65 da06 696d 6c69 6e6b da08 7365 7474  me..imlink..sett
+000002a0: 696e 6773 a900 7215 0000 00fa 5d2f 686f  ings..r.....]/ho
+000002b0: 6d65 2f61 6e74 686f 6e79 2f44 6f63 756d  me/anthony/Docum
+000002c0: 656e 7473 2f69 6e67 696e 696f 7573 2d64  ents/inginious-d
+000002d0: 6576 2f49 4e47 496e 696f 7573 2f69 6e67  ev/INGInious/ing
+000002e0: 696e 696f 7573 2f66 726f 6e74 656e 642f  inious/frontend/
+000002f0: 706c 7567 696e 732f 6175 7468 2f73 616d  plugins/auth/sam
+00000300: 6c32 5f61 7574 682e 7079 da08 5f5f 696e  l2_auth.py..__in
+00000310: 6974 5f5f 1f00 0000 7308 0000 0006 0106  it__....s.......
+00000320: 0106 010a 017a 1753 414d 4c41 7574 684d  .....z.SAMLAuthM
+00000330: 6574 686f 642e 5f5f 696e 6974 5f5f 6301  ethod.__init__c.
+00000340: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000350: 0000 0043 0000 00f3 0600 0000 7c00 6a00  ...C........|.j.
+00000360: 5300 720b 0000 0029 0172 0c00 0000 a901  S.r....).r......
+00000370: 7210 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000380: 1600 0000 da06 6765 745f 6964 2500 0000  ......get_id%...
+00000390: f302 0000 0006 017a 1553 414d 4c41 7574  .......z.SAMLAut
+000003a0: 684d 6574 686f 642e 6765 745f 6964 6301  hMethod.get_idc.
+000003b0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000003c0: 0000 0043 0000 0072 1800 0000 720b 0000  ...C...r....r...
+000003d0: 0029 0172 0d00 0000 7219 0000 0072 1500  .).r....r....r..
+000003e0: 0000 7215 0000 0072 1600 0000 da08 6765  ..r....r......ge
+000003f0: 745f 6e61 6d65 2800 0000 721b 0000 007a  t_name(...r....z
+00000400: 1753 414d 4c41 7574 684d 6574 686f 642e  .SAMLAuthMethod.
+00000410: 6765 745f 6e61 6d65 6301 0000 0000 0000  get_namec.......
+00000420: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000430: 0073 1800 0000 7c00 6a00 720a 6401 7c00  .s....|.j.r.d.|.
+00000440: 6a00 1700 6402 1700 5300 6403 5300 2904  j...d...S.d.S.).
+00000450: 4e7a 0a3c 696d 6720 7372 633d 227a 6322  Nz.<img src="zc"
+00000460: 2073 7479 6c65 3d22 2d6d 6f7a 2d75 7365   style="-moz-use
+00000470: 722d 7365 6c65 6374 3a20 6e6f 6e65 3b20  r-select: none; 
+00000480: 2d77 6562 6b69 742d 7573 6572 2d73 656c  -webkit-user-sel
+00000490: 6563 743a 206e 6f6e 653b 2075 7365 722d  ect: none; user-
+000004a0: 7365 6c65 6374 3a20 6e6f 6e65 3b20 6d61  select: none; ma
+000004b0: 782d 6865 6967 6874 3a35 3070 783b 2220  x-height:50px;" 
+000004c0: 2f3e 7a44 3c69 2063 6c61 7373 3d22 6661  />zD<i class="fa
+000004d0: 2066 612d 6964 2d63 6172 6422 2073 7479   fa-id-card" sty
+000004e0: 6c65 3d22 666f 6e74 2d73 697a 653a 3530  le="font-size:50
+000004f0: 7078 3b20 636f 6c6f 723a 2330 3030 3030  px; color:#00000
+00000500: 303b 223e 3c2f 693e 2901 720e 0000 0072  0;"></i>).r....r
+00000510: 1900 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000520: 0000 00da 0a67 6574 5f69 6d6c 696e 6b2b  .....get_imlink+
+00000530: 0000 0073 0a00 0000 0601 0801 0201 04ff  ...s............
+00000540: 0404 7a19 5341 4d4c 4175 7468 4d65 7468  ..z.SAMLAuthMeth
+00000550: 6f64 2e67 6574 5f69 6d6c 696e 6b63 0200  od.get_imlinkc..
+00000560: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00000570: 0000 4300 0000 7322 0000 0074 0074 017c  ..C...s"...t.t.|
+00000580: 006a 0283 017c 006a 0283 027d 027c 02a0  .j...|.j...}.|..
+00000590: 0374 04a0 057c 01a1 01a1 0153 0072 0b00  .t...|.....S.r..
+000005a0: 0000 2906 7206 0000 00da 0f70 7265 7061  ..).r......prepa
+000005b0: 7265 5f72 6571 7565 7374 720f 0000 00da  re_requestr.....
+000005c0: 056c 6f67 696e da04 6a73 6f6e da05 6475  .login..json..du
+000005d0: 6d70 7329 0372 1000 0000 da0c 6175 7468  mps).r......auth
+000005e0: 5f73 746f 7261 6765 da04 6175 7468 7215  _storage..authr.
+000005f0: 0000 0072 1500 0000 7216 0000 00da 0d67  ...r....r......g
+00000600: 6574 5f61 7574 685f 6c69 6e6b 3300 0000  et_auth_link3...
+00000610: 7304 0000 0012 0110 017a 1c53 414d 4c41  s........z.SAMLA
+00000620: 7574 684d 6574 686f 642e 6765 745f 6175  uthMethod.get_au
+00000630: 7468 5f6c 696e 6b63 0200 0000 0000 0000  th_linkc........
+00000640: 0000 0000 1000 0000 0900 0000 4300 0000  ............C...
+00000650: 73ce 0100 0074 007c 006a 0183 017d 0274  s....t.|.j...}.t
+00000660: 026a 036a 047d 0364 017c 0376 0172 2474  .j.j.}.d.|.v.r$t
+00000670: 0574 0664 0264 036a 0774 08a0 097c 0364  .t.d.d.j.t...|.d
+00000680: 0419 00a1 0174 08a0 097c 0364 0519 00a1  .....t...|.d....
+00000690: 0164 068d 0264 078d 0283 0182 0174 0a7c  .d...d.......t.|
+000006a0: 027c 006a 0183 027d 047c 04a0 0ba1 0001  .|.j...}.|......
+000006b0: 007c 04a0 0ca1 007d 057c 006a 0164 0819  .|.....}.|.j.d..
+000006c0: 00a0 0d64 0967 00a1 0244 005d 297d 067c  ...d.g...D.])}.|
+000006d0: 04a0 0ea1 0064 0a6b 0272 6474 0fa0 1064  .....d.k.rdt...d
+000006e0: 0ba1 01a0 1164 0ca1 0101 0074 12a0 137c  .....d.....t...|
+000006f0: 006a 01a1 017d 077c 067c 0764 0819 0064  .j...}.|.|.d...d
+00000700: 0d3c 0074 0a7c 027c 0783 027d 047c 04a0  .<.t.|.|...}.|..
+00000710: 0ba1 0001 007c 04a0 0ca1 007d 0571 3b74  .....|.....}.q;t
+00000720: 147c 0583 0164 0e6b 0272 d864 0f7c 006a  .|...d.k.r.d.|.j
+00000730: 0176 0072 d87c 04a0 15a1 007d 087c 087c  .v.r.|.....}.|.|
+00000740: 006a 0164 0f19 0064 1019 0019 0064 0e19  .j.d...d.....d..
+00000750: 007d 097c 087c 006a 0164 0f19 0064 1119  .}.|.|.j.d...d..
+00000760: 0019 0064 0e19 007d 0a7c 087c 006a 0164  ...d...}.|.|.j.d
+00000770: 0f19 0064 1219 0019 0064 0e19 007d 0b69  ...d.....d...}.i
+00000780: 007d 0c7c 006a 01a0 0d64 1369 00a1 02a0  .}.|.j...d.i....
+00000790: 16a1 0044 005d 125c 027d 0d7d 0e7c 0e7c  ...D.].\.}.}.|.|
+000007a0: 0876 0072 ae7c 087c 0e19 0064 0e19 006e  .v.r.|.|...d...n
+000007b0: 0164 147c 0c7c 0d3c 0071 a074 17a0 187c  .d.|.|.<.q.t...|
+000007c0: 02a1 017d 0f64 047c 0376 0072 d47c 0f7c  ...}.d.|.v.r.|.|
+000007d0: 0364 0419 006b 0372 d67c 01a0 1974 1aa0  .d...k.r.|...t..
+000007e0: 1b7c 0364 0419 00a1 01a1 0101 0074 1c7c  .|.d.........t.|
+000007f0: 0983 017c 0a7c 0b7c 0c66 0453 0064 0053  ...|.|.|.f.S.d.S
+00000800: 0064 0053 0074 0fa0 1064 0ba1 01a0 1d64  .d.S.t...d.....d
+00000810: 1564 16a0 1e7c 05a1 0117 00a1 0101 0064  .d...|.........d
+00000820: 0053 0029 174e 5a11 616c 7265 6164 7952  .S.).NZ.alreadyR
+00000830: 6564 6972 6563 7465 64e9 c800 0000 61f8  edirected.....a.
+00000840: 0400 000a 2020 2020 2020 2020 2020 2020  ....            
+00000850: 2020 2020 3c21 444f 4354 5950 4520 6874      <!DOCTYPE ht
+00000860: 6d6c 3e0a 2020 2020 2020 2020 2020 2020  ml>.            
+00000870: 2020 2020 3c68 746d 6c3e 0a20 2020 2020      <html>.     
+00000880: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000890: 6865 6164 3e0a 2020 2020 2020 2020 2020  head>.          
+000008a0: 2020 2020 2020 2020 2020 2020 2020 3c6d                <m
+000008b0: 6574 6120 6368 6172 7365 743d 2275 7466  eta charset="utf
+000008c0: 2d38 2220 2f3e 0a20 2020 2020 2020 2020  -8" />.         
+000008d0: 2020 2020 2020 2020 2020 203c 2f68 6561             </hea
+000008e0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+000008f0: 2020 2020 2020 203c 626f 6479 206f 6e6c         <body onl
+00000900: 6f61 643d 2264 6f63 756d 656e 742e 666f  oad="document.fo
+00000910: 726d 735b 305d 2e73 7562 6d69 7428 2922  rms[0].submit()"
+00000920: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000930: 2020 2020 2020 2020 2020 3c6e 6f73 6372            <noscr
+00000940: 6970 743e 0a20 2020 2020 2020 2020 2020  ipt>.           
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 203c 703e 0a20 2020 2020 2020 2020 2020   <p>.           
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 203c 7374 726f 6e67 3e4e 6f74       <strong>Not
+00000990: 653a 3c2f 7374 726f 6e67 3e20 5369 6e63  e:</strong> Sinc
+000009a0: 6520 796f 7572 2062 726f 7773 6572 2064  e your browser d
+000009b0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+000009c0: 4a61 7661 5363 7269 7074 2c0a 2020 2020  JavaScript,.    
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 2020 2020 2020 796f 7520              you 
+000009f0: 6d75 7374 2070 7265 7373 2074 6865 2043  must press the C
+00000a00: 6f6e 7469 6e75 6520 6275 7474 6f6e 206f  ontinue button o
+00000a10: 6e63 6520 746f 2070 726f 6365 6564 2e0a  nce to proceed..
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2020 2020 2020 2020 2020 2020 3c2f 703e              </p>
+00000a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a50: 2020 2020 2020 2020 203c 2f6e 6f73 6372           </noscr
+00000a60: 6970 743e 0a20 2020 2020 2020 2020 2020  ipt>.           
+00000a70: 2020 2020 2020 2020 2020 2020 203c 666f               <fo
+00000a80: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
+00000a90: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000ab0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+00000ae0: 2268 6964 6465 6e22 206e 616d 653d 2252  "hidden" name="R
+00000af0: 656c 6179 5374 6174 6522 2076 616c 7565  elayState" value
+00000b00: 3d22 7b52 656c 6179 5374 6174 657d 222f  ="{RelayState}"/
+00000b10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 3c69 6e70 7574 2074 7970 653d 2268    <input type="h
+00000b40: 6964 6465 6e22 206e 616d 653d 2253 414d  idden" name="SAM
+00000b50: 4c52 6573 706f 6e73 6522 2076 616c 7565  LResponse" value
+00000b60: 3d22 7b53 414d 4c52 6573 706f 6e73 657d  ="{SAMLResponse}
+00000b70: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+00000ba0: 2268 6964 6465 6e22 206e 616d 653d 2261  "hidden" name="a
+00000bb0: 6c72 6561 6479 5265 6469 7265 6374 6564  lreadyRedirected
+00000bc0: 2220 7661 6c75 653d 2279 6573 222f 3e0a  " value="yes"/>.
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000bf0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00000c00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000c10: 6e6f 7363 7269 7074 3e0a 2020 2020 2020  noscript>.      
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c30: 2020 2020 2020 2020 2020 3c64 6976 3e0a            <div>.
 00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 3c64 6976 3e0a 2020 2020 2020      <div>.      
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000c80: 6e70 7574 2074 7970 653d 2273 7562 6d69  nput type="submi
-00000c90: 7422 2076 616c 7565 3d22 436f 6e74 696e  t" value="Contin
-00000ca0: 7565 222f 3e0a 2020 2020 2020 2020 2020  ue"/>.          
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 203c 2f6e 6f73 6372           </noscr
-00000cf0: 6970 743e 0a20 2020 2020 2020 2020 2020  ipt>.           
-00000d00: 2020 2020 2020 2020 2020 2020 203c 2f66               </f
-00000d10: 6f72 6d3e 0a20 2020 2020 2020 2020 2020  orm>.           
-00000d20: 2020 2020 2020 2020 203c 2f62 6f64 793e           </body>
-00000d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d40: 203c 2f68 746d 6c3e 0a20 2020 2020 2020   </html>.       
-00000d50: 2020 2020 20da 0a52 656c 6179 5374 6174       ..RelayStat
-00000d60: 65da 0c53 414d 4c52 6573 706f 6e73 6529  e..SAMLResponse)
-00000d70: 0272 2700 0000 7228 0000 0029 02da 0673  .r'...r(...)...s
-00000d80: 7461 7475 73da 0872 6573 706f 6e73 655a  tatus..responseZ
-00000d90: 0369 6470 5a13 6164 6469 7469 6f6e 616c  .idpZ.additional
-00000da0: 5835 3039 6365 7274 737a 3353 6967 6e61  X509certsz3Signa
-00000db0: 7475 7265 2076 616c 6964 6174 696f 6e20  ture validation 
-00000dc0: 6661 696c 6564 2e20 5341 4d4c 2052 6573  failed. SAML Res
-00000dd0: 706f 6e73 6520 7265 6a65 6374 6564 7a21  ponse rejectedz!
-00000de0: 696e 6769 6e69 6f75 732e 7765 6261 7070  inginious.webapp
-00000df0: 2e70 6c75 6769 6e2e 6175 7468 2e73 616d  .plugin.auth.sam
-00000e00: 6c7a 1d54 7279 696e 6720 616e 6f74 6865  lz.Trying anothe
-00000e10: 7220 6365 7274 6966 6963 6174 652e 2e2e  r certificate...
-00000e20: 5a08 7835 3039 6365 7274 7201 0000 00da  Z.x509certr.....
-00000e30: 0a61 7474 7269 6275 7465 73da 0375 6964  .attributes..uid
-00000e40: da02 636e da05 656d 6169 6cda 0a61 6464  ..cn..email..add
-00000e50: 6974 696f 6e61 6cda 007a 2345 7272 6f72  itional..z#Error
-00000e60: 7320 7768 696c 6520 7072 6f63 6573 7369  s while processi
-00000e70: 6e67 2072 6573 706f 6e73 6520 3a20 fa02  ng response : ..
-00000e80: 2c20 291f 721e 0000 0072 0f00 0000 da05  , ).r....r......
-00000e90: 666c 6173 6bda 0772 6571 7565 7374 da04  flask..request..
-00000ea0: 666f 726d 7204 0000 0072 0300 0000 da06  formr....r......
-00000eb0: 666f 726d 6174 da04 6874 6d6c da06 6573  format..html..es
-00000ec0: 6361 7065 7206 0000 00da 1070 726f 6365  caper......proce
-00000ed0: 7373 5f72 6573 706f 6e73 655a 0a67 6574  ss_responseZ.get
-00000ee0: 5f65 7272 6f72 73da 0367 6574 5a15 6765  _errors..getZ.ge
-00000ef0: 745f 6c61 7374 5f65 7272 6f72 5f72 6561  t_last_error_rea
-00000f00: 736f 6eda 076c 6f67 6769 6e67 da09 6765  son..logging..ge
-00000f10: 744c 6f67 6765 72da 0564 6562 7567 da04  tLogger..debug..
-00000f20: 636f 7079 da08 6465 6570 636f 7079 da03  copy..deepcopy..
-00000f30: 6c65 6e5a 0e67 6574 5f61 7474 7269 6275  lenZ.get_attribu
-00000f40: 7465 73da 0569 7465 6d73 7207 0000 005a  tes..itemsr....Z
-00000f50: 0c67 6574 5f73 656c 665f 7572 6cda 0675  .get_self_url..u
-00000f60: 7064 6174 6572 2000 0000 da05 6c6f 6164  pdater .....load
-00000f70: 73da 0373 7472 da05 6572 726f 72da 046a  s..str..error..j
-00000f80: 6f69 6e29 1072 1000 0000 7222 0000 00da  oin).r....r"....
-00000f90: 0372 6571 da0a 696e 7075 745f 6461 7461  .req..input_data
-00000fa0: 7224 0000 00da 0665 7272 6f72 73da 0463  r$.....errors..c
-00000fb0: 6572 74da 0c6e 6577 5f73 6574 7469 6e67  ert..new_setting
-00000fc0: 73da 0561 7474 7273 da08 7573 6572 6e61  s..attrs..userna
-00000fd0: 6d65 da08 7265 616c 6e61 6d65 722e 0000  me..realnamer...
-00000fe0: 0072 2f00 0000 da05 6669 656c 64da 0375  .r/.....field..u
-00000ff0: 726e 5a08 7365 6c66 5f75 726c 7215 0000  rnZ.self_urlr...
-00001000: 0072 1500 0000 7216 0000 00da 0863 616c  .r....r......cal
-00001010: 6c62 6163 6b37 0000 0073 4600 0000 0a01  lback7...sF.....
-00001020: 0801 0802 0801 1a1b 0ce5 0c1d 0801 0801  ................
-00001030: 1604 0c01 1002 0c01 0c01 0a02 0801 0801  ................
-00001040: 0280 1602 0801 1601 1601 1601 0402 1a01  ................
-00001050: 1e01 0a03 1401 1401 1002 08fd 0c05 0801  ................
-00001060: 06ff 0402 7a17 5341 4d4c 4175 7468 4d65  ....z.SAMLAuthMe
-00001070: 7468 6f64 2e63 616c 6c62 6163 6b63 0600  thod.callbackc..
-00001080: 0000 0000 0000 0000 0000 0600 0000 0100  ................
-00001090: 0000 4300 0000 f304 0000 0064 0153 00a9  ..C........d.S..
-000010a0: 024e 4672 1500 0000 2906 7210 0000 0072  .NFr....).r....r
-000010b0: 2200 0000 da06 636f 7572 7365 da04 7461  ".....course..ta
-000010c0: 736b da0a 7375 626d 6973 7369 6f6e da08  sk..submission..
-000010d0: 6c61 6e67 7561 6765 7215 0000 0072 1500  languager....r..
-000010e0: 0000 7216 0000 0072 2300 0000 7f00 0000  ..r....r#.......
-000010f0: f302 0000 0004 017a 1453 414d 4c41 7574  .......z.SAMLAut
-00001100: 684d 6574 686f 642e 7368 6172 6563 0100  hMethod.sharec..
-00001110: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00001120: 0000 4300 0000 7251 0000 0072 5200 0000  ..C...rQ...rR...
-00001130: 7215 0000 0072 1900 0000 7215 0000 0072  r....r....r....r
-00001140: 1500 0000 7216 0000 00da 0b61 6c6c 6f77  ....r......allow
-00001150: 5f73 6861 7265 8200 0000 7257 0000 007a  _share....rW...z
-00001160: 1a53 414d 4c41 7574 684d 6574 686f 642e  .SAMLAuthMethod.
-00001170: 616c 6c6f 775f 7368 6172 6563 0100 0000  allow_sharec....
-00001180: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001190: 4300 0000 7218 0000 0072 0b00 0000 2901  C...r....r....).
-000011a0: 720f 0000 0072 1900 0000 7215 0000 0072  r....r....r....r
-000011b0: 1500 0000 7216 0000 00da 0c67 6574 5f73  ....r......get_s
-000011c0: 6574 7469 6e67 7385 0000 0072 1b00 0000  ettings....r....
-000011d0: 7a1b 5341 4d4c 4175 7468 4d65 7468 6f64  z.SAMLAuthMethod
-000011e0: 2e67 6574 5f73 6574 7469 6e67 734e 2901  .get_settingsN).
-000011f0: 4629 0dda 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
-00001200: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001210: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00001220: 7217 0000 0072 1a00 0000 721c 0000 0072  r....r....r....r
-00001230: 1d00 0000 7225 0000 0072 5000 0000 7223  ....r%...rP...r#
-00001240: 0000 0072 5800 0000 7259 0000 0072 1500  ...rX...rY...r..
-00001250: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001260: 0072 0a00 0000 1a00 0000 7316 0000 0008  .r........s.....
-00001270: 0004 0108 0408 0608 0308 030a 0808 0408  ................
-00001280: 4808 030c 0372 0a00 0000 6301 0000 0000  H....r....c.....
-00001290: 0000 0000 0000 0002 0000 0008 0000 0043  ...............C
-000012a0: 0000 0073 7000 0000 7400 6a01 6a02 6401  ...sp...t.j.j.d.
-000012b0: 1700 7c00 6402 1900 1700 6403 6404 9c02  ..|.d.....d.d...
-000012c0: 7c00 6405 1900 6406 3c00 7403 7400 6a01  |.d...d.<.t.t.j.
-000012d0: 6a04 8301 7d01 7400 6a01 6a05 6407 6b02  j...}.t.j.j.d.k.
-000012e0: 721f 6408 6e01 6409 7400 6a01 6a06 7c01  r.d.n.d.t.j.j.|.
-000012f0: 6a07 7400 6a01 6a08 7400 6a01 6a09 a00a  j.t.j.j.t.j.j...
-00001300: a100 7400 6a01 6a0b a00a a100 7400 6a01  ..t.j.j.....t.j.
-00001310: 6a0c 640a 9c07 5300 290b 7a16 2050 7265  j.d...S.).z. Pre
-00001320: 7061 7265 2053 414d 4c20 7265 7175 6573  pare SAML reques
-00001330: 7420 7a0e 6175 7468 2f63 616c 6c62 6163  t z.auth/callbac
-00001340: 6b2f 7211 0000 007a 2e75 726e 3a6f 6173  k/r....z.urn:oas
-00001350: 6973 3a6e 616d 6573 3a74 633a 5341 4d4c  is:names:tc:SAML
-00001360: 3a32 2e30 3a62 696e 6469 6e67 733a 4854  :2.0:bindings:HT
-00001370: 5450 2d50 4f53 5429 02da 0375 726c da07  TP-POST)...url..
-00001380: 6269 6e64 696e 67da 0273 705a 1861 7373  binding..spZ.ass
-00001390: 6572 7469 6f6e 436f 6e73 756d 6572 5365  ertionConsumerSe
-000013a0: 7276 6963 65da 0568 7474 7073 da02 6f6e  rvice..https..on
-000013b0: da03 6f66 6629 0772 6100 0000 5a09 6874  ..off).ra...Z.ht
-000013c0: 7470 5f68 6f73 74da 0b73 6572 7665 725f  tp_host..server_
-000013d0: 706f 7274 da0b 7363 7269 7074 5f6e 616d  port..script_nam
-000013e0: 65da 0867 6574 5f64 6174 615a 0970 6f73  e..get_dataZ.pos
-000013f0: 745f 6461 7461 da0c 7175 6572 795f 7374  t_data..query_st
-00001400: 7269 6e67 290d 7232 0000 0072 3300 0000  ring).r2...r3...
-00001410: da08 7572 6c5f 726f 6f74 7202 0000 0072  ..url_rootr....r
-00001420: 5e00 0000 da06 7363 6865 6d65 da04 686f  ^.....scheme..ho
-00001430: 7374 da04 706f 7274 da04 7061 7468 da04  st..port..path..
-00001440: 6172 6773 723d 0000 0072 3400 0000 7267  argsr=...r4...rg
-00001450: 0000 0029 0272 1400 0000 5a08 7572 6c5f  ...).r....Z.url_
-00001460: 6461 7461 7215 0000 0072 1500 0000 7216  datar....r....r.
-00001470: 0000 0072 1e00 0000 8900 0000 7318 0000  ...r........s...
-00001480: 0012 0502 010e fe0c 0612 0206 0104 0106  ................
-00001490: 010a 010a 0106 0306 f772 1e00 0000 6300  .........r....c.
-000014a0: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-000014b0: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-000014c0: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
-000014d0: 2904 da0c 4d65 7461 6461 7461 5061 6765  )...MetadataPage
-000014e0: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-000014f0: 0005 0000 0043 0000 0073 6200 0000 7c00  .....C...sb...|.
-00001500: 6a00 a001 7c01 a101 a002 a100 7d02 7403  j...|.......}.t.
-00001510: 7404 7c02 8301 7c02 8302 7d03 7c03 a002  t.|...|...}.|...
-00001520: a100 a005 a100 7d04 7c03 a002 a100 a006  ......}.|.......
-00001530: 7c04 a101 7d05 7407 7c05 8301 6401 6b02  |...}.t.|...d.k.
-00001540: 7229 7408 7c04 6402 6403 6404 8d03 5300  r)t.|.d.d.d...S.
-00001550: 7409 6405 a00a 7c05 a101 6406 8d01 8201  t.d...|...d.....
-00001560: 2907 4e72 0100 0000 7226 0000 007a 0874  ).Nr....r&...z.t
-00001570: 6578 742f 786d 6c29 0372 2a00 0000 7229  ext/xml).r*...r)
-00001580: 0000 00da 086d 696d 6574 7970 6572 3100  .....mimetyper1.
-00001590: 0000 2901 da0b 6465 7363 7269 7074 696f  ..)...descriptio
-000015a0: 6e29 0bda 0c75 7365 725f 6d61 6e61 6765  n)...user_manage
-000015b0: 72da 0f67 6574 5f61 7574 685f 6d65 7468  r..get_auth_meth
-000015c0: 6f64 7259 0000 0072 0600 0000 721e 0000  odrY...r....r...
-000015d0: 005a 0f67 6574 5f73 705f 6d65 7461 6461  .Z.get_sp_metada
-000015e0: 7461 da11 7661 6c69 6461 7465 5f6d 6574  ta..validate_met
-000015f0: 6164 6174 6172 3f00 0000 7203 0000 0072  adatar?...r....r
-00001600: 0500 0000 7245 0000 0029 0672 1000 0000  ....rE...).r....
-00001610: 7211 0000 0072 1400 0000 7224 0000 00da  r....r....r$....
-00001620: 086d 6574 6164 6174 6172 4800 0000 7215  .metadatarH...r.
-00001630: 0000 0072 1500 0000 7216 0000 00da 0347  ...r....r......G
-00001640: 4554 a200 0000 730e 0000 0010 010e 010c  ET....s.........
-00001650: 010e 010c 020e 0110 027a 104d 6574 6164  .........z.Metad
-00001660: 6174 6150 6167 652e 4745 544e 2904 725a  ataPage.GETN).rZ
-00001670: 0000 0072 5b00 0000 725c 0000 0072 7500  ...r[...r\...ru.
-00001680: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00001690: 0072 1600 0000 726e 0000 00a1 0000 0073  .r....rn.......s
-000016a0: 0400 0000 0800 0c01 726e 0000 0063 0400  ........rn...c..
-000016b0: 0000 0000 0000 0000 0000 0400 0000 0900  ................
-000016c0: 0000 4300 0000 734a 0000 007c 00a0 0064  ..C...sJ...|...d
-000016d0: 0174 01a0 0264 027c 03a0 0364 03a1 0117  .t...d.|...d....
-000016e0: 00a1 01a1 0201 007c 00a0 0474 057c 03a0  .......|...t.|..
-000016f0: 0364 03a1 017c 03a0 0364 0464 05a1 027c  .d...|...d.d...|
-00001700: 03a0 0364 0664 07a1 027c 0383 04a1 0101  ...d.d...|......
-00001710: 0064 0053 0029 084e 7a13 2f61 7574 682f  .d.S.).Nz./auth/
-00001720: 3c69 643e 2f6d 6574 6164 6174 615a 0d6d  <id>/metadataZ.m
-00001730: 6574 6164 6174 6170 6167 655f 7211 0000  etadatapage_r...
-00001740: 0072 1200 0000 5a04 5341 4d4c 7213 0000  .r....Z.SAMLr...
-00001750: 0072 3000 0000 2906 da08 6164 645f 7061  .r0...)...add_pa
-00001760: 6765 726e 0000 00da 0761 735f 7669 6577  gern.....as_view
-00001770: 7239 0000 00da 1472 6567 6973 7465 725f  r9.....register_
-00001780: 6175 7468 5f6d 6574 686f 6472 0a00 0000  auth_methodr....
-00001790: 2904 da0e 706c 7567 696e 5f6d 616e 6167  )...plugin_manag
-000017a0: 6572 da0e 636f 7572 7365 5f66 6163 746f  er..course_facto
-000017b0: 7279 da06 636c 6965 6e74 da04 636f 6e66  ry..client..conf
-000017c0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-000017d0: 0469 6e69 74ae 0000 0073 0400 0000 1c01  .init....s......
-000017e0: 2e01 727d 0000 0029 1972 5d00 0000 723d  ..r}...).r]...r=
-000017f0: 0000 0072 3600 0000 7220 0000 0072 3a00  ...r6...r ...r:.
-00001800: 0000 7232 0000 00da 0c75 726c 6c69 622e  ..r2.....urllib.
-00001810: 7061 7273 6572 0200 0000 7203 0000 005a  parser....r....Z
-00001820: 1377 6572 6b7a 6575 672e 6578 6365 7074  .werkzeug.except
-00001830: 696f 6e73 7204 0000 0072 0500 0000 5a13  ionsr....r....Z.
-00001840: 6f6e 656c 6f67 696e 2e73 616d 6c32 2e61  onelogin.saml2.a
-00001850: 7574 6872 0600 0000 5a14 6f6e 656c 6f67  uthr....Z.onelog
-00001860: 696e 2e73 616d 6c32 2e75 7469 6c73 7207  in.saml2.utilsr.
-00001870: 0000 00da 1e69 6e67 696e 696f 7573 2e66  .....inginious.f
-00001880: 726f 6e74 656e 642e 7061 6765 732e 7574  rontend.pages.ut
-00001890: 696c 7372 0800 0000 da1f 696e 6769 6e69  ilsr......ingini
-000018a0: 6f75 732e 6672 6f6e 7465 6e64 2e75 7365  ous.frontend.use
-000018b0: 725f 6d61 6e61 6765 7272 0900 0000 7214  r_managerr....r.
-000018c0: 0000 0072 0a00 0000 721e 0000 0072 6e00  ...r....r....rn.
-000018d0: 0000 727d 0000 0072 1500 0000 7215 0000  ..r}...r....r...
-000018e0: 0072 1500 0000 7216 0000 00da 083c 6d6f  .r....r......<mo
-000018f0: 6475 6c65 3e01 0000 0073 2400 0000 0405  dule>....s$.....
-00001900: 0802 0801 0801 0801 0801 0c02 0c01 1001  ................
-00001910: 0c01 0c01 0c02 0c01 0402 1003 086f 1018  .............o..
-00001920: 0c0d                                     ..
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+00000c70: 2273 7562 6d69 7422 2076 616c 7565 3d22  "submit" value="
+00000c80: 436f 6e74 696e 7565 222f 3e0a 2020 2020  Continue"/>.    
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000cb0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000cd0: 2f6e 6f73 6372 6970 743e 0a20 2020 2020  /noscript>.     
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
+00000d00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000d10: 2f62 6f64 793e 0a20 2020 2020 2020 2020  /body>.         
+00000d20: 2020 2020 2020 203c 2f68 746d 6c3e 0a20         </html>. 
+00000d30: 2020 2020 2020 2020 2020 20da 0a52 656c             ..Rel
+00000d40: 6179 5374 6174 65da 0c53 414d 4c52 6573  ayState..SAMLRes
+00000d50: 706f 6e73 6529 0272 2600 0000 7227 0000  ponse).r&...r'..
+00000d60: 0029 02da 0673 7461 7475 73da 0872 6573  .)...status..res
+00000d70: 706f 6e73 655a 0369 6470 5a13 6164 6469  ponseZ.idpZ.addi
+00000d80: 7469 6f6e 616c 5835 3039 6365 7274 737a  tionalX509certsz
+00000d90: 3353 6967 6e61 7475 7265 2076 616c 6964  3Signature valid
+00000da0: 6174 696f 6e20 6661 696c 6564 2e20 5341  ation failed. SA
+00000db0: 4d4c 2052 6573 706f 6e73 6520 7265 6a65  ML Response reje
+00000dc0: 6374 6564 7a21 696e 6769 6e69 6f75 732e  ctedz!inginious.
+00000dd0: 7765 6261 7070 2e70 6c75 6769 6e2e 6175  webapp.plugin.au
+00000de0: 7468 2e73 616d 6c7a 1d54 7279 696e 6720  th.samlz.Trying 
+00000df0: 616e 6f74 6865 7220 6365 7274 6966 6963  another certific
+00000e00: 6174 652e 2e2e 5a08 7835 3039 6365 7274  ate...Z.x509cert
+00000e10: 7201 0000 00da 0a61 7474 7269 6275 7465  r......attribute
+00000e20: 73da 0375 6964 da02 636e da05 656d 6169  s..uid..cn..emai
+00000e30: 6cda 0a61 6464 6974 696f 6e61 6cda 007a  l..additional..z
+00000e40: 2345 7272 6f72 7320 7768 696c 6520 7072  #Errors while pr
+00000e50: 6f63 6573 7369 6e67 2072 6573 706f 6e73  ocessing respons
+00000e60: 6520 3a20 fa02 2c20 291f 721e 0000 0072  e : .., ).r....r
+00000e70: 0f00 0000 da05 666c 6173 6bda 0772 6571  ......flask..req
+00000e80: 7565 7374 da04 666f 726d 7204 0000 0072  uest..formr....r
+00000e90: 0300 0000 da06 666f 726d 6174 da04 6874  ......format..ht
+00000ea0: 6d6c da06 6573 6361 7065 7206 0000 00da  ml..escaper.....
+00000eb0: 1070 726f 6365 7373 5f72 6573 706f 6e73  .process_respons
+00000ec0: 655a 0a67 6574 5f65 7272 6f72 73da 0367  eZ.get_errors..g
+00000ed0: 6574 5a15 6765 745f 6c61 7374 5f65 7272  etZ.get_last_err
+00000ee0: 6f72 5f72 6561 736f 6eda 076c 6f67 6769  or_reason..loggi
+00000ef0: 6e67 da09 6765 744c 6f67 6765 72da 0564  ng..getLogger..d
+00000f00: 6562 7567 da04 636f 7079 da08 6465 6570  ebug..copy..deep
+00000f10: 636f 7079 da03 6c65 6e5a 0e67 6574 5f61  copy..lenZ.get_a
+00000f20: 7474 7269 6275 7465 73da 0569 7465 6d73  ttributes..items
+00000f30: 7207 0000 005a 0c67 6574 5f73 656c 665f  r....Z.get_self_
+00000f40: 7572 6cda 0675 7064 6174 6572 2000 0000  url..updater ...
+00000f50: da05 6c6f 6164 73da 0373 7472 da05 6572  ..loads..str..er
+00000f60: 726f 72da 046a 6f69 6e29 1072 1000 0000  ror..join).r....
+00000f70: 7222 0000 00da 0372 6571 da0a 696e 7075  r".....req..inpu
+00000f80: 745f 6461 7461 7223 0000 00da 0665 7272  t_datar#.....err
+00000f90: 6f72 73da 0463 6572 74da 0c6e 6577 5f73  ors..cert..new_s
+00000fa0: 6574 7469 6e67 73da 0561 7474 7273 da08  ettings..attrs..
+00000fb0: 7573 6572 6e61 6d65 da08 7265 616c 6e61  username..realna
+00000fc0: 6d65 722d 0000 0072 2e00 0000 da05 6669  mer-...r......fi
+00000fd0: 656c 64da 0375 726e 5a08 7365 6c66 5f75  eld..urnZ.self_u
+00000fe0: 726c 7215 0000 0072 1500 0000 7216 0000  rlr....r....r...
+00000ff0: 00da 0863 616c 6c62 6163 6b37 0000 0073  ...callback7...s
+00001000: 4600 0000 0a01 0801 0802 0801 1a1b 0ce5  F...............
+00001010: 0c1d 0801 0801 1604 0c01 1002 0c01 0c01  ................
+00001020: 0a02 0801 0801 0280 1602 0801 1601 1601  ................
+00001030: 1601 0402 1a01 1e01 0a03 1401 1401 1002  ................
+00001040: 08fd 0c05 0801 06ff 0402 7a17 5341 4d4c  ..........z.SAML
+00001050: 4175 7468 4d65 7468 6f64 2e63 616c 6c62  AuthMethod.callb
+00001060: 6163 6b63 0100 0000 0000 0000 0000 0000  ackc............
+00001070: 0100 0000 0100 0000 4300 0000 7218 0000  ........C...r...
+00001080: 0072 0b00 0000 2901 720f 0000 0072 1900  .r....).r....r..
+00001090: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000010a0: 00da 0c67 6574 5f73 6574 7469 6e67 737f  ...get_settings.
+000010b0: 0000 0072 1b00 0000 7a1b 5341 4d4c 4175  ...r....z.SAMLAu
+000010c0: 7468 4d65 7468 6f64 2e67 6574 5f73 6574  thMethod.get_set
+000010d0: 7469 6e67 734e 290b da08 5f5f 6e61 6d65  tingsN)...__name
+000010e0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000010f0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00001100: 646f 635f 5f72 1700 0000 721a 0000 0072  doc__r....r....r
+00001110: 1c00 0000 721d 0000 0072 2400 0000 724f  ....r....r$...rO
+00001120: 0000 0072 5000 0000 7215 0000 0072 1500  ...rP...r....r..
+00001130: 0000 7215 0000 0072 1600 0000 720a 0000  ..r....r....r...
+00001140: 001a 0000 0073 1200 0000 0800 0401 0804  .....s..........
+00001150: 0806 0803 0803 0808 0804 0c48 720a 0000  ...........Hr...
+00001160: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001170: 0000 0800 0000 4300 0000 7370 0000 0074  ......C...sp...t
+00001180: 006a 016a 0264 0117 007c 0064 0219 0017  .j.j.d...|.d....
+00001190: 0064 0364 049c 027c 0064 0519 0064 063c  .d.d...|.d...d.<
+000011a0: 0074 0374 006a 016a 0483 017d 0174 006a  .t.t.j.j...}.t.j
+000011b0: 016a 0564 076b 0272 1f64 086e 0164 0974  .j.d.k.r.d.n.d.t
+000011c0: 006a 016a 067c 016a 0774 006a 016a 0874  .j.j.|.j.t.j.j.t
+000011d0: 006a 016a 09a0 0aa1 0074 006a 016a 0ba0  .j.j.....t.j.j..
+000011e0: 0aa1 0074 006a 016a 0c64 0a9c 0753 0029  ...t.j.j.d...S.)
+000011f0: 0b7a 1620 5072 6570 6172 6520 5341 4d4c  .z. Prepare SAML
+00001200: 2072 6571 7565 7374 207a 0e61 7574 682f   request z.auth/
+00001210: 6361 6c6c 6261 636b 2f72 1100 0000 7a2e  callback/r....z.
+00001220: 7572 6e3a 6f61 7369 733a 6e61 6d65 733a  urn:oasis:names:
+00001230: 7463 3a53 414d 4c3a 322e 303a 6269 6e64  tc:SAML:2.0:bind
+00001240: 696e 6773 3a48 5454 502d 504f 5354 2902  ings:HTTP-POST).
+00001250: da03 7572 6cda 0762 696e 6469 6e67 da02  ..url..binding..
+00001260: 7370 5a18 6173 7365 7274 696f 6e43 6f6e  spZ.assertionCon
+00001270: 7375 6d65 7253 6572 7669 6365 da05 6874  sumerService..ht
+00001280: 7470 73da 026f 6eda 036f 6666 2907 7258  tps..on..off).rX
+00001290: 0000 005a 0968 7474 705f 686f 7374 da0b  ...Z.http_host..
+000012a0: 7365 7276 6572 5f70 6f72 74da 0b73 6372  server_port..scr
+000012b0: 6970 745f 6e61 6d65 da08 6765 745f 6461  ipt_name..get_da
+000012c0: 7461 5a09 706f 7374 5f64 6174 61da 0c71  taZ.post_data..q
+000012d0: 7565 7279 5f73 7472 696e 6729 0d72 3100  uery_string).r1.
+000012e0: 0000 7232 0000 00da 0875 726c 5f72 6f6f  ..r2.....url_roo
+000012f0: 7472 0200 0000 7255 0000 00da 0673 6368  tr....rU.....sch
+00001300: 656d 65da 0468 6f73 74da 0470 6f72 74da  eme..host..port.
+00001310: 0470 6174 68da 0461 7267 7372 3c00 0000  .path..argsr<...
+00001320: 7233 0000 0072 5e00 0000 2902 7214 0000  r3...r^...).r...
+00001330: 005a 0875 726c 5f64 6174 6172 1500 0000  .Z.url_datar....
+00001340: 7215 0000 0072 1600 0000 721e 0000 0083  r....r....r.....
+00001350: 0000 0073 1800 0000 1205 0201 0efe 0c06  ...s............
+00001360: 1202 0601 0401 0601 0a01 0a01 0603 06f7  ................
+00001370: 721e 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001380: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
+00001390: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+000013a0: 005a 0364 0353 0029 04da 0c4d 6574 6164  .Z.d.S.)...Metad
+000013b0: 6174 6150 6167 6563 0200 0000 0000 0000  ataPagec........
+000013c0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+000013d0: 7362 0000 007c 006a 00a0 017c 01a1 01a0  sb...|.j...|....
+000013e0: 02a1 007d 0274 0374 047c 0283 017c 0283  ...}.t.t.|...|..
+000013f0: 027d 037c 03a0 02a1 00a0 05a1 007d 047c  .}.|.........}.|
+00001400: 03a0 02a1 00a0 067c 04a1 017d 0574 077c  .......|...}.t.|
+00001410: 0583 0164 016b 0272 2974 087c 0464 0264  ...d.k.r)t.|.d.d
+00001420: 0364 048d 0353 0074 0964 05a0 0a7c 05a1  .d...S.t.d...|..
+00001430: 0164 068d 0182 0129 074e 7201 0000 0072  .d.....).Nr....r
+00001440: 2500 0000 7a08 7465 7874 2f78 6d6c 2903  %...z.text/xml).
+00001450: 7229 0000 0072 2800 0000 da08 6d69 6d65  r)...r(.....mime
+00001460: 7479 7065 7230 0000 0029 01da 0b64 6573  typer0...)...des
+00001470: 6372 6970 7469 6f6e 290b da0c 7573 6572  cription)...user
+00001480: 5f6d 616e 6167 6572 da0f 6765 745f 6175  _manager..get_au
+00001490: 7468 5f6d 6574 686f 6472 5000 0000 7206  th_methodrP...r.
+000014a0: 0000 0072 1e00 0000 5a0f 6765 745f 7370  ...r....Z.get_sp
+000014b0: 5f6d 6574 6164 6174 61da 1176 616c 6964  _metadata..valid
+000014c0: 6174 655f 6d65 7461 6461 7461 723e 0000  ate_metadatar>..
+000014d0: 0072 0300 0000 7205 0000 0072 4400 0000  .r....r....rD...
+000014e0: 2906 7210 0000 0072 1100 0000 7214 0000  ).r....r....r...
+000014f0: 0072 2300 0000 da08 6d65 7461 6461 7461  .r#.....metadata
+00001500: 7247 0000 0072 1500 0000 7215 0000 0072  rG...r....r....r
+00001510: 1600 0000 da03 4745 549c 0000 0073 0e00  ......GET....s..
+00001520: 0000 1001 0e01 0c01 0e01 0c02 0e01 1002  ................
+00001530: 7a10 4d65 7461 6461 7461 5061 6765 2e47  z.MetadataPage.G
+00001540: 4554 4e29 0472 5100 0000 7252 0000 0072  ETN).rQ...rR...r
+00001550: 5300 0000 726c 0000 0072 1500 0000 7215  S...rl...r....r.
+00001560: 0000 0072 1500 0000 7216 0000 0072 6500  ...r....r....re.
+00001570: 0000 9b00 0000 7304 0000 0008 000c 0172  ......s........r
+00001580: 6500 0000 6304 0000 0000 0000 0000 0000  e...c...........
+00001590: 0004 0000 0009 0000 0043 0000 0073 4a00  .........C...sJ.
+000015a0: 0000 7c00 a000 6401 7401 a002 6402 7c03  ..|...d.t...d.|.
+000015b0: a003 6403 a101 1700 a101 a102 0100 7c00  ..d...........|.
+000015c0: a004 7405 7c03 a003 6403 a101 7c03 a003  ..t.|...d...|...
+000015d0: 6404 6405 a102 7c03 a003 6406 6407 a102  d.d...|...d.d...
+000015e0: 7c03 8304 a101 0100 6400 5300 2908 4e7a  |.......d.S.).Nz
+000015f0: 132f 6175 7468 2f3c 6964 3e2f 6d65 7461  ./auth/<id>/meta
+00001600: 6461 7461 5a0d 6d65 7461 6461 7461 7061  dataZ.metadatapa
+00001610: 6765 5f72 1100 0000 7212 0000 005a 0453  ge_r....r....Z.S
+00001620: 414d 4c72 1300 0000 722f 0000 0029 06da  AMLr....r/...)..
+00001630: 0861 6464 5f70 6167 6572 6500 0000 da07  .add_pagere.....
+00001640: 6173 5f76 6965 7772 3800 0000 da14 7265  as_viewr8.....re
+00001650: 6769 7374 6572 5f61 7574 685f 6d65 7468  gister_auth_meth
+00001660: 6f64 720a 0000 0029 04da 0e70 6c75 6769  odr....)...plugi
+00001670: 6e5f 6d61 6e61 6765 72da 0e63 6f75 7273  n_manager..cours
+00001680: 655f 6661 6374 6f72 79da 0663 6c69 656e  e_factory..clien
+00001690: 74da 0463 6f6e 6672 1500 0000 7215 0000  t..confr....r...
+000016a0: 0072 1600 0000 da04 696e 6974 a800 0000  .r......init....
+000016b0: 7304 0000 001c 012e 0172 7400 0000 2919  s........rt...).
+000016c0: 7254 0000 0072 3c00 0000 7235 0000 0072  rT...r<...r5...r
+000016d0: 2000 0000 7239 0000 0072 3100 0000 da0c   ...r9...r1.....
+000016e0: 7572 6c6c 6962 2e70 6172 7365 7202 0000  urllib.parser...
+000016f0: 0072 0300 0000 5a13 7765 726b 7a65 7567  .r....Z.werkzeug
+00001700: 2e65 7863 6570 7469 6f6e 7372 0400 0000  .exceptionsr....
+00001710: 7205 0000 005a 136f 6e65 6c6f 6769 6e2e  r....Z.onelogin.
+00001720: 7361 6d6c 322e 6175 7468 7206 0000 005a  saml2.authr....Z
+00001730: 146f 6e65 6c6f 6769 6e2e 7361 6d6c 322e  .onelogin.saml2.
+00001740: 7574 696c 7372 0700 0000 da1e 696e 6769  utilsr......ingi
+00001750: 6e69 6f75 732e 6672 6f6e 7465 6e64 2e70  nious.frontend.p
+00001760: 6167 6573 2e75 7469 6c73 7208 0000 00da  ages.utilsr.....
+00001770: 1f69 6e67 696e 696f 7573 2e66 726f 6e74  .inginious.front
+00001780: 656e 642e 7573 6572 5f6d 616e 6167 6572  end.user_manager
+00001790: 7209 0000 0072 1400 0000 720a 0000 0072  r....r....r....r
+000017a0: 1e00 0000 7265 0000 0072 7400 0000 7215  ....re...rt...r.
+000017b0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000017c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000017d0: 7324 0000 0004 0508 0208 0108 0108 0108  s$..............
+000017e0: 010c 020c 0110 010c 010c 010c 020c 0104  ................
+000017f0: 0210 0308 6910 180c 0d                   ....i....
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/custom_auth_form.html` & `INGInious-0.8.7/inginious/frontend/plugins/auth/custom_auth_form.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/facebook_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/facebook_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/github_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/github_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/google_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/google_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/ldap_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/ldap_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/linkedin_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/linkedin_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/saml2_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/saml2_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/auth/twitter_auth.py` & `INGInious-0.8.7/inginious/frontend/plugins/auth/twitter_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/contests/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 09:42:50 2023 UTC, .py size: 11265 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1af2 4864 012c 0000  o.........Hd.,..
+00000000: 610d 0d0a 0000 0000 5fdd 8760 012c 0000  a......._..`.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6405 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
@@ -41,454 +41,456 @@
 00000280: 686f 6d65 2f61 6e74 686f 6e79 2f44 6f63  home/anthony/Doc
 00000290: 756d 656e 7473 2f69 6e67 696e 696f 7573  uments/inginious
 000002a0: 2d64 6576 2f49 4e47 496e 696f 7573 2f69  -dev/INGInious/i
 000002b0: 6e67 696e 696f 7573 2f66 726f 6e74 656e  nginious/fronten
 000002c0: 642f 706c 7567 696e 732f 636f 6e74 6573  d/plugins/contes
 000002d0: 7473 2f5f 5f69 6e69 745f 5f2e 7079 da0e  ts/__init__.py..
 000002e0: 6164 645f 6164 6d69 6e5f 6d65 6e75 1500  add_admin_menu..
-000002f0: 0000 7302 0000 0004 0272 0d00 0000 6303  ..s......r....c.
+000002f0: 0000 7302 0000 0000 0272 0d00 0000 6303  ..s......r....c.
 00000300: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00000310: 0000 0043 0000 0073 2400 0000 7400 7c00  ...C...s$...t.|.
-00000320: 8301 7d03 7c03 6401 1900 7210 7401 7c03  ..}.|.d...r.t.|.
+00000310: 0000 0043 0000 0073 2800 0000 7400 7c00  ...C...s(...t.|.
+00000320: 8301 7d03 7c03 6401 1900 7220 7401 7c03  ..}.|.d...r t.|.
 00000330: 6402 1900 6403 1700 8301 5300 7c02 5300  d...d.....S.|.S.
-00000340: 2904 4eda 0765 6e61 626c 6564 da05 7374  ).N..enabled..st
-00000350: 6172 74fa 012f 2902 da10 6765 745f 636f  art../)...get_co
-00000360: 6e74 6573 745f 6461 7461 7206 0000 0029  ntest_datar....)
-00000370: 0472 0b00 0000 da04 7461 736b da07 6465  .r......task..de
-00000380: 6661 756c 74da 0c63 6f6e 7465 7374 5f64  fault..contest_d
-00000390: 6174 6172 0900 0000 7209 0000 0072 0c00  atar....r....r..
-000003a0: 0000 da12 7461 736b 5f61 6363 6573 7369  ....task_accessi
-000003b0: 6269 6c69 7479 1a00 0000 7308 0000 0008  bility....s.....
-000003c0: 0108 0110 0104 0272 1500 0000 6300 0000  .......r....c...
-000003d0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000003e0: 0043 0000 0073 2800 0000 6401 7400 6a01  .C...s(...d.t.j.
-000003f0: 6a02 1700 6402 1700 7400 6a01 6a02 1700  j...d...t.j.j...
-00000400: 6403 1700 7400 6a01 6a02 1700 6404 1700  d...t.j.j...d...
-00000410: 5300 2905 7a19 2041 6464 6974 696f 6e61  S.).z. Additiona
-00000420: 6c20 4854 4d4c 2068 6561 6465 7273 207a  l HTML headers z
-00000430: 0c3c 6c69 6e6b 2068 7265 663d 227a 472f  .<link href="zG/
-00000440: 7374 6174 6963 2f70 6c75 6769 6e73 2f63  static/plugins/c
-00000450: 6f6e 7465 7374 732f 7363 6f72 6562 6f61  ontests/scoreboa
-00000460: 7264 2e63 7373 2220 7265 6c3d 2273 7479  rd.css" rel="sty
-00000470: 6c65 7368 6565 7422 3e3c 7363 7269 7074  lesheet"><script
-00000480: 2073 7263 3d22 7a48 2f73 7461 7469 632f   src="zH/static/
-00000490: 706c 7567 696e 732f 636f 6e74 6573 7473  plugins/contests
-000004a0: 2f6a 7175 6572 792e 636f 756e 7464 6f77  /jquery.countdow
-000004b0: 6e2e 6d69 6e2e 6a73 223e 3c2f 7363 7269  n.min.js"></scri
-000004c0: 7074 3e3c 7363 7269 7074 2073 7263 3d22  pt><script src="
-000004d0: 7a2f 2f73 7461 7469 632f 706c 7567 696e  z//static/plugin
-000004e0: 732f 636f 6e74 6573 7473 2f63 6f6e 7465  s/contests/conte
-000004f0: 7374 732e 6a73 223e 3c2f 7363 7269 7074  sts.js"></script
-00000500: 3e29 03da 0566 6c61 736b da07 7265 7175  >)...flask..requ
-00000510: 6573 74da 0875 726c 5f72 6f6f 7472 0900  est..url_rootr..
-00000520: 0000 7209 0000 0072 0900 0000 720c 0000  ..r....r....r...
-00000530: 00da 1261 6464 6974 696f 6e61 6c5f 6865  ...additional_he
-00000540: 6164 6572 7322 0000 0073 1600 0000 0a02  aders"...s......
-00000550: 0201 02ff 0602 02fe 0202 02fe 0603 02fd  ................
-00000560: 0203 04fd 7219 0000 0063 0100 0000 0000  ....r....c......
-00000570: 0000 0000 0000 0100 0000 0900 0000 4300  ..............C.
-00000580: 0000 733a 0000 007c 00a0 00a1 00a0 0164  ..s:...|.......d
-00000590: 0164 0274 02a0 03a1 00a0 0464 03a1 0174  .d.t.......d...t
-000005a0: 02a0 03a1 0074 0564 0464 058d 0117 00a0  .....t.d.d......
-000005b0: 0464 03a1 0164 0664 0764 089c 05a1 0253  .d...d.d.d.....S
-000005c0: 0029 097a 3520 5265 7475 726e 7320 7468  .).z5 Returns th
-000005d0: 6520 7365 7474 696e 6773 206f 6620 7468  e settings of th
-000005e0: 6520 636f 6e74 6573 7420 666f 7220 7468  e contest for th
-000005f0: 6973 2063 6f75 7273 6520 da10 636f 6e74  is course ..cont
-00000600: 6573 745f 7365 7474 696e 6773 46fa 1125  est_settingsF..%
-00000610: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
-00000620: e901 0000 00a9 01da 0568 6f75 7273 7201  .........hoursr.
-00000630: 0000 00e9 1400 0000 2905 720e 0000 0072  ........).r....r
-00000640: 0f00 0000 da03 656e 64da 0862 6c61 636b  ......end..black
-00000650: 6f75 74da 0770 656e 616c 7479 2906 da0e  out..penalty)...
-00000660: 6765 745f 6465 7363 7269 7074 6f72 da03  get_descriptor..
-00000670: 6765 7472 0300 0000 da03 6e6f 77da 0873  getr......now..s
-00000680: 7472 6674 696d 6572 0400 0000 720a 0000  trftimer....r...
-00000690: 0072 0900 0000 7209 0000 0072 0c00 0000  .r....r....r....
-000006a0: 7211 0000 002a 0000 0073 1000 0000 0c02  r....*...s......
-000006b0: 0c01 1201 0201 02ff 0202 0201 08fb 7211  ..............r.
-000006c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000006d0: 0600 0000 0800 0000 4300 0000 735c 0000  ........C...s\..
-000006e0: 0074 007c 0083 017d 027c 0264 0119 0072  .t.|...}.|.d...r
-000006f0: 2c74 01a0 027c 0264 0219 0064 03a1 027d  ,t...|.d...d...}
-00000700: 0374 01a0 027c 0264 0419 0064 03a1 027d  .t...|.d...d...}
-00000710: 047c 0474 037c 0264 0519 0064 068d 0118  .|.t.|.d...d....
-00000720: 007d 057c 016a 0464 0764 087c 007c 037c  .}.|.j.d.d.|.|.|
-00000730: 047c 0564 098d 0653 0064 0a53 0029 0b7a  .|.d...S.d.S.).z
-00000740: 4020 4469 7370 6c61 7973 2073 6f6d 6520  @ Displays some 
-00000750: 696e 666f 726d 6174 696f 6e73 2061 626f  informations abo
-00000760: 7574 2074 6865 2063 6f6e 7465 7374 206f  ut the contest o
-00000770: 6e20 7468 6520 636f 7572 7365 2070 6167  n the course pag
-00000780: 6572 0e00 0000 720f 0000 0072 1b00 0000  er....r....r....
-00000790: 7220 0000 0072 2100 0000 721d 0000 007a  r ...r!...r....z
-000007a0: 1063 6f75 7273 655f 6d65 6e75 2e68 746d  .course_menu.htm
-000007b0: 6cfa 1966 726f 6e74 656e 642f 706c 7567  l..frontend/plug
-000007c0: 696e 732f 636f 6e74 6573 7473 2905 da0f  ins/contests)...
-000007d0: 7465 6d70 6c61 7465 5f66 6f6c 6465 7272  template_folderr
-000007e0: 0b00 0000 720f 0000 0072 2000 0000 7221  ....r....r ...r!
-000007f0: 0000 004e 2905 7211 0000 0072 0300 0000  ...N).r....r....
-00000800: da08 7374 7270 7469 6d65 7204 0000 00da  ..strptimer.....
-00000810: 0672 656e 6465 7229 0672 0b00 0000 da0f  .render).r......
-00000820: 7465 6d70 6c61 7465 5f68 656c 7065 7272  template_helperr
-00000830: 1400 0000 720f 0000 0072 2000 0000 7221  ....r....r ...r!
-00000840: 0000 0072 0900 0000 7209 0000 0072 0c00  ...r....r....r..
-00000850: 0000 da0b 636f 7572 7365 5f6d 656e 7534  ....course_menu4
-00000860: 0000 0073 1200 0000 0802 0801 1001 1001  ...s............
-00000870: 1201 0801 0801 06ff 0403 722c 0000 0063  ..........r,...c
-00000880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000890: 0200 0000 4000 0000 7318 0000 0065 005a  ....@...s....e.Z
-000008a0: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
-000008b0: 0464 0453 0029 05da 1143 6f6e 7465 7374  .d.S.)...Contest
-000008c0: 5363 6f72 6562 6f61 7264 7a28 2044 6973  Scoreboardz( Dis
-000008d0: 706c 6179 7320 7468 6520 7363 6f72 6562  plays the scoreb
-000008e0: 6f61 7264 206f 6620 7468 6520 636f 6e74  oard of the cont
-000008f0: 6573 7420 6302 0000 0000 0000 0000 0000  est c...........
-00000900: 0016 0000 000b 0000 0003 0000 0073 8a03  .............s..
-00000910: 0000 8800 6a00 a001 7c01 a101 7d02 7402  ....j...|...}.t.
-00000920: 7c02 8301 7d03 7c03 6401 1900 7311 7403  |...}.|.d...s.t.
-00000930: 8300 8201 7404 a005 7c03 6402 1900 6403  ....t...|.d...d.
-00000940: a102 7d04 7404 a005 7c03 6404 1900 6403  ..}.t...|.d...d.
-00000950: a102 7d05 7c05 7406 7c03 6405 1900 6406  ..}.|.t.|.d...d.
-00000960: 8d01 1800 7d06 8800 6a07 a008 7c02 a101  ....}...j...|...
-00000970: 7d07 7409 7c02 a00a a100 a00b a100 8301  }.t.|...........
-00000980: 7d08 8800 6a0c 6a0d a00e 6407 7c07 6901  }...j.j...d.|.i.
-00000990: 7c01 7c04 7c06 6408 9c02 6409 640a 9c04  |.|.|.d...d.d...
-000009a0: 640b 640c 640b 640b 640b 640d 9c05 a102  d.d.d.d.d.d.....
-000009b0: a00f 640e 7410 6a11 6602 6701 a101 7d09  ..d.t.j.f.g...}.
-000009c0: 640f 6410 8400 7c08 4400 8301 8901 8700  d.d...|.D.......
-000009d0: 8701 6602 6411 6410 8408 7c07 4400 8301  ..f.d.d...|.D...
-000009e0: 7d0a 6700 7d0b 6412 6410 8400 7c08 4400  }.g.}.d.d...|.D.
-000009f0: 8301 7d0c 7c09 4400 5dba 7d0d 7c0d 6413  ..}.|.D.].}.|.d.
-00000a00: 1900 4400 5db3 7d0e 7c0d 6414 1900 7c08  ..D.].}.|.d...|.
-00000a10: 7601 7282 7179 7c0e 7c07 7601 7287 7179  v.r.qy|.|.v.r.qy
-00000a20: 7c0a 7c0e 1900 6415 1900 7c0d 6414 1900  |.|...d...|.d...
-00000a30: 1900 7d0f 7c0f 6416 1900 6417 6b02 739d  ..}.|.d...d.k.s.
-00000a40: 7c0f 6416 1900 6418 6b02 729e 7179 7c0d  |.d...d.k.r.qy|.
-00000a50: 6419 1900 641a 6b02 72e1 7c0c 7c0d 6414  d...d.k.r.|.|.d.
-00000a60: 1900 1900 73b5 6418 7c0f 6416 3c00 640b  ....s.d.|.d.<.d.
-00000a70: 7c0c 7c0d 6414 1900 3c00 6e04 6417 7c0f  |.|.d...<.n.d.|.
-00000a80: 6416 3c00 7c0f 641b 0500 1900 641c 3700  d.<.|.d.....d.7.
-00000a90: 0300 3c00 7c0d 640e 1900 7c0f 641d 3c00  ..<.|.d...|.d.<.
-00000aa0: 7c0d 640e 1900 7406 7c03 641e 1900 7c0f  |.d...t.|.d...|.
-00000ab0: 641b 1900 641c 1800 1400 641f 8d01 1700  d...d.....d.....
-00000ac0: 7c04 1800 a012 a100 6420 1b00 7c0f 6421  |.......d ..|.d!
-00000ad0: 3c00 6e2e 7c0d 6419 1900 6422 6b02 73ed  <.n.|.d...d"k.s.
-00000ae0: 7c0d 6419 1900 6423 6b02 72fa 6424 7c0f  |.d...d#k.r.d$|.
-00000af0: 6416 3c00 7c0f 641b 0500 1900 641c 3700  d.<.|.d.....d.7.
-00000b00: 0300 3c00 6e15 7c0d 6419 1900 6425 6b02  ..<.n.|.d...d%k.
-00000b10: 9001 720e 6426 7c0f 6416 3c00 7c0f 641b  ..r.d&|.d.<.|.d.
-00000b20: 0500 1900 641c 3700 0300 3c00 6e01 7179  ....d.7...<.n.qy
-00000b30: 7c0b a013 7c0a 7c0e 1900 6427 1900 7c0d  |...|.|...d'..|.
-00000b40: 640e 1900 7c0f 6416 1900 6417 6b02 9001  d...|.d...d.k...
-00000b50: 7025 7c0f 6416 1900 6418 6b02 7c0d 6414  p%|.d...d.k.|.d.
-00000b60: 1900 6428 9c04 a101 0100 7179 7173 7c0b  ..d(......qyqs|.
-00000b70: a014 a100 0100 7c0a 4400 5d34 7d10 6429  ......|.D.]4}.d)
-00000b80: 6429 6702 7d11 7409 7c0a 7c10 1900 6415  d)g.}.t.|.|...d.
-00000b90: 1900 a015 a100 8301 4400 5d1a 7d12 6421  ........D.].}.d!
-00000ba0: 7c12 7600 9001 725d 7c11 6429 0500 1900  |.v...r]|.d)....
-00000bb0: 641c 3700 0300 3c00 7c11 641c 0500 1900  d.7...<.|.d.....
-00000bc0: 7c12 6421 1900 3700 0300 3c00 9001 7144  |.d!..7...<...qD
-00000bd0: 7416 7c11 8301 7c0a 7c10 1900 6421 3c00  t.|...|.|...d!<.
-00000be0: 9001 7134 7417 7418 7409 7c0a a019 a100  ..q4t.t.t.|.....
-00000bf0: 8301 642a 642b 8400 642c 8d02 8301 7d0a  ..d*d+..d,....}.
-00000c00: 6400 7d13 6429 7d14 741a 7c0a a00b a100  d.}.d)}.t.|.....
-00000c10: 8301 4400 5d34 5c02 7d15 7d10 7c0a 7c10  ..D.]4\.}.}.|.|.
-00000c20: 1900 6421 1900 7c13 6b03 9001 72a8 7c0a  ..d!..|.k...r.|.
-00000c30: 7c10 1900 6421 1900 7d13 7c15 641c 1700  |...d!..}.|.d...
-00000c40: 7d14 7c14 7c0a 7c10 1900 642d 3c00 741b  }.|.|.|...d-<.t.
-00000c50: 7c14 8301 7c0a 7c10 1900 642e 3c00 9001  |...|.|...d.<...
-00000c60: 7181 7c14 7c0a 7c10 1900 642d 3c00 642f  q.|.|.|...d-<.d/
-00000c70: 7c0a 7c10 1900 642e 3c00 9001 7181 8800  |.|...d.<...q...
-00000c80: 6a1c 6a1d 6430 6431 7c02 7c04 7c05 7c06  j.j.d0d1|.|.|.|.
-00000c90: 7c08 7c0a 7c0b 6432 8d09 5300 2933 4e72  |.|.|.d2..S.)3Nr
-00000ca0: 0e00 0000 720f 0000 0072 1b00 0000 7220  ....r....r....r 
-00000cb0: 0000 0072 2100 0000 721d 0000 007a 0324  ...r!...r....z.$
-00000cc0: 696e 2902 7a04 2467 7465 7a03 246c 74da  in).z.$gtez.$lt.
-00000cd0: 0464 6f6e 6529 04da 0875 7365 726e 616d  .done)...usernam
-00000ce0: 65da 0863 6f75 7273 6569 64da 0c73 7562  e..courseid..sub
-00000cf0: 6d69 7474 6564 5f6f 6eda 0673 7461 7475  mitted_on..statu
-00000d00: 7354 4629 0572 2f00 0000 da03 5f69 64da  sTF).r/....._id.
-00000d10: 0674 6173 6b69 64da 0672 6573 756c 7472  .taskid..resultr
-00000d20: 3100 0000 7231 0000 0063 0100 0000 0000  1...r1...c......
-00000d30: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
-00000d40: 0000 7318 0000 0069 007c 005d 087d 017c  ..s....i.|.].}.|
-00000d50: 0164 0064 0164 029c 0293 0271 0253 0029  .d.d.d.....q.S.)
-00000d60: 03da 024e 4172 0100 0000 2902 7232 0000  ...NAr....).r2..
-00000d70: 00da 0574 7269 6573 7209 0000 00a9 02da  ...triesr.......
-00000d80: 022e 3072 3400 0000 7209 0000 0072 0900  ..0r4...r....r..
-00000d90: 0000 720c 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
-00000da0: 6d70 3e57 0000 0073 0200 0000 1800 7a2e  mp>W...s......z.
-00000db0: 436f 6e74 6573 7453 636f 7265 626f 6172  ContestScoreboar
-00000dc0: 642e 4745 545f 4155 5448 2e3c 6c6f 6361  d.GET_AUTH.<loca
-00000dd0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 6301  ls>.<dictcomp>c.
-00000de0: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-00000df0: 0000 0013 0000 0073 2600 0000 6900 7c00  .......s&...i.|.
-00000e00: 5d0f 7d01 7c01 8800 6a00 a001 7c01 a101  ].}.|...j...|...
-00000e10: 7402 a003 8801 a101 6400 9c02 9302 7102  t.......d.....q.
-00000e20: 5300 2901 2902 da04 6e61 6d65 da05 7461  S.).)...name..ta
-00000e30: 736b 7329 04da 0c75 7365 725f 6d61 6e61  sks)...user_mana
-00000e40: 6765 72da 1167 6574 5f75 7365 725f 7265  ger..get_user_re
-00000e50: 616c 6e61 6d65 da04 636f 7079 da08 6465  alname..copy..de
-00000e60: 6570 636f 7079 2902 7239 0000 0072 2f00  epcopy).r9...r/.
-00000e70: 0000 a902 da04 7365 6c66 5a0b 7461 736b  ......selfZ.task
-00000e80: 5f73 7461 7475 7372 0900 0000 720c 0000  _statusr....r...
-00000e90: 0072 3a00 0000 5800 0000 7302 0000 0026  .r:...X...s....&
-00000ea0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000eb0: 0000 0400 0000 5300 0000 7312 0000 0069  ......S...s....i
-00000ec0: 007c 005d 057d 017c 0164 0093 0271 0253  .|.].}.|.d...q.S
-00000ed0: 0029 0146 7209 0000 0072 3800 0000 7209  .).Fr....r8...r.
-00000ee0: 0000 0072 0900 0000 720c 0000 0072 3a00  ...r....r....r:.
-00000ef0: 0000 5c00 0000 7302 0000 0012 0072 2f00  ..\...s......r/.
-00000f00: 0000 7234 0000 0072 3c00 0000 7232 0000  ..r4...r<...r2..
-00000f10: 00da 0241 435a 0341 4346 7235 0000 00da  ...ACZ.ACFr5....
-00000f20: 0773 7563 6365 7373 7237 0000 0072 1c00  .successr7...r..
-00000f30: 0000 da04 7469 6d65 7222 0000 0029 01da  ....timer"...)..
-00000f40: 076d 696e 7574 6573 e93c 0000 00da 0573  .minutes.<.....s
-00000f50: 636f 7265 da06 6661 696c 6564 da06 6b69  core..failed..ki
-00000f60: 6c6c 6564 5a02 5741 da07 7469 6d65 6f75  lledZ.WA..timeou
-00000f70: 745a 0354 4c45 723b 0000 0029 04da 0475  tZ.TLEr;...)...u
-00000f80: 7365 72da 0477 6865 6e72 3500 0000 7234  ser..whenr5...r4
-00000f90: 0000 0072 0100 0000 6301 0000 0000 0000  ...r....c.......
-00000fa0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
-00000fb0: 0073 2200 0000 7c00 6401 1900 6402 1900  .s"...|.d...d...
-00000fc0: 6403 1900 0b00 7c00 6401 1900 6402 1900  d.....|.d...d...
-00000fd0: 6401 1900 6602 5300 2904 4e72 1c00 0000  d...f.S.).Nr....
-00000fe0: 7248 0000 0072 0100 0000 7209 0000 0029  rH...r....r....)
-00000ff0: 01da 0174 7209 0000 0072 0900 0000 720c  ...tr....r....r.
-00001000: 0000 00da 083c 6c61 6d62 6461 3e89 0000  .....<lambda>...
-00001010: 0073 0200 0000 2200 7a2c 436f 6e74 6573  .s....".z,Contes
-00001020: 7453 636f 7265 626f 6172 642e 4745 545f  tScoreboard.GET_
-00001030: 4155 5448 2e3c 6c6f 6361 6c73 3e2e 3c6c  AUTH.<locals>.<l
-00001040: 616d 6264 613e 2901 da03 6b65 79da 0472  ambda>)...key..r
-00001050: 616e 6b5a 0e64 6973 706c 6179 6564 5f72  ankZ.displayed_r
-00001060: 616e 6bda 007a 0f73 636f 7265 626f 6172  ank..z.scoreboar
-00001070: 642e 6874 6d6c 7227 0000 0029 0872 2800  d.htmlr'...).r(.
-00001080: 0000 720b 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
-00001090: 0072 2100 0000 723c 0000 00da 0772 6573  .r!...r<.....res
-000010a0: 756c 7473 da08 6163 7469 7669 7479 291e  ults..activity).
-000010b0: da0e 636f 7572 7365 5f66 6163 746f 7279  ..course_factory
-000010c0: da0a 6765 745f 636f 7572 7365 7211 0000  ..get_courser...
-000010d0: 0072 0500 0000 7203 0000 0072 2900 0000  .r....r....r)...
-000010e0: 7204 0000 0072 3d00 0000 da1b 6765 745f  r....r=.....get_
-000010f0: 636f 7572 7365 5f72 6567 6973 7465 7265  course_registere
-00001100: 645f 7573 6572 73da 046c 6973 74da 0967  d_users..list..g
-00001110: 6574 5f74 6173 6b73 da04 6b65 7973 da08  et_tasks..keys..
-00001120: 6461 7461 6261 7365 da0b 7375 626d 6973  database..submis
-00001130: 7369 6f6e 73da 0466 696e 64da 0473 6f72  sions..find..sor
-00001140: 74da 0770 796d 6f6e 676f da09 4153 4345  t..pymongo..ASCE
-00001150: 4e44 494e 47da 0d74 6f74 616c 5f73 6563  NDING..total_sec
-00001160: 6f6e 6473 da06 6170 7065 6e64 da07 7265  onds..append..re
-00001170: 7665 7273 65da 0676 616c 7565 73da 0574  verse..values..t
-00001180: 7570 6c65 7202 0000 00da 0673 6f72 7465  upler......sorte
-00001190: 64da 0569 7465 6d73 da09 656e 756d 6572  d..items..enumer
-000011a0: 6174 65da 0373 7472 722b 0000 0072 2a00  ate..strr+...r*.
-000011b0: 0000 2916 7242 0000 0072 3000 0000 720b  ..).rB...r0...r.
-000011c0: 0000 0072 1400 0000 720f 0000 0072 2000  ...r....r....r .
-000011d0: 0000 7221 0000 00da 0575 7365 7273 723c  ..r!.....usersr<
-000011e0: 0000 005a 0a64 625f 7265 7375 6c74 7372  ...Z.db_resultsr
-000011f0: 5300 0000 7254 0000 00da 0e74 6173 6b5f  S...rT.....task_
-00001200: 7375 6363 6565 6465 64da 0a73 7562 6d69  succeeded..submi
-00001210: 7373 696f 6e72 2f00 0000 7232 0000 0072  ssionr/...r2...r
-00001220: 4c00 0000 7248 0000 00da 0464 6174 61da  L...rH.....data.
-00001230: 036f 6c64 5a0c 6375 7272 656e 745f 7261  .oldZ.current_ra
-00001240: 6e6b da03 6369 6472 0900 0000 7241 0000  nk..cidr....rA..
-00001250: 0072 0c00 0000 da08 4745 545f 4155 5448  .r......GET_AUTH
-00001260: 4400 0000 73a6 0000 000c 0108 0108 0106  D...s...........
-00001270: 0110 0110 0112 010c 0210 0108 0206 0102  ................
-00001280: 0108 0102 0104 fc0e 0502 fb0e 0502 fb0e  ................
-00001290: 0714 0104 010e 0308 010c 010c 0102 0108  ................
-000012a0: 0102 0114 0118 0102 010c 020c 0108 010e  ................
-000012b0: 0108 0210 010c 0106 0118 0102 ff02 0202  ................
-000012c0: fe06 020a fe18 0308 0112 010e 0108 0112  ................
-000012d0: 0102 020e 0106 0118 0106 010a fd02 e408  ................
-000012e0: 2008 0208 0118 010a 0110 0114 0104 8014   ...............
-000012f0: 011c 0304 0304 0114 0112 010c 0108 010c  ................
-00001300: 0114 010c 0210 010a 020a 0104 0106 fe7a  ...............z
-00001310: 1a43 6f6e 7465 7374 5363 6f72 6562 6f61  .ContestScoreboa
-00001320: 7264 2e47 4554 5f41 5554 484e 2905 da08  rd.GET_AUTHN)...
-00001330: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00001340: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00001350: 5f5f da07 5f5f 646f 635f 5f72 7000 0000  __..__doc__rp...
-00001360: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00001370: 0c00 0000 722d 0000 0041 0000 0073 0600  ....r-...A...s..
-00001380: 0000 0800 0401 0c02 722d 0000 0063 0000  ........r-...c..
-00001390: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-000013a0: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
-000013b0: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-000013c0: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-000013d0: 0853 0029 09da 0c43 6f6e 7465 7374 4164  .S.)...ContestAd
-000013e0: 6d69 6e7a 1f20 436f 6e74 6573 7420 7365  minz. Contest se
-000013f0: 7474 696e 6773 2066 6f72 2061 2063 6f75  ttings for a cou
-00001400: 7273 6520 6303 0000 0000 0000 0000 0000  rse c...........
-00001410: 0004 0000 0004 0000 0043 0000 0073 2e00  .........C...s..
-00001420: 0000 7c00 6a00 a001 7c01 a002 a100 a101  ..|.j...|.......
-00001430: 7d03 7c02 7c03 6401 3c00 7c00 6a00 a003  }.|.|.d.<.|.j...
-00001440: 7c01 a002 a100 7c03 a102 0100 6402 5300  |.....|.....d.S.
-00001450: 2903 7a2b 2053 6176 6573 2075 7064 6174  ).z+ Saves updat
-00001460: 6564 2063 6f6e 7465 7374 2064 6174 6120  ed contest data 
-00001470: 666f 7220 7468 6520 636f 7572 7365 2072  for the course r
-00001480: 1a00 0000 4e29 0472 5500 0000 da1d 6765  ....N).rU.....ge
-00001490: 745f 636f 7572 7365 5f64 6573 6372 6970  t_course_descrip
-000014a0: 746f 725f 636f 6e74 656e 74da 0667 6574  tor_content..get
-000014b0: 5f69 64da 2075 7064 6174 655f 636f 7572  _id. update_cour
-000014c0: 7365 5f64 6573 6372 6970 746f 725f 636f  se_descriptor_co
-000014d0: 6e74 656e 7429 0472 4200 0000 720b 0000  ntent).rB...r...
-000014e0: 0072 1400 0000 da0e 636f 7572 7365 5f63  .r......course_c
-000014f0: 6f6e 7465 6e74 7209 0000 0072 0900 0000  ontentr....r....
-00001500: 720c 0000 00da 1173 6176 655f 636f 6e74  r......save_cont
-00001510: 6573 745f 6461 7461 a000 0000 7306 0000  est_data....s...
-00001520: 0010 0208 0116 017a 1e43 6f6e 7465 7374  .......z.Contest
-00001530: 4164 6d69 6e2e 7361 7665 5f63 6f6e 7465  Admin.save_conte
-00001540: 7374 5f64 6174 6163 0200 0000 0000 0000  st_datac........
-00001550: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
-00001560: 7332 0000 007c 006a 007c 0164 0164 028d  s2...|.j.|.d.d..
-00001570: 025c 027d 027d 0374 017c 0283 017d 047c  .\.}.}.t.|...}.|
-00001580: 006a 026a 0364 0364 047c 027c 0464 0564  .j.j.d.d.|.|.d.d
-00001590: 0164 068d 0653 0029 077a 2620 4745 5420  .d...S.).z& GET 
-000015a0: 7265 7175 6573 743a 2073 696d 706c 7920  request: simply 
-000015b0: 6469 7370 6c61 7920 7468 6520 666f 726d  display the form
-000015c0: 2046 a901 da0f 616c 6c6f 775f 616c 6c5f   F....allow_all_
-000015d0: 7374 6166 66fa 0a61 646d 696e 2e68 746d  staff..admin.htm
-000015e0: 6c72 2700 0000 4ea9 0572 2800 0000 720b  lr'...N..r(...r.
-000015f0: 0000 0072 6d00 0000 da06 6572 726f 7273  ...rm.....errors
-00001600: da05 7361 7665 6429 04da 1b67 6574 5f63  ..saved)...get_c
-00001610: 6f75 7273 655f 616e 645f 6368 6563 6b5f  ourse_and_check_
-00001620: 7269 6768 7473 7211 0000 0072 2b00 0000  rightsr....r+...
-00001630: 722a 0000 0029 0572 4200 0000 7230 0000  r*...).rB...r0..
-00001640: 0072 0b00 0000 da02 5f5f 7214 0000 0072  .r......__r....r
-00001650: 0900 0000 7209 0000 0072 0c00 0000 7270  ....r....r....rp
-00001660: 0000 00a6 0000 0073 0a00 0000 1202 0801  .......s........
-00001670: 0c01 0601 06ff 7a15 436f 6e74 6573 7441  ......z.ContestA
-00001680: 646d 696e 2e47 4554 5f41 5554 4863 0200  dmin.GET_AUTHc..
-00001690: 0000 0000 0000 0000 0000 0900 0000 0800  ................
-000016a0: 0000 4300 0000 739c 0100 007c 006a 007c  ..C...s....|.j.|
-000016b0: 0164 0164 028d 025c 027d 027d 0374 017c  .d.d...\.}.}.t.|
-000016c0: 0283 017d 0474 026a 036a 047d 0567 007d  ...}.t.j.j.}.g.}
-000016d0: 067a 8d7c 05a0 0564 0364 04a1 0264 056b  .z.|...d.d...d.k
-000016e0: 027c 0464 033c 007c 0564 0619 007c 0464  .|.d.<.|.d...|.d
-000016f0: 063c 007c 0564 0719 007c 0464 073c 007a  .<.|.d...|.d.<.z
-00001700: 0a74 06a0 077c 0464 0619 0064 08a1 027d  .t...|.d...d...}
-00001710: 0757 006e 0901 0001 0001 007c 06a0 0864  .W.n.......|...d
-00001720: 09a1 0101 0059 007a 0a74 06a0 077c 0464  .....Y.z.t...|.d
-00001730: 0719 0064 08a1 027d 0857 006e 0901 0001  ...d...}.W.n....
-00001740: 0001 007c 06a0 0864 0aa1 0101 0059 0074  ...|...d.....Y.t
-00001750: 097c 0683 0164 0b6b 0272 617c 077c 086b  .|...d.k.ra|.|.k
-00001760: 0572 617c 06a0 0864 0ca1 0101 007a 1574  .ra|...d.....z.t
-00001770: 0a7c 0564 0d19 0083 017c 0464 0d3c 007c  .|.d.....|.d.<.|
-00001780: 0464 0d19 0064 0b6b 0072 757c 06a0 0864  .d...d.k.ru|...d
-00001790: 0ea1 0101 0057 006e 0901 0001 0001 007c  .....W.n.......|
-000017a0: 06a0 0864 0fa1 0101 0059 007a 1574 0a7c  ...d.....Y.z.t.|
-000017b0: 0564 1019 0083 017c 0464 103c 007c 0464  .d.....|.d.<.|.d
-000017c0: 1019 0064 0b6b 0072 947c 06a0 0864 11a1  ...d.k.r.|...d..
-000017d0: 0101 0057 006e 0901 0001 0001 007c 06a0  ...W.n.......|..
-000017e0: 0864 12a1 0101 0059 0057 006e 0901 0001  .d.....Y.W.n....
-000017f0: 0001 007c 06a0 0864 13a1 0101 0059 0074  ...|...d.....Y.t
-00001800: 097c 0683 0164 0b6b 0272 c27c 00a0 0b7c  .|...d.k.r.|...|
-00001810: 027c 04a1 0201 007c 006a 0c6a 0d64 1464  .|.....|.j.j.d.d
-00001820: 157c 027c 0464 1664 1764 188d 0653 007c  .|.|.d.d.d...S.|
-00001830: 006a 0c6a 0d64 1464 157c 027c 047c 0664  .j.j.d.d.|.|.|.d
-00001840: 0164 188d 0653 0029 197a 2320 504f 5354  .d...S.).z# POST
-00001850: 2072 6571 7565 7374 3a20 7570 6461 7465   request: update
-00001860: 2074 6865 2073 6574 7469 6e67 7320 4672   the settings Fr
-00001870: 7b00 0000 720e 0000 00da 0130 da01 3172  {...r......0..1r
-00001880: 0f00 0000 7220 0000 0072 1b00 0000 7a12  ....r ...r....z.
-00001890: 496e 7661 6c69 6420 7374 6172 7420 6461  Invalid start da
-000018a0: 7465 7a10 496e 7661 6c69 6420 656e 6420  tez.Invalid end 
-000018b0: 6461 7465 7201 0000 007a 2453 7461 7274  dater....z$Start
-000018c0: 2064 6174 6520 7368 6f75 6c64 2062 6520   date should be 
-000018d0: 6265 666f 7265 2065 6e64 2064 6174 6572  before end dater
-000018e0: 2100 0000 7a42 496e 7661 6c69 6420 6e75  !...zBInvalid nu
-000018f0: 6d62 6572 206f 6620 686f 7572 7320 666f  mber of hours fo
-00001900: 7220 7468 6520 626c 6163 6b6f 7574 3a20  r the blackout: 
-00001910: 7368 6f75 6c64 2062 6520 6772 6561 7465  should be greate
-00001920: 7220 7468 616e 2030 7a28 496e 7661 6c69  r than 0z(Invali
-00001930: 6420 6e75 6d62 6572 206f 6620 686f 7572  d number of hour
-00001940: 7320 666f 7220 7468 6520 626c 6163 6b6f  s for the blacko
-00001950: 7574 7222 0000 007a 4349 6e76 616c 6964  utr"...zCInvalid
-00001960: 206e 756d 6265 7220 6f66 206d 696e 7574   number of minut
-00001970: 6573 2066 6f72 2074 6865 2070 656e 616c  es for the penal
-00001980: 7479 3a20 7368 6f75 6c64 2062 6520 6772  ty: should be gr
-00001990: 6561 7465 7220 7468 616e 2030 7a29 496e  eater than 0z)In
-000019a0: 7661 6c69 6420 6e75 6d62 6572 206f 6620  valid number of 
-000019b0: 6d69 6e75 7465 7320 666f 7220 7468 6520  minutes for the 
-000019c0: 7065 6e61 6c74 797a 1d55 7365 7220 7265  penaltyz.User re
-000019d0: 7475 726e 6564 2061 6e20 696e 7661 6c69  turned an invali
-000019e0: 6420 666f 726d 727d 0000 0072 2700 0000  d formr}...r'...
-000019f0: 4e54 727e 0000 0029 0e72 8100 0000 7211  NTr~...).r....r.
-00001a00: 0000 0072 1600 0000 7217 0000 00da 0466  ...r....r......f
-00001a10: 6f72 6d72 2400 0000 7203 0000 0072 2900  ormr$...r....r).
-00001a20: 0000 7262 0000 00da 036c 656e da03 696e  ..rb.....len..in
-00001a30: 7472 7a00 0000 722b 0000 0072 2a00 0000  trz...r+...r*...
-00001a40: 2909 7242 0000 0072 3000 0000 720b 0000  ).rB...r0...r...
-00001a50: 0072 8200 0000 7214 0000 00da 086e 6577  .r....r......new
-00001a60: 5f64 6174 6172 7f00 0000 720f 0000 0072  _datar....r....r
-00001a70: 2000 0000 7209 0000 0072 0900 0000 720c   ...r....r....r.
-00001a80: 0000 00da 0950 4f53 545f 4155 5448 ad00  .....POST_AUTH..
-00001a90: 0000 7358 0000 0012 0208 0108 0204 0102  ..sX............
-00001aa0: 0114 010c 010c 0102 0214 0106 010c 0102  ................
-00001ab0: 0214 0106 010c 010c 0208 010a 0102 0210  ................
-00001ac0: 010c 010a 0104 8006 010c 0102 0210 010c  ................
-00001ad0: 010a 0104 8006 010c 0104 8006 010c 010c  ................
-00001ae0: 020c 010c 0106 0106 ff0c 0306 0106 ff7a  ...............z
-00001af0: 1643 6f6e 7465 7374 4164 6d69 6e2e 504f  .ContestAdmin.PO
-00001b00: 5354 5f41 5554 484e 2907 7271 0000 0072  ST_AUTHN).rq...r
-00001b10: 7200 0000 7273 0000 0072 7400 0000 727a  r...rs...rt...rz
-00001b20: 0000 0072 7000 0000 7289 0000 0072 0900  ...rp...r....r..
-00001b30: 0000 7209 0000 0072 0900 0000 720c 0000  ..r....r....r...
-00001b40: 0072 7500 0000 9d00 0000 730a 0000 0008  .ru.......s.....
-00001b50: 0004 0108 0208 060c 0772 7500 0000 6304  .........ru...c.
-00001b60: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00001b70: 0000 0043 0000 0073 5800 0000 7c00 a000  ...C...sX...|...
-00001b80: 6401 7401 a002 6402 a101 a102 0100 7c00  d.t...d.......|.
-00001b90: a000 6403 7403 a002 6404 a101 a102 0100  ..d.t...d.......
-00001ba0: 7c00 a004 6405 7405 a102 0100 7c00 a004  |...d.t.....|...
-00001bb0: 6406 7406 a102 0100 7c00 a004 6407 7407  d.t.....|...d.t.
-00001bc0: a102 0100 7c00 a004 6408 7408 a102 0100  ....|...d.t.....
-00001bd0: 6409 5300 290a 7ab6 0a20 2020 2020 2020  d.S.).z..       
-00001be0: 2049 6e69 7420 7468 6520 636f 6e74 6573   Init the contes
-00001bf0: 7420 706c 7567 696e 2e0a 2020 2020 2020  t plugin..      
-00001c00: 2020 4176 6169 6c61 626c 6520 636f 6e66    Available conf
-00001c10: 6967 7572 6174 696f 6e3a 0a20 2020 2020  iguration:.     
-00001c20: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
-00001c30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001c40: 2020 2020 2022 706c 7567 696e 5f6d 6f64       "plugin_mod
-00001c50: 756c 6522 3a20 2269 6e67 696e 696f 7573  ule": "inginious
-00001c60: 2e66 726f 6e74 656e 642e 706c 7567 696e  .frontend.plugin
-00001c70: 732e 636f 6e74 6573 7473 220a 2020 2020  s.contests".    
-00001c80: 2020 2020 2020 2020 7d0a 2020 2020 7a13          }.    z.
-00001c90: 2f63 6f6e 7465 7374 2f3c 636f 7572 7365  /contest/<course
-00001ca0: 6964 3e5a 1163 6f6e 7465 7374 7363 6f72  id>Z.contestscor
-00001cb0: 6562 6f61 7264 7a19 2f61 646d 696e 2f3c  eboardz./admin/<
-00001cc0: 636f 7572 7365 6964 3e2f 636f 6e74 6573  courseid>/contes
-00001cd0: 745a 0c63 6f6e 7465 7374 6164 6d69 6eda  tZ.contestadmin.
-00001ce0: 1163 6f75 7273 655f 6164 6d69 6e5f 6d65  .course_admin_me
-00001cf0: 6e75 7215 0000 00da 0b68 6561 6465 725f  nur......header_
-00001d00: 6874 6d6c 722c 0000 004e 2909 da08 6164  htmlr,...N)...ad
-00001d10: 645f 7061 6765 722d 0000 00da 0761 735f  d_pager-.....as_
-00001d20: 7669 6577 7275 0000 00da 0861 6464 5f68  viewru.....add_h
-00001d30: 6f6f 6b72 0d00 0000 7215 0000 0072 1900  ookr....r....r..
-00001d40: 0000 722c 0000 0029 04da 0e70 6c75 6769  ..r,...)...plugi
-00001d50: 6e5f 6d61 6e61 6765 7272 5500 0000 da06  n_managerrU.....
-00001d60: 636c 6965 6e74 da06 636f 6e66 6967 7209  client..configr.
-00001d70: 0000 0072 0900 0000 720c 0000 00da 0469  ...r....r......i
-00001d80: 6e69 74e0 0000 0073 0c00 0000 120b 1201  nit....s........
-00001d90: 0c01 0c01 0c01 1001 7292 0000 0029 1872  ........r....).r
-00001da0: 7400 0000 723f 0000 00da 0b63 6f6c 6c65  t...r?.....colle
-00001db0: 6374 696f 6e73 7202 0000 0072 0300 0000  ctionsr....r....
-00001dc0: 7204 0000 0072 5f00 0000 7216 0000 005a  r....r_...r....Z
-00001dd0: 1377 6572 6b7a 6575 672e 6578 6365 7074  .werkzeug.except
-00001de0: 696f 6e73 7205 0000 00da 2269 6e67 696e  ionsr....."ingin
-00001df0: 696f 7573 2e66 726f 6e74 656e 642e 6163  ious.frontend.ac
-00001e00: 6365 7373 6962 6c65 5f74 696d 6572 0600  cessible_timer..
-00001e10: 0000 da2b 696e 6769 6e69 6f75 732e 6672  ...+inginious.fr
-00001e20: 6f6e 7465 6e64 2e70 6167 6573 2e63 6f75  ontend.pages.cou
-00001e30: 7273 655f 6164 6d69 6e2e 7574 696c 7372  rse_admin.utilsr
-00001e40: 0700 0000 da1e 696e 6769 6e69 6f75 732e  ......inginious.
-00001e50: 6672 6f6e 7465 6e64 2e70 6167 6573 2e75  frontend.pages.u
-00001e60: 7469 6c73 7208 0000 0072 0d00 0000 7215  tilsr....r....r.
-00001e70: 0000 0072 1900 0000 7211 0000 0072 2c00  ...r....r....r,.
-00001e80: 0000 722d 0000 0072 7500 0000 7292 0000  ..r-...ru...r...
-00001e90: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00001ea0: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001eb0: 0000 0073 2400 0000 0405 0802 0c01 1001  ...s$...........
-00001ec0: 0802 0801 0c02 0c01 0c01 0c01 0803 0805  ................
-00001ed0: 0808 0808 080a 100d 105c 0c43            .........\.C
+00000340: 6400 5300 2904 4eda 0765 6e61 626c 6564  d.S.).N..enabled
+00000350: da05 7374 6172 74fa 012f 2902 da10 6765  ..start../)...ge
+00000360: 745f 636f 6e74 6573 745f 6461 7461 7206  t_contest_datar.
+00000370: 0000 0029 0472 0b00 0000 da04 7461 736b  ...).r......task
+00000380: da07 6465 6661 756c 74da 0c63 6f6e 7465  ..default..conte
+00000390: 7374 5f64 6174 6172 0900 0000 7209 0000  st_datar....r...
+000003a0: 0072 0c00 0000 da12 7461 736b 5f61 6363  .r......task_acc
+000003b0: 6573 7369 6269 6c69 7479 1a00 0000 7308  essibility....s.
+000003c0: 0000 0000 0108 0108 0110 0272 1500 0000  ...........r....
+000003d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000003e0: 0002 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
+000003f0: 7400 6a01 6a02 1700 6402 1700 7400 6a01  t.j.j...d...t.j.
+00000400: 6a02 1700 6403 1700 7400 6a01 6a02 1700  j...d...t.j.j...
+00000410: 6404 1700 5300 2905 7a19 2041 6464 6974  d...S.).z. Addit
+00000420: 696f 6e61 6c20 4854 4d4c 2068 6561 6465  ional HTML heade
+00000430: 7273 207a 0c3c 6c69 6e6b 2068 7265 663d  rs z.<link href=
+00000440: 227a 472f 7374 6174 6963 2f70 6c75 6769  "zG/static/plugi
+00000450: 6e73 2f63 6f6e 7465 7374 732f 7363 6f72  ns/contests/scor
+00000460: 6562 6f61 7264 2e63 7373 2220 7265 6c3d  eboard.css" rel=
+00000470: 2273 7479 6c65 7368 6565 7422 3e3c 7363  "stylesheet"><sc
+00000480: 7269 7074 2073 7263 3d22 7a48 2f73 7461  ript src="zH/sta
+00000490: 7469 632f 706c 7567 696e 732f 636f 6e74  tic/plugins/cont
+000004a0: 6573 7473 2f6a 7175 6572 792e 636f 756e  ests/jquery.coun
+000004b0: 7464 6f77 6e2e 6d69 6e2e 6a73 223e 3c2f  tdown.min.js"></
+000004c0: 7363 7269 7074 3e3c 7363 7269 7074 2073  script><script s
+000004d0: 7263 3d22 7a2f 2f73 7461 7469 632f 706c  rc="z//static/pl
+000004e0: 7567 696e 732f 636f 6e74 6573 7473 2f63  ugins/contests/c
+000004f0: 6f6e 7465 7374 732e 6a73 223e 3c2f 7363  ontests.js"></sc
+00000500: 7269 7074 3e29 03da 0566 6c61 736b da07  ript>)...flask..
+00000510: 7265 7175 6573 74da 0875 726c 5f72 6f6f  request..url_roo
+00000520: 7472 0900 0000 7209 0000 0072 0900 0000  tr....r....r....
+00000530: 720c 0000 00da 1261 6464 6974 696f 6e61  r......additiona
+00000540: 6c5f 6865 6164 6572 7322 0000 0073 1600  l_headers"...s..
+00000550: 0000 0002 0a01 02ff 0202 06fe 0202 02fe  ................
+00000560: 0203 06fd 0203 02fd 7219 0000 0063 0100  ........r....c..
+00000570: 0000 0000 0000 0000 0000 0100 0000 0900  ................
+00000580: 0000 4300 0000 733a 0000 007c 00a0 00a1  ..C...s:...|....
+00000590: 00a0 0164 0164 0274 02a0 03a1 00a0 0464  ...d.d.t.......d
+000005a0: 03a1 0174 02a0 03a1 0074 0564 0464 058d  ...t.....t.d.d..
+000005b0: 0117 00a0 0464 03a1 0164 0664 0764 089c  .....d...d.d.d..
+000005c0: 05a1 0253 0029 097a 3520 5265 7475 726e  ...S.).z5 Return
+000005d0: 7320 7468 6520 7365 7474 696e 6773 206f  s the settings o
+000005e0: 6620 7468 6520 636f 6e74 6573 7420 666f  f the contest fo
+000005f0: 7220 7468 6973 2063 6f75 7273 6520 da10  r this course ..
+00000600: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+00000610: 46fa 1125 592d 256d 2d25 6420 2548 3a25  F..%Y-%m-%d %H:%
+00000620: 4d3a 2553 e901 0000 00a9 01da 0568 6f75  M:%S.........hou
+00000630: 7273 7201 0000 00e9 1400 0000 2905 720e  rsr.........).r.
+00000640: 0000 0072 0f00 0000 da03 656e 64da 0862  ...r......end..b
+00000650: 6c61 636b 6f75 74da 0770 656e 616c 7479  lackout..penalty
+00000660: 2906 da0e 6765 745f 6465 7363 7269 7074  )...get_descript
+00000670: 6f72 da03 6765 7472 0300 0000 da03 6e6f  or..getr......no
+00000680: 77da 0873 7472 6674 696d 6572 0400 0000  w..strftimer....
+00000690: 720a 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+000006a0: 0c00 0000 7211 0000 002a 0000 0073 1000  ....r....*...s..
+000006b0: 0000 0002 0c01 0c01 1201 02ff 0202 0201  ................
+000006c0: 02fb 7211 0000 0063 0200 0000 0000 0000  ..r....c........
+000006d0: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
+000006e0: 7360 0000 0074 007c 0083 017d 027c 0264  s`...t.|...}.|.d
+000006f0: 0119 0072 5874 01a0 027c 0264 0219 0064  ...rXt...|.d...d
+00000700: 03a1 027d 0374 01a0 027c 0264 0419 0064  ...}.t...|.d...d
+00000710: 03a1 027d 047c 0474 037c 0264 0519 0064  ...}.|.t.|.d...d
+00000720: 068d 0118 007d 057c 016a 0464 0764 087c  .....}.|.j.d.d.|
+00000730: 007c 037c 047c 0564 098d 0653 0064 0a53  .|.|.|.d...S.d.S
+00000740: 0064 0a53 0029 0b7a 4020 4469 7370 6c61  .d.S.).z@ Displa
+00000750: 7973 2073 6f6d 6520 696e 666f 726d 6174  ys some informat
+00000760: 696f 6e73 2061 626f 7574 2074 6865 2063  ions about the c
+00000770: 6f6e 7465 7374 206f 6e20 7468 6520 636f  ontest on the co
+00000780: 7572 7365 2070 6167 6572 0e00 0000 720f  urse pager....r.
+00000790: 0000 0072 1b00 0000 7220 0000 0072 2100  ...r....r ...r!.
+000007a0: 0000 721d 0000 007a 1063 6f75 7273 655f  ..r....z.course_
+000007b0: 6d65 6e75 2e68 746d 6cfa 1966 726f 6e74  menu.html..front
+000007c0: 656e 642f 706c 7567 696e 732f 636f 6e74  end/plugins/cont
+000007d0: 6573 7473 2905 da0f 7465 6d70 6c61 7465  ests)...template
+000007e0: 5f66 6f6c 6465 7272 0b00 0000 720f 0000  _folderr....r...
+000007f0: 0072 2000 0000 7221 0000 004e 2905 7211  .r ...r!...N).r.
+00000800: 0000 0072 0300 0000 da08 7374 7270 7469  ...r......strpti
+00000810: 6d65 7204 0000 00da 0672 656e 6465 7229  mer......render)
+00000820: 0672 0b00 0000 da0f 7465 6d70 6c61 7465  .r......template
+00000830: 5f68 656c 7065 7272 1400 0000 720f 0000  _helperr....r...
+00000840: 0072 2000 0000 7221 0000 0072 0900 0000  .r ...r!...r....
+00000850: 7209 0000 0072 0c00 0000 da0b 636f 7572  r....r......cour
+00000860: 7365 5f6d 656e 7534 0000 0073 1200 0000  se_menu4...s....
+00000870: 0002 0801 0801 1001 1001 1201 0801 08ff  ................
+00000880: 0603 722c 0000 0063 0000 0000 0000 0000  ..r,...c........
+00000890: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000008a0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+000008b0: 0364 0264 0384 005a 0464 0453 0029 05da  .d.d...Z.d.S.)..
+000008c0: 1143 6f6e 7465 7374 5363 6f72 6562 6f61  .ContestScoreboa
+000008d0: 7264 7a28 2044 6973 706c 6179 7320 7468  rdz( Displays th
+000008e0: 6520 7363 6f72 6562 6f61 7264 206f 6620  e scoreboard of 
+000008f0: 7468 6520 636f 6e74 6573 7420 6302 0000  the contest c...
+00000900: 0000 0000 0000 0000 0016 0000 000b 0000  ................
+00000910: 0003 0000 0073 9a03 0000 8800 6a00 a001  .....s......j...
+00000920: 7c01 a101 7d02 7402 7c02 8301 7d03 7c03  |...}.t.|...}.|.
+00000930: 6401 1900 7322 7403 8300 8201 7404 a005  d...s"t.....t...
+00000940: 7c03 6402 1900 6403 a102 7d04 7404 a005  |.d...d...}.t...
+00000950: 7c03 6404 1900 6403 a102 7d05 7c05 7406  |.d...d...}.|.t.
+00000960: 7c03 6405 1900 6406 8d01 1800 7d06 8800  |.d...d.....}...
+00000970: 6a07 a008 7c02 a101 7d07 7409 7c02 a00a  j...|...}.t.|...
+00000980: a100 a00b a100 8301 7d08 8800 6a0c 6a0d  ........}...j.j.
+00000990: a00e 6407 7c07 6901 7c01 7c04 7c06 6408  ..d.|.i.|.|.|.d.
+000009a0: 9c02 6409 640a 9c04 640b 640c 640b 640b  ..d.d...d.d.d.d.
+000009b0: 640b 640d 9c05 a102 a00f 640e 7410 6a11  d.d.......d.t.j.
+000009c0: 6602 6701 a101 7d09 640f 6410 8400 7c08  f.g...}.d.d...|.
+000009d0: 4400 8301 8901 8700 8701 6602 6411 6410  D.........f.d.d.
+000009e0: 8408 7c07 4400 8301 7d0a 6700 7d0b 6412  ..|.D...}.g.}.d.
+000009f0: 6410 8400 7c08 4400 8301 7d0c 7c09 4400  d...|.D...}.|.D.
+00000a00: 9001 5d84 7d0d 7c0d 6413 1900 4400 9001  ..].}.|.d...D...
+00000a10: 5d74 7d0e 7c0d 6414 1900 7c08 7601 9001  ]t}.|.d...|.v...
+00000a20: 720a 71f4 7c0e 7c07 7601 9001 7216 71f4  r.q.|.|.v...r.q.
+00000a30: 7c0a 7c0e 1900 6415 1900 7c0d 6414 1900  |.|...d...|.d...
+00000a40: 1900 7d0f 7c0f 6416 1900 6417 6b02 73f4  ..}.|.d...d.k.s.
+00000a50: 7c0f 6416 1900 6418 6b02 9001 7248 71f4  |.d...d.k...rHq.
+00000a60: 71f4 7c0d 6419 1900 641a 6b02 9001 72d2  q.|.d...d.k...r.
+00000a70: 7c0c 7c0d 6414 1900 1900 9001 737a 6418  |.|.d.......szd.
+00000a80: 7c0f 6416 3c00 640b 7c0c 7c0d 6414 1900  |.d.<.d.|.|.d...
+00000a90: 3c00 6e08 6417 7c0f 6416 3c00 7c0f 641b  <.n.d.|.d.<.|.d.
+00000aa0: 0500 1900 641c 3700 0300 3c00 7c0d 640e  ....d.7...<.|.d.
+00000ab0: 1900 7c0f 641d 3c00 7c0d 640e 1900 7406  ..|.d.<.|.d...t.
+00000ac0: 7c03 641e 1900 7c0f 641b 1900 641c 1800  |.d...|.d...d...
+00000ad0: 1400 641f 8d01 1700 7c04 1800 a012 a100  ..d.....|.......
+00000ae0: 6420 1b00 7c0f 6421 3c00 6e5e 7c0d 6419  d ..|.d!<.n^|.d.
+00000af0: 1900 6422 6b02 9001 73ee 7c0d 6419 1900  ..d"k...s.|.d...
+00000b00: 6423 6b02 9002 7208 6424 7c0f 6416 3c00  d#k...r.d$|.d.<.
+00000b10: 7c0f 641b 0500 1900 641c 3700 0300 3c00  |.d.....d.7...<.
+00000b20: 6e28 7c0d 6419 1900 6425 6b02 72f4 6426  n(|.d...d%k.r.d&
+00000b30: 7c0f 6416 3c00 7c0f 641b 0500 1900 641c  |.d.<.|.d.....d.
+00000b40: 3700 0300 3c00 6e02 71f4 7c0b a013 7c0a  7...<.n.q.|...|.
+00000b50: 7c0e 1900 6427 1900 7c0d 640e 1900 7c0f  |...d'..|.d...|.
+00000b60: 6416 1900 6417 6b02 9002 705c 7c0f 6416  d...d.k...p\|.d.
+00000b70: 1900 6418 6b02 7c0d 6414 1900 6428 9c04  ..d.k.|.d...d(..
+00000b80: a101 0100 71f4 71e6 7c0b a014 a100 0100  ....q.q.|.......
+00000b90: 7c0a 4400 5d68 7d10 6429 6429 6702 7d11  |.D.]h}.d)d)g.}.
+00000ba0: 7409 7c0a 7c10 1900 6415 1900 a015 a100  t.|.|...d.......
+00000bb0: 8301 4400 5d34 7d12 6421 7c12 7600 9002  ..D.]4}.d!|.v...
+00000bc0: 729a 7c11 6429 0500 1900 641c 3700 0300  r.|.d)....d.7...
+00000bd0: 3c00 7c11 641c 0500 1900 7c12 6421 1900  <.|.d.....|.d!..
+00000be0: 3700 0300 3c00 9002 719a 7416 7c11 8301  7...<...q.t.|...
+00000bf0: 7c0a 7c10 1900 6421 3c00 9002 717a 7417  |.|...d!<...qzt.
+00000c00: 7418 7409 7c0a a019 a100 8301 642a 642b  t.t.|.......d*d+
+00000c10: 8400 642c 8d02 8301 7d0a 6400 7d13 6429  ..d,....}.d.}.d)
+00000c20: 7d14 741a 7c0a a00b a100 8301 4400 5d66  }.t.|.......D.]f
+00000c30: 5c02 7d15 7d10 7c0a 7c10 1900 6421 1900  \.}.}.|.|...d!..
+00000c40: 7c13 6b03 9003 7260 7c0a 7c10 1900 6421  |.k...r`|.|...d!
+00000c50: 1900 7d13 7c15 641c 1700 7d14 7c14 7c0a  ..}.|.d...}.|.|.
+00000c60: 7c10 1900 642d 3c00 741b 7c14 8301 7c0a  |...d-<.t.|...|.
+00000c70: 7c10 1900 642e 3c00 6e18 7c14 7c0a 7c10  |...d.<.n.|.|.|.
+00000c80: 1900 642d 3c00 642f 7c0a 7c10 1900 642e  ..d-<.d/|.|...d.
+00000c90: 3c00 9003 7114 8800 6a1c 6a1d 6430 6431  <...q...j.j.d0d1
+00000ca0: 7c02 7c04 7c05 7c06 7c08 7c0a 7c0b 6432  |.|.|.|.|.|.|.d2
+00000cb0: 8d09 5300 2933 4e72 0e00 0000 720f 0000  ..S.)3Nr....r...
+00000cc0: 0072 1b00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00000cd0: 721d 0000 007a 0324 696e 2902 7a04 2467  r....z.$in).z.$g
+00000ce0: 7465 7a03 246c 74da 0464 6f6e 6529 04da  tez.$lt..done)..
+00000cf0: 0875 7365 726e 616d 65da 0863 6f75 7273  .username..cours
+00000d00: 6569 64da 0c73 7562 6d69 7474 6564 5f6f  eid..submitted_o
+00000d10: 6eda 0673 7461 7475 7354 4629 0572 2f00  n..statusTF).r/.
+00000d20: 0000 da03 5f69 64da 0674 6173 6b69 64da  ...._id..taskid.
+00000d30: 0672 6573 756c 7472 3100 0000 7231 0000  .resultr1...r1..
+00000d40: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000d50: 0000 0600 0000 5300 0000 7318 0000 0069  ......S...s....i
+00000d60: 007c 005d 107d 017c 0164 0064 0164 029c  .|.].}.|.d.d.d..
+00000d70: 0293 0271 0453 0029 03da 024e 4172 0100  ...q.S.)...NAr..
+00000d80: 0000 2902 7232 0000 00da 0574 7269 6573  ..).r2.....tries
+00000d90: 7209 0000 00a9 02da 022e 3072 3400 0000  r.........0r4...
+00000da0: 7209 0000 0072 0900 0000 720c 0000 00da  r....r....r.....
+00000db0: 0a3c 6469 6374 636f 6d70 3e57 0000 00f3  .<dictcomp>W....
+00000dc0: 0000 0000 7a2e 436f 6e74 6573 7453 636f  ....z.ContestSco
+00000dd0: 7265 626f 6172 642e 4745 545f 4155 5448  reboard.GET_AUTH
+00000de0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000df0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00000e00: 0002 0000 0007 0000 0013 0000 0073 2600  .............s&.
+00000e10: 0000 6900 7c00 5d1e 7d01 7c01 8800 6a00  ..i.|.].}.|...j.
+00000e20: a001 7c01 a101 7402 a003 8801 a101 6400  ..|...t.......d.
+00000e30: 9c02 9302 7104 5300 2901 2902 da04 6e61  ....q.S.).)...na
+00000e40: 6d65 da05 7461 736b 7329 04da 0c75 7365  me..tasks)...use
+00000e50: 725f 6d61 6e61 6765 72da 1167 6574 5f75  r_manager..get_u
+00000e60: 7365 725f 7265 616c 6e61 6d65 da04 636f  ser_realname..co
+00000e70: 7079 da08 6465 6570 636f 7079 2902 7239  py..deepcopy).r9
+00000e80: 0000 0072 2f00 0000 a902 da04 7365 6c66  ...r/.......self
+00000e90: 5a0b 7461 736b 5f73 7461 7475 7372 0900  Z.task_statusr..
+00000ea0: 0000 720c 0000 0072 3a00 0000 5800 0000  ..r....r:...X...
+00000eb0: 723b 0000 0063 0100 0000 0000 0000 0000  r;...c..........
+00000ec0: 0000 0200 0000 0400 0000 5300 0000 7312  ..........S...s.
+00000ed0: 0000 0069 007c 005d 0a7d 017c 0164 0093  ...i.|.].}.|.d..
+00000ee0: 0271 0453 0029 0146 7209 0000 0072 3800  .q.S.).Fr....r8.
+00000ef0: 0000 7209 0000 0072 0900 0000 720c 0000  ..r....r....r...
+00000f00: 0072 3a00 0000 5c00 0000 723b 0000 0072  .r:...\...r;...r
+00000f10: 2f00 0000 7234 0000 0072 3d00 0000 7232  /...r4...r=...r2
+00000f20: 0000 00da 0241 435a 0341 4346 7235 0000  .....ACZ.ACFr5..
+00000f30: 00da 0773 7563 6365 7373 7237 0000 0072  ...successr7...r
+00000f40: 1c00 0000 da04 7469 6d65 7222 0000 0029  ......timer"...)
+00000f50: 01da 076d 696e 7574 6573 e93c 0000 00da  ...minutes.<....
+00000f60: 0573 636f 7265 da06 6661 696c 6564 da06  .score..failed..
+00000f70: 6b69 6c6c 6564 5a02 5741 da07 7469 6d65  killedZ.WA..time
+00000f80: 6f75 745a 0354 4c45 723c 0000 0029 04da  outZ.TLEr<...)..
+00000f90: 0475 7365 72da 0477 6865 6e72 3500 0000  .user..whenr5...
+00000fa0: 7234 0000 0072 0100 0000 6301 0000 0000  r4...r....c.....
+00000fb0: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
+00000fc0: 0000 0073 2200 0000 7c00 6401 1900 6402  ...s"...|.d...d.
+00000fd0: 1900 6403 1900 0b00 7c00 6401 1900 6402  ..d.....|.d...d.
+00000fe0: 1900 6401 1900 6602 5300 2904 4e72 1c00  ..d...f.S.).Nr..
+00000ff0: 0000 7249 0000 0072 0100 0000 7209 0000  ..rI...r....r...
+00001000: 0029 01da 0174 7209 0000 0072 0900 0000  .)...tr....r....
+00001010: 720c 0000 00da 083c 6c61 6d62 6461 3e89  r......<lambda>.
+00001020: 0000 0072 3b00 0000 7a2c 436f 6e74 6573  ...r;...z,Contes
+00001030: 7453 636f 7265 626f 6172 642e 4745 545f  tScoreboard.GET_
+00001040: 4155 5448 2e3c 6c6f 6361 6c73 3e2e 3c6c  AUTH.<locals>.<l
+00001050: 616d 6264 613e 2901 da03 6b65 79da 0472  ambda>)...key..r
+00001060: 616e 6b5a 0e64 6973 706c 6179 6564 5f72  ankZ.displayed_r
+00001070: 616e 6bda 007a 0f73 636f 7265 626f 6172  ank..z.scoreboar
+00001080: 642e 6874 6d6c 7227 0000 0029 0872 2800  d.htmlr'...).r(.
+00001090: 0000 720b 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
+000010a0: 0072 2100 0000 723d 0000 00da 0772 6573  .r!...r=.....res
+000010b0: 756c 7473 da08 6163 7469 7669 7479 291e  ults..activity).
+000010c0: da0e 636f 7572 7365 5f66 6163 746f 7279  ..course_factory
+000010d0: da0a 6765 745f 636f 7572 7365 7211 0000  ..get_courser...
+000010e0: 0072 0500 0000 7203 0000 0072 2900 0000  .r....r....r)...
+000010f0: 7204 0000 0072 3e00 0000 da1b 6765 745f  r....r>.....get_
+00001100: 636f 7572 7365 5f72 6567 6973 7465 7265  course_registere
+00001110: 645f 7573 6572 73da 046c 6973 74da 0967  d_users..list..g
+00001120: 6574 5f74 6173 6b73 da04 6b65 7973 da08  et_tasks..keys..
+00001130: 6461 7461 6261 7365 da0b 7375 626d 6973  database..submis
+00001140: 7369 6f6e 73da 0466 696e 64da 0473 6f72  sions..find..sor
+00001150: 74da 0770 796d 6f6e 676f da09 4153 4345  t..pymongo..ASCE
+00001160: 4e44 494e 47da 0d74 6f74 616c 5f73 6563  NDING..total_sec
+00001170: 6f6e 6473 da06 6170 7065 6e64 da07 7265  onds..append..re
+00001180: 7665 7273 65da 0676 616c 7565 73da 0574  verse..values..t
+00001190: 7570 6c65 7202 0000 00da 0673 6f72 7465  upler......sorte
+000011a0: 64da 0569 7465 6d73 da09 656e 756d 6572  d..items..enumer
+000011b0: 6174 65da 0373 7472 722b 0000 0072 2a00  ate..strr+...r*.
+000011c0: 0000 2916 7243 0000 0072 3000 0000 720b  ..).rC...r0...r.
+000011d0: 0000 0072 1400 0000 720f 0000 0072 2000  ...r....r....r .
+000011e0: 0000 7221 0000 00da 0575 7365 7273 723d  ..r!.....usersr=
+000011f0: 0000 005a 0a64 625f 7265 7375 6c74 7372  ...Z.db_resultsr
+00001200: 5400 0000 7255 0000 00da 0e74 6173 6b5f  T...rU.....task_
+00001210: 7375 6363 6565 6465 64da 0a73 7562 6d69  succeeded..submi
+00001220: 7373 696f 6e72 2f00 0000 7232 0000 0072  ssionr/...r2...r
+00001230: 4d00 0000 7249 0000 00da 0464 6174 61da  M...rI.....data.
+00001240: 036f 6c64 5a0c 6375 7272 656e 745f 7261  .oldZ.current_ra
+00001250: 6e6b da03 6369 6472 0900 0000 7242 0000  nk..cidr....rB..
+00001260: 0072 0c00 0000 da08 4745 545f 4155 5448  .r......GET_AUTH
+00001270: 4400 0000 73a2 0000 0000 010c 0108 0108  D...s...........
+00001280: 0106 0110 0110 0112 020c 0110 0208 0106  ................
+00001290: 0102 0108 0102 fc04 050e fb04 050a fb04  ................
+000012a0: 070e 0114 0104 030e 010a 010e 010e 0102  ................
+000012b0: 010a 0102 0114 011a 0104 020e 010e 0108  ................
+000012c0: 010e 0208 0110 010c 0106 0118 ff02 0202  ................
+000012d0: fe06 0202 fe0a 031c 0108 0112 010c 0108  ................
+000012e0: 0112 0202 010e 0106 0118 0106 fd0c 0408  ................
+000012f0: 0208 0108 0118 010a 0110 0118 0114 031c  ................
+00001300: 0304 0104 0114 0112 010c 0108 010c 0112  ................
+00001310: 020c 0110 020a 010a 0104 fe7a 1a43 6f6e  ...........z.Con
+00001320: 7465 7374 5363 6f72 6562 6f61 7264 2e47  testScoreboard.G
+00001330: 4554 5f41 5554 484e 2905 da08 5f5f 6e61  ET_AUTHN)...__na
+00001340: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00001350: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00001360: 5f5f 646f 635f 5f72 7100 0000 7209 0000  __doc__rq...r...
+00001370: 0072 0900 0000 7209 0000 0072 0c00 0000  .r....r....r....
+00001380: 722d 0000 0041 0000 0073 0400 0000 0801  r-...A...s......
+00001390: 0402 722d 0000 0063 0000 0000 0000 0000  ..r-...c........
+000013a0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000013b0: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
+000013c0: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
+000013d0: 0564 0664 0784 005a 0664 0853 0029 09da  .d.d...Z.d.S.)..
+000013e0: 0c43 6f6e 7465 7374 4164 6d69 6e7a 1f20  .ContestAdminz. 
+000013f0: 436f 6e74 6573 7420 7365 7474 696e 6773  Contest settings
+00001400: 2066 6f72 2061 2063 6f75 7273 6520 6303   for a course c.
+00001410: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001420: 0000 0043 0000 0073 2e00 0000 7c00 6a00  ...C...s....|.j.
+00001430: a001 7c01 a002 a100 a101 7d03 7c02 7c03  ..|.......}.|.|.
+00001440: 6401 3c00 7c00 6a00 a003 7c01 a002 a100  d.<.|.j...|.....
+00001450: 7c03 a102 0100 6402 5300 2903 7a2b 2053  |.....d.S.).z+ S
+00001460: 6176 6573 2075 7064 6174 6564 2063 6f6e  aves updated con
+00001470: 7465 7374 2064 6174 6120 666f 7220 7468  test data for th
+00001480: 6520 636f 7572 7365 2072 1a00 0000 4e29  e course r....N)
+00001490: 0472 5600 0000 da1d 6765 745f 636f 7572  .rV.....get_cour
+000014a0: 7365 5f64 6573 6372 6970 746f 725f 636f  se_descriptor_co
+000014b0: 6e74 656e 74da 0667 6574 5f69 64da 2075  ntent..get_id. u
+000014c0: 7064 6174 655f 636f 7572 7365 5f64 6573  pdate_course_des
+000014d0: 6372 6970 746f 725f 636f 6e74 656e 7429  criptor_content)
+000014e0: 0472 4300 0000 720b 0000 0072 1400 0000  .rC...r....r....
+000014f0: da0e 636f 7572 7365 5f63 6f6e 7465 6e74  ..course_content
+00001500: 7209 0000 0072 0900 0000 720c 0000 00da  r....r....r.....
+00001510: 1173 6176 655f 636f 6e74 6573 745f 6461  .save_contest_da
+00001520: 7461 a000 0000 7306 0000 0000 0210 0108  ta....s.........
+00001530: 017a 1e43 6f6e 7465 7374 4164 6d69 6e2e  .z.ContestAdmin.
+00001540: 7361 7665 5f63 6f6e 7465 7374 5f64 6174  save_contest_dat
+00001550: 6163 0200 0000 0000 0000 0000 0000 0500  ac..............
+00001560: 0000 0800 0000 4300 0000 7332 0000 007c  ......C...s2...|
+00001570: 006a 007c 0164 0164 028d 025c 027d 027d  .j.|.d.d...\.}.}
+00001580: 0374 017c 0283 017d 047c 006a 026a 0364  .t.|...}.|.j.j.d
+00001590: 0364 047c 027c 0464 0564 0164 068d 0653  .d.|.|.d.d.d...S
+000015a0: 0029 077a 2620 4745 5420 7265 7175 6573  .).z& GET reques
+000015b0: 743a 2073 696d 706c 7920 6469 7370 6c61  t: simply displa
+000015c0: 7920 7468 6520 666f 726d 2046 a901 da0f  y the form F....
+000015d0: 616c 6c6f 775f 616c 6c5f 7374 6166 66fa  allow_all_staff.
+000015e0: 0a61 646d 696e 2e68 746d 6c72 2700 0000  .admin.htmlr'...
+000015f0: 4ea9 0572 2800 0000 720b 0000 0072 6e00  N..r(...r....rn.
+00001600: 0000 da06 6572 726f 7273 da05 7361 7665  ....errors..save
+00001610: 6429 04da 1b67 6574 5f63 6f75 7273 655f  d)...get_course_
+00001620: 616e 645f 6368 6563 6b5f 7269 6768 7473  and_check_rights
+00001630: 7211 0000 0072 2b00 0000 722a 0000 0029  r....r+...r*...)
+00001640: 0572 4300 0000 7230 0000 0072 0b00 0000  .rC...r0...r....
+00001650: da02 5f5f 7214 0000 0072 0900 0000 7209  ..__r....r....r.
+00001660: 0000 0072 0c00 0000 7271 0000 00a6 0000  ...r....rq......
+00001670: 0073 0a00 0000 0002 1201 0801 0c01 06ff  .s..............
+00001680: 7a15 436f 6e74 6573 7441 646d 696e 2e47  z.ContestAdmin.G
+00001690: 4554 5f41 5554 4863 0200 0000 0000 0000  ET_AUTHc........
+000016a0: 0000 0000 0900 0000 0800 0000 4300 0000  ............C...
+000016b0: 73ba 0100 007c 006a 007c 0164 0164 028d  s....|.j.|.d.d..
+000016c0: 025c 027d 027d 0374 017c 0283 017d 0474  .\.}.}.t.|...}.t
+000016d0: 026a 036a 047d 0567 007d 0690 017a 2c7c  .j.j.}.g.}...z,|
+000016e0: 05a0 0564 0364 04a1 0264 056b 027c 0464  ...d.d...d.k.|.d
+000016f0: 033c 007c 0564 0619 007c 0464 063c 007c  .<.|.d...|.d.<.|
+00001700: 0564 0719 007c 0464 073c 007a 1474 06a0  .d...|.d.<.z.t..
+00001710: 077c 0464 0619 0064 08a1 027d 0757 006e  .|.d...d...}.W.n
+00001720: 1601 0001 0001 007c 06a0 0864 09a1 0101  .......|...d....
+00001730: 0059 006e 0230 007a 1474 06a0 077c 0464  .Y.n.0.z.t...|.d
+00001740: 0719 0064 08a1 027d 0857 006e 1601 0001  ...d...}.W.n....
+00001750: 0001 007c 06a0 0864 0aa1 0101 0059 006e  ...|...d.....Y.n
+00001760: 0230 0074 097c 0683 0164 0b6b 0272 cc7c  .0.t.|...d.k.r.|
+00001770: 077c 086b 0572 cc7c 06a0 0864 0ca1 0101  .|.k.r.|...d....
+00001780: 007a 2a74 0a7c 0564 0d19 0083 017c 0464  .z*t.|.d.....|.d
+00001790: 0d3c 007c 0464 0d19 0064 0b6b 0072 f47c  .<.|.d...d.k.r.|
+000017a0: 06a0 0864 0ea1 0101 0057 006e 1601 0001  ...d.....W.n....
+000017b0: 0001 007c 06a0 0864 0fa1 0101 0059 006e  ...|...d.....Y.n
+000017c0: 0230 007a 2c74 0a7c 0564 1019 0083 017c  .0.z,t.|.d.....|
+000017d0: 0464 103c 007c 0464 1019 0064 0b6b 0090  .d.<.|.d...d.k..
+000017e0: 0172 387c 06a0 0864 11a1 0101 0057 006e  .r8|...d.....W.n
+000017f0: 1601 0001 0001 007c 06a0 0864 12a1 0101  .......|...d....
+00001800: 0059 006e 0230 0057 006e 1601 0001 0001  .Y.n.0.W.n......
+00001810: 007c 06a0 0864 13a1 0101 0059 006e 0230  .|...d.....Y.n.0
+00001820: 0074 097c 0683 0164 0b6b 0290 0172 9e7c  .t.|...d.k...r.|
+00001830: 00a0 0b7c 027c 04a1 0201 007c 006a 0c6a  ...|.|.....|.j.j
+00001840: 0d64 1464 157c 027c 0464 1664 1764 188d  .d.d.|.|.d.d.d..
+00001850: 0653 007c 006a 0c6a 0d64 1464 157c 027c  .S.|.j.j.d.d.|.|
+00001860: 047c 0664 0164 188d 0653 0064 1653 0029  .|.d.d...S.d.S.)
+00001870: 197a 2320 504f 5354 2072 6571 7565 7374  .z# POST request
+00001880: 3a20 7570 6461 7465 2074 6865 2073 6574  : update the set
+00001890: 7469 6e67 7320 4672 7c00 0000 720e 0000  tings Fr|...r...
+000018a0: 00da 0130 da01 3172 0f00 0000 7220 0000  ...0..1r....r ..
+000018b0: 0072 1b00 0000 7a12 496e 7661 6c69 6420  .r....z.Invalid 
+000018c0: 7374 6172 7420 6461 7465 7a10 496e 7661  start datez.Inva
+000018d0: 6c69 6420 656e 6420 6461 7465 7201 0000  lid end dater...
+000018e0: 007a 2453 7461 7274 2064 6174 6520 7368  .z$Start date sh
+000018f0: 6f75 6c64 2062 6520 6265 666f 7265 2065  ould be before e
+00001900: 6e64 2064 6174 6572 2100 0000 7a42 496e  nd dater!...zBIn
+00001910: 7661 6c69 6420 6e75 6d62 6572 206f 6620  valid number of 
+00001920: 686f 7572 7320 666f 7220 7468 6520 626c  hours for the bl
+00001930: 6163 6b6f 7574 3a20 7368 6f75 6c64 2062  ackout: should b
+00001940: 6520 6772 6561 7465 7220 7468 616e 2030  e greater than 0
+00001950: 7a28 496e 7661 6c69 6420 6e75 6d62 6572  z(Invalid number
+00001960: 206f 6620 686f 7572 7320 666f 7220 7468   of hours for th
+00001970: 6520 626c 6163 6b6f 7574 7222 0000 007a  e blackoutr"...z
+00001980: 4349 6e76 616c 6964 206e 756d 6265 7220  CInvalid number 
+00001990: 6f66 206d 696e 7574 6573 2066 6f72 2074  of minutes for t
+000019a0: 6865 2070 656e 616c 7479 3a20 7368 6f75  he penalty: shou
+000019b0: 6c64 2062 6520 6772 6561 7465 7220 7468  ld be greater th
+000019c0: 616e 2030 7a29 496e 7661 6c69 6420 6e75  an 0z)Invalid nu
+000019d0: 6d62 6572 206f 6620 6d69 6e75 7465 7320  mber of minutes 
+000019e0: 666f 7220 7468 6520 7065 6e61 6c74 797a  for the penaltyz
+000019f0: 1d55 7365 7220 7265 7475 726e 6564 2061  .User returned a
+00001a00: 6e20 696e 7661 6c69 6420 666f 726d 727e  n invalid formr~
+00001a10: 0000 0072 2700 0000 4e54 727f 0000 0029  ...r'...NTr....)
+00001a20: 0e72 8200 0000 7211 0000 0072 1600 0000  .r....r....r....
+00001a30: 7217 0000 00da 0466 6f72 6d72 2400 0000  r......formr$...
+00001a40: 7203 0000 0072 2900 0000 7263 0000 00da  r....r)...rc....
+00001a50: 036c 656e da03 696e 7472 7b00 0000 722b  .len..intr{...r+
+00001a60: 0000 0072 2a00 0000 2909 7243 0000 0072  ...r*...).rC...r
+00001a70: 3000 0000 720b 0000 0072 8300 0000 7214  0...r....r....r.
+00001a80: 0000 00da 086e 6577 5f64 6174 6172 8000  .....new_datar..
+00001a90: 0000 720f 0000 0072 2000 0000 7209 0000  ..r....r ...r...
+00001aa0: 0072 0900 0000 720c 0000 00da 0950 4f53  .r....r......POS
+00001ab0: 545f 4155 5448 ad00 0000 7352 0000 0000  T_AUTH....sR....
+00001ac0: 0212 0108 0208 0104 0104 0114 010c 010c  ................
+00001ad0: 0202 0114 0106 0110 0202 0114 0106 0110  ................
+00001ae0: 020c 0108 010a 0202 0110 010c 010e 0106  ................
+00001af0: 0110 0202 0110 010e 010e 0106 0114 0106  ................
+00001b00: 0110 020e 010c 010c 0106 ff06 030c 0106  ................
+00001b10: ff7a 1643 6f6e 7465 7374 4164 6d69 6e2e  .z.ContestAdmin.
+00001b20: 504f 5354 5f41 5554 484e 2907 7272 0000  POST_AUTHN).rr..
+00001b30: 0072 7300 0000 7274 0000 0072 7500 0000  .rs...rt...ru...
+00001b40: 727b 0000 0072 7100 0000 728a 0000 0072  r{...rq...r....r
+00001b50: 0900 0000 7209 0000 0072 0900 0000 720c  ....r....r....r.
+00001b60: 0000 0072 7600 0000 9d00 0000 7308 0000  ...rv.......s...
+00001b70: 0008 0104 0208 0608 0772 7600 0000 6304  .........rv...c.
+00001b80: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00001b90: 0000 0043 0000 0073 5800 0000 7c00 a000  ...C...sX...|...
+00001ba0: 6401 7401 a002 6402 a101 a102 0100 7c00  d.t...d.......|.
+00001bb0: a000 6403 7403 a002 6404 a101 a102 0100  ..d.t...d.......
+00001bc0: 7c00 a004 6405 7405 a102 0100 7c00 a004  |...d.t.....|...
+00001bd0: 6406 7406 a102 0100 7c00 a004 6407 7407  d.t.....|...d.t.
+00001be0: a102 0100 7c00 a004 6408 7408 a102 0100  ....|...d.t.....
+00001bf0: 6409 5300 290a 7ab6 0a20 2020 2020 2020  d.S.).z..       
+00001c00: 2049 6e69 7420 7468 6520 636f 6e74 6573   Init the contes
+00001c10: 7420 706c 7567 696e 2e0a 2020 2020 2020  t plugin..      
+00001c20: 2020 4176 6169 6c61 626c 6520 636f 6e66    Available conf
+00001c30: 6967 7572 6174 696f 6e3a 0a20 2020 2020  iguration:.     
+00001c40: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
+00001c50: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00001c60: 2020 2020 2022 706c 7567 696e 5f6d 6f64       "plugin_mod
+00001c70: 756c 6522 3a20 2269 6e67 696e 696f 7573  ule": "inginious
+00001c80: 2e66 726f 6e74 656e 642e 706c 7567 696e  .frontend.plugin
+00001c90: 732e 636f 6e74 6573 7473 220a 2020 2020  s.contests".    
+00001ca0: 2020 2020 2020 2020 7d0a 2020 2020 7a13          }.    z.
+00001cb0: 2f63 6f6e 7465 7374 2f3c 636f 7572 7365  /contest/<course
+00001cc0: 6964 3e5a 1163 6f6e 7465 7374 7363 6f72  id>Z.contestscor
+00001cd0: 6562 6f61 7264 7a19 2f61 646d 696e 2f3c  eboardz./admin/<
+00001ce0: 636f 7572 7365 6964 3e2f 636f 6e74 6573  courseid>/contes
+00001cf0: 745a 0c63 6f6e 7465 7374 6164 6d69 6eda  tZ.contestadmin.
+00001d00: 1163 6f75 7273 655f 6164 6d69 6e5f 6d65  .course_admin_me
+00001d10: 6e75 7215 0000 00da 0b68 6561 6465 725f  nur......header_
+00001d20: 6874 6d6c 722c 0000 004e 2909 da08 6164  htmlr,...N)...ad
+00001d30: 645f 7061 6765 722d 0000 00da 0761 735f  d_pager-.....as_
+00001d40: 7669 6577 7276 0000 00da 0861 6464 5f68  viewrv.....add_h
+00001d50: 6f6f 6b72 0d00 0000 7215 0000 0072 1900  ookr....r....r..
+00001d60: 0000 722c 0000 0029 04da 0e70 6c75 6769  ..r,...)...plugi
+00001d70: 6e5f 6d61 6e61 6765 7272 5600 0000 da06  n_managerrV.....
+00001d80: 636c 6965 6e74 da06 636f 6e66 6967 7209  client..configr.
+00001d90: 0000 0072 0900 0000 720c 0000 00da 0469  ...r....r......i
+00001da0: 6e69 74e0 0000 0073 0c00 0000 000b 1201  nit....s........
+00001db0: 1201 0c01 0c01 0c01 7293 0000 0029 1872  ........r....).r
+00001dc0: 7500 0000 7240 0000 00da 0b63 6f6c 6c65  u...r@.....colle
+00001dd0: 6374 696f 6e73 7202 0000 0072 0300 0000  ctionsr....r....
+00001de0: 7204 0000 0072 6000 0000 7216 0000 005a  r....r`...r....Z
+00001df0: 1377 6572 6b7a 6575 672e 6578 6365 7074  .werkzeug.except
+00001e00: 696f 6e73 7205 0000 005a 2269 6e67 696e  ionsr....Z"ingin
+00001e10: 696f 7573 2e66 726f 6e74 656e 642e 6163  ious.frontend.ac
+00001e20: 6365 7373 6962 6c65 5f74 696d 6572 0600  cessible_timer..
+00001e30: 0000 da2b 696e 6769 6e69 6f75 732e 6672  ...+inginious.fr
+00001e40: 6f6e 7465 6e64 2e70 6167 6573 2e63 6f75  ontend.pages.cou
+00001e50: 7273 655f 6164 6d69 6e2e 7574 696c 7372  rse_admin.utilsr
+00001e60: 0700 0000 da1e 696e 6769 6e69 6f75 732e  ......inginious.
+00001e70: 6672 6f6e 7465 6e64 2e70 6167 6573 2e75  frontend.pages.u
+00001e80: 7469 6c73 7208 0000 0072 0d00 0000 7215  tilsr....r....r.
+00001e90: 0000 0072 1900 0000 7211 0000 0072 2c00  ...r....r....r,.
+00001ea0: 0000 722d 0000 0072 7600 0000 7293 0000  ..r-...rv...r...
+00001eb0: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00001ec0: 720c 0000 00da 083c 6d6f 6475 6c65 3e06  r......<module>.
+00001ed0: 0000 0073 2200 0000 0402 0801 0c01 1002  ...s"...........
+00001ee0: 0801 0802 0c01 0c01 0c01 0c03 0805 0808  ................
+00001ef0: 0808 080a 080d 105c 1043                 .......\.C
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 27 09:46:07 2021 UTC, .py size: 11265 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,496 +1,603 @@
-00000000: 610d 0d0a 0000 0000 5fdd 8760 012c 0000  a......._..`.,..
+00000000: 6f0d 0d0a 0000 0000 8247 4a64 bd31 0000  o........GJd.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6405 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000080: 6407 6c0c 6d0d 5a0d 0100 6401 6408 6c0e  d.l.m.Z...d.d.l.
-00000090: 6d0f 5a0f 0100 6409 640a 8400 5a10 640b  m.Z...d.d...Z.d.
-000000a0: 640c 8400 5a11 640d 640e 8400 5a12 640f  d...Z.d.d...Z.d.
-000000b0: 6410 8400 5a13 6411 6412 8400 5a14 4700  d...Z.d.d...Z.G.
-000000c0: 6413 6414 8400 6414 650f 8303 5a15 4700  d.d...d.e...Z.G.
-000000d0: 6415 6416 8400 6416 650d 8303 5a16 6417  d.d...d.e...Z.d.
-000000e0: 6418 8400 5a17 6402 5300 2919 7a66 2041  d...Z.d.S.).zf A
-000000f0: 6e20 616c 676f 7269 7468 6d20 636f 6e74  n algorithm cont
-00000100: 6573 7420 706c 7567 696e 2066 6f72 2049  est plugin for I
-00000110: 4e47 496e 696f 7573 2e20 4261 7365 6420  NGInious. Based 
-00000120: 6f6e 2074 6865 2073 616d 6520 7072 696e  on the same prin
-00000130: 6369 706c 6573 2074 6861 6e20 636f 6e74  ciples than cont
-00000140: 6573 7473 206c 696b 6520 4143 4d2d 4943  ests like ACM-IC
-00000150: 5043 2e20 e900 0000 004e 2901 da0b 4f72  PC. .....N)...Or
-00000160: 6465 7265 6444 6963 7429 02da 0864 6174  deredDict)...dat
-00000170: 6574 696d 65da 0974 696d 6564 656c 7461  etime..timedelta
-00000180: 2901 da08 4e6f 7446 6f75 6e64 2901 da0e  )...NotFound)...
-00000190: 4163 6365 7373 6962 6c65 5469 6d65 2901  AccessibleTime).
-000001a0: da12 494e 4749 6e69 6f75 7341 646d 696e  ..INGIniousAdmin
-000001b0: 5061 6765 2901 da11 494e 4749 6e69 6f75  Page)...INGIniou
-000001c0: 7341 7574 6850 6167 6563 0100 0000 0000  sAuthPagec......
-000001d0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-000001e0: 0000 7304 0000 0064 0153 0029 027a 3b20  ..s....d.S.).z; 
-000001f0: 4164 6420 6120 6d65 6e75 2066 6f72 2074  Add a menu for t
-00000200: 6865 2063 6f6e 7465 7374 2073 6574 7469  he contest setti
-00000210: 6e67 7320 696e 2074 6865 2061 646d 696e  ngs in the admin
-00000220: 6973 7472 6174 696f 6e20 2902 5a07 636f  istration ).Z.co
-00000230: 6e74 6573 747a 303c 6920 636c 6173 733d  ntestz0<i class=
-00000240: 2266 6120 6661 2d74 726f 7068 7920 6661  "fa fa-trophy fa
-00000250: 2d66 7722 3e3c 2f69 3e26 6e62 7370 3b20  -fw"></i>&nbsp; 
-00000260: 436f 6e74 6573 74a9 00a9 01da 0663 6f75  Contest......cou
-00000270: 7273 6572 0900 0000 7209 0000 00fa 5f2f  rser....r....._/
-00000280: 686f 6d65 2f61 6e74 686f 6e79 2f44 6f63  home/anthony/Doc
-00000290: 756d 656e 7473 2f69 6e67 696e 696f 7573  uments/inginious
-000002a0: 2d64 6576 2f49 4e47 496e 696f 7573 2f69  -dev/INGInious/i
-000002b0: 6e67 696e 696f 7573 2f66 726f 6e74 656e  nginious/fronten
-000002c0: 642f 706c 7567 696e 732f 636f 6e74 6573  d/plugins/contes
-000002d0: 7473 2f5f 5f69 6e69 745f 5f2e 7079 da0e  ts/__init__.py..
-000002e0: 6164 645f 6164 6d69 6e5f 6d65 6e75 1500  add_admin_menu..
-000002f0: 0000 7302 0000 0000 0272 0d00 0000 6303  ..s......r....c.
-00000300: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00000310: 0000 0043 0000 0073 2800 0000 7400 7c00  ...C...s(...t.|.
-00000320: 8301 7d03 7c03 6401 1900 7220 7401 7c03  ..}.|.d...r t.|.
-00000330: 6402 1900 6403 1700 8301 5300 7c02 5300  d...d.....S.|.S.
-00000340: 6400 5300 2904 4eda 0765 6e61 626c 6564  d.S.).N..enabled
-00000350: da05 7374 6172 74fa 012f 2902 da10 6765  ..start../)...ge
-00000360: 745f 636f 6e74 6573 745f 6461 7461 7206  t_contest_datar.
-00000370: 0000 0029 0472 0b00 0000 da04 7461 736b  ...).r......task
-00000380: da07 6465 6661 756c 74da 0c63 6f6e 7465  ..default..conte
-00000390: 7374 5f64 6174 6172 0900 0000 7209 0000  st_datar....r...
-000003a0: 0072 0c00 0000 da12 7461 736b 5f61 6363  .r......task_acc
-000003b0: 6573 7369 6269 6c69 7479 1a00 0000 7308  essibility....s.
-000003c0: 0000 0000 0108 0108 0110 0272 1500 0000  ...........r....
-000003d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000003e0: 0002 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
-000003f0: 7400 6a01 6a02 1700 6402 1700 7400 6a01  t.j.j...d...t.j.
-00000400: 6a02 1700 6403 1700 7400 6a01 6a02 1700  j...d...t.j.j...
-00000410: 6404 1700 5300 2905 7a19 2041 6464 6974  d...S.).z. Addit
-00000420: 696f 6e61 6c20 4854 4d4c 2068 6561 6465  ional HTML heade
-00000430: 7273 207a 0c3c 6c69 6e6b 2068 7265 663d  rs z.<link href=
-00000440: 227a 472f 7374 6174 6963 2f70 6c75 6769  "zG/static/plugi
-00000450: 6e73 2f63 6f6e 7465 7374 732f 7363 6f72  ns/contests/scor
-00000460: 6562 6f61 7264 2e63 7373 2220 7265 6c3d  eboard.css" rel=
-00000470: 2273 7479 6c65 7368 6565 7422 3e3c 7363  "stylesheet"><sc
-00000480: 7269 7074 2073 7263 3d22 7a48 2f73 7461  ript src="zH/sta
-00000490: 7469 632f 706c 7567 696e 732f 636f 6e74  tic/plugins/cont
-000004a0: 6573 7473 2f6a 7175 6572 792e 636f 756e  ests/jquery.coun
-000004b0: 7464 6f77 6e2e 6d69 6e2e 6a73 223e 3c2f  tdown.min.js"></
-000004c0: 7363 7269 7074 3e3c 7363 7269 7074 2073  script><script s
-000004d0: 7263 3d22 7a2f 2f73 7461 7469 632f 706c  rc="z//static/pl
-000004e0: 7567 696e 732f 636f 6e74 6573 7473 2f63  ugins/contests/c
-000004f0: 6f6e 7465 7374 732e 6a73 223e 3c2f 7363  ontests.js"></sc
-00000500: 7269 7074 3e29 03da 0566 6c61 736b da07  ript>)...flask..
-00000510: 7265 7175 6573 74da 0875 726c 5f72 6f6f  request..url_roo
-00000520: 7472 0900 0000 7209 0000 0072 0900 0000  tr....r....r....
-00000530: 720c 0000 00da 1261 6464 6974 696f 6e61  r......additiona
-00000540: 6c5f 6865 6164 6572 7322 0000 0073 1600  l_headers"...s..
-00000550: 0000 0002 0a01 02ff 0202 06fe 0202 02fe  ................
-00000560: 0203 06fd 0203 02fd 7219 0000 0063 0100  ........r....c..
-00000570: 0000 0000 0000 0000 0000 0100 0000 0900  ................
-00000580: 0000 4300 0000 733a 0000 007c 00a0 00a1  ..C...s:...|....
-00000590: 00a0 0164 0164 0274 02a0 03a1 00a0 0464  ...d.d.t.......d
-000005a0: 03a1 0174 02a0 03a1 0074 0564 0464 058d  ...t.....t.d.d..
-000005b0: 0117 00a0 0464 03a1 0164 0664 0764 089c  .....d...d.d.d..
-000005c0: 05a1 0253 0029 097a 3520 5265 7475 726e  ...S.).z5 Return
-000005d0: 7320 7468 6520 7365 7474 696e 6773 206f  s the settings o
-000005e0: 6620 7468 6520 636f 6e74 6573 7420 666f  f the contest fo
-000005f0: 7220 7468 6973 2063 6f75 7273 6520 da10  r this course ..
-00000600: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00000610: 46fa 1125 592d 256d 2d25 6420 2548 3a25  F..%Y-%m-%d %H:%
-00000620: 4d3a 2553 e901 0000 00a9 01da 0568 6f75  M:%S.........hou
-00000630: 7273 7201 0000 00e9 1400 0000 2905 720e  rsr.........).r.
-00000640: 0000 0072 0f00 0000 da03 656e 64da 0862  ...r......end..b
-00000650: 6c61 636b 6f75 74da 0770 656e 616c 7479  lackout..penalty
-00000660: 2906 da0e 6765 745f 6465 7363 7269 7074  )...get_descript
-00000670: 6f72 da03 6765 7472 0300 0000 da03 6e6f  or..getr......no
-00000680: 77da 0873 7472 6674 696d 6572 0400 0000  w..strftimer....
-00000690: 720a 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-000006a0: 0c00 0000 7211 0000 002a 0000 0073 1000  ....r....*...s..
-000006b0: 0000 0002 0c01 0c01 1201 02ff 0202 0201  ................
-000006c0: 02fb 7211 0000 0063 0200 0000 0000 0000  ..r....c........
-000006d0: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
-000006e0: 7360 0000 0074 007c 0083 017d 027c 0264  s`...t.|...}.|.d
-000006f0: 0119 0072 5874 01a0 027c 0264 0219 0064  ...rXt...|.d...d
-00000700: 03a1 027d 0374 01a0 027c 0264 0419 0064  ...}.t...|.d...d
-00000710: 03a1 027d 047c 0474 037c 0264 0519 0064  ...}.|.t.|.d...d
-00000720: 068d 0118 007d 057c 016a 0464 0764 087c  .....}.|.j.d.d.|
-00000730: 007c 037c 047c 0564 098d 0653 0064 0a53  .|.|.|.d...S.d.S
-00000740: 0064 0a53 0029 0b7a 4020 4469 7370 6c61  .d.S.).z@ Displa
-00000750: 7973 2073 6f6d 6520 696e 666f 726d 6174  ys some informat
-00000760: 696f 6e73 2061 626f 7574 2074 6865 2063  ions about the c
-00000770: 6f6e 7465 7374 206f 6e20 7468 6520 636f  ontest on the co
-00000780: 7572 7365 2070 6167 6572 0e00 0000 720f  urse pager....r.
-00000790: 0000 0072 1b00 0000 7220 0000 0072 2100  ...r....r ...r!.
-000007a0: 0000 721d 0000 007a 1063 6f75 7273 655f  ..r....z.course_
-000007b0: 6d65 6e75 2e68 746d 6cfa 1966 726f 6e74  menu.html..front
-000007c0: 656e 642f 706c 7567 696e 732f 636f 6e74  end/plugins/cont
-000007d0: 6573 7473 2905 da0f 7465 6d70 6c61 7465  ests)...template
-000007e0: 5f66 6f6c 6465 7272 0b00 0000 720f 0000  _folderr....r...
-000007f0: 0072 2000 0000 7221 0000 004e 2905 7211  .r ...r!...N).r.
-00000800: 0000 0072 0300 0000 da08 7374 7270 7469  ...r......strpti
-00000810: 6d65 7204 0000 00da 0672 656e 6465 7229  mer......render)
-00000820: 0672 0b00 0000 da0f 7465 6d70 6c61 7465  .r......template
-00000830: 5f68 656c 7065 7272 1400 0000 720f 0000  _helperr....r...
-00000840: 0072 2000 0000 7221 0000 0072 0900 0000  .r ...r!...r....
-00000850: 7209 0000 0072 0c00 0000 da0b 636f 7572  r....r......cour
-00000860: 7365 5f6d 656e 7534 0000 0073 1200 0000  se_menu4...s....
-00000870: 0002 0801 0801 1001 1001 1201 0801 08ff  ................
-00000880: 0603 722c 0000 0063 0000 0000 0000 0000  ..r,...c........
-00000890: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000008a0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000008b0: 0364 0264 0384 005a 0464 0453 0029 05da  .d.d...Z.d.S.)..
-000008c0: 1143 6f6e 7465 7374 5363 6f72 6562 6f61  .ContestScoreboa
-000008d0: 7264 7a28 2044 6973 706c 6179 7320 7468  rdz( Displays th
-000008e0: 6520 7363 6f72 6562 6f61 7264 206f 6620  e scoreboard of 
-000008f0: 7468 6520 636f 6e74 6573 7420 6302 0000  the contest c...
-00000900: 0000 0000 0000 0000 0016 0000 000b 0000  ................
-00000910: 0003 0000 0073 9a03 0000 8800 6a00 a001  .....s......j...
-00000920: 7c01 a101 7d02 7402 7c02 8301 7d03 7c03  |...}.t.|...}.|.
-00000930: 6401 1900 7322 7403 8300 8201 7404 a005  d...s"t.....t...
-00000940: 7c03 6402 1900 6403 a102 7d04 7404 a005  |.d...d...}.t...
-00000950: 7c03 6404 1900 6403 a102 7d05 7c05 7406  |.d...d...}.|.t.
-00000960: 7c03 6405 1900 6406 8d01 1800 7d06 8800  |.d...d.....}...
-00000970: 6a07 a008 7c02 a101 7d07 7409 7c02 a00a  j...|...}.t.|...
-00000980: a100 a00b a100 8301 7d08 8800 6a0c 6a0d  ........}...j.j.
-00000990: a00e 6407 7c07 6901 7c01 7c04 7c06 6408  ..d.|.i.|.|.|.d.
-000009a0: 9c02 6409 640a 9c04 640b 640c 640b 640b  ..d.d...d.d.d.d.
-000009b0: 640b 640d 9c05 a102 a00f 640e 7410 6a11  d.d.......d.t.j.
-000009c0: 6602 6701 a101 7d09 640f 6410 8400 7c08  f.g...}.d.d...|.
-000009d0: 4400 8301 8901 8700 8701 6602 6411 6410  D.........f.d.d.
-000009e0: 8408 7c07 4400 8301 7d0a 6700 7d0b 6412  ..|.D...}.g.}.d.
-000009f0: 6410 8400 7c08 4400 8301 7d0c 7c09 4400  d...|.D...}.|.D.
-00000a00: 9001 5d84 7d0d 7c0d 6413 1900 4400 9001  ..].}.|.d...D...
-00000a10: 5d74 7d0e 7c0d 6414 1900 7c08 7601 9001  ]t}.|.d...|.v...
-00000a20: 720a 71f4 7c0e 7c07 7601 9001 7216 71f4  r.q.|.|.v...r.q.
-00000a30: 7c0a 7c0e 1900 6415 1900 7c0d 6414 1900  |.|...d...|.d...
-00000a40: 1900 7d0f 7c0f 6416 1900 6417 6b02 73f4  ..}.|.d...d.k.s.
-00000a50: 7c0f 6416 1900 6418 6b02 9001 7248 71f4  |.d...d.k...rHq.
-00000a60: 71f4 7c0d 6419 1900 641a 6b02 9001 72d2  q.|.d...d.k...r.
-00000a70: 7c0c 7c0d 6414 1900 1900 9001 737a 6418  |.|.d.......szd.
-00000a80: 7c0f 6416 3c00 640b 7c0c 7c0d 6414 1900  |.d.<.d.|.|.d...
-00000a90: 3c00 6e08 6417 7c0f 6416 3c00 7c0f 641b  <.n.d.|.d.<.|.d.
-00000aa0: 0500 1900 641c 3700 0300 3c00 7c0d 640e  ....d.7...<.|.d.
-00000ab0: 1900 7c0f 641d 3c00 7c0d 640e 1900 7406  ..|.d.<.|.d...t.
-00000ac0: 7c03 641e 1900 7c0f 641b 1900 641c 1800  |.d...|.d...d...
-00000ad0: 1400 641f 8d01 1700 7c04 1800 a012 a100  ..d.....|.......
-00000ae0: 6420 1b00 7c0f 6421 3c00 6e5e 7c0d 6419  d ..|.d!<.n^|.d.
-00000af0: 1900 6422 6b02 9001 73ee 7c0d 6419 1900  ..d"k...s.|.d...
-00000b00: 6423 6b02 9002 7208 6424 7c0f 6416 3c00  d#k...r.d$|.d.<.
-00000b10: 7c0f 641b 0500 1900 641c 3700 0300 3c00  |.d.....d.7...<.
-00000b20: 6e28 7c0d 6419 1900 6425 6b02 72f4 6426  n(|.d...d%k.r.d&
-00000b30: 7c0f 6416 3c00 7c0f 641b 0500 1900 641c  |.d.<.|.d.....d.
-00000b40: 3700 0300 3c00 6e02 71f4 7c0b a013 7c0a  7...<.n.q.|...|.
-00000b50: 7c0e 1900 6427 1900 7c0d 640e 1900 7c0f  |...d'..|.d...|.
-00000b60: 6416 1900 6417 6b02 9002 705c 7c0f 6416  d...d.k...p\|.d.
-00000b70: 1900 6418 6b02 7c0d 6414 1900 6428 9c04  ..d.k.|.d...d(..
-00000b80: a101 0100 71f4 71e6 7c0b a014 a100 0100  ....q.q.|.......
-00000b90: 7c0a 4400 5d68 7d10 6429 6429 6702 7d11  |.D.]h}.d)d)g.}.
-00000ba0: 7409 7c0a 7c10 1900 6415 1900 a015 a100  t.|.|...d.......
-00000bb0: 8301 4400 5d34 7d12 6421 7c12 7600 9002  ..D.]4}.d!|.v...
-00000bc0: 729a 7c11 6429 0500 1900 641c 3700 0300  r.|.d)....d.7...
-00000bd0: 3c00 7c11 641c 0500 1900 7c12 6421 1900  <.|.d.....|.d!..
-00000be0: 3700 0300 3c00 9002 719a 7416 7c11 8301  7...<...q.t.|...
-00000bf0: 7c0a 7c10 1900 6421 3c00 9002 717a 7417  |.|...d!<...qzt.
-00000c00: 7418 7409 7c0a a019 a100 8301 642a 642b  t.t.|.......d*d+
-00000c10: 8400 642c 8d02 8301 7d0a 6400 7d13 6429  ..d,....}.d.}.d)
-00000c20: 7d14 741a 7c0a a00b a100 8301 4400 5d66  }.t.|.......D.]f
-00000c30: 5c02 7d15 7d10 7c0a 7c10 1900 6421 1900  \.}.}.|.|...d!..
-00000c40: 7c13 6b03 9003 7260 7c0a 7c10 1900 6421  |.k...r`|.|...d!
-00000c50: 1900 7d13 7c15 641c 1700 7d14 7c14 7c0a  ..}.|.d...}.|.|.
-00000c60: 7c10 1900 642d 3c00 741b 7c14 8301 7c0a  |...d-<.t.|...|.
-00000c70: 7c10 1900 642e 3c00 6e18 7c14 7c0a 7c10  |...d.<.n.|.|.|.
-00000c80: 1900 642d 3c00 642f 7c0a 7c10 1900 642e  ..d-<.d/|.|...d.
-00000c90: 3c00 9003 7114 8800 6a1c 6a1d 6430 6431  <...q...j.j.d0d1
-00000ca0: 7c02 7c04 7c05 7c06 7c08 7c0a 7c0b 6432  |.|.|.|.|.|.|.d2
-00000cb0: 8d09 5300 2933 4e72 0e00 0000 720f 0000  ..S.)3Nr....r...
-00000cc0: 0072 1b00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000cd0: 721d 0000 007a 0324 696e 2902 7a04 2467  r....z.$in).z.$g
-00000ce0: 7465 7a03 246c 74da 0464 6f6e 6529 04da  tez.$lt..done)..
-00000cf0: 0875 7365 726e 616d 65da 0863 6f75 7273  .username..cours
-00000d00: 6569 64da 0c73 7562 6d69 7474 6564 5f6f  eid..submitted_o
-00000d10: 6eda 0673 7461 7475 7354 4629 0572 2f00  n..statusTF).r/.
-00000d20: 0000 da03 5f69 64da 0674 6173 6b69 64da  ...._id..taskid.
-00000d30: 0672 6573 756c 7472 3100 0000 7231 0000  .resultr1...r1..
-00000d40: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000d50: 0000 0600 0000 5300 0000 7318 0000 0069  ......S...s....i
-00000d60: 007c 005d 107d 017c 0164 0064 0164 029c  .|.].}.|.d.d.d..
-00000d70: 0293 0271 0453 0029 03da 024e 4172 0100  ...q.S.)...NAr..
-00000d80: 0000 2902 7232 0000 00da 0574 7269 6573  ..).r2.....tries
-00000d90: 7209 0000 00a9 02da 022e 3072 3400 0000  r.........0r4...
-00000da0: 7209 0000 0072 0900 0000 720c 0000 00da  r....r....r.....
-00000db0: 0a3c 6469 6374 636f 6d70 3e57 0000 00f3  .<dictcomp>W....
-00000dc0: 0000 0000 7a2e 436f 6e74 6573 7453 636f  ....z.ContestSco
-00000dd0: 7265 626f 6172 642e 4745 545f 4155 5448  reboard.GET_AUTH
-00000de0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000df0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-00000e00: 0002 0000 0007 0000 0013 0000 0073 2600  .............s&.
-00000e10: 0000 6900 7c00 5d1e 7d01 7c01 8800 6a00  ..i.|.].}.|...j.
-00000e20: a001 7c01 a101 7402 a003 8801 a101 6400  ..|...t.......d.
-00000e30: 9c02 9302 7104 5300 2901 2902 da04 6e61  ....q.S.).)...na
-00000e40: 6d65 da05 7461 736b 7329 04da 0c75 7365  me..tasks)...use
-00000e50: 725f 6d61 6e61 6765 72da 1167 6574 5f75  r_manager..get_u
-00000e60: 7365 725f 7265 616c 6e61 6d65 da04 636f  ser_realname..co
-00000e70: 7079 da08 6465 6570 636f 7079 2902 7239  py..deepcopy).r9
-00000e80: 0000 0072 2f00 0000 a902 da04 7365 6c66  ...r/.......self
-00000e90: 5a0b 7461 736b 5f73 7461 7475 7372 0900  Z.task_statusr..
-00000ea0: 0000 720c 0000 0072 3a00 0000 5800 0000  ..r....r:...X...
-00000eb0: 723b 0000 0063 0100 0000 0000 0000 0000  r;...c..........
-00000ec0: 0000 0200 0000 0400 0000 5300 0000 7312  ..........S...s.
-00000ed0: 0000 0069 007c 005d 0a7d 017c 0164 0093  ...i.|.].}.|.d..
-00000ee0: 0271 0453 0029 0146 7209 0000 0072 3800  .q.S.).Fr....r8.
-00000ef0: 0000 7209 0000 0072 0900 0000 720c 0000  ..r....r....r...
-00000f00: 0072 3a00 0000 5c00 0000 723b 0000 0072  .r:...\...r;...r
-00000f10: 2f00 0000 7234 0000 0072 3d00 0000 7232  /...r4...r=...r2
-00000f20: 0000 00da 0241 435a 0341 4346 7235 0000  .....ACZ.ACFr5..
-00000f30: 00da 0773 7563 6365 7373 7237 0000 0072  ...successr7...r
-00000f40: 1c00 0000 da04 7469 6d65 7222 0000 0029  ......timer"...)
-00000f50: 01da 076d 696e 7574 6573 e93c 0000 00da  ...minutes.<....
-00000f60: 0573 636f 7265 da06 6661 696c 6564 da06  .score..failed..
-00000f70: 6b69 6c6c 6564 5a02 5741 da07 7469 6d65  killedZ.WA..time
-00000f80: 6f75 745a 0354 4c45 723c 0000 0029 04da  outZ.TLEr<...)..
-00000f90: 0475 7365 72da 0477 6865 6e72 3500 0000  .user..whenr5...
-00000fa0: 7234 0000 0072 0100 0000 6301 0000 0000  r4...r....c.....
-00000fb0: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-00000fc0: 0000 0073 2200 0000 7c00 6401 1900 6402  ...s"...|.d...d.
-00000fd0: 1900 6403 1900 0b00 7c00 6401 1900 6402  ..d.....|.d...d.
-00000fe0: 1900 6401 1900 6602 5300 2904 4e72 1c00  ..d...f.S.).Nr..
-00000ff0: 0000 7249 0000 0072 0100 0000 7209 0000  ..rI...r....r...
-00001000: 0029 01da 0174 7209 0000 0072 0900 0000  .)...tr....r....
-00001010: 720c 0000 00da 083c 6c61 6d62 6461 3e89  r......<lambda>.
-00001020: 0000 0072 3b00 0000 7a2c 436f 6e74 6573  ...r;...z,Contes
-00001030: 7453 636f 7265 626f 6172 642e 4745 545f  tScoreboard.GET_
-00001040: 4155 5448 2e3c 6c6f 6361 6c73 3e2e 3c6c  AUTH.<locals>.<l
-00001050: 616d 6264 613e 2901 da03 6b65 79da 0472  ambda>)...key..r
-00001060: 616e 6b5a 0e64 6973 706c 6179 6564 5f72  ankZ.displayed_r
-00001070: 616e 6bda 007a 0f73 636f 7265 626f 6172  ank..z.scoreboar
-00001080: 642e 6874 6d6c 7227 0000 0029 0872 2800  d.htmlr'...).r(.
-00001090: 0000 720b 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
-000010a0: 0072 2100 0000 723d 0000 00da 0772 6573  .r!...r=.....res
-000010b0: 756c 7473 da08 6163 7469 7669 7479 291e  ults..activity).
-000010c0: da0e 636f 7572 7365 5f66 6163 746f 7279  ..course_factory
-000010d0: da0a 6765 745f 636f 7572 7365 7211 0000  ..get_courser...
-000010e0: 0072 0500 0000 7203 0000 0072 2900 0000  .r....r....r)...
-000010f0: 7204 0000 0072 3e00 0000 da1b 6765 745f  r....r>.....get_
-00001100: 636f 7572 7365 5f72 6567 6973 7465 7265  course_registere
-00001110: 645f 7573 6572 73da 046c 6973 74da 0967  d_users..list..g
-00001120: 6574 5f74 6173 6b73 da04 6b65 7973 da08  et_tasks..keys..
-00001130: 6461 7461 6261 7365 da0b 7375 626d 6973  database..submis
-00001140: 7369 6f6e 73da 0466 696e 64da 0473 6f72  sions..find..sor
-00001150: 74da 0770 796d 6f6e 676f da09 4153 4345  t..pymongo..ASCE
-00001160: 4e44 494e 47da 0d74 6f74 616c 5f73 6563  NDING..total_sec
-00001170: 6f6e 6473 da06 6170 7065 6e64 da07 7265  onds..append..re
-00001180: 7665 7273 65da 0676 616c 7565 73da 0574  verse..values..t
-00001190: 7570 6c65 7202 0000 00da 0673 6f72 7465  upler......sorte
-000011a0: 64da 0569 7465 6d73 da09 656e 756d 6572  d..items..enumer
-000011b0: 6174 65da 0373 7472 722b 0000 0072 2a00  ate..strr+...r*.
-000011c0: 0000 2916 7243 0000 0072 3000 0000 720b  ..).rC...r0...r.
-000011d0: 0000 0072 1400 0000 720f 0000 0072 2000  ...r....r....r .
-000011e0: 0000 7221 0000 00da 0575 7365 7273 723d  ..r!.....usersr=
-000011f0: 0000 005a 0a64 625f 7265 7375 6c74 7372  ...Z.db_resultsr
-00001200: 5400 0000 7255 0000 00da 0e74 6173 6b5f  T...rU.....task_
-00001210: 7375 6363 6565 6465 64da 0a73 7562 6d69  succeeded..submi
-00001220: 7373 696f 6e72 2f00 0000 7232 0000 0072  ssionr/...r2...r
-00001230: 4d00 0000 7249 0000 00da 0464 6174 61da  M...rI.....data.
-00001240: 036f 6c64 5a0c 6375 7272 656e 745f 7261  .oldZ.current_ra
-00001250: 6e6b da03 6369 6472 0900 0000 7242 0000  nk..cidr....rB..
-00001260: 0072 0c00 0000 da08 4745 545f 4155 5448  .r......GET_AUTH
-00001270: 4400 0000 73a2 0000 0000 010c 0108 0108  D...s...........
-00001280: 0106 0110 0110 0112 020c 0110 0208 0106  ................
-00001290: 0102 0108 0102 fc04 050e fb04 050a fb04  ................
-000012a0: 070e 0114 0104 030e 010a 010e 010e 0102  ................
-000012b0: 010a 0102 0114 011a 0104 020e 010e 0108  ................
-000012c0: 010e 0208 0110 010c 0106 0118 ff02 0202  ................
-000012d0: fe06 0202 fe0a 031c 0108 0112 010c 0108  ................
-000012e0: 0112 0202 010e 0106 0118 0106 fd0c 0408  ................
-000012f0: 0208 0108 0118 010a 0110 0118 0114 031c  ................
-00001300: 0304 0104 0114 0112 010c 0108 010c 0112  ................
-00001310: 020c 0110 020a 010a 0104 fe7a 1a43 6f6e  ...........z.Con
-00001320: 7465 7374 5363 6f72 6562 6f61 7264 2e47  testScoreboard.G
-00001330: 4554 5f41 5554 484e 2905 da08 5f5f 6e61  ET_AUTHN)...__na
-00001340: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001350: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00001360: 5f5f 646f 635f 5f72 7100 0000 7209 0000  __doc__rq...r...
-00001370: 0072 0900 0000 7209 0000 0072 0c00 0000  .r....r....r....
-00001380: 722d 0000 0041 0000 0073 0400 0000 0801  r-...A...s......
-00001390: 0402 722d 0000 0063 0000 0000 0000 0000  ..r-...c........
-000013a0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000013b0: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
-000013c0: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
-000013d0: 0564 0664 0784 005a 0664 0853 0029 09da  .d.d...Z.d.S.)..
-000013e0: 0c43 6f6e 7465 7374 4164 6d69 6e7a 1f20  .ContestAdminz. 
-000013f0: 436f 6e74 6573 7420 7365 7474 696e 6773  Contest settings
-00001400: 2066 6f72 2061 2063 6f75 7273 6520 6303   for a course c.
-00001410: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00001420: 0000 0043 0000 0073 2e00 0000 7c00 6a00  ...C...s....|.j.
-00001430: a001 7c01 a002 a100 a101 7d03 7c02 7c03  ..|.......}.|.|.
-00001440: 6401 3c00 7c00 6a00 a003 7c01 a002 a100  d.<.|.j...|.....
-00001450: 7c03 a102 0100 6402 5300 2903 7a2b 2053  |.....d.S.).z+ S
-00001460: 6176 6573 2075 7064 6174 6564 2063 6f6e  aves updated con
-00001470: 7465 7374 2064 6174 6120 666f 7220 7468  test data for th
-00001480: 6520 636f 7572 7365 2072 1a00 0000 4e29  e course r....N)
-00001490: 0472 5600 0000 da1d 6765 745f 636f 7572  .rV.....get_cour
-000014a0: 7365 5f64 6573 6372 6970 746f 725f 636f  se_descriptor_co
-000014b0: 6e74 656e 74da 0667 6574 5f69 64da 2075  ntent..get_id. u
-000014c0: 7064 6174 655f 636f 7572 7365 5f64 6573  pdate_course_des
-000014d0: 6372 6970 746f 725f 636f 6e74 656e 7429  criptor_content)
-000014e0: 0472 4300 0000 720b 0000 0072 1400 0000  .rC...r....r....
-000014f0: da0e 636f 7572 7365 5f63 6f6e 7465 6e74  ..course_content
-00001500: 7209 0000 0072 0900 0000 720c 0000 00da  r....r....r.....
-00001510: 1173 6176 655f 636f 6e74 6573 745f 6461  .save_contest_da
-00001520: 7461 a000 0000 7306 0000 0000 0210 0108  ta....s.........
-00001530: 017a 1e43 6f6e 7465 7374 4164 6d69 6e2e  .z.ContestAdmin.
-00001540: 7361 7665 5f63 6f6e 7465 7374 5f64 6174  save_contest_dat
-00001550: 6163 0200 0000 0000 0000 0000 0000 0500  ac..............
-00001560: 0000 0800 0000 4300 0000 7332 0000 007c  ......C...s2...|
-00001570: 006a 007c 0164 0164 028d 025c 027d 027d  .j.|.d.d...\.}.}
-00001580: 0374 017c 0283 017d 047c 006a 026a 0364  .t.|...}.|.j.j.d
-00001590: 0364 047c 027c 0464 0564 0164 068d 0653  .d.|.|.d.d.d...S
-000015a0: 0029 077a 2620 4745 5420 7265 7175 6573  .).z& GET reques
-000015b0: 743a 2073 696d 706c 7920 6469 7370 6c61  t: simply displa
-000015c0: 7920 7468 6520 666f 726d 2046 a901 da0f  y the form F....
-000015d0: 616c 6c6f 775f 616c 6c5f 7374 6166 66fa  allow_all_staff.
-000015e0: 0a61 646d 696e 2e68 746d 6c72 2700 0000  .admin.htmlr'...
-000015f0: 4ea9 0572 2800 0000 720b 0000 0072 6e00  N..r(...r....rn.
-00001600: 0000 da06 6572 726f 7273 da05 7361 7665  ....errors..save
-00001610: 6429 04da 1b67 6574 5f63 6f75 7273 655f  d)...get_course_
-00001620: 616e 645f 6368 6563 6b5f 7269 6768 7473  and_check_rights
-00001630: 7211 0000 0072 2b00 0000 722a 0000 0029  r....r+...r*...)
-00001640: 0572 4300 0000 7230 0000 0072 0b00 0000  .rC...r0...r....
-00001650: da02 5f5f 7214 0000 0072 0900 0000 7209  ..__r....r....r.
-00001660: 0000 0072 0c00 0000 7271 0000 00a6 0000  ...r....rq......
-00001670: 0073 0a00 0000 0002 1201 0801 0c01 06ff  .s..............
-00001680: 7a15 436f 6e74 6573 7441 646d 696e 2e47  z.ContestAdmin.G
-00001690: 4554 5f41 5554 4863 0200 0000 0000 0000  ET_AUTHc........
-000016a0: 0000 0000 0900 0000 0800 0000 4300 0000  ............C...
-000016b0: 73ba 0100 007c 006a 007c 0164 0164 028d  s....|.j.|.d.d..
-000016c0: 025c 027d 027d 0374 017c 0283 017d 0474  .\.}.}.t.|...}.t
-000016d0: 026a 036a 047d 0567 007d 0690 017a 2c7c  .j.j.}.g.}...z,|
-000016e0: 05a0 0564 0364 04a1 0264 056b 027c 0464  ...d.d...d.k.|.d
-000016f0: 033c 007c 0564 0619 007c 0464 063c 007c  .<.|.d...|.d.<.|
-00001700: 0564 0719 007c 0464 073c 007a 1474 06a0  .d...|.d.<.z.t..
-00001710: 077c 0464 0619 0064 08a1 027d 0757 006e  .|.d...d...}.W.n
-00001720: 1601 0001 0001 007c 06a0 0864 09a1 0101  .......|...d....
-00001730: 0059 006e 0230 007a 1474 06a0 077c 0464  .Y.n.0.z.t...|.d
-00001740: 0719 0064 08a1 027d 0857 006e 1601 0001  ...d...}.W.n....
-00001750: 0001 007c 06a0 0864 0aa1 0101 0059 006e  ...|...d.....Y.n
-00001760: 0230 0074 097c 0683 0164 0b6b 0272 cc7c  .0.t.|...d.k.r.|
-00001770: 077c 086b 0572 cc7c 06a0 0864 0ca1 0101  .|.k.r.|...d....
-00001780: 007a 2a74 0a7c 0564 0d19 0083 017c 0464  .z*t.|.d.....|.d
-00001790: 0d3c 007c 0464 0d19 0064 0b6b 0072 f47c  .<.|.d...d.k.r.|
-000017a0: 06a0 0864 0ea1 0101 0057 006e 1601 0001  ...d.....W.n....
-000017b0: 0001 007c 06a0 0864 0fa1 0101 0059 006e  ...|...d.....Y.n
-000017c0: 0230 007a 2c74 0a7c 0564 1019 0083 017c  .0.z,t.|.d.....|
-000017d0: 0464 103c 007c 0464 1019 0064 0b6b 0090  .d.<.|.d...d.k..
-000017e0: 0172 387c 06a0 0864 11a1 0101 0057 006e  .r8|...d.....W.n
-000017f0: 1601 0001 0001 007c 06a0 0864 12a1 0101  .......|...d....
-00001800: 0059 006e 0230 0057 006e 1601 0001 0001  .Y.n.0.W.n......
-00001810: 007c 06a0 0864 13a1 0101 0059 006e 0230  .|...d.....Y.n.0
-00001820: 0074 097c 0683 0164 0b6b 0290 0172 9e7c  .t.|...d.k...r.|
-00001830: 00a0 0b7c 027c 04a1 0201 007c 006a 0c6a  ...|.|.....|.j.j
-00001840: 0d64 1464 157c 027c 0464 1664 1764 188d  .d.d.|.|.d.d.d..
-00001850: 0653 007c 006a 0c6a 0d64 1464 157c 027c  .S.|.j.j.d.d.|.|
-00001860: 047c 0664 0164 188d 0653 0064 1653 0029  .|.d.d...S.d.S.)
-00001870: 197a 2320 504f 5354 2072 6571 7565 7374  .z# POST request
-00001880: 3a20 7570 6461 7465 2074 6865 2073 6574  : update the set
-00001890: 7469 6e67 7320 4672 7c00 0000 720e 0000  tings Fr|...r...
-000018a0: 00da 0130 da01 3172 0f00 0000 7220 0000  ...0..1r....r ..
-000018b0: 0072 1b00 0000 7a12 496e 7661 6c69 6420  .r....z.Invalid 
-000018c0: 7374 6172 7420 6461 7465 7a10 496e 7661  start datez.Inva
-000018d0: 6c69 6420 656e 6420 6461 7465 7201 0000  lid end dater...
-000018e0: 007a 2453 7461 7274 2064 6174 6520 7368  .z$Start date sh
-000018f0: 6f75 6c64 2062 6520 6265 666f 7265 2065  ould be before e
-00001900: 6e64 2064 6174 6572 2100 0000 7a42 496e  nd dater!...zBIn
-00001910: 7661 6c69 6420 6e75 6d62 6572 206f 6620  valid number of 
-00001920: 686f 7572 7320 666f 7220 7468 6520 626c  hours for the bl
-00001930: 6163 6b6f 7574 3a20 7368 6f75 6c64 2062  ackout: should b
-00001940: 6520 6772 6561 7465 7220 7468 616e 2030  e greater than 0
-00001950: 7a28 496e 7661 6c69 6420 6e75 6d62 6572  z(Invalid number
-00001960: 206f 6620 686f 7572 7320 666f 7220 7468   of hours for th
-00001970: 6520 626c 6163 6b6f 7574 7222 0000 007a  e blackoutr"...z
-00001980: 4349 6e76 616c 6964 206e 756d 6265 7220  CInvalid number 
-00001990: 6f66 206d 696e 7574 6573 2066 6f72 2074  of minutes for t
-000019a0: 6865 2070 656e 616c 7479 3a20 7368 6f75  he penalty: shou
-000019b0: 6c64 2062 6520 6772 6561 7465 7220 7468  ld be greater th
-000019c0: 616e 2030 7a29 496e 7661 6c69 6420 6e75  an 0z)Invalid nu
-000019d0: 6d62 6572 206f 6620 6d69 6e75 7465 7320  mber of minutes 
-000019e0: 666f 7220 7468 6520 7065 6e61 6c74 797a  for the penaltyz
-000019f0: 1d55 7365 7220 7265 7475 726e 6564 2061  .User returned a
-00001a00: 6e20 696e 7661 6c69 6420 666f 726d 727e  n invalid formr~
-00001a10: 0000 0072 2700 0000 4e54 727f 0000 0029  ...r'...NTr....)
-00001a20: 0e72 8200 0000 7211 0000 0072 1600 0000  .r....r....r....
-00001a30: 7217 0000 00da 0466 6f72 6d72 2400 0000  r......formr$...
-00001a40: 7203 0000 0072 2900 0000 7263 0000 00da  r....r)...rc....
-00001a50: 036c 656e da03 696e 7472 7b00 0000 722b  .len..intr{...r+
-00001a60: 0000 0072 2a00 0000 2909 7243 0000 0072  ...r*...).rC...r
-00001a70: 3000 0000 720b 0000 0072 8300 0000 7214  0...r....r....r.
-00001a80: 0000 00da 086e 6577 5f64 6174 6172 8000  .....new_datar..
-00001a90: 0000 720f 0000 0072 2000 0000 7209 0000  ..r....r ...r...
-00001aa0: 0072 0900 0000 720c 0000 00da 0950 4f53  .r....r......POS
-00001ab0: 545f 4155 5448 ad00 0000 7352 0000 0000  T_AUTH....sR....
-00001ac0: 0212 0108 0208 0104 0104 0114 010c 010c  ................
-00001ad0: 0202 0114 0106 0110 0202 0114 0106 0110  ................
-00001ae0: 020c 0108 010a 0202 0110 010c 010e 0106  ................
-00001af0: 0110 0202 0110 010e 010e 0106 0114 0106  ................
-00001b00: 0110 020e 010c 010c 0106 ff06 030c 0106  ................
-00001b10: ff7a 1643 6f6e 7465 7374 4164 6d69 6e2e  .z.ContestAdmin.
-00001b20: 504f 5354 5f41 5554 484e 2907 7272 0000  POST_AUTHN).rr..
-00001b30: 0072 7300 0000 7274 0000 0072 7500 0000  .rs...rt...ru...
-00001b40: 727b 0000 0072 7100 0000 728a 0000 0072  r{...rq...r....r
-00001b50: 0900 0000 7209 0000 0072 0900 0000 720c  ....r....r....r.
-00001b60: 0000 0072 7600 0000 9d00 0000 7308 0000  ...rv.......s...
-00001b70: 0008 0104 0208 0608 0772 7600 0000 6304  .........rv...c.
-00001b80: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00001b90: 0000 0043 0000 0073 5800 0000 7c00 a000  ...C...sX...|...
-00001ba0: 6401 7401 a002 6402 a101 a102 0100 7c00  d.t...d.......|.
-00001bb0: a000 6403 7403 a002 6404 a101 a102 0100  ..d.t...d.......
-00001bc0: 7c00 a004 6405 7405 a102 0100 7c00 a004  |...d.t.....|...
-00001bd0: 6406 7406 a102 0100 7c00 a004 6407 7407  d.t.....|...d.t.
-00001be0: a102 0100 7c00 a004 6408 7408 a102 0100  ....|...d.t.....
-00001bf0: 6409 5300 290a 7ab6 0a20 2020 2020 2020  d.S.).z..       
-00001c00: 2049 6e69 7420 7468 6520 636f 6e74 6573   Init the contes
-00001c10: 7420 706c 7567 696e 2e0a 2020 2020 2020  t plugin..      
-00001c20: 2020 4176 6169 6c61 626c 6520 636f 6e66    Available conf
-00001c30: 6967 7572 6174 696f 6e3a 0a20 2020 2020  iguration:.     
-00001c40: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
-00001c50: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001c60: 2020 2020 2022 706c 7567 696e 5f6d 6f64       "plugin_mod
-00001c70: 756c 6522 3a20 2269 6e67 696e 696f 7573  ule": "inginious
-00001c80: 2e66 726f 6e74 656e 642e 706c 7567 696e  .frontend.plugin
-00001c90: 732e 636f 6e74 6573 7473 220a 2020 2020  s.contests".    
-00001ca0: 2020 2020 2020 2020 7d0a 2020 2020 7a13          }.    z.
-00001cb0: 2f63 6f6e 7465 7374 2f3c 636f 7572 7365  /contest/<course
-00001cc0: 6964 3e5a 1163 6f6e 7465 7374 7363 6f72  id>Z.contestscor
-00001cd0: 6562 6f61 7264 7a19 2f61 646d 696e 2f3c  eboardz./admin/<
-00001ce0: 636f 7572 7365 6964 3e2f 636f 6e74 6573  courseid>/contes
-00001cf0: 745a 0c63 6f6e 7465 7374 6164 6d69 6eda  tZ.contestadmin.
-00001d00: 1163 6f75 7273 655f 6164 6d69 6e5f 6d65  .course_admin_me
-00001d10: 6e75 7215 0000 00da 0b68 6561 6465 725f  nur......header_
-00001d20: 6874 6d6c 722c 0000 004e 2909 da08 6164  htmlr,...N)...ad
-00001d30: 645f 7061 6765 722d 0000 00da 0761 735f  d_pager-.....as_
-00001d40: 7669 6577 7276 0000 00da 0861 6464 5f68  viewrv.....add_h
-00001d50: 6f6f 6b72 0d00 0000 7215 0000 0072 1900  ookr....r....r..
-00001d60: 0000 722c 0000 0029 04da 0e70 6c75 6769  ..r,...)...plugi
-00001d70: 6e5f 6d61 6e61 6765 7272 5600 0000 da06  n_managerrV.....
-00001d80: 636c 6965 6e74 da06 636f 6e66 6967 7209  client..configr.
-00001d90: 0000 0072 0900 0000 720c 0000 00da 0469  ...r....r......i
-00001da0: 6e69 74e0 0000 0073 0c00 0000 000b 1201  nit....s........
-00001db0: 1201 0c01 0c01 0c01 7293 0000 0029 1872  ........r....).r
-00001dc0: 7500 0000 7240 0000 00da 0b63 6f6c 6c65  u...r@.....colle
-00001dd0: 6374 696f 6e73 7202 0000 0072 0300 0000  ctionsr....r....
-00001de0: 7204 0000 0072 6000 0000 7216 0000 005a  r....r`...r....Z
-00001df0: 1377 6572 6b7a 6575 672e 6578 6365 7074  .werkzeug.except
-00001e00: 696f 6e73 7205 0000 005a 2269 6e67 696e  ionsr....Z"ingin
-00001e10: 696f 7573 2e66 726f 6e74 656e 642e 6163  ious.frontend.ac
-00001e20: 6365 7373 6962 6c65 5f74 696d 6572 0600  cessible_timer..
-00001e30: 0000 da2b 696e 6769 6e69 6f75 732e 6672  ...+inginious.fr
-00001e40: 6f6e 7465 6e64 2e70 6167 6573 2e63 6f75  ontend.pages.cou
-00001e50: 7273 655f 6164 6d69 6e2e 7574 696c 7372  rse_admin.utilsr
-00001e60: 0700 0000 da1e 696e 6769 6e69 6f75 732e  ......inginious.
-00001e70: 6672 6f6e 7465 6e64 2e70 6167 6573 2e75  frontend.pages.u
-00001e80: 7469 6c73 7208 0000 0072 0d00 0000 7215  tilsr....r....r.
-00001e90: 0000 0072 1900 0000 7211 0000 0072 2c00  ...r....r....r,.
-00001ea0: 0000 722d 0000 0072 7600 0000 7293 0000  ..r-...rv...r...
-00001eb0: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00001ec0: 720c 0000 00da 083c 6d6f 6475 6c65 3e06  r......<module>.
-00001ed0: 0000 0073 2200 0000 0402 0801 0c01 1002  ...s"...........
-00001ee0: 0801 0802 0c01 0c01 0c01 0c03 0805 0808  ................
-00001ef0: 0808 080a 080d 105c 1043                 .......\.C
+00000090: 6d0f 5a0f 0100 6401 6409 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 0100 640a 640b 8400 5a12 4700 640c 640d  ..d.d...Z.G.d.d.
+000000b0: 8400 640d 6511 8303 5a13 640e 640f 8400  ..d.e...Z.d.d...
+000000c0: 5a14 6410 6411 8400 5a15 4700 6412 6413  Z.d.d...Z.G.d.d.
+000000d0: 8400 6413 650f 8303 5a16 4700 6414 6415  ..d.e...Z.G.d.d.
+000000e0: 8400 6415 650d 8303 5a17 6416 6417 8400  ..d.e...Z.d.d...
+000000f0: 5a18 6402 5300 2918 7a66 2041 6e20 616c  Z.d.S.).zf An al
+00000100: 676f 7269 7468 6d20 636f 6e74 6573 7420  gorithm contest 
+00000110: 706c 7567 696e 2066 6f72 2049 4e47 496e  plugin for INGIn
+00000120: 696f 7573 2e20 4261 7365 6420 6f6e 2074  ious. Based on t
+00000130: 6865 2073 616d 6520 7072 696e 6369 706c  he same principl
+00000140: 6573 2074 6861 6e20 636f 6e74 6573 7473  es than contests
+00000150: 206c 696b 6520 4143 4d2d 4943 5043 2e20   like ACM-ICPC. 
+00000160: e900 0000 004e 2901 da0b 4f72 6465 7265  .....N)...Ordere
+00000170: 6444 6963 7429 02da 0864 6174 6574 696d  dDict)...datetim
+00000180: 65da 0974 696d 6564 656c 7461 2901 da08  e..timedelta)...
+00000190: 4e6f 7446 6f75 6e64 a901 da0e 4163 6365  NotFound....Acce
+000001a0: 7373 6962 6c65 5469 6d65 2901 da12 494e  ssibleTime)...IN
+000001b0: 4749 6e69 6f75 7341 646d 696e 5061 6765  GIniousAdminPage
+000001c0: 2901 da11 494e 4749 6e69 6f75 7341 7574  )...INGIniousAut
+000001d0: 6850 6167 6529 01da 0f54 6162 6c65 4f66  hPage)...TableOf
+000001e0: 436f 6e74 656e 7473 6301 0000 0000 0000  Contentsc.......
+000001f0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000200: 0073 2000 0000 7c00 a000 a100 7d01 7c01  .s ...|.....}.|.
+00000210: a001 a100 7402 a001 a100 6b02 720e 6401  ....t.....k.r.d.
+00000220: 5300 6402 5300 2903 7a3b 2041 6464 2061  S.d.S.).z; Add a
+00000230: 206d 656e 7520 666f 7220 7468 6520 636f   menu for the co
+00000240: 6e74 6573 7420 7365 7474 696e 6773 2069  ntest settings i
+00000250: 6e20 7468 6520 6164 6d69 6e69 7374 7261  n the administra
+00000260: 7469 6f6e 2029 02da 0763 6f6e 7465 7374  tion )...contest
+00000270: 7a30 3c69 2063 6c61 7373 3d22 6661 2066  z0<i class="fa f
+00000280: 612d 7472 6f70 6879 2066 612d 6677 223e  a-trophy fa-fw">
+00000290: 3c2f 693e 266e 6273 703b 2043 6f6e 7465  </i>&nbsp; Conte
+000002a0: 7374 4e29 03da 1267 6574 5f74 6173 6b5f  stN)...get_task_
+000002b0: 6469 7370 656e 7365 72da 0667 6574 5f69  dispenser..get_i
+000002c0: 64da 0743 6f6e 7465 7374 2902 da06 636f  d..Contest)...co
+000002d0: 7572 7365 da0e 7461 736b 5f64 6973 7065  urse..task_dispe
+000002e0: 6e73 6572 a900 7211 0000 00fa 5f2f 686f  nser..r....._/ho
+000002f0: 6d65 2f61 6e74 686f 6e79 2f44 6f63 756d  me/anthony/Docum
+00000300: 656e 7473 2f69 6e67 696e 696f 7573 2d64  ents/inginious-d
+00000310: 6576 2f49 4e47 496e 696f 7573 2f69 6e67  ev/INGInious/ing
+00000320: 696e 696f 7573 2f66 726f 6e74 656e 642f  inious/frontend/
+00000330: 706c 7567 696e 732f 636f 6e74 6573 7473  plugins/contests
+00000340: 2f5f 5f69 6e69 745f 5f2e 7079 da0e 6164  /__init__.py..ad
+00000350: 645f 6164 6d69 6e5f 6d65 6e75 1600 0000  d_admin_menu....
+00000360: 7308 0000 0008 0210 0104 0104 0272 1300  s............r..
+00000370: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000380: 0000 0003 0000 0040 0000 0073 4400 0000  .......@...sD...
+00000390: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+000003a0: 6504 6403 6404 8400 8301 5a05 6504 6405  e.d.d.....Z.e.d.
+000003b0: 6406 8400 8301 5a06 6407 6408 8400 5a07  d.....Z.d.d...Z.
+000003c0: 6409 640a 8400 5a08 640b 640c 8400 5a09  d.d...Z.d.d...Z.
+000003d0: 640d 5300 290e 720e 0000 0063 0500 0000  d.S.).r....c....
+000003e0: 0000 0000 0000 0000 0500 0000 0900 0000  ................
+000003f0: 4300 0000 7356 0000 0074 00a0 017c 007c  C...sV...t...|.|
+00000400: 017c 02a0 0264 0169 00a1 027c 037c 04a1  .|...d.i...|.|..
+00000410: 0501 007c 02a0 0264 0264 0374 03a0 04a1  ...|...d.d.t....
+00000420: 00a0 0564 04a1 0174 03a0 04a1 0074 0664  ...d...t.....t.d
+00000430: 0564 068d 0117 00a0 0564 04a1 0164 0764  .d.......d...d.d
+00000440: 0864 099c 05a1 027c 005f 0764 0053 0029  .d.....|._.d.S.)
+00000450: 0a4e da08 746f 635f 6461 7461 da10 636f  .N..toc_data..co
+00000460: 6e74 6573 745f 7365 7474 696e 6773 46fa  ntest_settingsF.
+00000470: 1125 592d 256d 2d25 6420 2548 3a25 4d3a  .%Y-%m-%d %H:%M:
+00000480: 2553 e901 0000 00a9 01da 0568 6f75 7273  %S.........hours
+00000490: 7201 0000 00e9 1400 0000 2905 da07 656e  r.........)...en
+000004a0: 6162 6c65 64da 0573 7461 7274 da03 656e  abled..start..en
+000004b0: 64da 0862 6c61 636b 6f75 74da 0770 656e  d..blackout..pen
+000004c0: 616c 7479 2908 720a 0000 00da 085f 5f69  alty).r......__i
+000004d0: 6e69 745f 5fda 0367 6574 7203 0000 00da  nit__..getr.....
+000004e0: 036e 6f77 da08 7374 7266 7469 6d65 7204  .now..strftimer.
+000004f0: 0000 00da 115f 636f 6e74 6573 745f 7365  ....._contest_se
+00000500: 7474 696e 6773 2905 da04 7365 6c66 da0e  ttings)...self..
+00000510: 7461 736b 5f6c 6973 745f 6675 6e63 da0e  task_list_func..
+00000520: 6469 7370 656e 7365 725f 6461 7461 da08  dispenser_data..
+00000530: 6461 7461 6261 7365 da09 636f 7572 7365  database..course
+00000540: 5f69 6472 1100 0000 7211 0000 0072 1200  _idr....r....r..
+00000550: 0000 7220 0000 0021 0000 0073 1400 0000  ..r ...!...s....
+00000560: 1a01 0401 0201 0201 0c01 1601 0201 0201  ................
+00000570: 04fc 0afe 7a10 436f 6e74 6573 742e 5f5f  ....z.Contest.__
+00000580: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000590: 0000 0001 0000 0001 0000 0043 0000 00f3  ...........C....
+000005a0: 0400 0000 6401 5300 2902 4e72 0b00 0000  ....d.S.).Nr....
+000005b0: 7211 0000 0029 01da 0363 6c73 7211 0000  r....)...clsr...
+000005c0: 0072 1100 0000 7212 0000 0072 0d00 0000  .r....r....r....
+000005d0: 2c00 0000 f302 0000 0004 027a 0e43 6f6e  ,..........z.Con
+000005e0: 7465 7374 2e67 6574 5f69 6463 0200 0000  test.get_idc....
+000005f0: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+00000600: 4300 0000 722a 0000 0029 024e 720e 0000  C...r*...).Nr...
+00000610: 0072 1100 0000 2902 722b 0000 00da 086c  .r....).r+.....l
+00000620: 616e 6775 6167 6572 1100 0000 7211 0000  anguager....r...
+00000630: 0072 1200 0000 da08 6765 745f 6e61 6d65  .r......get_name
+00000640: 3000 0000 722c 0000 007a 1043 6f6e 7465  0...r,...z.Conte
+00000650: 7374 2e67 6574 5f6e 616d 6563 0200 0000  st.get_namec....
+00000660: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000670: 4300 0000 732c 0000 0074 00a0 017c 007c  C...s,...t...|.|
+00000680: 01a1 025c 027d 027d 037c 0272 127c 027c  ...\.}.}.|.r.|.|
+00000690: 006a 0264 019c 027c 0366 0253 0064 027c  .j.d...|.f.S.d.|
+000006a0: 0366 0253 0029 037a 4e20 4368 6563 6b73  .f.S.).zN Checks
+000006b0: 2074 6865 2064 6973 7065 6e73 6572 2064   the dispenser d
+000006c0: 6174 6120 6173 2066 6f72 6d61 7474 6564  ata as formatted
+000006d0: 2062 7920 7468 6520 666f 726d 2066 726f   by the form fro
+000006e0: 6d20 7265 6e64 6572 5f65 6469 7420 6675  m render_edit fu
+000006f0: 6e63 7469 6f6e 2029 0272 1400 0000 7215  nction ).r....r.
+00000700: 0000 004e 2903 720a 0000 00da 1463 6865  ...N).r......che
+00000710: 636b 5f64 6973 7065 6e73 6572 5f64 6174  ck_dispenser_dat
+00000720: 6172 2400 0000 2904 7225 0000 0072 2700  ar$...).r%...r'.
+00000730: 0000 da04 6461 7461 da06 6572 726f 7273  ....data..errors
+00000740: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000750: 2f00 0000 3400 0000 7304 0000 0010 021c  /...4...s.......
+00000760: 017a 1c43 6f6e 7465 7374 2e63 6865 636b  .z.Contest.check
+00000770: 5f64 6973 7065 6e73 6572 5f64 6174 6163  _dispenser_datac
+00000780: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000790: 0500 0000 0300 0000 7332 0000 007c 00a0  ........s2...|..
+000007a0: 00a1 0089 0088 0064 0119 0072 1287 0087  .......d...r....
+000007b0: 0166 0264 0264 0384 087c 0244 0083 0153  .f.d.d...|.D...S
+000007c0: 0074 01a0 027c 0088 017c 02a1 0353 0029  .t...|...|...S.)
+000007d0: 044e 721b 0000 0063 0100 0000 0000 0000  .Nr....c........
+000007e0: 0000 0000 0200 0000 0600 0000 1300 0000  ................
+000007f0: 7320 0000 0069 007c 005d 0c7d 017c 0187  s ...i.|.].}.|..
+00000800: 0066 0164 0064 0184 0888 0144 0083 0193  .f.d.d.....D....
+00000810: 0271 0253 0029 0263 0100 0000 0000 0000  .q.S.).c........
+00000820: 0000 0000 0200 0000 0600 0000 1300 0000  ................
+00000830: 731e 0000 0069 007c 005d 0b7d 017c 0174  s....i.|.].}.|.t
+00000840: 0088 0064 0019 0064 0117 0083 0193 0271  ...d...d.......q
+00000850: 0253 0029 0272 1c00 0000 fa01 2f72 0600  .S.).r....../r..
+00000860: 0000 a902 da02 2e30 da06 7461 736b 6964  .......0..taskid
+00000870: 2901 da0c 636f 6e74 6573 745f 6461 7461  )...contest_data
+00000880: 7211 0000 0072 1200 0000 da0a 3c64 6963  r....r......<dic
+00000890: 7463 6f6d 703e 3c00 0000 7302 0000 001e  tcomp><...s.....
+000008a0: 007a 3a43 6f6e 7465 7374 2e67 6574 5f61  .z:Contest.get_a
+000008b0: 6363 6573 7369 6269 6c69 7469 6573 2e3c  ccessibilities.<
+000008c0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+000008d0: 703e 2e3c 6469 6374 636f 6d70 3e72 1100  p>.<dictcomp>r..
+000008e0: 0000 a902 7234 0000 00da 0875 7365 726e  ....r4.....usern
+000008f0: 616d 65a9 0272 3600 0000 da07 7461 736b  ame..r6.....task
+00000900: 6964 7372 1100 0000 7212 0000 0072 3700  idsr....r....r7.
+00000910: 0000 3c00 0000 7302 0000 0020 007a 2f43  ..<...s.... .z/C
+00000920: 6f6e 7465 7374 2e67 6574 5f61 6363 6573  ontest.get_acces
+00000930: 7369 6269 6c69 7469 6573 2e3c 6c6f 6361  sibilities.<loca
+00000940: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2903  ls>.<dictcomp>).
+00000950: da10 6765 745f 636f 6e74 6573 745f 6461  ..get_contest_da
+00000960: 7461 720a 0000 00da 1367 6574 5f61 6363  tar......get_acc
+00000970: 6573 7369 6269 6c69 7469 6573 2903 7225  essibilities).r%
+00000980: 0000 0072 3b00 0000 da09 7573 6572 6e61  ...r;.....userna
+00000990: 6d65 7372 1100 0000 723a 0000 0072 1200  mesr....r:...r..
+000009a0: 0000 723d 0000 0039 0000 0073 0800 0000  ..r=...9...s....
+000009b0: 0801 0801 1401 0e02 7a1b 436f 6e74 6573  ........z.Contes
+000009c0: 742e 6765 745f 6163 6365 7373 6962 696c  t.get_accessibil
+000009d0: 6974 6965 7363 0100 0000 0000 0000 0000  itiesc..........
+000009e0: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+000009f0: 0000 007c 006a 0053 0029 017a 3520 5265  ...|.j.S.).z5 Re
+00000a00: 7475 726e 7320 7468 6520 7365 7474 696e  turns the settin
+00000a10: 6773 206f 6620 7468 6520 636f 6e74 6573  gs of the contes
+00000a20: 7420 666f 7220 7468 6973 2063 6f75 7273  t for this cours
+00000a30: 6520 2901 7224 0000 0029 0172 2500 0000  e ).r$...).r%...
+00000a40: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000a50: 3c00 0000 4000 0000 7302 0000 0006 027a  <...@...s......z
+00000a60: 1843 6f6e 7465 7374 2e67 6574 5f63 6f6e  .Contest.get_con
+00000a70: 7465 7374 5f64 6174 614e 290a da08 5f5f  test_dataN)...__
+00000a80: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000a90: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000aa0: 7220 0000 00da 0b63 6c61 7373 6d65 7468  r .....classmeth
+00000ab0: 6f64 720d 0000 0072 2e00 0000 722f 0000  odr....r....r/..
+00000ac0: 0072 3d00 0000 723c 0000 0072 1100 0000  .r=...r<...r....
+00000ad0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000ae0: 0e00 0000 1f00 0000 7312 0000 0008 0008  ........s.......
+00000af0: 0202 0b0a 0102 030a 0108 0308 050c 0772  ...............r
+00000b00: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000b10: 0000 0000 0002 0000 0043 0000 0073 2800  .........C...s(.
+00000b20: 0000 6401 7400 6a01 6a02 1700 6402 1700  ..d.t.j.j...d...
+00000b30: 7400 6a01 6a02 1700 6403 1700 7400 6a01  t.j.j...d...t.j.
+00000b40: 6a02 1700 6404 1700 5300 2905 7a19 2041  j...d...S.).z. A
+00000b50: 6464 6974 696f 6e61 6c20 4854 4d4c 2068  dditional HTML h
+00000b60: 6561 6465 7273 207a 0c3c 6c69 6e6b 2068  eaders z.<link h
+00000b70: 7265 663d 227a 472f 7374 6174 6963 2f70  ref="zG/static/p
+00000b80: 6c75 6769 6e73 2f63 6f6e 7465 7374 732f  lugins/contests/
+00000b90: 7363 6f72 6562 6f61 7264 2e63 7373 2220  scoreboard.css" 
+00000ba0: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
+00000bb0: 3e3c 7363 7269 7074 2073 7263 3d22 7a48  ><script src="zH
+00000bc0: 2f73 7461 7469 632f 706c 7567 696e 732f  /static/plugins/
+00000bd0: 636f 6e74 6573 7473 2f6a 7175 6572 792e  contests/jquery.
+00000be0: 636f 756e 7464 6f77 6e2e 6d69 6e2e 6a73  countdown.min.js
+00000bf0: 223e 3c2f 7363 7269 7074 3e3c 7363 7269  "></script><scri
+00000c00: 7074 2073 7263 3d22 7a2f 2f73 7461 7469  pt src="z//stati
+00000c10: 632f 706c 7567 696e 732f 636f 6e74 6573  c/plugins/contes
+00000c20: 7473 2f63 6f6e 7465 7374 732e 6a73 223e  ts/contests.js">
+00000c30: 3c2f 7363 7269 7074 3e29 03da 0566 6c61  </script>)...fla
+00000c40: 736b da07 7265 7175 6573 74da 0875 726c  sk..request..url
+00000c50: 5f72 6f6f 7472 1100 0000 7211 0000 0072  _rootr....r....r
+00000c60: 1100 0000 7212 0000 00da 1261 6464 6974  ....r......addit
+00000c70: 696f 6e61 6c5f 6865 6164 6572 7345 0000  ional_headersE..
+00000c80: 0073 1600 0000 0a02 0201 02ff 0602 02fe  .s..............
+00000c90: 0202 02fe 0603 02fd 0203 04fd 7246 0000  ............rF..
+00000ca0: 0063 0200 0000 0000 0000 0000 0000 0700  .c..............
+00000cb0: 0000 0800 0000 4300 0000 7378 0000 007c  ......C...sx...|
+00000cc0: 00a0 00a1 007d 027c 02a0 01a1 0074 02a0  .....}.|.....t..
+00000cd0: 01a1 006b 0273 0e64 0153 007c 02a0 03a1  ...k.s.d.S.|....
+00000ce0: 007d 037c 0364 0219 0072 3a74 04a0 057c  .}.|.d...r:t...|
+00000cf0: 0364 0319 0064 04a1 027d 0474 04a0 057c  .d...d...}.t...|
+00000d00: 0364 0519 0064 04a1 027d 057c 0574 067c  .d...d...}.|.t.|
+00000d10: 0364 0619 0064 078d 0118 007d 067c 016a  .d...d.....}.|.j
+00000d20: 0764 0864 097c 007c 047c 057c 0664 0a8d  .d.d.|.|.|.|.d..
+00000d30: 0653 0064 0153 0029 0b7a 4020 4469 7370  .S.d.S.).z@ Disp
+00000d40: 6c61 7973 2073 6f6d 6520 696e 666f 726d  lays some inform
+00000d50: 6174 696f 6e73 2061 626f 7574 2074 6865  ations about the
+00000d60: 2063 6f6e 7465 7374 206f 6e20 7468 6520   contest on the 
+00000d70: 636f 7572 7365 2070 6167 654e 721b 0000  course pageNr...
+00000d80: 0072 1c00 0000 7216 0000 0072 1d00 0000  .r....r....r....
+00000d90: 721e 0000 0072 1800 0000 7a10 636f 7572  r....r....z.cour
+00000da0: 7365 5f6d 656e 752e 6874 6d6c fa19 6672  se_menu.html..fr
+00000db0: 6f6e 7465 6e64 2f70 6c75 6769 6e73 2f63  ontend/plugins/c
+00000dc0: 6f6e 7465 7374 7329 05da 0f74 656d 706c  ontests)...templ
+00000dd0: 6174 655f 666f 6c64 6572 720f 0000 0072  ate_folderr....r
+00000de0: 1c00 0000 721d 0000 0072 1e00 0000 2908  ....r....r....).
+00000df0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000e00: 3c00 0000 7203 0000 00da 0873 7472 7074  <...r......strpt
+00000e10: 696d 6572 0400 0000 da06 7265 6e64 6572  imer......render
+00000e20: 2907 720f 0000 00da 0f74 656d 706c 6174  ).r......templat
+00000e30: 655f 6865 6c70 6572 7210 0000 0072 3600  e_helperr....r6.
+00000e40: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000e50: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000e60: da0b 636f 7572 7365 5f6d 656e 754d 0000  ..course_menuM..
+00000e70: 0073 1800 0000 0802 1001 0401 0802 0801  .s..............
+00000e80: 1001 1001 1201 0801 0801 06ff 0403 724c  ..............rL
+00000e90: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000ea0: 0000 0000 0200 0000 4000 0000 7318 0000  ........@...s...
+00000eb0: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00000ec0: 0384 005a 0464 0453 0029 05da 1143 6f6e  ...Z.d.S.)...Con
+00000ed0: 7465 7374 5363 6f72 6562 6f61 7264 7a28  testScoreboardz(
+00000ee0: 2044 6973 706c 6179 7320 7468 6520 7363   Displays the sc
+00000ef0: 6f72 6562 6f61 7264 206f 6620 7468 6520  oreboard of the 
+00000f00: 636f 6e74 6573 7420 6302 0000 0000 0000  contest c.......
+00000f10: 0000 0000 0017 0000 000b 0000 0003 0000  ................
+00000f20: 0073 aa03 0000 8800 6a00 a001 7c01 a101  .s......j...|...
+00000f30: 7d02 7c02 a002 a100 7d03 7c03 a003 a100  }.|.....}.|.....
+00000f40: 7404 a003 a100 6b02 7315 7405 8300 8201  t.....k.s.t.....
+00000f50: 7c03 a006 a100 7d04 7c04 6401 1900 7320  |.....}.|.d...s 
+00000f60: 7405 8300 8201 7407 a008 7c04 6402 1900  t.....t...|.d...
+00000f70: 6403 a102 7d05 7407 a008 7c04 6404 1900  d...}.t...|.d...
+00000f80: 6403 a102 7d06 7c06 7409 7c04 6405 1900  d...}.|.t.|.d...
+00000f90: 6406 8d01 1800 7d07 8800 6a0a a00b 7c02  d.....}...j...|.
+00000fa0: a101 7d08 740c 7c02 a00d a100 a00e a100  ..}.t.|.........
+00000fb0: 8301 7d09 8800 6a0f 6a10 a011 6407 7c08  ..}...j.j...d.|.
+00000fc0: 6901 7c01 7c05 7c07 6408 9c02 6409 640a  i.|.|.|.d...d.d.
+00000fd0: 9c04 640b 640c 640b 640b 640b 640d 9c05  ..d.d.d.d.d.d...
+00000fe0: a102 a012 640e 7413 6a14 6602 6701 a101  ....d.t.j.f.g...
+00000ff0: 7d0a 640f 6410 8400 7c09 4400 8301 8901  }.d.d...|.D.....
+00001000: 8700 8701 6602 6411 6410 8408 7c08 4400  ....f.d.d...|.D.
+00001010: 8301 7d0b 6700 7d0c 6412 6410 8400 7c09  ..}.g.}.d.d...|.
+00001020: 4400 8301 7d0d 7c0a 4400 5dbb 7d0e 7c0e  D...}.|.D.].}.|.
+00001030: 6413 1900 4400 5db4 7d0f 7c0e 6414 1900  d...D.].}.|.d...
+00001040: 7c09 7601 7291 7188 7c0f 7c08 7601 7296  |.v.r.q.|.|.v.r.
+00001050: 7188 7c0b 7c0f 1900 6415 1900 7c0e 6414  q.|.|...d...|.d.
+00001060: 1900 1900 7d10 7c10 6416 1900 6417 6b02  ....}.|.d...d.k.
+00001070: 73ac 7c10 6416 1900 6418 6b02 72ad 7188  s.|.d...d.k.r.q.
+00001080: 7c0e 6419 1900 641a 6b02 72f0 7c0d 7c0e  |.d...d.k.r.|.|.
+00001090: 6414 1900 1900 73c4 6418 7c10 6416 3c00  d.....s.d.|.d.<.
+000010a0: 640b 7c0d 7c0e 6414 1900 3c00 6e04 6417  d.|.|.d...<.n.d.
+000010b0: 7c10 6416 3c00 7c10 641b 0500 1900 641c  |.d.<.|.d.....d.
+000010c0: 3700 0300 3c00 7c0e 640e 1900 7c10 641d  7...<.|.d...|.d.
+000010d0: 3c00 7c0e 640e 1900 7409 7c04 641e 1900  <.|.d...t.|.d...
+000010e0: 7c10 641b 1900 641c 1800 1400 641f 8d01  |.d...d.....d...
+000010f0: 1700 7c05 1800 a015 a100 6420 1b00 7c10  ..|.......d ..|.
+00001100: 6421 3c00 6e2f 7c0e 6419 1900 6422 6b02  d!<.n/|.d...d"k.
+00001110: 73fd 7c0e 6419 1900 6423 6b02 9001 720a  s.|.d...d#k...r.
+00001120: 6424 7c10 6416 3c00 7c10 641b 0500 1900  d$|.d.<.|.d.....
+00001130: 641c 3700 0300 3c00 6e15 7c0e 6419 1900  d.7...<.n.|.d...
+00001140: 6425 6b02 9001 721e 6426 7c10 6416 3c00  d%k...r.d&|.d.<.
+00001150: 7c10 641b 0500 1900 641c 3700 0300 3c00  |.d.....d.7...<.
+00001160: 6e01 7188 7c0c a016 7c0b 7c0f 1900 6427  n.q.|...|.|...d'
+00001170: 1900 7c0e 640e 1900 7c10 6416 1900 6417  ..|.d...|.d...d.
+00001180: 6b02 9001 7035 7c10 6416 1900 6418 6b02  k...p5|.d...d.k.
+00001190: 7c0e 6414 1900 6428 9c04 a101 0100 7188  |.d...d(......q.
+000011a0: 7182 7c0c a017 a100 0100 7c0b 4400 5d34  q.|.......|.D.]4
+000011b0: 7d11 6429 6429 6702 7d12 740c 7c0b 7c11  }.d)d)g.}.t.|.|.
+000011c0: 1900 6415 1900 a018 a100 8301 4400 5d1a  ..d.........D.].
+000011d0: 7d13 6421 7c13 7600 9001 726d 7c12 6429  }.d!|.v...rm|.d)
+000011e0: 0500 1900 641c 3700 0300 3c00 7c12 641c  ....d.7...<.|.d.
+000011f0: 0500 1900 7c13 6421 1900 3700 0300 3c00  ....|.d!..7...<.
+00001200: 9001 7154 7419 7c12 8301 7c0b 7c11 1900  ..qTt.|...|.|...
+00001210: 6421 3c00 9001 7144 741a 741b 740c 7c0b  d!<...qDt.t.t.|.
+00001220: a01c a100 8301 642a 642b 8400 642c 8d02  ......d*d+..d,..
+00001230: 8301 7d0b 6400 7d14 6429 7d15 741d 7c0b  ..}.d.}.d)}.t.|.
+00001240: a00e a100 8301 4400 5d34 5c02 7d16 7d11  ......D.]4\.}.}.
+00001250: 7c0b 7c11 1900 6421 1900 7c14 6b03 9001  |.|...d!..|.k...
+00001260: 72b8 7c0b 7c11 1900 6421 1900 7d14 7c16  r.|.|...d!..}.|.
+00001270: 641c 1700 7d15 7c15 7c0b 7c11 1900 642d  d...}.|.|.|...d-
+00001280: 3c00 741e 7c15 8301 7c0b 7c11 1900 642e  <.t.|...|.|...d.
+00001290: 3c00 9001 7191 7c15 7c0b 7c11 1900 642d  <...q.|.|.|...d-
+000012a0: 3c00 642f 7c0b 7c11 1900 642e 3c00 9001  <.d/|.|...d.<...
+000012b0: 7191 8800 6a1f 6a20 6430 6431 7c02 7c05  q...j.j d0d1|.|.
+000012c0: 7c06 7c07 7c09 7c0b 7c0c 6432 8d09 5300  |.|.|.|.|.d2..S.
+000012d0: 2933 4e72 1b00 0000 721c 0000 0072 1600  )3Nr....r....r..
+000012e0: 0000 721d 0000 0072 1e00 0000 7218 0000  ..r....r....r...
+000012f0: 007a 0324 696e 2902 7a04 2467 7465 7a03  .z.$in).z.$gtez.
+00001300: 246c 74da 0464 6f6e 6529 0472 3900 0000  $lt..done).r9...
+00001310: da08 636f 7572 7365 6964 da0c 7375 626d  ..courseid..subm
+00001320: 6974 7465 645f 6f6e da06 7374 6174 7573  itted_on..status
+00001330: 5446 2905 7239 0000 00da 035f 6964 7235  TF).r9....._idr5
+00001340: 0000 00da 0672 6573 756c 7472 5000 0000  .....resultrP...
+00001350: 7250 0000 0063 0100 0000 0000 0000 0000  rP...c..........
+00001360: 0000 0200 0000 0600 0000 5300 0000 7318  ..........S...s.
+00001370: 0000 0069 007c 005d 087d 017c 0164 0064  ...i.|.].}.|.d.d
+00001380: 0164 029c 0293 0271 0253 0029 03da 024e  .d.....q.S.)...N
+00001390: 4172 0100 0000 2902 7251 0000 00da 0574  Ar....).rQ.....t
+000013a0: 7269 6573 7211 0000 0072 3300 0000 7211  riesr....r3...r.
+000013b0: 0000 0072 1100 0000 7212 0000 0072 3700  ...r....r....r7.
+000013c0: 0000 7700 0000 7302 0000 0018 007a 2e43  ..w...s......z.C
+000013d0: 6f6e 7465 7374 5363 6f72 6562 6f61 7264  ontestScoreboard
+000013e0: 2e47 4554 5f41 5554 482e 3c6c 6f63 616c  .GET_AUTH.<local
+000013f0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
+00001400: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00001410: 0000 1300 0000 7326 0000 0069 007c 005d  ......s&...i.|.]
+00001420: 0f7d 017c 0188 006a 00a0 017c 01a1 0174  .}.|...j...|...t
+00001430: 02a0 0388 01a1 0164 009c 0293 0271 0253  .......d.....q.S
+00001440: 0029 0129 02da 046e 616d 65da 0574 6173  .).)...name..tas
+00001450: 6b73 2904 da0c 7573 6572 5f6d 616e 6167  ks)...user_manag
+00001460: 6572 da11 6765 745f 7573 6572 5f72 6561  er..get_user_rea
+00001470: 6c6e 616d 65da 0463 6f70 79da 0864 6565  lname..copy..dee
+00001480: 7063 6f70 7972 3800 0000 a902 7225 0000  pcopyr8.....r%..
+00001490: 005a 0b74 6173 6b5f 7374 6174 7573 7211  .Z.task_statusr.
+000014a0: 0000 0072 1200 0000 7237 0000 0078 0000  ...r....r7...x..
+000014b0: 0073 0200 0000 2600 6301 0000 0000 0000  .s....&.c.......
+000014c0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+000014d0: 0073 1200 0000 6900 7c00 5d05 7d01 7c01  .s....i.|.].}.|.
+000014e0: 6400 9302 7102 5300 2901 4672 1100 0000  d...q.S.).Fr....
+000014f0: 7233 0000 0072 1100 0000 7211 0000 0072  r3...r....r....r
+00001500: 1200 0000 7237 0000 007c 0000 0073 0200  ....r7...|...s..
+00001510: 0000 1200 7239 0000 0072 3500 0000 7257  ....r9...r5...rW
+00001520: 0000 0072 5100 0000 da02 4143 5a03 4143  ...rQ.....ACZ.AC
+00001530: 4672 5300 0000 da07 7375 6363 6573 7372  FrS.....successr
+00001540: 5500 0000 7217 0000 00da 0474 696d 6572  U...r......timer
+00001550: 1f00 0000 2901 da07 6d69 6e75 7465 73e9  ....)...minutes.
+00001560: 3c00 0000 da05 7363 6f72 65da 0666 6169  <.....score..fai
+00001570: 6c65 64da 066b 696c 6c65 645a 0257 41da  led..killedZ.WA.
+00001580: 0774 696d 656f 7574 5a03 544c 4572 5600  .timeoutZ.TLErV.
+00001590: 0000 2904 da04 7573 6572 da04 7768 656e  ..)...user..when
+000015a0: 7253 0000 0072 3500 0000 7201 0000 0063  rS...r5...r....c
+000015b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000015c0: 0300 0000 5300 0000 7322 0000 007c 0064  ....S...s"...|.d
+000015d0: 0119 0064 0219 0064 0319 000b 007c 0064  ...d...d.....|.d
+000015e0: 0119 0064 0219 0064 0119 0066 0253 0029  ...d...d...f.S.)
+000015f0: 044e 7217 0000 0072 6200 0000 7201 0000  .Nr....rb...r...
+00001600: 0072 1100 0000 2901 da01 7472 1100 0000  .r....)...tr....
+00001610: 7211 0000 0072 1200 0000 da08 3c6c 616d  r....r......<lam
+00001620: 6264 613e a900 0000 7302 0000 0022 007a  bda>....s....".z
+00001630: 2c43 6f6e 7465 7374 5363 6f72 6562 6f61  ,ContestScoreboa
+00001640: 7264 2e47 4554 5f41 5554 482e 3c6c 6f63  rd.GET_AUTH.<loc
+00001650: 616c 733e 2e3c 6c61 6d62 6461 3e29 01da  als>.<lambda>)..
+00001660: 036b 6579 da04 7261 6e6b 5a0e 6469 7370  .key..rankZ.disp
+00001670: 6c61 7965 645f 7261 6e6b da00 7a0f 7363  layed_rank..z.sc
+00001680: 6f72 6562 6f61 7264 2e68 746d 6c72 4700  oreboard.htmlrG.
+00001690: 0000 2908 7248 0000 0072 0f00 0000 721c  ..).rH...r....r.
+000016a0: 0000 0072 1d00 0000 721e 0000 0072 5700  ...r....r....rW.
+000016b0: 0000 da07 7265 7375 6c74 73da 0861 6374  ....results..act
+000016c0: 6976 6974 7929 21da 0e63 6f75 7273 655f  ivity)!..course_
+000016d0: 6661 6374 6f72 79da 0a67 6574 5f63 6f75  factory..get_cou
+000016e0: 7273 6572 0c00 0000 720d 0000 0072 0e00  rser....r....r..
+000016f0: 0000 7205 0000 0072 3c00 0000 7203 0000  ..r....r<...r...
+00001700: 0072 4900 0000 7204 0000 0072 5800 0000  .rI...r....rX...
+00001710: da1b 6765 745f 636f 7572 7365 5f72 6567  ..get_course_reg
+00001720: 6973 7465 7265 645f 7573 6572 73da 046c  istered_users..l
+00001730: 6973 74da 0967 6574 5f74 6173 6b73 da04  ist..get_tasks..
+00001740: 6b65 7973 7228 0000 00da 0b73 7562 6d69  keysr(.....submi
+00001750: 7373 696f 6e73 da04 6669 6e64 da04 736f  ssions..find..so
+00001760: 7274 da07 7079 6d6f 6e67 6fda 0941 5343  rt..pymongo..ASC
+00001770: 454e 4449 4e47 da0d 746f 7461 6c5f 7365  ENDING..total_se
+00001780: 636f 6e64 73da 0661 7070 656e 64da 0772  conds..append..r
+00001790: 6576 6572 7365 da06 7661 6c75 6573 da05  everse..values..
+000017a0: 7475 706c 6572 0200 0000 da06 736f 7274  tupler......sort
+000017b0: 6564 da05 6974 656d 73da 0965 6e75 6d65  ed..items..enume
+000017c0: 7261 7465 da03 7374 7272 4b00 0000 724a  rate..strrK...rJ
+000017d0: 0000 0029 1772 2500 0000 724f 0000 0072  ...).r%...rO...r
+000017e0: 0f00 0000 7210 0000 0072 3600 0000 721c  ....r....r6...r.
+000017f0: 0000 0072 1d00 0000 721e 0000 00da 0575  ...r....r......u
+00001800: 7365 7273 7257 0000 005a 0a64 625f 7265  sersrW...Z.db_re
+00001810: 7375 6c74 7372 6d00 0000 726e 0000 00da  sultsrm...rn....
+00001820: 0e74 6173 6b5f 7375 6363 6565 6465 64da  .task_succeeded.
+00001830: 0a73 7562 6d69 7373 696f 6e72 3900 0000  .submissionr9...
+00001840: 7251 0000 0072 6600 0000 7262 0000 0072  rQ...rf...rb...r
+00001850: 3000 0000 da03 6f6c 645a 0c63 7572 7265  0.....oldZ.curre
+00001860: 6e74 5f72 616e 6bda 0363 6964 7211 0000  nt_rank..cidr...
+00001870: 0072 5c00 0000 7212 0000 00da 0847 4554  .r\...r......GET
+00001880: 5f41 5554 4861 0000 0073 ac00 0000 0c01  _AUTHa...s......
+00001890: 0801 1001 0601 0801 0801 0601 1001 1001  ................
+000018a0: 1201 0c02 1001 0802 0601 0201 0801 0201  ................
+000018b0: 04fc 0e05 02fb 0e05 02fb 0e07 1401 0401  ................
+000018c0: 0e03 0801 0c01 0c01 0201 0801 0201 1401  ................
+000018d0: 1801 0201 0c02 0c01 0801 0e01 0802 1001  ................
+000018e0: 0c01 0601 1801 02ff 0202 02fe 0602 0afe  ................
+000018f0: 1a03 0801 1201 0e01 0801 1201 0202 0e01  ................
+00001900: 0601 1801 0601 0afd 02e4 0820 0802 0801  ........... ....
+00001910: 1801 0a01 1001 1401 0480 1401 1c03 0403  ................
+00001920: 0401 1401 1201 0c01 0801 0c01 1401 0c02  ................
+00001930: 1001 0a02 0a01 0401 06fe 7a1a 436f 6e74  ..........z.Cont
+00001940: 6573 7453 636f 7265 626f 6172 642e 4745  estScoreboard.GE
+00001950: 545f 4155 5448 4e29 0572 3f00 0000 7240  T_AUTHN).r?...r@
+00001960: 0000 0072 4100 0000 da07 5f5f 646f 635f  ...rA.....__doc_
+00001970: 5f72 8800 0000 7211 0000 0072 1100 0000  _r....r....r....
+00001980: 7211 0000 0072 1200 0000 724d 0000 005e  r....r....rM...^
+00001990: 0000 0073 0600 0000 0800 0401 0c02 724d  ...s..........rM
+000019a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000019b0: 0000 0000 0200 0000 4000 0000 7328 0000  ........@...s(..
+000019c0: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+000019d0: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
+000019e0: 0784 005a 0664 0853 0029 09da 0c43 6f6e  ...Z.d.S.)...Con
+000019f0: 7465 7374 4164 6d69 6e7a 1f20 436f 6e74  testAdminz. Cont
+00001a00: 6573 7420 7365 7474 696e 6773 2066 6f72  est settings for
+00001a10: 2061 2063 6f75 7273 6520 6303 0000 0000   a course c.....
+00001a20: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00001a30: 0000 0073 3200 0000 7c00 6a00 a001 7c01  ...s2...|.j...|.
+00001a40: a002 a100 a101 7d03 7c02 7c03 6401 1900  ......}.|.|.d...
+00001a50: 6402 3c00 7c00 6a00 a003 7c01 a002 a100  d.<.|.j...|.....
+00001a60: 7c03 a102 0100 6403 5300 2904 7a2b 2053  |.....d.S.).z+ S
+00001a70: 6176 6573 2075 7064 6174 6564 2063 6f6e  aves updated con
+00001a80: 7465 7374 2064 6174 6120 666f 7220 7468  test data for th
+00001a90: 6520 636f 7572 7365 2072 2700 0000 7215  e course r'...r.
+00001aa0: 0000 004e 2904 726f 0000 00da 1d67 6574  ...N).ro.....get
+00001ab0: 5f63 6f75 7273 655f 6465 7363 7269 7074  _course_descript
+00001ac0: 6f72 5f63 6f6e 7465 6e74 720d 0000 00da  or_contentr.....
+00001ad0: 2075 7064 6174 655f 636f 7572 7365 5f64   update_course_d
+00001ae0: 6573 6372 6970 746f 725f 636f 6e74 656e  escriptor_conten
+00001af0: 7429 0472 2500 0000 720f 0000 0072 3600  t).r%...r....r6.
+00001b00: 0000 da0e 636f 7572 7365 5f63 6f6e 7465  ....course_conte
+00001b10: 6e74 7211 0000 0072 1100 0000 7212 0000  ntr....r....r...
+00001b20: 00da 1173 6176 655f 636f 6e74 6573 745f  ...save_contest_
+00001b30: 6461 7461 c000 0000 7306 0000 0010 020c  data....s.......
+00001b40: 0116 017a 1e43 6f6e 7465 7374 4164 6d69  ...z.ContestAdmi
+00001b50: 6e2e 7361 7665 5f63 6f6e 7465 7374 5f64  n.save_contest_d
+00001b60: 6174 6163 0200 0000 0000 0000 0000 0000  atac............
+00001b70: 0600 0000 0800 0000 4300 0000 7350 0000  ........C...sP..
+00001b80: 007c 006a 007c 0164 0164 028d 025c 027d  .|.j.|.d.d...\.}
+00001b90: 027d 037c 02a0 01a1 007d 047c 04a0 02a1  .}.|.....}.|....
+00001ba0: 0074 03a0 02a1 006b 0273 1874 0483 0082  .t.....k.s.t....
+00001bb0: 017c 04a0 05a1 007d 057c 006a 066a 0764  .|.....}.|.j.j.d
+00001bc0: 0364 047c 027c 0564 0564 0164 068d 0653  .d.|.|.d.d.d...S
+00001bd0: 0029 077a 2620 4745 5420 7265 7175 6573  .).z& GET reques
+00001be0: 743a 2073 696d 706c 7920 6469 7370 6c61  t: simply displa
+00001bf0: 7920 7468 6520 666f 726d 2046 a901 da0f  y the form F....
+00001c00: 616c 6c6f 775f 616c 6c5f 7374 6166 66fa  allow_all_staff.
+00001c10: 0a61 646d 696e 2e68 746d 6c72 4700 0000  .admin.htmlrG...
+00001c20: 4ea9 0572 4800 0000 720f 0000 0072 3000  N..rH...r....r0.
+00001c30: 0000 7231 0000 00da 0573 6176 6564 2908  ..r1.....saved).
+00001c40: da1b 6765 745f 636f 7572 7365 5f61 6e64  ..get_course_and
+00001c50: 5f63 6865 636b 5f72 6967 6874 7372 0c00  _check_rightsr..
+00001c60: 0000 720d 0000 0072 0e00 0000 7205 0000  ..r....r....r...
+00001c70: 0072 3c00 0000 724b 0000 0072 4a00 0000  .r<...rK...rJ...
+00001c80: 2906 7225 0000 0072 4f00 0000 720f 0000  ).r%...rO...r...
+00001c90: 00da 025f 5f72 1000 0000 7236 0000 0072  ...__r....r6...r
+00001ca0: 1100 0000 7211 0000 0072 1200 0000 7288  ....r....r....r.
+00001cb0: 0000 00c6 0000 0073 1000 0000 1202 0801  .......s........
+00001cc0: 1001 0601 0801 0c01 0601 06ff 7a15 436f  ............z.Co
+00001cd0: 6e74 6573 7441 646d 696e 2e47 4554 5f41  ntestAdmin.GET_A
+00001ce0: 5554 4863 0200 0000 0000 0000 0000 0000  UTHc............
+00001cf0: 0a00 0000 0800 0000 4300 0000 73ba 0100  ........C...s...
+00001d00: 007c 006a 007c 0164 0164 028d 025c 027d  .|.j.|.d.d...\.}
+00001d10: 027d 037c 02a0 01a1 007d 047c 04a0 02a1  .}.|.....}.|....
+00001d20: 0074 03a0 02a1 006b 0273 1874 0483 0082  .t.....k.s.t....
+00001d30: 017c 04a0 05a1 007d 0574 066a 076a 087d  .|.....}.t.j.j.}
+00001d40: 0667 007d 077a 8d7c 06a0 0964 0364 04a1  .g.}.z.|...d.d..
+00001d50: 0264 056b 027c 0564 033c 007c 0664 0619  .d.k.|.d.<.|.d..
+00001d60: 007c 0564 063c 007c 0664 0719 007c 0564  .|.d.<.|.d...|.d
+00001d70: 073c 007a 0a74 0aa0 0b7c 0564 0619 0064  .<.z.t...|.d...d
+00001d80: 08a1 027d 0857 006e 0901 0001 0001 007c  ...}.W.n.......|
+00001d90: 07a0 0c64 09a1 0101 0059 007a 0a74 0aa0  ...d.....Y.z.t..
+00001da0: 0b7c 0564 0719 0064 08a1 027d 0957 006e  .|.d...d...}.W.n
+00001db0: 0901 0001 0001 007c 07a0 0c64 0aa1 0101  .......|...d....
+00001dc0: 0059 0074 0d7c 0783 0164 0b6b 0272 707c  .Y.t.|...d.k.rp|
+00001dd0: 087c 096b 0572 707c 07a0 0c64 0ca1 0101  .|.k.rp|...d....
+00001de0: 007a 1574 0e7c 0664 0d19 0083 017c 0564  .z.t.|.d.....|.d
+00001df0: 0d3c 007c 0564 0d19 0064 0b6b 0072 847c  .<.|.d...d.k.r.|
+00001e00: 07a0 0c64 0ea1 0101 0057 006e 0901 0001  ...d.....W.n....
+00001e10: 0001 007c 07a0 0c64 0fa1 0101 0059 007a  ...|...d.....Y.z
+00001e20: 1574 0e7c 0664 1019 0083 017c 0564 103c  .t.|.d.....|.d.<
+00001e30: 007c 0564 1019 0064 0b6b 0072 a37c 07a0  .|.d...d.k.r.|..
+00001e40: 0c64 11a1 0101 0057 006e 0901 0001 0001  .d.....W.n......
+00001e50: 007c 07a0 0c64 12a1 0101 0059 0057 006e  .|...d.....Y.W.n
+00001e60: 0901 0001 0001 007c 07a0 0c64 13a1 0101  .......|...d....
+00001e70: 0059 0074 0d7c 0783 0164 0b6b 0272 d17c  .Y.t.|...d.k.r.|
+00001e80: 00a0 0f7c 027c 05a1 0201 007c 006a 106a  ...|.|.....|.j.j
+00001e90: 1164 1464 157c 027c 0564 1664 1764 188d  .d.d.|.|.d.d.d..
+00001ea0: 0653 007c 006a 106a 1164 1464 157c 027c  .S.|.j.j.d.d.|.|
+00001eb0: 057c 0764 0164 188d 0653 0029 197a 2320  .|.d.d...S.).z# 
+00001ec0: 504f 5354 2072 6571 7565 7374 3a20 7570  POST request: up
+00001ed0: 6461 7465 2074 6865 2073 6574 7469 6e67  date the setting
+00001ee0: 7320 4672 8f00 0000 721b 0000 00da 0130  s Fr....r......0
+00001ef0: da01 3172 1c00 0000 721d 0000 0072 1600  ..1r....r....r..
+00001f00: 0000 7a12 496e 7661 6c69 6420 7374 6172  ..z.Invalid star
+00001f10: 7420 6461 7465 7a10 496e 7661 6c69 6420  t datez.Invalid 
+00001f20: 656e 6420 6461 7465 7201 0000 007a 2453  end dater....z$S
+00001f30: 7461 7274 2064 6174 6520 7368 6f75 6c64  tart date should
+00001f40: 2062 6520 6265 666f 7265 2065 6e64 2064   be before end d
+00001f50: 6174 6572 1e00 0000 7a42 496e 7661 6c69  ater....zBInvali
+00001f60: 6420 6e75 6d62 6572 206f 6620 686f 7572  d number of hour
+00001f70: 7320 666f 7220 7468 6520 626c 6163 6b6f  s for the blacko
+00001f80: 7574 3a20 7368 6f75 6c64 2062 6520 6772  ut: should be gr
+00001f90: 6561 7465 7220 7468 616e 2030 7a28 496e  eater than 0z(In
+00001fa0: 7661 6c69 6420 6e75 6d62 6572 206f 6620  valid number of 
+00001fb0: 686f 7572 7320 666f 7220 7468 6520 626c  hours for the bl
+00001fc0: 6163 6b6f 7574 721f 0000 007a 4349 6e76  ackoutr....zCInv
+00001fd0: 616c 6964 206e 756d 6265 7220 6f66 206d  alid number of m
+00001fe0: 696e 7574 6573 2066 6f72 2074 6865 2070  inutes for the p
+00001ff0: 656e 616c 7479 3a20 7368 6f75 6c64 2062  enalty: should b
+00002000: 6520 6772 6561 7465 7220 7468 616e 2030  e greater than 0
+00002010: 7a29 496e 7661 6c69 6420 6e75 6d62 6572  z)Invalid number
+00002020: 206f 6620 6d69 6e75 7465 7320 666f 7220   of minutes for 
+00002030: 7468 6520 7065 6e61 6c74 797a 1d55 7365  the penaltyz.Use
+00002040: 7220 7265 7475 726e 6564 2061 6e20 696e  r returned an in
+00002050: 7661 6c69 6420 666f 726d 7291 0000 0072  valid formr....r
+00002060: 4700 0000 4e54 7292 0000 0029 1272 9400  G...NTr....).r..
+00002070: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00002080: 0072 0500 0000 723c 0000 0072 4300 0000  .r....r<...rC...
+00002090: 7244 0000 00da 0466 6f72 6d72 2100 0000  rD.....formr!...
+000020a0: 7203 0000 0072 4900 0000 727b 0000 00da  r....rI...r{....
+000020b0: 036c 656e da03 696e 7472 8e00 0000 724b  .len..intr....rK
+000020c0: 0000 0072 4a00 0000 290a 7225 0000 0072  ...rJ...).r%...r
+000020d0: 4f00 0000 720f 0000 0072 9500 0000 7210  O...r....r....r.
+000020e0: 0000 0072 3600 0000 da08 6e65 775f 6461  ...r6.....new_da
+000020f0: 7461 7231 0000 0072 1c00 0000 721d 0000  tar1...r....r...
+00002100: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00002110: da09 504f 5354 5f41 5554 48d0 0000 0073  ..POST_AUTH....s
+00002120: 5e00 0000 1202 0801 1001 0601 0801 0802  ^...............
+00002130: 0401 0201 1401 0c01 0c01 0202 1401 0601  ................
+00002140: 0c01 0202 1401 0601 0c01 0c02 0801 0a01  ................
+00002150: 0202 1001 0c01 0a01 0480 0601 0c01 0202  ................
+00002160: 1001 0c01 0a01 0480 0601 0c01 0480 0601  ................
+00002170: 0c01 0c02 0c01 0c01 0601 06ff 0c03 0601  ................
+00002180: 06ff 7a16 436f 6e74 6573 7441 646d 696e  ..z.ContestAdmin
+00002190: 2e50 4f53 545f 4155 5448 4e29 0772 3f00  .POST_AUTHN).r?.
+000021a0: 0000 7240 0000 0072 4100 0000 7289 0000  ..r@...rA...r...
+000021b0: 0072 8e00 0000 7288 0000 0072 9c00 0000  .r....r....r....
+000021c0: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+000021d0: 1200 0000 728a 0000 00bd 0000 0073 0a00  ....r........s..
+000021e0: 0000 0800 0401 0802 0806 0c0a 728a 0000  ............r...
+000021f0: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
+00002200: 0000 0600 0000 4300 0000 7356 0000 007c  ......C...sV...|
+00002210: 00a0 0064 0174 01a0 0264 02a1 01a1 0201  ...d.t...d......
+00002220: 007c 00a0 0064 0374 03a0 0264 04a1 01a1  .|...d.t...d....
+00002230: 0201 007c 00a0 0464 0574 05a1 0201 007c  ...|...d.t.....|
+00002240: 00a0 0464 0674 06a1 0201 007c 00a0 0464  ...d.t.....|...d
+00002250: 0774 07a1 0201 007c 01a0 0874 09a1 0101  .t.....|...t....
+00002260: 0064 0853 0029 097a b60a 2020 2020 2020  .d.S.).z..      
+00002270: 2020 496e 6974 2074 6865 2063 6f6e 7465    Init the conte
+00002280: 7374 2070 6c75 6769 6e2e 0a20 2020 2020  st plugin..     
+00002290: 2020 2041 7661 696c 6162 6c65 2063 6f6e     Available con
+000022a0: 6669 6775 7261 7469 6f6e 3a0a 2020 2020  figuration:.    
+000022b0: 2020 2020 3a3a 0a0a 2020 2020 2020 2020      ::..        
+000022c0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000022d0: 2020 2020 2020 2270 6c75 6769 6e5f 6d6f        "plugin_mo
+000022e0: 6475 6c65 223a 2022 696e 6769 6e69 6f75  dule": "inginiou
+000022f0: 732e 6672 6f6e 7465 6e64 2e70 6c75 6769  s.frontend.plugi
+00002300: 6e73 2e63 6f6e 7465 7374 7322 0a20 2020  ns.contests".   
+00002310: 2020 2020 2020 2020 207d 0a20 2020 207a           }.    z
+00002320: 132f 636f 6e74 6573 742f 3c63 6f75 7273  ./contest/<cours
+00002330: 6569 643e 5a11 636f 6e74 6573 7473 636f  eid>Z.contestsco
+00002340: 7265 626f 6172 647a 192f 6164 6d69 6e2f  reboardz./admin/
+00002350: 3c63 6f75 7273 6569 643e 2f63 6f6e 7465  <courseid>/conte
+00002360: 7374 5a0c 636f 6e74 6573 7461 646d 696e  stZ.contestadmin
+00002370: da11 636f 7572 7365 5f61 646d 696e 5f6d  ..course_admin_m
+00002380: 656e 75da 0b68 6561 6465 725f 6874 6d6c  enu..header_html
+00002390: 724c 0000 004e 290a da08 6164 645f 7061  rL...N)...add_pa
+000023a0: 6765 724d 0000 00da 0761 735f 7669 6577  gerM.....as_view
+000023b0: 728a 0000 00da 0861 6464 5f68 6f6f 6b72  r......add_hookr
+000023c0: 1300 0000 7246 0000 0072 4c00 0000 da12  ....rF...rL.....
+000023d0: 6164 645f 7461 736b 5f64 6973 7065 6e73  add_task_dispens
+000023e0: 6572 720e 0000 0029 04da 0e70 6c75 6769  err....)...plugi
+000023f0: 6e5f 6d61 6e61 6765 7272 6f00 0000 da06  n_managerro.....
+00002400: 636c 6965 6e74 da06 636f 6e66 6967 7211  client..configr.
+00002410: 0000 0072 1100 0000 7212 0000 00da 0469  ...r....r......i
+00002420: 6e69 7406 0100 0073 0c00 0000 120b 1201  nit....s........
+00002430: 0c01 0c01 0c01 0e01 72a6 0000 0029 1972  ........r....).r
+00002440: 8900 0000 725a 0000 00da 0b63 6f6c 6c65  ....rZ.....colle
+00002450: 6374 696f 6e73 7202 0000 0072 0300 0000  ctionsr....r....
+00002460: 7204 0000 0072 7800 0000 7243 0000 005a  r....rx...rC...Z
+00002470: 1377 6572 6b7a 6575 672e 6578 6365 7074  .werkzeug.except
+00002480: 696f 6e73 7205 0000 00da 2269 6e67 696e  ionsr....."ingin
+00002490: 696f 7573 2e66 726f 6e74 656e 642e 6163  ious.frontend.ac
+000024a0: 6365 7373 6962 6c65 5f74 696d 6572 0700  cessible_timer..
+000024b0: 0000 da2b 696e 6769 6e69 6f75 732e 6672  ...+inginious.fr
+000024c0: 6f6e 7465 6e64 2e70 6167 6573 2e63 6f75  ontend.pages.cou
+000024d0: 7273 655f 6164 6d69 6e2e 7574 696c 7372  rse_admin.utilsr
+000024e0: 0800 0000 da1e 696e 6769 6e69 6f75 732e  ......inginious.
+000024f0: 6672 6f6e 7465 6e64 2e70 6167 6573 2e75  frontend.pages.u
+00002500: 7469 6c73 7209 0000 00da 2669 6e67 696e  tilsr.....&ingin
+00002510: 696f 7573 2e66 726f 6e74 656e 642e 7461  ious.frontend.ta
+00002520: 736b 5f64 6973 7065 6e73 6572 732e 746f  sk_dispensers.to
+00002530: 6372 0a00 0000 7213 0000 0072 0e00 0000  cr....r....r....
+00002540: 7246 0000 0072 4c00 0000 724d 0000 0072  rF...rL...rM...r
+00002550: 8a00 0000 72a6 0000 0072 1100 0000 7211  ....r....r....r.
+00002560: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
+00002570: 6d6f 6475 6c65 3e01 0000 0073 2400 0000  module>....s$...
+00002580: 0405 0802 0c01 1001 0802 0801 0c02 0c01  ................
+00002590: 0c01 0c01 0c01 0803 1009 0826 0808 1011  ...........&....
+000025a0: 105f 0c49                                ._.I
```

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/admin.html` & `INGInious-0.8.7/inginious/frontend/plugins/contests/admin.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/course_menu.html` & `INGInious-0.8.7/inginious/frontend/plugins/contests/course_menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/contests/scoreboard.html` & `INGInious-0.8.7/inginious/frontend/plugins/contests/scoreboard.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/demo/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/git_repo/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/git_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/ltibestsubmission/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/main.html` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/main.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/scoreboard.html` & `INGInious-0.8.7/inginious/frontend/plugins/scoreboard/scoreboard.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/simple_grader/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/simple_grader/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/task_editor_hook_example/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html` & `INGInious-0.8.7/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/json_reader.py` & `INGInious-0.8.7/inginious/frontend/plugins/task_file_readers/json_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/__init__.py` & `INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html` & `INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html` & `INGInious-0.8.7/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/INGInious.css` & `INGInious-0.8.7/inginious/frontend/static/css/INGInious.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/INGInious.less` & `INGInious-0.8.7/inginious/frontend/static/css/INGInious.less`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/bootstrap-datetimepicker.min.css` & `INGInious-0.8.7/inginious/frontend/static/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/bootstrap.min.css` & `INGInious-0.8.7/inginious/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/codemirror.css` & `INGInious-0.8.7/inginious/frontend/static/css/codemirror.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/common.less` & `INGInious-0.8.7/inginious/frontend/static/css/common.less`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/font-awesome.min.css` & `INGInious-0.8.7/inginious/frontend/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/lti.css` & `INGInious-0.8.7/inginious/frontend/static/css/lti.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/css/selectize.css` & `INGInious-0.8.7/inginious/frontend/static/css/selectize.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/FontAwesome.otf` & `INGInious-0.8.7/inginious/frontend/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.eot` & `INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.svg` & `INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.ttf` & `INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff` & `INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff2` & `INGInious-0.8.7/inginious/frontend/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot` & `INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg` & `INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf` & `INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff` & `INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2` & `INGInious-0.8.7/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-114x114.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-120x120.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-144x144.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-152x152.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-57x57.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-60x60.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-72x72.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-76x76.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-precomposed.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon.png` & `INGInious-0.8.7/inginious/frontend/static/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon-160x160.png` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon-160x160.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon-16x16.png` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon-196x196.png` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon-196x196.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon-32x32.png` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon-96x96.png` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/favicon.ico` & `INGInious-0.8.7/inginious/frontend/static/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/google-icon.svg` & `INGInious-0.8.7/inginious/frontend/static/icons/google-icon.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/mstile-144x144.png` & `INGInious-0.8.7/inginious/frontend/static/icons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/mstile-150x150.png` & `INGInious-0.8.7/inginious/frontend/static/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x150.png` & `INGInious-0.8.7/inginious/frontend/static/icons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x310.png` & `INGInious-0.8.7/inginious/frontend/static/icons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/mstile-70x70.png` & `INGInious-0.8.7/inginious/frontend/static/icons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/wb.png` & `INGInious-0.8.7/inginious/frontend/static/icons/wb.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/icons/wb.svg` & `INGInious-0.8.7/inginious/frontend/static/icons/wb.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/header.png` & `INGInious-0.8.7/inginious/frontend/static/images/header.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/inginious_full.svg` & `INGInious-0.8.7/inginious/frontend/static/images/inginious_full.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/inginious_full_logo_only.svg` & `INGInious-0.8.7/inginious/frontend/static/images/inginious_full_logo_only.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/inginious_horiz.svg` & `INGInious-0.8.7/inginious/frontend/static/images/inginious_horiz.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/inginious_vert.svg` & `INGInious-0.8.7/inginious/frontend/static/images/inginious_vert.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/logo.png` & `INGInious-0.8.7/inginious/frontend/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/images/logo_maintenance.png` & `INGInious-0.8.7/inginious/frontend/static/images/logo_maintenance.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/admin.js` & `INGInious-0.8.7/inginious/frontend/static/js/admin.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/all-minified.js` & `INGInious-0.8.7/inginious/frontend/static/js/all-minified.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/audiences.js` & `INGInious-0.8.7/inginious/frontend/static/js/audiences.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/checked-list-group.js` & `INGInious-0.8.7/inginious/frontend/static/js/checked-list-group.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/LICENSE` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/codemirror.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/apl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/apl/apl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/apl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asn.1/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/asterisk/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/clike.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/scala.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clike/scala.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/clojure/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cmake/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cobol/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/crystal/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/css.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/gss.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/less.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less_test.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/less_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/scss.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss_test.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/css/scss_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/cypher/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/d.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/d/d.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/d/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/dart.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dart/dart.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dart/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/diff.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/diff/diff.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/diff/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/django.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/django/django.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/django/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dtd/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/dylan/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ebnf/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ecl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/eiffel/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/elm.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/elm/elm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/elm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/erlang/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/factor.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/factor/factor.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/factor/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fcl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/forth.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/forth/forth.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/forth/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/fortran/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/gas.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gas/gas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gfm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/gherkin/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/go.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/go/go.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/go/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/groovy/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/haml.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haml/haml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/handlebars/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/haxe/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/http.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/http/http.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/http/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/idl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/idl/idl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/idl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jinja2/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jsx/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/julia/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/julia.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/julia/julia.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/livescript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/lua/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/lua.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/lua/lua.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/markdown/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mathematica/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mbox/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/meta.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/meta.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mirc/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mllike/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/modelica/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mumps/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nginx/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nsis/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ntriples/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/octave/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/octave.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/octave/octave.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/oz/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/oz.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/oz/oz.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pascal/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pegjs/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/perl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/perl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/perl/perl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/php/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/php.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/php/php.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pig/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/pig.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pig/pig.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/powershell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/properties/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/properties.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/properties/properties.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/protobuf/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pug/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/pug.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/pug/pug.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/puppet/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/python.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/q/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/q.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/q/q.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/r/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/r.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/r/r.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rst/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/rst.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rst/rst.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ruby/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rust/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/rust.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/rust/rust.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/sas.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sas/sas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sass/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/sass.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sass/sass.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/scheme/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/shell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/shell.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/shell/shell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sieve/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/slim/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/slim.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/slim/slim.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smarty/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/solr/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/solr.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/solr/solr.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/soy/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/soy.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/soy/soy.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sparql/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sql/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/sql.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/sql/sql.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stex/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/stex.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stex/stex.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stylus/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/swift/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/swift.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/swift/swift.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tcl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/textile/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/textile.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/textile/textile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/toml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/toml.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/toml/toml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tornado/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/troff/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/troff.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/troff/troff.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/turtle/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/twig/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/twig.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/twig/twig.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vb/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/vb.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vb/vb.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vbscript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/velocity/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/verilog/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vhdl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vue/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/vue.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/vue/vue.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/webidl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/xml.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xquery/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yacas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/index.html` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/z80/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/z80.js` & `INGInious-0.8.7/inginious/frontend/static/js/codemirror/mode/z80/z80.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/common.js` & `INGInious-0.8.7/inginious/frontend/static/js/common.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/groups.js` & `INGInious-0.8.7/inginious/frontend/static/js/groups.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/Sortable.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/chart.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/chart.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.form.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/moment.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/moment.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/popper.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/popper.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/selectize.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/selectize.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/libs/sentry-io-bundle.min.js` & `INGInious-0.8.7/inginious/frontend/static/js/libs/sentry-io-bundle.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/studio.js` & `INGInious-0.8.7/inginious/frontend/static/js/studio.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/task.js` & `INGInious-0.8.7/inginious/frontend/static/js/task.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/task_dispensers.js` & `INGInious-0.8.7/inginious/frontend/static/js/task_dispensers.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/js/webapp.js` & `INGInious-0.8.7/inginious/frontend/static/js/webapp.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/plugins/contests/contests.js` & `INGInious-0.8.7/inginious/frontend/static/plugins/contests/contests.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/plugins/contests/jquery.countdown.min.js` & `INGInious-0.8.7/inginious/frontend/static/plugins/contests/jquery.countdown.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/static/plugins/contests/scoreboard.css` & `INGInious-0.8.7/inginious/frontend/static/plugins/contests/scoreboard.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/submission_manager.py` & `INGInious-0.8.7/inginious/frontend/submission_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_dispensers/__init__.py` & `INGInious-0.8.7/inginious/frontend/task_dispensers/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_dispensers/combinatory_test.py` & `INGInious-0.8.7/inginious/frontend/task_dispensers/combinatory_test.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_dispensers/toc.py` & `INGInious-0.8.7/inginious/frontend/task_dispensers/toc.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_dispensers/util.py` & `INGInious-0.8.7/inginious/frontend/task_dispensers/util.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_factory.py` & `INGInious-0.8.7/inginious/frontend/task_factory.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/task_problems.py` & `INGInious-0.8.7/inginious/frontend/task_problems.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tasks.py` & `INGInious-0.8.7/inginious/frontend/tasks.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/template_helper.py` & `INGInious-0.8.7/inginious/frontend/template_helper.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/admin/admin_users.html` & `INGInious-0.8.7/inginious/frontend/templates/admin/admin_users.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/auth.html` & `INGInious-0.8.7/inginious/frontend/templates/auth.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course.html` & `INGInious-0.8.7/inginious/frontend/templates/course.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/audience_edit.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/audience_edit.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/danger_zone.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/danger_zone.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/basic.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/basic.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/environment.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/environment.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/files.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/files.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/menu.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/settings.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/settings.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/stats.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/stats.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_info.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/student_info.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/student_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list_table.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/student_list_table.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/submission.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/submission.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/submissions.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions_query.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/submissions_query.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/code.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/file.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/file.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/match.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/match.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/tags.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/tags.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_config.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section_config.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_list.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/toc.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/toc.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/util.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_edit.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_edit.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_list.html` & `INGInious-0.8.7/inginious/frontend/templates/course_admin/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_register.html` & `INGInious-0.8.7/inginious/frontend/templates/course_register.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/course_unavailable.html` & `INGInious-0.8.7/inginious/frontend/templates/course_unavailable.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/courselist.html` & `INGInious-0.8.7/inginious/frontend/templates/courselist.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/group.html` & `INGInious-0.8.7/inginious/frontend/templates/group.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/internalerror.html` & `INGInious-0.8.7/inginious/frontend/templates/internalerror.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/layout.html` & `INGInious-0.8.7/inginious/frontend/templates/layout.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/lti_bind.html` & `INGInious-0.8.7/inginious/frontend/templates/lti_bind.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/lti_login.html` & `INGInious-0.8.7/inginious/frontend/templates/lti_login.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/maintenance.html` & `INGInious-0.8.7/inginious/frontend/templates/maintenance.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/marketplace.html` & `INGInious-0.8.7/inginious/frontend/templates/marketplace.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/marketplace_course.html` & `INGInious-0.8.7/inginious/frontend/templates/marketplace_course.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/mycourses.html` & `INGInious-0.8.7/inginious/frontend/templates/mycourses.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/preferences/bindings.html` & `INGInious-0.8.7/inginious/frontend/templates/preferences/bindings.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/preferences/delete.html` & `INGInious-0.8.7/inginious/frontend/templates/preferences/delete.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/preferences/profile.html` & `INGInious-0.8.7/inginious/frontend/templates/preferences/profile.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/queue.html` & `INGInious-0.8.7/inginious/frontend/templates/queue.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/register.html` & `INGInious-0.8.7/inginious/frontend/templates/register.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/signin_button.html` & `INGInious-0.8.7/inginious/frontend/templates/signin_button.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/task.html` & `INGInious-0.8.7/inginious/frontend/templates/task.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/task_dispensers/task_list.html` & `INGInious-0.8.7/inginious/frontend/templates/task_dispensers/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/task_dispensers/toc.html` & `INGInious-0.8.7/inginious/frontend/templates/task_dispensers/toc.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/task_unavailable.html` & `INGInious-0.8.7/inginious/frontend/templates/task_unavailable.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/tasks/code.html` & `INGInious-0.8.7/inginious/frontend/templates/tasks/code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/tasks/file.html` & `INGInious-0.8.7/inginious/frontend/templates/tasks/file.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/tasks/multiple_choice.html` & `INGInious-0.8.7/inginious/frontend/templates/tasks/multiple_choice.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/tasks/single_line_code.html` & `INGInious-0.8.7/inginious/frontend/templates/tasks/single_line_code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/templates/unregister_modal.html` & `INGInious-0.8.7/inginious/frontend/templates/unregister_modal.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/SeleniumFormatter.js` & `INGInious-0.8.7/inginious/frontend/tests/SeleniumFormatter.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/SeleniumTest.py` & `INGInious-0.8.7/inginious/frontend/tests/SeleniumTest.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestCourse.py` & `INGInious-0.8.7/inginious/frontend/tests/TestCourse.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestLogin.py` & `INGInious-0.8.7/inginious/frontend/tests/TestLogin.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestParsableText.py` & `INGInious-0.8.7/inginious/frontend/tests/TestParsableText.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestPluginManager.py` & `INGInious-0.8.7/inginious/frontend/tests/TestPluginManager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestTask.py` & `INGInious-0.8.7/inginious/frontend/tests/TestTask.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestTaskDisplay.py` & `INGInious-0.8.7/inginious/frontend/tests/TestTaskDisplay.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/TestTaskSubmission.py` & `INGInious-0.8.7/inginious/frontend/tests/TestTaskSubmission.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/task.yaml` & `INGInious-0.8.7/inginious/frontend/tests/tasks/test/task1/task.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/task.yaml` & `INGInious-0.8.7/inginious/frontend/tests/tasks/test2/task3/task.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/user_manager.py` & `INGInious-0.8.7/inginious/frontend/user_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious/frontend/webdav.py` & `INGInious-0.8.7/inginious/frontend/webdav.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-agent-docker` & `INGInious-0.8.7/inginious-agent-docker`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-agent-mcq` & `INGInious-0.8.7/inginious-agent-mcq`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-autotest` & `INGInious-0.8.7/inginious-autotest`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-backend` & `INGInious-0.8.7/inginious-backend`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-install` & `INGInious-0.8.7/inginious-install`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-webapp` & `INGInious-0.8.7/inginious-webapp`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/inginious-webdav` & `INGInious-0.8.7/inginious-webdav`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/setup.py` & `INGInious-0.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import sys
 import os
 from setuptools import setup, find_packages
 
 install_requires = [
     "docker>=3.0",
+    "requests < 2.29.0",  # TODO: remove when https://github.com/docker/docker-py/issues/3113 is closed.
     "docutils>=0.14",
     "pymongo>=3.2.2",
     "PyYAML>=3.11",
     "Jinja2 >= 2.10",
     "lti>=0.9.0",
     "oauth2>=1.9.0.post1",
     "httplib2>=0.9",
@@ -22,15 +23,15 @@
     "pyzmq >= 15.3.0",
     "natsort >= 5.0.1",
     "psutil >= 4.4.2",
     "zipstream >= 1.1.4",
     "WsgiDAV >= 3.0.0",
     "Werkzeug >= 1.0.0",
     "itsdangerous >= 1.1.0",
-    "Flask >= 1.1.0",
+    "Flask >= 2.0.0",
     "Flask-Mail >= 0.9.1",
     "importlib_metadata >= 3.7.0",
     'dataclasses >= 0.8; python_version < "3.7.0"',
     "pytidylib>=0.2.4",
     "sphinx-autodoc-typehints>=1.12.0",
 ]
```

### Comparing `INGInious-0.8.6/utils/container_update/inginious-container-update` & `INGInious-0.8.7/utils/container_update/inginious-container-update`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/utils/database_updater/inginious-database-update` & `INGInious-0.8.7/utils/database_updater/inginious-database-update`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/utils/minify/Gruntfile.js` & `INGInious-0.8.7/utils/minify/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/utils/minify/watchers.xml` & `INGInious-0.8.7/utils/minify/watchers.xml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.6/utils/sync/inginious-synchronize` & `INGInious-0.8.7/utils/sync/inginious-synchronize`

 * *Files identical despite different names*

