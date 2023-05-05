# Comparing `tmp/java-test-genie-0.1.1.tar.gz` & `tmp/java-test-genie-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java-test-genie-0.1.1.tar", last modified: Wed May  3 18:04:19 2023, max compression
+gzip compressed data, was "java-test-genie-1.0.tar", last modified: Fri May  5 13:55:31 2023, max compression
```

## Comparing `java-test-genie-0.1.1.tar` & `java-test-genie-1.0.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.642155 java-test-genie-0.1.1/
--rw-r--r--   0 boraelci   (501) staff       (20)     1066 2023-04-16 01:51:44.000000 java-test-genie-0.1.1/LICENSE
--rw-r--r--   0 boraelci   (501) staff       (20)      350 2023-04-16 01:55:32.000000 java-test-genie-0.1.1/MANIFEST.in
--rw-r--r--   0 boraelci   (501) staff       (20)     2560 2023-04-27 11:25:30.000000 java-test-genie-0.1.1/Makefile
--rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-05-03 18:04:19.641988 java-test-genie-0.1.1/PKG-INFO
--rw-r--r--   0 boraelci   (501) staff       (20)     2327 2023-05-03 17:50:35.000000 java-test-genie-0.1.1/README.md
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.619947 java-test-genie-0.1.1/evaluation/
--rw-r--r--   0 boraelci   (501) staff       (20)     4105 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/evaluation/evaluate.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.621007 java-test-genie-0.1.1/evaluation/resources/
--rw-r--r--   0 boraelci   (501) staff       (20)     1123 2023-04-30 10:32:29.000000 java-test-genie-0.1.1/evaluation/resources/gpt_pred.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      466 2023-04-30 11:22:22.000000 java-test-genie-0.1.1/evaluation/resources/gpt_system_prompt_evaluation.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.618079 java-test-genie-0.1.1/evaluation/results/
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.622048 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/
--rw-r--r--   0 boraelci   (501) staff       (20)     2044 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/bleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     1987 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/codebleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 13:08:30.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/summary.txt
--rw-r--r--   0 boraelci   (501) staff       (20)    54823 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/tests.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.623427 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/
--rw-r--r--   0 boraelci   (501) staff       (20)     2041 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/bleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     1985 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/codebleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 13:08:59.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/summary.txt
--rw-r--r--   0 boraelci   (501) staff       (20)    51477 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/tests.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.624739 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/
--rw-r--r--   0 boraelci   (501) staff       (20)     2034 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/bleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/codebleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:38:13.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/summary.txt
--rw-r--r--   0 boraelci   (501) staff       (20)    54938 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/tests.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.626348 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/
--rw-r--r--   0 boraelci   (501) staff       (20)    20266 2023-04-30 17:42:13.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/bleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)    19805 2023-04-30 17:31:33.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/codebleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 17:41:54.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/summary.txt
--rw-r--r--   0 boraelci   (501) staff       (20)   426119 2023-04-30 17:31:33.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/tests.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.629129 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/
--rw-r--r--   0 boraelci   (501) staff       (20)     2049 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/bleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/codebleus.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:53:55.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/summary.txt
--rw-r--r--   0 boraelci   (501) staff       (20)    55264 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/tests.txt
--rw-r--r--   0 boraelci   (501) staff       (20)   158769 2023-04-30 18:28:38.000000 java-test-genie-0.1.1/evaluation/visualizations.ipynb
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.629665 java-test-genie-0.1.1/genie/
--rw-r--r--   0 boraelci   (501) staff       (20)       22 2023-05-03 17:51:18.000000 java-test-genie-0.1.1/genie/__init__.py
--rw-r--r--   0 boraelci   (501) staff       (20)     5766 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/main.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.630438 java-test-genie-0.1.1/genie/parsers/
--rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-04-27 12:00:47.000000 java-test-genie-0.1.1/genie/parsers/ClassParser.py
--rw-r--r--   0 boraelci   (501) staff       (20)     2299 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/parsers/ConfigParser.py
--rw-r--r--   0 boraelci   (501) staff       (20)    11237 2023-04-27 05:28:04.000000 java-test-genie-0.1.1/genie/parsers/TestParser.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.633582 java-test-genie-0.1.1/genie/resources/
--rw-r--r--   0 boraelci   (501) staff       (20)     7356 2023-04-27 07:30:28.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed.json
--rw-r--r--   0 boraelci   (501) staff       (20)     3642 2023-04-27 07:49:35.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed_broken.json
--rw-r--r--   0 boraelci   (501) staff       (20)     4493 2023-05-03 17:40:57.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_raw.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      870 2023-04-27 07:15:06.000000 java-test-genie-0.1.1/genie/resources/gpt_system_prompt_parsed.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      493 2023-05-03 17:26:50.000000 java-test-genie-0.1.1/genie/resources/gpt_system_prompt_raw.txt
--rwxr-xr-x   0 boraelci   (501) staff       (20)   322200 2023-04-01 00:09:20.000000 java-test-genie-0.1.1/genie/resources/java-grammar.so
--rwxr-xr-x   0 boraelci   (501) staff       (20)   496550 2023-04-20 17:59:44.000000 java-test-genie-0.1.1/genie/resources/libtree-sitter-java.dylib
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.634897 java-test-genie-0.1.1/genie/wrappers/
--rw-r--r--   0 boraelci   (501) staff       (20)     1138 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/wrappers/GptWrapper.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.635968 java-test-genie-0.1.1/java_test_genie.egg-info/
--rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/PKG-INFO
--rw-r--r--   0 boraelci   (501) staff       (20)     1934 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/SOURCES.txt
--rw-r--r--   0 boraelci   (501) staff       (20)        1 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/dependency_links.txt
--rw-r--r--   0 boraelci   (501) staff       (20)       43 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/entry_points.txt
--rw-r--r--   0 boraelci   (501) staff       (20)        6 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/top_level.txt
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.641635 java-test-genie-0.1.1/milestones/
--rw-r--r--   0 boraelci   (501) staff       (20)  1820165 2023-05-03 17:45:22.000000 java-test-genie-0.1.1/milestones/Final Report - Bora Elci.pdf
--rw-r--r--   0 boraelci   (501) staff       (20)    91567 2023-05-01 10:32:57.000000 java-test-genie-0.1.1/milestones/Project Progress Report - Bora Elci.pdf
--rw-r--r--   0 boraelci   (501) staff       (20)    97124 2023-05-01 10:33:08.000000 java-test-genie-0.1.1/milestones/Revised Project Proposal - Bora Elci.pdf
--rw-r--r--   0 boraelci   (501) staff       (20)      100 2023-05-01 10:33:52.000000 java-test-genie-0.1.1/milestones/Slides link.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     2214 2023-05-03 18:01:02.000000 java-test-genie-0.1.1/pyproject.toml
--rw-r--r--   0 boraelci   (501) staff       (20)       38 2023-05-03 18:04:19.642205 java-test-genie-0.1.1/setup.cfg
--rw-r--r--   0 boraelci   (501) staff       (20)      659 2023-05-03 18:01:43.000000 java-test-genie-0.1.1/setup.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.540988 java-test-genie-1.0/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1066 2023-04-16 01:51:44.000000 java-test-genie-1.0/LICENSE
+-rw-r--r--   0 boraelci   (501) staff       (20)      350 2023-04-16 01:55:32.000000 java-test-genie-1.0/MANIFEST.in
+-rw-r--r--   0 boraelci   (501) staff       (20)     2560 2023-04-27 11:25:30.000000 java-test-genie-1.0/Makefile
+-rw-r--r--   0 boraelci   (501) staff       (20)     4137 2023-05-05 13:55:31.540841 java-test-genie-1.0/PKG-INFO
+-rw-r--r--   0 boraelci   (501) staff       (20)     3821 2023-05-05 13:46:37.000000 java-test-genie-1.0/README.md
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.516060 java-test-genie-1.0/evaluation/
+-rw-r--r--   0 boraelci   (501) staff       (20)     4105 2023-05-03 17:42:55.000000 java-test-genie-1.0/evaluation/evaluate.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.517475 java-test-genie-1.0/evaluation/resources/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1123 2023-04-30 10:32:29.000000 java-test-genie-1.0/evaluation/resources/gpt_pred.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      466 2023-04-30 11:22:22.000000 java-test-genie-1.0/evaluation/resources/gpt_system_prompt_evaluation.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.514276 java-test-genie-1.0/evaluation/results/
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.518715 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2044 2023-04-30 13:03:15.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1987 2023-04-30 13:03:15.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 13:08:30.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    54823 2023-04-30 13:03:15.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.519950 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2041 2023-04-30 13:03:49.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1985 2023-04-30 13:03:49.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 13:08:59.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    51477 2023-04-30 13:03:49.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.521184 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2034 2023-04-30 12:37:20.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:37:20.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:38:13.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    54938 2023-04-30 12:37:20.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.522622 java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/
+-rw-r--r--   0 boraelci   (501) staff       (20)    20266 2023-04-30 17:42:13.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    19805 2023-04-30 17:31:33.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 17:41:54.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)   426119 2023-04-30 17:31:33.000000 java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.524767 java-test-genie-1.0/evaluation/results/gpt4-s100-t1/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2049 2023-04-30 12:51:30.000000 java-test-genie-1.0/evaluation/results/gpt4-s100-t1/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:51:30.000000 java-test-genie-1.0/evaluation/results/gpt4-s100-t1/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:53:55.000000 java-test-genie-1.0/evaluation/results/gpt4-s100-t1/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    55264 2023-04-30 12:51:30.000000 java-test-genie-1.0/evaluation/results/gpt4-s100-t1/tests.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)   158769 2023-04-30 18:28:38.000000 java-test-genie-1.0/evaluation/visualizations.ipynb
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.526127 java-test-genie-1.0/genie/
+-rw-r--r--   0 boraelci   (501) staff       (20)       20 2023-05-05 13:52:14.000000 java-test-genie-1.0/genie/__init__.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.526518 java-test-genie-1.0/genie/images/
+-rw-r--r--   0 boraelci   (501) staff       (20)   260055 2023-05-05 13:51:12.000000 java-test-genie-1.0/genie/images/video-thumbnail.png
+-rw-r--r--   0 boraelci   (501) staff       (20)    10562 2023-05-05 13:33:00.000000 java-test-genie-1.0/genie/main.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.528083 java-test-genie-1.0/genie/parsers/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-05-04 22:23:15.000000 java-test-genie-1.0/genie/parsers/ClassParser.py
+-rw-r--r--   0 boraelci   (501) staff       (20)     2299 2023-05-03 17:42:55.000000 java-test-genie-1.0/genie/parsers/ConfigParser.py
+-rw-r--r--   0 boraelci   (501) staff       (20)    11237 2023-04-27 05:28:04.000000 java-test-genie-1.0/genie/parsers/TestParser.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.532895 java-test-genie-1.0/genie/resources/
+-rw-r--r--   0 boraelci   (501) staff       (20)      905 2023-05-04 22:43:58.000000 java-test-genie-1.0/genie/resources/generate_by_methods_prompt.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     7356 2023-04-27 07:30:28.000000 java-test-genie-1.0/genie/resources/gpt_response_for_parsed.json
+-rw-r--r--   0 boraelci   (501) staff       (20)     3642 2023-04-27 07:49:35.000000 java-test-genie-1.0/genie/resources/gpt_response_for_parsed_broken.json
+-rw-r--r--   0 boraelci   (501) staff       (20)     4493 2023-05-03 17:40:57.000000 java-test-genie-1.0/genie/resources/gpt_response_for_raw.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      870 2023-04-27 07:15:06.000000 java-test-genie-1.0/genie/resources/gpt_system_prompt_parsed.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      493 2023-05-03 17:26:50.000000 java-test-genie-1.0/genie/resources/gpt_system_prompt_raw.txt
+-rwxr-xr-x   0 boraelci   (501) staff       (20)   322200 2023-04-01 00:09:20.000000 java-test-genie-1.0/genie/resources/java-grammar.so
+-rwxr-xr-x   0 boraelci   (501) staff       (20)   496550 2023-04-20 17:59:44.000000 java-test-genie-1.0/genie/resources/libtree-sitter-java.dylib
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.534576 java-test-genie-1.0/genie/wrappers/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1193 2023-05-04 22:29:03.000000 java-test-genie-1.0/genie/wrappers/GptWrapper.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.536243 java-test-genie-1.0/java_test_genie.egg-info/
+-rw-r--r--   0 boraelci   (501) staff       (20)     4137 2023-05-05 13:55:31.000000 java-test-genie-1.0/java_test_genie.egg-info/PKG-INFO
+-rw-r--r--   0 boraelci   (501) staff       (20)     2014 2023-05-05 13:55:31.000000 java-test-genie-1.0/java_test_genie.egg-info/SOURCES.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)        1 2023-05-05 13:55:31.000000 java-test-genie-1.0/java_test_genie.egg-info/dependency_links.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)       43 2023-05-05 13:55:31.000000 java-test-genie-1.0/java_test_genie.egg-info/entry_points.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)        6 2023-05-05 13:55:31.000000 java-test-genie-1.0/java_test_genie.egg-info/top_level.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-05 13:55:31.540522 java-test-genie-1.0/milestones/
+-rw-r--r--   0 boraelci   (501) staff       (20)  1820163 2023-05-03 18:14:09.000000 java-test-genie-1.0/milestones/Final Report - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)    91567 2023-05-01 10:32:57.000000 java-test-genie-1.0/milestones/Project Progress Report - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)    97124 2023-05-01 10:33:08.000000 java-test-genie-1.0/milestones/Revised Project Proposal - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)      100 2023-05-01 10:33:52.000000 java-test-genie-1.0/milestones/Slides link.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     2212 2023-05-05 13:52:18.000000 java-test-genie-1.0/pyproject.toml
+-rw-r--r--   0 boraelci   (501) staff       (20)       38 2023-05-05 13:55:31.541034 java-test-genie-1.0/setup.cfg
+-rw-r--r--   0 boraelci   (501) staff       (20)      659 2023-05-04 21:15:53.000000 java-test-genie-1.0/setup.py
```

### Comparing `java-test-genie-0.1.1/LICENSE` & `java-test-genie-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/Makefile` & `java-test-genie-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/PKG-INFO` & `java-test-genie-1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: java-test-genie
-Version: 0.1.1
+Version: 1.0
 Summary: AI-Driven Unit Test Generation for Java
 Home-page: https://github.com/boraelci/java-test-genie
 Author: Bora Elci
 Author-email: bora.elci@columbia.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JavaTestGenie
-![MIT License](https://img.shields.io/github/license/boraelci/review-master)
+[![MIT License](https://img.shields.io/github/license/boraelci/java-test-genie)](https://github.com/boraelci/java-test-genie/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/java-test-genie)](https://pypi.org/project/java-test-genie/)
 
+## Demo
+Click on the image to watch the video
+[![Video](https://github.com/boraelci/java-test-genie/blob/main/genie/images/video-thumbnail.png)](https://drive.google.com/file/d/1W8TnxP7CN2rSFGRzgUXU7qNrg4EGsbIk/view?usp=share_link)
+
 ## Installation
 
 ```bash
 pip install java-test-genie
 ```
 
 ## Usage
@@ -35,35 +39,51 @@
       "parent_dir": "src/main/java/com/ase/restservice",
       "dir_names": ["service"],
       "file_names": []
     }
   ],
   "exclude": [
     {
-      "parent_dir": "src/main/java/com/ase/restservice/service",
-      "dir_names": ["interface"],
+      "parent_dir": "src/main/java/com/ase/restservice",
+      "dir_names": ["service/interface"],
       "file_names": []
     }
   ]
 }
 ```
 
-The file is case-sensitive. Ensure that you do not list files in the "exclude" section unless they match a path in the "include" section. Excluding a path will delete all matches, even if a specific class is explicitly listed in the "include" section. For instance, if you exclude "model/" but include "model/Account.java", it will not work. Instead, simply include "model/Account.java" and leave the "exclude" section empty, as the "model/" directory is already skipped.
+The file is case-sensitive. Ensure that you do not list files in the "exclude" section unless they already match a path in the "include" section. Excluding a path will delete all matches, even if a specific class is explicitly listed in the "include" section. For instance, if you exclude "model/" but include "model/Account.java", it will not work. Instead, simply include "model/Account.java" and leave the "exclude" section empty, as the "model/" directory is already skipped.
 
 Finally, you can run it with:
 
 ```bash
 genie
 ```
 
 ## Example
-
 Here is an example repo that you can use the config file above with.
 
-`git clone https://github.com/boraelci/kaiserschmarrn.git`
+```bash
+git clone https://github.com/boraelci/kaiserschmarrn.git
+```
+
+## Arguments
+
+1. `--help`: Displays the help message and lists all available arguments.
+2. `--mode`: Allows you to switch between two modes:
+   - `methods` (default): Generates test methods for individual methods within the input class. This mode is suitable for large input classes.
+   - `classes`: Generates a complete test class, including imports, package name, and setup. This mode provides more comprehensive functionality but is not suitable for large input classes. If the input class is too large, you may encounter an error like `Error: this file is too large`.
+   
+3. `--do_overwrite`: Enables automatic overwriting of existing test files without asking for confirmation. By default, this is set to false to protect existing test files. To enable automatic overwriting, just include `--do_overwrite` without specifying a parameter.
+
+4. `--batch-size`: Specifies the number of methods to process at the same time. It defaults to 15, but you can adjust this value based on your requirements.
+
+## Limitations
+
+Currently, only 1 class per Java file is supported. The tool may produce errors if you supply a path that corresponds to a file with more than 1 class in it.
 
 ## Grammar
 
 Parsing Java files with the Tree-sitter library requires grammar files. They were obtained in the following way for this tool.
 
 ### For macOS
```

### Comparing `java-test-genie-0.1.1/evaluation/evaluate.py` & `java-test-genie-1.0/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/resources/gpt_pred.txt` & `java-test-genie-1.0/evaluation/resources/gpt_pred.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/bleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/bleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/codebleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/codebleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/tests.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0/tests.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/bleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/bleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/codebleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/codebleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/tests.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t0.5/tests.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/bleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/bleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/codebleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/codebleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/tests.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s100-t1/tests.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/bleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/bleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/codebleus.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/codebleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/tests.txt` & `java-test-genie-1.0/evaluation/results/gpt3.5-s1000-t0/tests.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/bleus.txt` & `java-test-genie-1.0/evaluation/results/gpt4-s100-t1/bleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/codebleus.txt` & `java-test-genie-1.0/evaluation/results/gpt4-s100-t1/codebleus.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/tests.txt` & `java-test-genie-1.0/evaluation/results/gpt4-s100-t1/tests.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/evaluation/visualizations.ipynb` & `java-test-genie-1.0/evaluation/visualizations.ipynb`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/parsers/ClassParser.py` & `java-test-genie-1.0/genie/parsers/ClassParser.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/parsers/ConfigParser.py` & `java-test-genie-1.0/genie/parsers/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/parsers/TestParser.py` & `java-test-genie-1.0/genie/parsers/TestParser.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed.json` & `java-test-genie-1.0/genie/resources/gpt_response_for_parsed.json`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed_broken.json` & `java-test-genie-1.0/genie/resources/gpt_response_for_parsed_broken.json`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/gpt_response_for_raw.txt` & `java-test-genie-1.0/genie/resources/gpt_response_for_raw.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/gpt_system_prompt_parsed.txt` & `java-test-genie-1.0/genie/resources/gpt_system_prompt_parsed.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/java-grammar.so` & `java-test-genie-1.0/genie/resources/java-grammar.so`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/resources/libtree-sitter-java.dylib` & `java-test-genie-1.0/genie/resources/libtree-sitter-java.dylib`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/genie/wrappers/GptWrapper.py` & `java-test-genie-1.0/genie/wrappers/GptWrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class GptWrapper:
     def __init__(self, system_prompt_path):
         with open(system_prompt_path, "r") as f:
             self.system_prompt = f.read()
 
     def query(self, message):
+        # print("submitting")
+        # print(message)
         openai.api_key = os.environ["OPENAI_API_KEY"]
         # model = "gpt-4"
         model = "gpt-3.5-turbo"
         temperature = 0
         input_token_count = self.get_input_token_count(model, message)
         if input_token_count > 3900:
             raise Exception("Error: this file is too large")
```

### Comparing `java-test-genie-0.1.1/java_test_genie.egg-info/PKG-INFO` & `java-test-genie-1.0/java_test_genie.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: java-test-genie
-Version: 0.1.1
+Version: 1.0
 Summary: AI-Driven Unit Test Generation for Java
 Home-page: https://github.com/boraelci/java-test-genie
 Author: Bora Elci
 Author-email: bora.elci@columbia.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JavaTestGenie
-![MIT License](https://img.shields.io/github/license/boraelci/review-master)
+[![MIT License](https://img.shields.io/github/license/boraelci/java-test-genie)](https://github.com/boraelci/java-test-genie/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/java-test-genie)](https://pypi.org/project/java-test-genie/)
 
+## Demo
+Click on the image to watch the video
+[![Video](https://github.com/boraelci/java-test-genie/blob/main/genie/images/video-thumbnail.png)](https://drive.google.com/file/d/1W8TnxP7CN2rSFGRzgUXU7qNrg4EGsbIk/view?usp=share_link)
+
 ## Installation
 
 ```bash
 pip install java-test-genie
 ```
 
 ## Usage
@@ -35,35 +39,51 @@
       "parent_dir": "src/main/java/com/ase/restservice",
       "dir_names": ["service"],
       "file_names": []
     }
   ],
   "exclude": [
     {
-      "parent_dir": "src/main/java/com/ase/restservice/service",
-      "dir_names": ["interface"],
+      "parent_dir": "src/main/java/com/ase/restservice",
+      "dir_names": ["service/interface"],
       "file_names": []
     }
   ]
 }
 ```
 
-The file is case-sensitive. Ensure that you do not list files in the "exclude" section unless they match a path in the "include" section. Excluding a path will delete all matches, even if a specific class is explicitly listed in the "include" section. For instance, if you exclude "model/" but include "model/Account.java", it will not work. Instead, simply include "model/Account.java" and leave the "exclude" section empty, as the "model/" directory is already skipped.
+The file is case-sensitive. Ensure that you do not list files in the "exclude" section unless they already match a path in the "include" section. Excluding a path will delete all matches, even if a specific class is explicitly listed in the "include" section. For instance, if you exclude "model/" but include "model/Account.java", it will not work. Instead, simply include "model/Account.java" and leave the "exclude" section empty, as the "model/" directory is already skipped.
 
 Finally, you can run it with:
 
 ```bash
 genie
 ```
 
 ## Example
-
 Here is an example repo that you can use the config file above with.
 
-`git clone https://github.com/boraelci/kaiserschmarrn.git`
+```bash
+git clone https://github.com/boraelci/kaiserschmarrn.git
+```
+
+## Arguments
+
+1. `--help`: Displays the help message and lists all available arguments.
+2. `--mode`: Allows you to switch between two modes:
+   - `methods` (default): Generates test methods for individual methods within the input class. This mode is suitable for large input classes.
+   - `classes`: Generates a complete test class, including imports, package name, and setup. This mode provides more comprehensive functionality but is not suitable for large input classes. If the input class is too large, you may encounter an error like `Error: this file is too large`.
+   
+3. `--do_overwrite`: Enables automatic overwriting of existing test files without asking for confirmation. By default, this is set to false to protect existing test files. To enable automatic overwriting, just include `--do_overwrite` without specifying a parameter.
+
+4. `--batch-size`: Specifies the number of methods to process at the same time. It defaults to 15, but you can adjust this value based on your requirements.
+
+## Limitations
+
+Currently, only 1 class per Java file is supported. The tool may produce errors if you supply a path that corresponds to a file with more than 1 class in it.
 
 ## Grammar
 
 Parsing Java files with the Tree-sitter library requires grammar files. They were obtained in the following way for this tool.
 
 ### For macOS
```

### Comparing `java-test-genie-0.1.1/java_test_genie.egg-info/SOURCES.txt` & `java-test-genie-1.0/java_test_genie.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 evaluation/results/gpt3.5-s1000-t0/tests.txt
 evaluation/results/gpt4-s100-t1/bleus.txt
 evaluation/results/gpt4-s100-t1/codebleus.txt
 evaluation/results/gpt4-s100-t1/summary.txt
 evaluation/results/gpt4-s100-t1/tests.txt
 genie/__init__.py
 genie/main.py
+genie/images/video-thumbnail.png
 genie/parsers/ClassParser.py
 genie/parsers/ConfigParser.py
 genie/parsers/TestParser.py
+genie/resources/generate_by_methods_prompt.txt
 genie/resources/gpt_response_for_parsed.json
 genie/resources/gpt_response_for_parsed_broken.json
 genie/resources/gpt_response_for_raw.txt
 genie/resources/gpt_system_prompt_parsed.txt
 genie/resources/gpt_system_prompt_raw.txt
 genie/resources/java-grammar.so
 genie/resources/libtree-sitter-java.dylib
```

### Comparing `java-test-genie-0.1.1/milestones/Final Report - Bora Elci.pdf` & `java-test-genie-1.0/milestones/Final Report - Bora Elci.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 1% similar despite different names*

#### pdftotext {} -

```diff
@@ -135,15 +135,15 @@
 Java classes via the tree-sitter library. However, the grammar file provided is not compatible
 with macOS, where we are running the experiment. Therefore, we compile the Java language file
 ourselves. The code and instructions to accomplish this can be found in our GitHub repository,
 although this is not needed to use our tool since we already distribute the grammar file within
 our releases. We make further adjustments to the scripts to make them compatible with macOS
 and plan to make an open-source contribution to the Methods2Test repository. Our adapted script
 brings any Java repository to the same FM+FC+C format that we selected to use. We create
-another script, evaluation.py, in a similar manner that allows us to evaluate OpenAI’s GPT models
+another script, evaluate.py, in a similar manner that allows us to evaluate OpenAI’s GPT models
 over the dataset. We sample the first 100 inputs and corresponding outputs from the evaluation
 set to compare model performances.
 
 Figure 4: Effect of model choice on performance
 
 4
```

### Comparing `java-test-genie-0.1.1/milestones/Project Progress Report - Bora Elci.pdf` & `java-test-genie-1.0/milestones/Project Progress Report - Bora Elci.pdf`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/milestones/Revised Project Proposal - Bora Elci.pdf` & `java-test-genie-1.0/milestones/Revised Project Proposal - Bora Elci.pdf`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.1/pyproject.toml` & `java-test-genie-1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "java-test-genie"
 authors = [{name = "Bora Elci", email = "bora.elci@columbia.edu"}]
 description="AI-Driven Unit Test Generation for Java"
 readme = "README.md"
-version = "0.1.1"
+version = "1.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "openai",
     "tiktoken",
     "tree-sitter"
 ]
```

### Comparing `java-test-genie-0.1.1/setup.py` & `java-test-genie-1.0/setup.py`

 * *Files identical despite different names*

