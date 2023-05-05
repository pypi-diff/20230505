# Comparing `tmp/PHASEfilter-0.3.7.tar.gz` & `tmp/PHASEfilter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PHASEfilter-0.3.7.tar", last modified: Fri Jan  7 16:13:56 2022, max compression
+gzip compressed data, was "dist/PHASEfilter-1.1.0.tar", last modified: Fri May  5 14:18:58 2023, max compression
```

## Comparing `PHASEfilter-0.3.7.tar` & `PHASEfilter-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)      399 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/entry_points.txt
--rw-rw-r--   0 mmp       (1000) mmp       (1000)       65 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/requires.txt
--rw-rw-r--   0 mmp       (1000) mmp       (1000)       12 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/top_level.txt
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     1596 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/SOURCES.txt
--rw-rw-r--   0 mmp       (1000) mmp       (1000)        1 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/dependency_links.txt
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    10138 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter.egg-info/PKG-INFO
--rw-rw-r--   0 mmp       (1000) mmp       (1000)      190 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/setup.cfg
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     7774 2022-01-07 16:10:28.000000 PHASEfilter-0.3.7/README.md
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/__init__.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/lib/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/__init__.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/lib/constants/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)      798 2022-01-07 16:04:26.000000 PHASEfilter-0.3.7/PHASEfilter/lib/constants/version.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)       45 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/constants/__init__.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)      114 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/constants/constants.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     7668 2022-01-07 12:50:14.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/reference.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    21626 2022-01-07 13:01:29.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/util.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)       46 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/__init__.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     3559 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/testing_software.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    29532 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/blast_two_sequences.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    24930 2021-09-22 16:11:34.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/vcf_process.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     4905 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/run_extra_software.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     6043 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/software.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     3662 2022-01-07 13:00:42.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/read_gff.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    38765 2021-10-27 16:47:56.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/lift_over_simple.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     5215 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/lib/utils/lastz_two_sequences.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/lib/process/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)       46 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/lib/process/__init__.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     9771 2021-09-24 13:12:37.000000 PHASEfilter-0.3.7/PHASEfilter/lib/process/process_genomes.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     9975 2021-10-28 12:32:37.000000 PHASEfilter-0.3.7/PHASEfilter/lib/process/process_references.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/tests/
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    19219 2021-10-28 12:44:45.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_lift_over.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     4147 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_reference.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     9308 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_process_genomes.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     1660 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_run_extra_software.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)      150 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/tests/__init__.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    25643 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_vcf.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     9020 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_software.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     7827 2021-10-27 16:41:32.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_utils.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     8526 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/tests/test_synchronization.py
-drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PHASEfilter/bin/
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     8745 2021-09-17 10:53:16.000000 PHASEfilter-0.3.7/PHASEfilter/bin/phasefilter_single.py
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     6700 2021-10-26 13:22:49.000000 PHASEfilter-0.3.7/PHASEfilter/bin/synchronize_genomes.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-0.3.7/PHASEfilter/bin/__init__.py
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     1485 2022-01-07 11:16:10.000000 PHASEfilter-0.3.7/PHASEfilter/bin/install_phasefilter_dependencies.sh
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     6664 2021-11-08 17:15:44.000000 PHASEfilter-0.3.7/PHASEfilter/bin/make_alignment.py
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     2969 2021-12-21 09:22:10.000000 PHASEfilter-0.3.7/PHASEfilter/bin/copy_raw_data_example_phasefilter.py
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     9637 2021-09-17 10:53:09.000000 PHASEfilter-0.3.7/PHASEfilter/bin/phasefilter.py
--rwxrwxr-x   0 mmp       (1000) mmp       (1000)     3021 2021-09-16 16:01:50.000000 PHASEfilter-0.3.7/PHASEfilter/bin/reference_statistics.py
--rw-rw-r--   0 mmp       (1000) mmp       (1000)    10138 2022-01-07 16:13:56.000000 PHASEfilter-0.3.7/PKG-INFO
--rw-rw-r--   0 mmp       (1000) mmp       (1000)     3688 2022-01-07 16:00:36.000000 PHASEfilter-0.3.7/setup.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)      399 2023-05-05 14:18:57.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/entry_points.txt
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)       81 2023-05-05 14:18:57.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/requires.txt
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)       12 2023-05-05 14:18:57.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/top_level.txt
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     1659 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)        1 2023-05-05 14:18:57.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    10878 2023-05-05 14:18:57.000000 PHASEfilter-1.1.0/PHASEfilter.egg-info/PKG-INFO
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)      190 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/setup.cfg
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     8473 2023-05-05 13:49:31.000000 PHASEfilter-1.1.0/README.md
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/__init__.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/lib/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/lib/__init__.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/lib/constants/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)      798 2023-05-05 13:40:11.000000 PHASEfilter-1.1.0/PHASEfilter/lib/constants/version.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)       45 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/lib/constants/__init__.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)      114 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/lib/constants/constants.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     7668 2022-01-07 12:50:14.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/reference.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    21626 2022-01-07 13:01:29.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/util.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     1720 2022-07-20 16:25:29.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/chain.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)       46 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/__init__.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     3736 2022-05-23 11:43:04.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/testing_software.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    29532 2021-09-16 16:01:50.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/blast_two_sequences.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    24889 2022-07-08 14:22:34.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/vcf_process.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     7071 2022-07-06 10:03:13.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/run_extra_software.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     6823 2022-07-06 10:35:34.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/software.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     3704 2022-07-07 08:48:23.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/read_gff.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    48639 2022-07-20 16:44:41.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/lift_over_simple.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     5215 2021-09-16 16:01:50.000000 PHASEfilter-1.1.0/PHASEfilter/lib/utils/lastz_two_sequences.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/lib/process/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)       46 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/lib/process/__init__.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    10246 2022-07-20 16:41:38.000000 PHASEfilter-1.1.0/PHASEfilter/lib/process/process_genomes.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    10188 2022-07-09 18:54:11.000000 PHASEfilter-1.1.0/PHASEfilter/lib/process/process_references.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/tests/
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    19261 2022-07-07 10:00:06.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_lift_over.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     4147 2021-09-16 16:01:50.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_reference.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     9338 2022-07-06 22:08:19.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_process_genomes.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     4232 2022-07-06 10:41:20.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_run_extra_software.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)      150 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/tests/__init__.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    25679 2022-07-06 22:13:11.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_vcf.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     9020 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_software.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     7898 2022-07-20 11:39:25.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_chain.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     7825 2022-07-06 11:35:39.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_utils.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     8544 2022-07-06 22:10:52.000000 PHASEfilter-1.1.0/PHASEfilter/tests/test_synchronization.py
+drwxrwxr-x   0 mmp       (1000) mmp       (1000)        0 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PHASEfilter/bin/
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     9120 2022-07-08 09:05:54.000000 PHASEfilter-1.1.0/PHASEfilter/bin/phasefilter_single.py
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     7018 2023-05-05 13:17:45.000000 PHASEfilter-1.1.0/PHASEfilter/bin/synchronize_genomes.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)        0 2021-07-07 11:22:09.000000 PHASEfilter-1.1.0/PHASEfilter/bin/__init__.py
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     1485 2022-07-07 09:01:22.000000 PHASEfilter-1.1.0/PHASEfilter/bin/install_phasefilter_dependencies.sh
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     6963 2022-07-09 18:52:01.000000 PHASEfilter-1.1.0/PHASEfilter/bin/make_alignment.py
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     3071 2022-07-07 09:26:29.000000 PHASEfilter-1.1.0/PHASEfilter/bin/copy_raw_data_example_phasefilter.py
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)    10871 2022-07-20 15:59:07.000000 PHASEfilter-1.1.0/PHASEfilter/bin/phasefilter.py
+-rwxrwxr-x   0 mmp       (1000) mmp       (1000)     3021 2021-09-16 16:01:50.000000 PHASEfilter-1.1.0/PHASEfilter/bin/reference_statistics.py
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)    10878 2023-05-05 14:18:58.000000 PHASEfilter-1.1.0/PKG-INFO
+-rw-rw-r--   0 mmp       (1000) mmp       (1000)     3741 2023-05-05 14:18:33.000000 PHASEfilter-1.1.0/setup.py
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter.egg-info/SOURCES.txt` & `PHASEfilter-1.1.0/PHASEfilter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 PHASEfilter/lib/constants/constants.py
 PHASEfilter/lib/constants/version.py
 PHASEfilter/lib/process/__init__.py
 PHASEfilter/lib/process/process_genomes.py
 PHASEfilter/lib/process/process_references.py
 PHASEfilter/lib/utils/__init__.py
 PHASEfilter/lib/utils/blast_two_sequences.py
+PHASEfilter/lib/utils/chain.py
 PHASEfilter/lib/utils/lastz_two_sequences.py
 PHASEfilter/lib/utils/lift_over_simple.py
 PHASEfilter/lib/utils/read_gff.py
 PHASEfilter/lib/utils/reference.py
 PHASEfilter/lib/utils/run_extra_software.py
 PHASEfilter/lib/utils/software.py
 PHASEfilter/lib/utils/testing_software.py
 PHASEfilter/lib/utils/util.py
 PHASEfilter/lib/utils/vcf_process.py
 PHASEfilter/tests/__init__.py
+PHASEfilter/tests/test_chain.py
 PHASEfilter/tests/test_lift_over.py
 PHASEfilter/tests/test_process_genomes.py
 PHASEfilter/tests/test_reference.py
 PHASEfilter/tests/test_run_extra_software.py
 PHASEfilter/tests/test_software.py
 PHASEfilter/tests/test_synchronization.py
 PHASEfilter/tests/test_utils.py
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter.egg-info/PKG-INFO` & `PHASEfilter-1.1.0/PHASEfilter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHASEfilter
-Version: 0.3.7
+Version: 1.1.0
 Summary: Software package to filter variants, SNPs and INDELs, that are present in heterozygous form in phased genomes.
 Home-page: https://github.com/ibigen/PHASEfilter
 Author: Miguel Pinheiro
 Author-email: monsanto@ua.pt
 License: MIT
 Project-URL: Bug Reports, https://github.com/ibigen/PHASEfilter/issues
 Project-URL: Source, https://github.com/ibigen/PHASEfilter
@@ -25,21 +25,21 @@
         ```
         $ pip3 install PHASEfilter
         ```
         
         ### Install with virtualenv
         
         ```
-        $ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 0.3.7) "
+        $ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 1.1.0) "
         $ . PHASEfilter/bin/activate
-        (phasefilter 0.3.7) $ pip install PHASEfilter
+        (phasefilter 1.1.0) $ pip install PHASEfilter
         
         ## install all Software dependencies of PHASEfilter 
-        (phasefilter 0.3.7) $ cd PHASEfilter/bin/
-        (phasefilter 0.3.7) $ ./install_phasefilter_dependencies.sh
+        (phasefilter 1.1.0) $ cd PHASEfilter/bin/
+        (phasefilter 1.1.0) $ ./install_phasefilter_dependencies.sh
         ```
         
         ### Install with conda
         
         ```
         $ wget https://raw.githubusercontent.com/ibigen/PHASEfilter/main/conda/conda_phasefilter_env.yml -O conda_phasefilter_env.yml
         $ conda env create -f conda_phasefilter_env.yml
@@ -64,14 +64,17 @@
         The variant file in analysis it is always the one passed in parameter '--vcf1'.
         
         ```
         $ phasefilter --help
         ## You can can copy some example data to test the commands
         $ copy_raw_data_example_phasefilter --out temp_raw_data
         $ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir
+        
+        ## you can use chain if exists
+        $ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir --chain_A_B temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain --chain_B_A temp_raw_data/Assembly22_hapB_To_Assembly22_hapA.over.chain
         ```
         
         Eighth possible files will be created after the commands ends. The outputs are from refrence A (ref1) to reference B (ref2), and from reference B (ref2) to reference A (ref1).
         
         -  report_[A]_to_[B].txt - has the statistics about the analysis;
         -  valid_[A]_to_[B].vcf.gz - has all variants that are not heterozygous between two references;
         -  removed_[A]_to_[B].vcf.gz - has all heterozygous variants;
@@ -102,14 +105,17 @@
         ## Filter variants in phased genomes but only one direction
         
         This tool do as the same of the previous script but only analysis from Reference A (ref1) to Reference B (ref2)
         
         ```
         $ phasefilter_single --help
         $ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz
+        
+        ## with chain
+        $ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz --chain temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain
         ```
         
         ## Synchronize annotation genomes
         
         Synchronize annotations genomes adapting the annotations that are in reference 1 to the reference 2, adding the tags 'StartHit' and 'EndHit' to the result file. In VCF type files only add 'StartHit' tag in Info. The annotations (input file need to be in VCF or GFF3 and belong to the reference 1.
         
         ```
@@ -155,15 +161,15 @@
         ```
         
         # Documentation
         
         PHASEfilter documentation is available in [ReadTheDocs: PHASEfilter](https://phasefilter.readthedocs.io/en/latest/)
         
 Keywords: SNPs INDEL phased genome filtering bioinformatics
-Platform: linux_x86_64
+Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `PHASEfilter-0.3.7/README.md` & `PHASEfilter-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 ```
 $ pip3 install PHASEfilter
 ```
 
 ### Install with virtualenv
 
 ```
-$ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 0.3.7) "
+$ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 1.1.0) "
 $ . PHASEfilter/bin/activate
-(phasefilter 0.3.7) $ pip install PHASEfilter
+(phasefilter 1.1.0) $ pip install PHASEfilter
 
 ## install all Software dependencies of PHASEfilter 
-(phasefilter 0.3.7) $ cd PHASEfilter/bin/
-(phasefilter 0.3.7) $ ./install_phasefilter_dependencies.sh
+(phasefilter 1.1.0) $ cd PHASEfilter/bin/
+(phasefilter 1.1.0) $ ./install_phasefilter_dependencies.sh
 ```
 
 ### Install with conda
 
 ```
 $ wget https://raw.githubusercontent.com/ibigen/PHASEfilter/main/conda/conda_phasefilter_env.yml -O conda_phasefilter_env.yml
 $ conda env create -f conda_phasefilter_env.yml
@@ -53,14 +53,17 @@
 The variant file in analysis it is always the one passed in parameter '--vcf1'.
 
 ```
 $ phasefilter --help
 ## You can can copy some example data to test the commands
 $ copy_raw_data_example_phasefilter --out temp_raw_data
 $ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir
+
+## you can use chain if exists
+$ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir --chain_A_B temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain --chain_B_A temp_raw_data/Assembly22_hapB_To_Assembly22_hapA.over.chain
 ```
 
 Eighth possible files will be created after the commands ends. The outputs are from refrence A (ref1) to reference B (ref2), and from reference B (ref2) to reference A (ref1).
 
 -  report_[A]_to_[B].txt - has the statistics about the analysis;
 -  valid_[A]_to_[B].vcf.gz - has all variants that are not heterozygous between two references;
 -  removed_[A]_to_[B].vcf.gz - has all heterozygous variants;
@@ -91,14 +94,17 @@
 ## Filter variants in phased genomes but only one direction
 
 This tool do as the same of the previous script but only analysis from Reference A (ref1) to Reference B (ref2)
 
 ```
 $ phasefilter_single --help
 $ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz
+
+## with chain
+$ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz --chain temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain
 ```
 
 ## Synchronize annotation genomes
 
 Synchronize annotations genomes adapting the annotations that are in reference 1 to the reference 2, adding the tags 'StartHit' and 'EndHit' to the result file. In VCF type files only add 'StartHit' tag in Info. The annotations (input file need to be in VCF or GFF3 and belong to the reference 1.
 
 ```
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/constants/version.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/constants/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 # 	1.2.0b1     # Beta Release
 # 	1.2.0rc1    # Release Candidate
 # 	1.2.0       # Final Release
 # 	1.2.0.post1 # Post Release
 # 	15.10       # Date based release
 # 	23          # Serial release
 
-VERSION_package = "0.3.7"				### For pypi
-VERSION_make_alignement = "0.3.3"		### version of this script
-VERSION_phase_filter = "0.3.4"
-VERSION_reference_statistics = "0.3.3"
-VERSION_synchronize_genomes = "0.3.5"
+VERSION_package = "1.1.0"				### For pypi
+VERSION_make_alignement = "1.1.0"		### version of this script
+VERSION_phase_filter = "1.1.0"
+VERSION_reference_statistics = "1.0.0"
+VERSION_synchronize_genomes = "1.1.0"
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/reference.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/reference.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/util.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/util.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/testing_software.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/testing_software.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,39 +10,43 @@
 	KEY_software_run_get_version = 'software_get_version'	## software calling by OS to get the version
 	KEY_version = 'version'									## version required MAJOR.MINOR
 	KEY_version_major_number = 'version_major_number' 		## if must be "equal" or "can be equal or greater"
 	KEY_version_minor_number = 'version_minor_number'		## if must be "equal" or "can be equal or greater"
 	KEY_version_pass_equal = 'equal'
 	KEY_version_pass_equal_or_bigger = 'equal_or_bigger'
 	
+	## used when thereis no version
+	KEY_no_version = 'No version'
+	
 	#### utils
 	utils = Utils()
 
 	def __init__(self):
 		pass
 	
 	def test_software(self, software):
 		"""
 		:param {'software' : <software to rum>, 'version' : <version string>}
 		"""
 		
 		tmp_file = self.utils.get_temp_file('file_name', '.txt')
 		cmd = "{} > {} 2>&1".format(software[SoftwareTest.KEY_software_run_get_version], tmp_file)
 		exist_status = os.system(cmd)
-		if (exist_status != 0 and exist_status != 256):
+		if (exist_status != 0 and exist_status != 256 and exist_status != 65280):
 			self.utils.remove_file(tmp_file)
 			raise Exception("Error: software '{}' is not present in your PATH".format(
 					software[SoftwareTest.KEY_software_name]))
 		
 		### read file
 		vect_data = self.utils.read_text_file(tmp_file)
 		self.utils.remove_file(tmp_file)
 		
 		### 
 		for line_ in vect_data:
+			if software[SoftwareTest.KEY_version] == SoftwareTest.KEY_no_version: return True
 			result = self.is_version_equal_or_bigger(line_, software)
 			if (result is None): continue
 			return result
 		return None
 
 
 	def is_version_equal_or_bigger(self, sz_string, software):
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/blast_two_sequences.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/blast_two_sequences.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/vcf_process.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/vcf_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 		self.dont_have_hit_postion += other.dont_have_hit_postion
 		self.total_alleles += other.total_alleles
 		self.could_not_fetch_vcf_record += other.could_not_fetch_vcf_record
 		self.filter_threshold_ratio_AD += other.filter_threshold_ratio_AD
 		return self
 
 	def add_line(self, line):
-		lst_data = line.split()
+		lst_data = line.split("\t")
 		if (len(lst_data) == 10 or len(lst_data) == 11):
 			self.equal_allele += int(lst_data[0])
 			self.diff_allele += int(lst_data[1])
 			self.loh_allele += int(lst_data[2])
 			self.pass_variation += int(lst_data[3])
 			self.dont_have_hit_postion += int(lst_data[4])
 			self.could_not_fetch_vcf_record += int(lst_data[5])
@@ -508,19 +508,17 @@
 
 		
 	def match_vcf_to(self, seq_name_a, lift_over_ligth, vcf_hit, seq_name_b, vcf_out,
 					vcf_out_removed_temp, vcf_out_LOH_temp):
 		"""
 		:out nothing
 		"""
-		if (self.is_zipped): handle_in = open(self.file_name, 'rb')
-		else: handle_in = open(self.file_name, 'r')
 		try:
-			
-			with open(vcf_out, 'w') as handle_vcf_out, open(vcf_out_removed_temp, 'w') as handle_vcf_remove_out,\
+			with (open(self.file_name, 'rb') if (self.is_zipped) else open(self.file_name, 'r')) as handle_in,\
+				open(vcf_out, 'w') as handle_vcf_out, open(vcf_out_removed_temp, 'w') as handle_vcf_remove_out,\
 					open(vcf_out_LOH_temp, 'w') as handle_vcf_LOH_out, open(vcf_hit, 'rb') as handle_hit:
 				vcf_reader = vcf.Reader(handle_in, compressed=self.is_zipped)
 				vcf_reader_hit = vcf.Reader(handle_hit, compressed=True)
 				vcf_write = vcf.VCFWriter(handle_vcf_out, vcf_reader)
 				vcf_write_removed = vcf.VCFWriter(handle_vcf_remove_out, vcf_reader)
 				vcf_write_LOH = vcf.VCFWriter(handle_vcf_LOH_out, vcf_reader)
 				
@@ -561,15 +559,15 @@
 								if (self.b_print_results):
 									print("Error FetchRecord: ", record.heterozygosity, record)
 									print("Position from: {}    Position To: {}".format(record.POS, position))
 								vcf_write.write_record(record)
 						else:
 							### save in an output
 							if (self.b_print_results):
-								print("Erro Pos: ", record.heterozygosity, record)
+								print("Error Pos: ", record.heterozygosity, record)
 								print("Position hit: {}    Position most left: {}".format(position, position_most_left))
 							vcf_write.write_record(record)
 							self.count_alleles.add_dont_have_hit_postion()
 					else:
 						self.count_alleles.add_pass_variation()
 						vcf_write.write_record(record)
 					
@@ -578,16 +576,14 @@
 					
 				#### save statistics results
 				if (self.b_print_results):
 					print(self.count_alleles.get_header()) 
 					print(self.count_alleles)
 		except Exception as e:
 			pass
-		finally:
-			handle_in.close()
 
 
 	def parse_vcf(self, file_result, vect_pass_ref, lift_over_ligth):
 		"""
 		:param file_result - output file
 		:param vect_pass_ref - don't parse this chr
 		:param lift_over_ligth - method to pass, ref_a is always the main reference
@@ -598,18 +594,17 @@
 		
 		tem_file = self.utils.get_temp_file("syncronize", ".vcf")
 		chr_name = ""	### nothing processed yet
 		chr_name_B = ""
 		(lines_parsed, lines_failed_parse) = (0, 0)
 		vect_fail_synch = []
 		
-		if (self.is_zipped): handle_in = open(self.file_name, 'rb')
-		else: handle_in = open(self.file_name, 'r')
 		try:
-			with open(tem_file, 'w') as handle_vcf_out:
+			with (open(self.file_name, 'rb') if self.is_zipped else open(self.file_name, 'r')) as handle_in,\
+				open(tem_file, 'w') as handle_vcf_out:
 				vcf_reader = vcf.Reader(handle_in, compressed=self.is_zipped)
 				vcf_reader.infos[TAG_TO_ADD] = _Info(id=TAG_TO_ADD, num=1, type='Integer', 
 					source=None, version=None, desc=\
 					'Has the synchronize position from the reference {} to {}'.format(\
 					lift_over_ligth.reference_from.get_reference_name(),
 					lift_over_ligth.reference_to.get_reference_name()))
 				vcf_write = vcf.VCFWriter(handle_vcf_out, vcf_reader)
@@ -621,15 +616,15 @@
 	
 					### if failed synch save line and continue
 					if (record.CHROM in vect_fail_synch):
 						vcf_write.write_record(record)
 						continue
 						
 					## test chr_name		
-					if (chr_name != record.CHROM):
+					if (not lift_over_ligth.chain.has_chain() and chr_name != record.CHROM):
 						chr_name = record.CHROM
 						if (chr_name.lower() in vect_pass_ref): continue	### chr to not process
 						
 						chr_name_B = lift_over_ligth.reference_to.get_chr_in_genome(chr_name)
 						if chr_name_B is None:
 							vect_fail_synch.append(record.CHROM)
 							continue
@@ -652,16 +647,14 @@
 						vcf_write.write_record(record)
 						lines_parsed += 1
 					else:
 						vcf_write.write_record(record)
 						lines_failed_parse += 1
 		except Exception as e:
 			pass
-		finally:
-			handle_in.close()
 				
 		### compress or copy
 		if (file_result.endswith(".gz")): 
 			self.utils.compress_file(tem_file, file_result)
 			self.utils.remove_file(tem_file)
 		else: self.utils.move_file(tem_file, file_result)
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/run_extra_software.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/run_extra_software.py`

 * *Files 26% similar despite different names*

```diff
@@ -148,9 +148,64 @@
 			raise Exception("Fail to run tabix.\n{}".format(cmd))
 		
 		if (file_to_write is None):
 			vect_out = self.utils.read_text_file(temp_file)
 			self.utils.remove_file(temp_file)
 			self.utils.remove_file(temp_file + ".tbi")
 			return vect_out
+		else:
+			return self.utils.read_text_file(temp_file)
 		return []
 
+	def get_position_by_chain(self, chain_file, seq_name_from, seq_name_to, pos_from,
+					 file_to_write = None, file_to_write_2 = None, file_to_write_3 = None):
+		"""
+		return position by chain name
+		liftOver: liftOver oldFile map.chain newFile unMapped
+		:out -1 if didn't found
+		"""
+		if (not file_to_write is None): temp_file = file_to_write
+		else: temp_file = self.utils.get_temp_file("out_chain", ".txt")
+		if (not file_to_write_2 is None): temp_file_2 = file_to_write_2
+		else: temp_file_2 = self.utils.get_temp_file("out_chain", ".txt")
+		if (not file_to_write_3 is None): temp_file_3 = file_to_write_3
+		else: temp_file_3 = self.utils.get_temp_file("out_chain", ".txt")
+		
+		## create temp file
+		with open(temp_file, 'w') as handle_write:
+			handle_write.write("{} {} {}".format(seq_name_from, pos_from, pos_from))
+			
+		cmd = "{} {} {} {} {}".format(self.software.get_liftOver(),\
+					temp_file, chain_file, temp_file_2, temp_file_3)
+		exist_status = os.system(cmd)
+		if (exist_status != 0):
+			raise Exception("Fail to run chain.\n{}".format(cmd))
+		
+		vect_out = self.utils.read_text_file(temp_file_2)
+		vect_out_not_mapped = self.utils.read_text_file(temp_file_3)
+		if len(vect_out_not_mapped) > 0: return -1
+		if len(vect_out) > 0 and vect_out[0].startswith(seq_name_to): return vect_out[0].split()[1]
+		
+		if (file_to_write is None): self.utils.remove_file(temp_file)
+		if (file_to_write_2 is None): self.utils.remove_file(temp_file_2)
+		if (file_to_write_3 is None): self.utils.remove_file(temp_file_3)
+
+		return -1
+
+	def get_position_by_chain_and_file(self, chain_file, file_in_bed, file_out, file_unmapped):
+		"""
+		return position by chain name
+		liftOver: liftOver oldFile map.chain newFile unMapped
+		:param file_in_bed in bed separated by spaces
+		chr1 743267 743268
+		chr1 766408 766409
+		chr1 773885 773886
+		:out file_out
+		"""
+		cmd = "{} {} {} {} {}".format(self.software.get_liftOver(),\
+					file_in_bed, chain_file, file_out, file_unmapped)
+		exist_status = os.system(cmd)
+		if (exist_status != 0):
+			raise Exception("Fail to run chain.\n{}".format(cmd))
+		
+		return file_out
+
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/software.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/software.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,19 +77,33 @@
 					SoftwareTest.KEY_software_run : 'bgzip', 
 					SoftwareTest.KEY_software_run_get_version : 'bgzip --version', 
 					SoftwareTest.KEY_version : '1.3',
 					SoftwareTest.KEY_version_major_number : SoftwareTest.KEY_version_pass_equal,
 					SoftwareTest.KEY_version_minor_number : SoftwareTest.KEY_version_pass_equal_or_bigger,
 				}
 	
+	SOFTWARE_liftOver_name = 'liftOver'
+	SOFTWARE_liftOver = {
+					SoftwareTest.KEY_software_name : SOFTWARE_liftOver_name, 
+					SoftwareTest.KEY_software_run : 'liftOver', 
+					SoftwareTest.KEY_software_run_get_version : 'liftOver', 
+					SoftwareTest.KEY_version : SoftwareTest.KEY_no_version,
+					SoftwareTest.KEY_version_major_number : SoftwareTest.KEY_version_pass_equal,
+					SoftwareTest.KEY_version_minor_number : SoftwareTest.KEY_version_pass_equal_or_bigger,
+				}
+	
 	### all software that is going to be tested
-	VECT_SOFTWARE_TO_TEST = [SOFTWARE_minimap2,\
+	VECT_SOFTWARE_TO_TEST = [
+			SOFTWARE_minimap2,\
 #			SOFTWARE_blast,\
-			SOFTWARE_bcftools, SOFTWARE_samtools, \
-			SOFTWARE_tabix, SOFTWARE_bgzip, \
+			SOFTWARE_bcftools,\
+			SOFTWARE_samtools,\
+			SOFTWARE_tabix,\
+			SOFTWARE_bgzip,\
+#			SOFTWARE_liftOver,\			### use pyliftover
 #			SOFTWARE_lastz
 			]
 	
 	### software that make the alignment
 	VECT_SOFTWARE_SAVE_ALIGNMENT = [\
 				SOFTWARE_minimap2[SoftwareTest.KEY_software_name],\
 #				SOFTWARE_lastz[SoftwareTest.KEY_software_name],\
@@ -127,49 +141,56 @@
 		return self.SOFTWARE_samtools[SoftwareTest.KEY_software_run]
 	
 	def get_blast(self):
 		return self.SOFTWARE_blast[SoftwareTest.KEY_software_run]
 
 	def get_minimap2(self):
 		return self.SOFTWARE_minimap2[SoftwareTest.KEY_software_run]
-	
+
 	def get_lastz(self):
 		return self.SOFTWARE_lastz[SoftwareTest.KEY_software_run]
-	
+
+	def get_liftOver(self):
+		return self.SOFTWARE_liftOver[SoftwareTest.KEY_software_run]
+
 	def get_application(self, app_name):
 		"""
 		:param name of applciation to return
 		:out application to run in OS
 		"""
 		for software in self.VECT_SOFTWARE_TO_TEST:
 			if software[SoftwareTest.KEY_software_name] == app_name:
 				return software[SoftwareTest.KEY_software_run]
 		raise Exception("Error: could not find this software '{}' in available softwares.".format(app_name))
 
 	def test_softwares(self):
 		"""
 		test all software, if fails exit the application
 		"""
-		
+
 		for software in self.VECT_SOFTWARE_TO_TEST:
 			result = self.test_software(software)
 			if result:
-				print("Software: '{}' version: '{}' is OK".format(
+				if software[Software.KEY_version] == self.KEY_no_version:
+					print("Software: '{}' version: is OK".format(
+						software[Software.KEY_software_name]))
+				else: print("Software: '{}' version: '{}' is OK".format(
 					software[Software.KEY_software_name], software[Software.KEY_version]))
 			else:
 				raise Exception("Error: software '{}' has a lower version than '{}'".format(
 					software[Software.KEY_software_name], software[Software.KEY_version]))
 
 	def print_all(self):
 		"""
 		print a list of a software need
 		"""
 		print("Software{: <10}version".format(" "))
 		for software in self.VECT_SOFTWARE_TO_TEST:
 			print("{: <18}{}".format(
 				software[Software.KEY_software_name], software[Software.KEY_version]))
-			
+
+
 if __name__ == '__main__':
 	
 	software = Software()
 	software.print_all()
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/read_gff.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/read_gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 	
 					### if failed synch save line and continue
 					if (line_gff["seqid"].lower() in vect_fail_synch):
 						handle_out.write(line_gff["line_raw"])
 						continue
 				
 					## test chr_name					
-					if (chr_name != line_gff["seqid"]):
+					if (not lift_over_ligth.chain.has_chain() and chr_name != line_gff["seqid"]):
 						chr_name = line_gff["seqid"]
 						if (chr_name.lower() in vect_pass_ref): continue	### chr to not process
 	
 						#### get chromosome name in other reference						
 						chr_name_B = lift_over_ligth.reference_to.get_chr_in_genome(chr_name)
 						if chr_name_B is None:
 							vect_fail_synch.append(chr_name)
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/lift_over_simple.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/lift_over_simple.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Created on 16/12/2019
 
 @author: mmp
 '''
 import sys, os
 from PHASEfilter.lib.utils.util import Utils, Cigar, CountLength, NucleotideCodes
+from PHASEfilter.lib.utils.chain import Chain
 from PHASEfilter.lib.utils.blast_two_sequences import BlastTwoSequences
 from PHASEfilter.lib.utils.lastz_two_sequences import LastzTwoSequences
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from PHASEfilter.lib.utils.software import Software
 from typing import Union
@@ -401,27 +402,30 @@
 	OVERLAP_SEQUENCE_SIZE_real = 1000
 	
 	PREFIX_SEQ_NAME_FROM = "from_"
 	PREFIX_SEQ_NAME_TO = "to_"
 	
 	software = Software()
 
-	def __init__(self, reference_from, reference_to, work_directory, impose_minimap2_only = False, b_test_mode = False):
+	def __init__(self, reference_from, reference_to, work_directory, chain_name = None,
+				impose_minimap2_only = False, threading = 1, b_test_mode = False):
 		'''
 		Constructor
 		'''
 		self.utils = Utils("synchronize")
 		
 		self.reference_from = reference_from
 		self.reference_to = reference_to
 		self.b_test_mode = b_test_mode
 		self.impose_minimap2_only = impose_minimap2_only
 		self.work_directory = work_directory
+		self.chain = Chain(chain_name)					## if it has a chain is mandatory
 		self.dt_chain = {}
 		self.dt_chain_best_method = {}
+		self.threading = threading
 	
 	def _get_temp_files(self, seq_name_from, seq_name_to, star_pos_from, star_pos_to):
 		"""
 		get temp files
 		"""
 		return (self._get_temp_file(seq_name_from, self.reference_from, star_pos_from),
 			self._get_temp_file(seq_name_to, self.reference_to, star_pos_to))
@@ -493,30 +497,46 @@
 		"""
 		:param pos_from, position "from" at one base in first sequence (source A)
 		:returns (position in second sequence (hit B), if does not have position return left most position)
 			-1 to no position
 			
 		IMPORTANT - don't give the best
 		"""
-		key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
-		if (software_name in self.dt_chain and key_chain_name in self.dt_chain[software_name]):
-			return self.dt_chain[software_name][key_chain_name].get_position_from_2_to(pos_from)
+		if (self.chain.has_chain()):	## it is mandatory
+			### run chain
+			try:
+				position = self.chain.get_position_by_chain(seq_name_from, seq_name_to, pos_from)
+				return (position, -1)
+			except:
+				return (-1, -1) 
+		else:
+			key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
+			if (software_name in self.dt_chain and key_chain_name in self.dt_chain[software_name]):
+				return self.dt_chain[software_name][key_chain_name].get_position_from_2_to(pos_from)
 		return (-1, -1)
 
 	def get_best_pos_in_target(self, seq_name_from: str, seq_name_to: str, pos_from: int) -> Union[int, None]:
 		"""
 		:param pos_from, position "from" at one base in first sequence (source A)
 		:returns (position in second sequence (hit B), if does not have position return left most position)
 			-1 to no position
 		"""
-		key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
-		
-		if (self.dt_chain_best_method[key_chain_name] in self.dt_chain and 
-				key_chain_name in self.dt_chain[self.dt_chain_best_method[key_chain_name]]):
-			return self.dt_chain[self.dt_chain_best_method[key_chain_name]][key_chain_name].get_position_from_2_to(pos_from)
+		if (self.chain.has_chain()):	## it is mandatory
+			### run chain
+			try:
+				position = self.chain.get_position_by_chain(seq_name_from, seq_name_to, pos_from)
+				return (position, -1)
+			except:
+				return (-1, -1) 
+		else:
+			key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
+			
+			if (self.dt_chain_best_method[key_chain_name] in self.dt_chain and 
+					key_chain_name in self.dt_chain[self.dt_chain_best_method[key_chain_name]]):
+				return self.dt_chain[self.dt_chain_best_method[key_chain_name]][key_chain_name].get_position_from_2_to(pos_from)
 		return (-1, -1)
 
 	def _run_minimap2(self, file_from, file_to):
 		"""
 		Create a file parsed from SAM from the minimap2
 		Out 
 		"""
@@ -524,17 +544,18 @@
 		### out file
 		temp_file_out = self.utils.get_temp_file("minimap_o_file", ".sam")
 		temp_file_out_2 = self.utils.get_temp_file("minimap_o_file_2", ".sam")
 
 		### minimap2 -L ca22_1A.fasta ca22_1B.fasta -a -o temp.sam
 		## sort by MappingScore and choose the best alignment
 		## dont print 256 - "not primary alignment" and 2048 - "supplementary alignment" 
-		cmd = "{} --secondary=no -H -L {} {} -a -o {}; tail -n +3 {} | ".format(
+		cmd = "{} --secondary=no -H -L {} {} -a -o {} -t {}; tail -n +3 {} | ".format(
 			self.software.get_minimap2(), \
-			file_from, file_to, temp_file_out_2, temp_file_out_2)
+			file_from, file_to, temp_file_out_2,
+			self.threading, temp_file_out_2)
 		cmd += "awk '{ " +  'print($2, " ", $4, " ", $6)' + " } '"		### to reduce the output size 
 		cmd += " > {}".format(temp_file_out)
 
 		exist_status = os.system(cmd)
 		if (exist_status != 0):
 			os.unlink(temp_file_out)
 			raise Exception("Fail to run minimap2")
@@ -624,14 +645,18 @@
 		return count_length.is_100_percent(self.reference_from.get_chr_length(seq_name_from),\
 								self.reference_to.get_chr_length(seq_name_to))
 
 	def get_percent_alignment(self, method, seq_name_from, seq_name_to):
 		"""
 		:out percentage of alignment
 		"""
+		### return no value if chain was passed
+		if self.chain.has_chain():
+			return self.get_percent_alignment_chain(seq_name_from, seq_name_to)
+		
 		count_length = self.get_count_cigar_length(method, seq_name_from, seq_name_to)
 		if count_length is None: return False
 		return count_length.get_percentage_coverage(self.reference_from.get_chr_length(seq_name_from),\
 								self.reference_to.get_chr_length(seq_name_to))
 				
 	def get_method(self, seq_name_from, seq_name_to):
 		"""
@@ -645,24 +670,34 @@
 				
 		return ",".join(vect_methods_out)
 
 	def get_method_best_method(self, seq_name_from, seq_name_to):
 		"""
 		get best method
 		"""
+		### return chain method if chain was passed
+		if self.chain.has_chain(): return "Chain"
+		
 		key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
 		return self.dt_chain_best_method[key_chain_name] if key_chain_name in self.dt_chain_best_method else ""
 	
 	def synchronize_sequences(self, seq_name_from, seq_name_to):
 		"""
 		:param seq_from -> name of sequence from 
 		:param seq_to -> name of sequence to, target 
 		:param work_directory place to save the chain, next run test if exist to read it instead fo run it 
 		:out { '<seq_name_from>_<seq_name_to>' : }
 		"""
+		
+		if self.chain.has_chain():
+			if self.chain.has_chain_name(seq_name_from, seq_name_to):
+				print("Not necessary to synchronize genome, chain available")
+				return True
+			print("Chain not available for chromosome from: {}  to: {}".format(seq_name_from, seq_name_to))
+			return False
 
 		### get key chan name		
 		key_chain_name = self._get_key_chain_name(seq_name_from, seq_name_to)
 		if key_chain_name in self.dt_chain: return True				## already in memory
 		
 		### get match positions to cut
 		try:
@@ -905,15 +940,15 @@
 						else:
 							handle_out.write(line)
 						
 						### 
 						if (len(last_line) == len(lst_data[1])):
 							sz_match_line = ""
 							for _ in range(len(last_line)):
-								if last_line[_] == lst_data[1][_] and last_line[_] != "-" \
+								if last_line[_].upper() == lst_data[1][_].upper() and last_line[_] != "-" \
 									and lst_data[1][_] != "-": sz_match_line += "*"
 								else: sz_match_line += " "
 							handle_out.write(space_before_seq + sz_match_line + "\n")
 						b_first = True
 			
 		self.utils.remove_file(temp_file)
 		return out_file
@@ -1002,10 +1037,229 @@
 			handle_out.write("Query start\tCigar\n")
 			for alignment in self.dt_chain[method][key_chain_name].get_vect_alignments():
 				handle_out.write("{}\t{}\n".format(alignment.start_query,
 						"\t".join(alignment.get_vect_cigar())))
 		return out_file
 
 
+	def create_alignment_file_chain(self, out_file, seq_name_from, seq_name_to, b_test = False):
+		"""
+		Create a file with the alignment, format clustal
+		:out None is something goes wrong
+		
+		size dt dq
+		size -- the size of the ungapped alignment
+		dt -- the difference between the end of this block and the beginning of the next block (reference/target sequence)
+		dq -- the difference between the end of this block and the beginning of the next block (query sequence)
+		
+		## from
+		chain 203372674 Ca22chr2A_C_albicans_SC5314 2231883 + 0 2231883 Ca22chr2B_C_albicans_SC5314 2231750 + 0 2231750 3
+		12522	14	14
+		55	1	0
+		55	1	1
+		224	2	2
+		21	1	1
+		## to
+		(0, 12522, 0)
+		(12536, 12591, 12536)
+		(12592, 12647, 12591)
+		12648 12872 12647
+		
+		## pass chainto block
+		while len(fields) == 3:
+            size, sgap, tgap = int(fields[0]), int(fields[1]), int(fields[2])
+            self.blocks.append((sfrom, sfrom+size, tfrom))
+            sfrom += size + sgap
+            tfrom += size + tgap
+		"""
+		b_print = False
 
+		## try to find chain with best score
+		## for each alignment
+		dt_fail_position = {}
+		for first_count, chain in enumerate(self.chain.get_chains(seq_name_from, seq_name_to)):
+		
+			## sequences...
+			seq_from = ""
+			seq_to = ""
+				
+			# Positions in the sequences
+			last_postion_sfrom = -1
+			last_postion_tfrom = -1
+			for second_count, block in enumerate(chain.blocks):
+				
+				if b_print:
+					seq_to += "--" + str(second_count) * 4
+					seq_from += "--" + str(second_count) * 4
+					print("###################################")
+					print("Count: ", second_count, "block: ", block[0], block[1], block[2], "Seq: ", len(seq_to), len(seq_from))
+				
+				### insert match parts
+				tfrom_size = (block[1] - block[0]) + block[2]
+				if (second_count > 0):
+					## add dash
+					if (block[2] - last_postion_tfrom) < (block[0] - last_postion_sfrom):
+						seq_to += "-" * ((block[0] - last_postion_sfrom) - (block[2] - last_postion_tfrom))
+						if b_print: print("add dot to: ", ((block[0] - last_postion_sfrom) - (block[2] - last_postion_tfrom)))
+					
+					## add dash
+					if (block[2] - last_postion_tfrom) > (block[0] - last_postion_sfrom):
+						seq_from += "-" * ((block[2] - last_postion_tfrom) - (block[0] - last_postion_sfrom))
+						if b_print: print("add dot from: ", (block[2] - last_postion_tfrom) - (block[0] - last_postion_sfrom))
+							
+					if block[2] > last_postion_tfrom:
+						if b_print: 
+							print(block[2] - last_postion_tfrom)
+							print("gap from: ", str(self.reference_from.reference_dict[seq_name_from].seq)[last_postion_tfrom: block[2]])
+						seq_from += str(self.reference_from.reference_dict[seq_name_from].seq)[last_postion_tfrom: block[2]]
+				seq_from += str(self.reference_from.reference_dict[seq_name_from].seq)[block[2]: tfrom_size]
+				if b_print: print("from: ", str(self.reference_from.reference_dict[seq_name_from].seq)[block[2]: tfrom_size][:5])
+				
+				if (second_count > 0):
+					if block[0] > last_postion_sfrom:
+						if b_print: 
+							print(block[0] - last_postion_sfrom)
+							print("gap to: ", str(self.reference_to.reference_dict[seq_name_to].seq)[last_postion_sfrom: block[0]])
+						seq_to += str(self.reference_to.reference_dict[seq_name_to].seq)[last_postion_sfrom: block[0]]
+				seq_to += str(self.reference_to.reference_dict[seq_name_to].seq)[block[0]: block[1]]
+				if b_print: print("to: ", str(self.reference_to.reference_dict[seq_name_to].seq)[block[0]: block[1]][:5])
+				
+				last_postion_sfrom = block[1]				## sfrom+size
+				last_postion_tfrom = tfrom_size		## tfrom+size
+				
+				## it is only testing
+				if b_test and second_count > 50: break
 
+			### save data
+			temp_file = self.utils.get_temp_file("set_numbers_align", ".aln")
+			seq_name_from_temp = seq_name_from
+			if (seq_name_from_temp == seq_name_to): seq_name_from_temp = seq_name_from_temp + "_from"
+			with open(temp_file, 'w') as handle_out:
+				if (len(seq_from) > len(seq_to)): seq_to += "-" * (len(seq_from) - len(seq_to))
+				elif (len(seq_from) < len(seq_to)): seq_from += "-" * (len(seq_to) - len(seq_from))
+				vect_data = [SeqRecord(Seq(seq_from), id = seq_name_from_temp, description=""),
+								SeqRecord(Seq(seq_to), id = seq_name_to, description="")
+							]
+				
+				SeqIO.write(vect_data, handle_out, "clustal")
+		
+			### change the name of the file
+			out_file_rename = out_file
+			if (len(self.chain.get_chains(seq_name_from, seq_name_to)) > 1):
+				out_file_rename = out_file.replace(".aln", "_alignment_{}.aln".format(first_count + 1))
+				
+			### set numbers
+			with open(temp_file) as handle_in, open(out_file_rename, 'w') as handle_out:
+				b_first = True
+				(count_first, count_second) = (chain.source_start, chain.target_start)
+	
+				count_line_total, hit_divergent = 0, -1
+				space_before_seq = ""
+				for line in handle_in:
+					sz_temp = line.strip()
+					if (line.startswith("CLUSTAL X") or len(sz_temp) == 0):
+						handle_out.write(line)
+						continue
+	
+					if (b_first):
+						lst_data = sz_temp.split()
+						if len(lst_data) == 2:
+							last_line = lst_data[1]
+							dash_count = last_line.count('-')
+							count_first += len(last_line) - dash_count
+							if (count_first == 0): handle_out.write(line)
+							else: handle_out.write('{}{:>10}\n'. format(sz_temp, count_first))
+							
+							### calculate space before sequences
+							if (len(space_before_seq) == 0):
+								space_before_seq = " " * line.index(lst_data[1])
+						else:
+							handle_out.write(line)
+						b_first = False
+					else:
+						lst_data = sz_temp.split()
+						if len(lst_data) == 2:
+							dash_count = lst_data[1].count('-')
+							count_second += len(lst_data[1]) - dash_count
+							if (count_second == 0): handle_out.write(line)
+							else: handle_out.write('{}{:>10}\n'. format(sz_temp, count_second))
+						else:
+							handle_out.write(line)
+						
+						### 
+						if (len(last_line) == len(lst_data[1])):
+							sz_match_line = ""
+							for _ in range(len(last_line)):
+								if (count_line_total + _) in dt_fail_position:
+									hit_divergent = count_line_total + _
+									sz_match_line += "+"
+								elif hit_divergent in dt_fail_position and dt_fail_position[hit_divergent] > count_line_total + _:
+									sz_match_line += "+"
+								elif last_line[_].upper() == lst_data[1][_].upper() and last_line[_] != "-" \
+									and lst_data[1][_] != "-":
+									hit_divergent = -1
+									sz_match_line += "*"
+								else: sz_match_line += " "
+							handle_out.write(space_before_seq + sz_match_line + "\n")
+							count_line_total += len(lst_data[1]) 
+						b_first = True
+
+		return out_file_rename
+
+
+	def get_percent_alignment_chain(self, seq_name_from, seq_name_to):
+		"""
+		Create a file with the alignment, format clustal
+		:out None is something goes wrong
+		
+		size dt dq
+		size -- the size of the ungapped alignment
+		dt -- the difference between the end of this block and the beginning of the next block (reference/target sequence)
+		dq -- the difference between the end of this block and the beginning of the next block (query sequence)
+		
+		## from
+		chain 203372674 Ca22chr2A_C_albicans_SC5314 2231883 + 0 2231883 Ca22chr2B_C_albicans_SC5314 2231750 + 0 2231750 3
+		12522	14	14
+		55	1	0
+		55	1	1
+		224	2	2
+		21	1	1
+		## to
+		(0, 12522, 0)
+		(12536, 12591, 12536)
+		(12592, 12647, 12591)
+		12648 12872 12647
+		
+		## pass chainto block
+		while len(fields) == 3:
+            size, sgap, tgap = int(fields[0]), int(fields[1]), int(fields[2])
+            self.blocks.append((sfrom, sfrom+size, tfrom))
+            sfrom += size + sgap
+            tfrom += size + tgap
+		"""
+
+		## for each alignment
+		total_size_genome = 0
+		total_fiz_gap = 0
+		for first_count, chain in enumerate(self.chain.get_chains(seq_name_from, seq_name_to)):
+		
+			# Positions in the sequences
+			last_postion_sfrom = -1
+			last_postion_tfrom = -1
+			total_size_genome += (chain.source_end - chain.source_start) + (chain.target_end - chain.target_start) 
+			for second_count, block in enumerate(chain.blocks):
+				
+				### insert match parts
+				tfrom_size = (block[1] - block[0]) + block[2]
+				if (second_count > 0):
+					## add dash
+					if (block[2] - last_postion_tfrom) < (block[0] - last_postion_sfrom):
+						total_fiz_gap +=  ((block[0] - last_postion_sfrom) - (block[2] - last_postion_tfrom))
+					
+					## add dash
+					if (block[2] - last_postion_tfrom) > (block[0] - last_postion_sfrom):
+						total_fiz_gap += ((block[2] - last_postion_tfrom) - (block[0] - last_postion_sfrom))
+				
+				last_postion_sfrom = block[1]		## sfrom+size
+				last_postion_tfrom = tfrom_size		## tfrom+size
 
+		return ((total_size_genome - total_fiz_gap) / total_size_genome) * 100
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/utils/lastz_two_sequences.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/utils/lastz_two_sequences.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/process/process_genomes.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/process/process_genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 '''
 from PHASEfilter.lib.utils.util import Utils
 from PHASEfilter.lib.utils.reference import Reference
 from PHASEfilter.lib.utils.vcf_process import VcfProcess, CountAlleles
 from PHASEfilter.lib.utils.lift_over_simple import LiftOverLight
 from PHASEfilter.lib.utils.run_extra_software import RunExtraSoftware
 import os
+from alembic.ddl import oracle
 
 class ProcessTwoGenomes(object):
 	
 	utils = Utils("synchronize")
 	run_extra_software = RunExtraSoftware()
 	
 	def __init__(self, reference_1, reference_2, vcf_1, vcf_2, threshold_heterozygous_ad,
-				threshold_remove_variant_ad, outfile_vcf):
+				threshold_remove_variant_ad, outfile_vcf, chain_from_to):
 		"""
 		set the data
 		"""
 		### read references
 		self.reference_1 = Reference(reference_1)
 		self.reference_2 = Reference(reference_2)
 		self.vcf_1 = vcf_1
 		self.vcf_2 = vcf_2
 		self.outfile_vcf = outfile_vcf
 		self.threshold_heterozygous_ad = threshold_heterozygous_ad
 		self.threshold_remove_variant_ad = threshold_remove_variant_ad
+		self.chain_name = chain_from_to
 	
 	def get_report_file(self):
 		"""
 		:out get file name where report will be saved
 		"""
 		return os.path.join(os.path.dirname(self.outfile_vcf),\
 			"{}_{}.txt".format("report",
@@ -91,15 +93,19 @@
 			
 			### processing chromosomes
 			vect_temp_report_file.append([chr_name_A, chr_name_B, report_out_temp])
 			(has_vcf_results, has_vcf_removed_results, has_vcf_loh_results) = \
 							self.process_chromosome(chr_name_A, chr_name_B, vcf_out_temp,
 							vcf_out_removed_temp, vcf_out_LOH_temp, report_out_temp,
 							print_results)
-
+			
+			### test if everything went well
+			if has_vcf_results is None or has_vcf_removed_results is None or \
+				has_vcf_loh_results is None: continue
+				
 			### test if has results
 			if (has_vcf_results):			### make gzip file
 				self.run_extra_software.make_bgz(vcf_out_temp, vcf_out_temp + ".gz")
 				has_vcf_results_global = True
 			else:
 				self.utils.remove_file(vcf_out_temp)
 				
@@ -165,16 +171,19 @@
 		process by chromosome
 		:out has vcf result file
 		"""
 		print("*" * 50 + "\n" + "*" * 50 + "\nStart processing {} chr: {} ->  {} chr: {}".format(self.reference_1.get_reference_name(),\
 					chr_name_A, self.reference_2.get_reference_name(), chr_name_B))
 		temp_work_dir = self.utils.get_temp_dir()
 		
-		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir)
-		lift_over_ligth.synchronize_sequences(chr_name_A, chr_name_B)
+		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir, self.chain_name)
+		
+		### test if synchronization was well done
+		if not lift_over_ligth.synchronize_sequences(chr_name_A, chr_name_B):
+			return (None, None, None)
 		
 		### get only vcf sequences from chr_name_A
 		(vcf_1_only_chr, number_of_records_1) = self.run_extra_software.get_vcf_with_only_chr(self.vcf_1, chr_name_A, temp_work_dir)
 		(vcf_2_only_chr, number_of_records_2) = self.run_extra_software.get_vcf_with_only_chr(self.vcf_2, chr_name_B, temp_work_dir)
 		
 		## all VCF files has variants
 		has_result_file = False
@@ -199,22 +208,24 @@
 			count_alleles.add_allele(number_of_records_2)
 			self.run_extra_software.make_unzip_bgz(vcf_1_only_chr, vcf_out_temp)
 			has_result_file = True
 
 		### write the report
 		best_method = lift_over_ligth.get_method_best_method(chr_name_A, chr_name_B)
 		with open(report_out_temp, 'w') as handle_write:
+			f_percent_alignment = lift_over_ligth.get_percent_alignment(best_method, chr_name_A, chr_name_B)
+			if self.utils.is_float(f_percent_alignment): f_percent_alignment = "{:.2f}".format(f_percent_alignment)
 			handle_write.write(str(count_alleles) +\
-					"\t{}\t{:.2f}\n".format(best_method,\
-					lift_over_ligth.get_percent_alignment(best_method, chr_name_A, chr_name_B)))
+					"\t{}\t{}\n".format(best_method, f_percent_alignment))
 
-			
 		### remove temp files
 		self.utils.remove_dir(temp_work_dir)
 		self.utils.remove_file(vcf_1_only_chr)
 		if (not vcf_1_only_chr is None): self.utils.remove_file(vcf_1_only_chr + ".tbi")
 		self.utils.remove_file(vcf_2_only_chr)
 		if (not vcf_2_only_chr is None): self.utils.remove_file(vcf_2_only_chr + ".tbi")
 		print("Processed {} chr: {} ->  {} chr: {}".format(self.reference_1.get_reference_name(),\
 					chr_name_A, self.reference_2.get_reference_name(), chr_name_B))
 		return (has_result_file, has_vcf_removed_results, has_vcf_loh_results)
-		
+
+
+
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/lib/process/process_references.py` & `PHASEfilter-1.1.0/PHASEfilter/lib/process/process_references.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 Created on 06/12/2019
 
 @author: mmp
 '''
 from PHASEfilter.lib.utils.util import Utils, NucleotideCodes
+from PHASEfilter.lib.utils.chain import Chain
 from PHASEfilter.lib.utils.reference import Reference
 from PHASEfilter.lib.utils.lift_over_simple import LiftOverLight
 from PHASEfilter.lib.utils.run_extra_software import RunExtraSoftware
 from PHASEfilter.lib.utils.read_gff import ReadGFF
 from PHASEfilter.lib.utils.software import Software
 from PHASEfilter.lib.utils.vcf_process import VcfProcess
 from Bio import SeqIO
@@ -17,28 +18,30 @@
 import os
 
 class ProcessTwoReferences(object):
 	
 	utils = Utils("synchronize")
 	run_extra_software = RunExtraSoftware()
 	
-	def __init__(self, reference_1, reference_2, outfile_report, out_path_alignments = None,
-				out_new_reference = None):
+	def __init__(self, reference_1, reference_2, outfile_report, chain_name = None, out_path_alignments = None,
+				out_new_reference = None, threading = 1):
 		"""
 		set the data
 		:param  reference_1 reference 1
 		:param  reference_2 reference 2
 		:param  outfile_report report file
 		"""
 		### read references
 		self.reference_1 = Reference(reference_1)
 		self.reference_2 = Reference(reference_2)
 		self.outfile = outfile_report
 		self.out_path_alignments = out_path_alignments
 		self.out_new_reference = out_new_reference
+		self.chain_name = chain_name
+		self.threading = threading
 
 	def process(self, vect_pass_ref = []):
 		"""
 		:param vect_pass_ref - chromosomes to not process
 		compare the alignments available
 		"""
 		print("\nStart processing....")
@@ -108,15 +111,16 @@
 		
 		print("*" * 50 + "\n" + "*" * 50 + "\nStart processing {} chr: {} ->  {} chr: {}".format(self.reference_1.get_reference_name(),\
 					chr_name_A, self.reference_2.get_reference_name(), chr_name_B))
 		handle_write.write("{}\t{}\t".format(chr_name_A, chr_name_B))
 		
 		temp_work_dir = self.utils.get_temp_dir()
 		
-		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir)
+		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir,
+									 None, False, self.threading)
 		lift_over_ligth.synchronize_sequences_all_methods(chr_name_A, chr_name_B)
 		
 		vect_out = []
 		for software in Software.VECT_SOFTWARE_SAVE_ALIGNMENT:
 			count_elements = lift_over_ligth.get_count_cigar_length(software, chr_name_A, chr_name_B)
 			
 			if (count_elements == None):
@@ -178,15 +182,15 @@
 		Tag add: StartHit and EndHit
 		"""
 		print("Start processing {} -> {}".format(self.reference_1.get_reference_name(),\
 					self.reference_2.get_reference_name()))
 
 		temp_work_dir = self.utils.get_temp_dir()		
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir, impose_minimap2_only, False)
+		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir, self.chain_name, impose_minimap2_only, False)
 		
 		read_gff = ReadGFF(gff_file_to_parse)
 		(lines_parsed, lines_failed_parse, vect_fail_synch) = read_gff.parse_gff(self.outfile, vect_type_to_process, vect_pass_ref, lift_over_ligth)
 		
 		print("Lines parsed: {}   Lines Failed to parse: {}".format(lines_parsed, lines_failed_parse))
 		if (len(vect_fail_synch) > 0): print("Chromosomes that Failed to synch.: {}".format(",".join(vect_fail_synch)))
 		self.utils.remove_dir(temp_work_dir)
@@ -199,15 +203,15 @@
 		Info add: HIT_POS
 		"""
 		print("Start processing {} -> {}".format(self.reference_1.get_reference_name(),\
 					self.reference_2.get_reference_name()))
 
 		temp_work_dir = self.utils.get_temp_dir()		
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir, impose_minimap2_only, False)
+		lift_over_ligth = LiftOverLight(self.reference_1, self.reference_2, temp_work_dir, self.chain_name, impose_minimap2_only, False)
 		
 		read_vcf = VcfProcess(vcf_file_to_parse, -1.0, -1.0)
 		(lines_parsed, lines_failed_parse, vect_fail_synch) = read_vcf.parse_vcf(self.outfile, vect_pass_ref, lift_over_ligth)
 		
 		print("Lines parsed: {}   Lines Failed to parse: {}".format(lines_parsed, lines_failed_parse))
 		if (len(vect_fail_synch) > 0): print("Chromosomes that Failed to synch.: {}".format(",".join(vect_fail_synch)))
 		self.utils.remove_dir(temp_work_dir)
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_lift_over.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_lift_over.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/first_file_b.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("A", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("A", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -161,15 +161,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/second_file_b.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = True
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("A", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("B", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -193,15 +193,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/second_file_a.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = True
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("B", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("A", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -228,15 +228,15 @@
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		seq_name_a = "chrX"
 		seq_name_b = "chrX_S01"
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 		self.assertEqual(Software.SOFTWARE_minimap2_name, lift_over_ligth.get_best_algorithm(seq_name_a, seq_name_b))
 	
 		temp_out = utils.get_temp_file("out_sync_saccharo", ".txt")
 		process_two_references = ProcessTwoReferences(seq_file_name_a, seq_file_name_b, temp_out)
 		process_two_references.process()
 	
@@ -272,15 +272,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/referenceSaccharo/S01_chrX_small.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences("chrX", "chrX")
 		self.assertEqual(Software.SOFTWARE_minimap2_name, lift_over_ligth.get_best_algorithm("chrX", "chrX"))
 		
 		self.assertTrue(['19M1D8M1I32M14I13M1I6M1I28M23I22M1I126M2D117M3I29M1I1694M', '99M132D60M'], \
 			lift_over_ligth.get_cigar_string(Software.SOFTWARE_lastz_name, "chrX", "chrX"))
 		self.assertEqual((261, -1), lift_over_ligth.get_best_pos_in_target("chrX", "chrX", 48))
 		self.assertEqual((438, -1), lift_over_ligth.get_best_pos_in_target("chrX", "chrX", 200))
@@ -310,21 +310,21 @@
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		seq_name_a = "chrX"
 		seq_name_b = "chrX_S01"
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 		self.assertEqual(Software.SOFTWARE_minimap2_name, lift_over_ligth.get_best_algorithm(seq_name_a, seq_name_b))
 	
 		temp_out_report = utils.get_temp_file_with_path(temp_work_dir, "out_sync_saccharo", ".txt")
 		temp_out_sync = utils.get_temp_file_with_path(temp_work_dir, "out_sync_saccharo", ".fasta")
-		process_two_references = ProcessTwoReferences(seq_file_name_a, seq_file_name_b, temp_out_report, None, temp_out_sync)
+		process_two_references = ProcessTwoReferences(seq_file_name_a, seq_file_name_b, temp_out_report, None, None, temp_out_sync)
 		process_two_references.process()
 
 		### test reference	
 		out_result_expected = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files/referenceSaccharo/out_new_ref_saccharo_X.fasta')
 		temp_diff = utils.get_temp_file_with_path(temp_work_dir, "diff_file", ".txt")
 		cmd = "diff {} {} > {}".format(temp_out_sync, out_result_expected, temp_diff)
 		os.system(cmd)
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_reference.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_process_genomes.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_process_genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		outfile_vcf = self.utils.get_temp_file("dont_care_", ".vcf")
 		outfile_vcf_removed = self.utils.get_temp_file("dont_care_2", ".vcf")
 		outfile_vcf_LOH_removed = self.utils.get_temp_file("dont_care_3", ".vcf")
 		report_out_temp = self.utils.get_temp_file("report_temp_", ".txt")
 		threshold_ad = -1.0
 		threshold_remove_variant_ad = -1.0
 		process_two_genomes = ProcessTwoGenomes(seq_file_name_a, seq_file_name_b, vcf_1, vcf_2, threshold_ad,
-						threshold_remove_variant_ad, outfile_vcf)
+						threshold_remove_variant_ad, outfile_vcf, None)
 	
 		chr_name_A = "Ca22chr1A_C_albicans_SC5314"
 		chr_name_B = "Ca22chr1B_C_albicans_SC5314"
 		print_results = False
 		self.assertEqual((True, True, False), process_two_genomes.process_chromosome(chr_name_A, chr_name_B, outfile_vcf,
 									outfile_vcf_removed, outfile_vcf_LOH_removed, report_out_temp, print_results))
 	
@@ -64,15 +64,15 @@
 		outfile_vcf = self.utils.get_temp_file("dont_care_", ".vcf")
 		outfile_vcf_removed = self.utils.get_temp_file("dont_care_2", ".vcf")
 		outfile_vcf_LOH_removed = self.utils.get_temp_file("dont_care_3", ".vcf")
 		report_out_temp = self.utils.get_temp_file("report_temp_", ".txt")
 		threshold_ad = 0.01
 		threshold_remove_variant_ad = -1.0
 		process_two_genomes = ProcessTwoGenomes(seq_file_name_a, seq_file_name_b, vcf_1, vcf_2, threshold_ad,
-						threshold_remove_variant_ad, outfile_vcf)
+						threshold_remove_variant_ad, outfile_vcf, None)
 	
 		chr_name_A = "Ca22chr1A_C_albicans_SC5314"
 		chr_name_B = "Ca22chr2B_C_albicans_SC5314"
 		print_results = False
 		self.assertEqual((True, False, False), process_two_genomes.process_chromosome(chr_name_A, chr_name_B, outfile_vcf,
 									outfile_vcf_removed, outfile_vcf_LOH_removed, report_out_temp, print_results))
 	
@@ -102,15 +102,15 @@
 		outfile_vcf = self.utils.get_temp_file("dont_care_", ".vcf")
 		outfile_vcf_removed = self.utils.get_temp_file("dont_care_2", ".vcf")
 		outfile_vcf_LOH_removed = self.utils.get_temp_file("dont_care_3", ".vcf")
 		report_out_temp = self.utils.get_temp_file("report_temp_", ".txt")
 		threshold_ad = 0.01
 		threshold_remove_variant_ad = -1.0
 		process_two_genomes = ProcessTwoGenomes(seq_file_name_a, seq_file_name_b, vcf_1, vcf_2, threshold_ad,
-						threshold_remove_variant_ad, outfile_vcf)
+						threshold_remove_variant_ad, outfile_vcf, None)
 	
 		chr_name_A = "Ca22chr2A_C_albicans_SC5314"
 		chr_name_B = "Ca22chr1B_C_albicans_SC5314"
 		print_results = False
 		self.assertEqual((False, False, False), process_two_genomes.process_chromosome(chr_name_A, chr_name_B, outfile_vcf,
 							outfile_vcf_removed, outfile_vcf_LOH_removed, report_out_temp, print_results))
 	
@@ -140,15 +140,15 @@
 		outfile_vcf = self.utils.get_temp_file("dont_care_", ".vcf")
 		outfile_vcf_removed = self.utils.get_temp_file("dont_care_2", ".vcf")
 		outfile_vcf_LOH_removed = self.utils.get_temp_file("dont_care_3", ".vcf")
 		report_out_temp = self.utils.get_temp_file("report_temp_", ".txt")
 		threshold_ad = 0.01
 		threshold_remove_variant_ad = -1.0
 		process_two_genomes = ProcessTwoGenomes(seq_file_name_a, seq_file_name_b, vcf_1, vcf_2, threshold_ad,
-						threshold_remove_variant_ad, outfile_vcf)
+						threshold_remove_variant_ad, outfile_vcf, None)
 	
 		chr_name_A = "Ca22chr2A_C_albicans_SC5314"
 		chr_name_B = "Ca22chr2B_C_albicans_SC5314"
 		print_results = False
 		self.assertEqual((False, False, False), process_two_genomes.process_chromosome(chr_name_A, chr_name_B, outfile_vcf,
 							outfile_vcf_removed, outfile_vcf_LOH_removed, report_out_temp, print_results))
 	
@@ -178,15 +178,15 @@
 		outfile_vcf = self.utils.get_temp_file("dont_care_", ".vcf")
 		outfile_vcf_removed = self.utils.get_temp_file("dont_care_2", ".vcf")
 		outfile_vcf_LOH_removed = self.utils.get_temp_file("dont_care_3", ".vcf")
 		report_out_temp = self.utils.get_temp_file("report_temp_", ".txt")
 		threshold_ad = 0.3
 		threshold_remove_variant_ad = 0.2
 		process_two_genomes = ProcessTwoGenomes(seq_file_name_a, seq_file_name_b, vcf_1, vcf_2, threshold_ad,
-						threshold_remove_variant_ad, outfile_vcf)
+						threshold_remove_variant_ad, outfile_vcf, None)
 
 		chr_name_A = "Ca22chr1A_C_albicans_SC5314"
 		chr_name_B = "Ca22chr1B_C_albicans_SC5314"
 		print_results = False
 		self.assertEqual((True, True, True), process_two_genomes.process_chromosome(chr_name_A, chr_name_B, outfile_vcf,
 									outfile_vcf_removed, outfile_vcf_LOH_removed, report_out_temp, print_results))
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_vcf.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 		
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 		
@@ -97,15 +97,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -157,15 +157,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -217,15 +217,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -276,15 +276,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
@@ -335,15 +335,15 @@
 		seq_file_name_b = os.path.join(os.path.dirname(os.path.abspath(__file__)), "files/ref/ref_ca22_1B.fasta")
 		self.assertTrue(os.path.exists(seq_file_name_a))
 		self.assertTrue(os.path.exists(seq_file_name_b))
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 	
 		seq_name_a = reference_a.get_first_seq()
 		self.assertEqual("Ca22chr1A_C_albicans_SC5314", seq_name_a)
 		seq_name_b = reference_b.get_chr_in_genome(seq_name_a)
 		self.assertEqual("Ca22chr1B_C_albicans_SC5314", seq_name_b)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_software.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_software.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_utils.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 import unittest, os
 from PHASEfilter.lib.utils.util import Utils, NucleotideCodes, CountLength, Cigar
 from PHASEfilter.lib.utils.reference import Reference
 from PHASEfilter.lib.utils.run_extra_software import RunExtraSoftware
 
 ### run command line
-# export PYTHONPATH='/home/mmp/git/PHASEfilter'
+# export PYTHONPATH=/home/mmp/git/PHASEfilter
 # python3 -m unittest -v tests.test_utils
 
 class Test(unittest.TestCase):
 
 
 	def setUp(self):
 		pass
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/tests/test_synchronization.py` & `PHASEfilter-1.1.0/PHASEfilter/tests/test_synchronization.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 	
 		seq_name_a = "chrXVI"
 		seq_name_b = "chrXVI"
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 		
 		self.assertEqual(Software.SOFTWARE_minimap2_name, lift_over_ligth.get_best_algorithm(seq_name_a, seq_name_b))
 		
 		### test positions
 		temp_file = utils.get_temp_file("base_name", ".fasta")
 		
@@ -84,15 +84,15 @@
 	
 		seq_name_a = "chrXVI"
 		seq_name_b = "chrXVI"
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = True
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
 		temp_file = utils.get_temp_file("base_name", ".fasta")
 	
 		### test some positions
 		position_to_test = 426
 		self.assertEqual((-1, -1), lift_over_ligth.get_pos_in_target(seq_name_a, seq_name_b, position_to_test))
@@ -129,15 +129,15 @@
 	
 		seq_name_a = "chrXVI"
 		seq_name_b = "chrXVI"
 	
 		reference_a = Reference(seq_file_name_a)
 		reference_b = Reference(seq_file_name_b)
 		impose_minimap2_only = False
-		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, impose_minimap2_only, True)
+		lift_over_ligth = LiftOverLight(reference_a, reference_b, temp_work_dir, None, impose_minimap2_only, True)
 		lift_over_ligth.synchronize_sequences(seq_name_a, seq_name_b)
 	
 		### impose lastz best alignment
 		lift_over_ligth.dt_chain_best_method[seq_name_a + "_" + seq_name_b] = Software.SOFTWARE_lastz_name
 		self.assertEqual(Software.SOFTWARE_lastz_name, lift_over_ligth.get_best_algorithm(seq_name_a, seq_name_b))
 		temp_file = utils.get_temp_file("base_name", ".fasta")
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/phasefilter_single.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/phasefilter_single.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # export PYTHONPATH='/home/mmp/git/PHASEfilter'
 # python3 phasefilter_single.py 
 #   --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta 
 #	--ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta
 #	--vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrA_filtered_snps.vcf.gz
 #	--vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrB_filtered_snps.vcf.gz
 #	--out_vcf file_name.vcf
-# python3 phasefilter_single.py --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta --ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta --vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf file_name.vcf
+# python3 phasefilter_single.py --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta --ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta --vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/T1_Fluc_5/T1_Fluc_5_chrA_filtered_snps.vcf.gz --vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/T1_Fluc_5/T1_Fluc_5_chrB_filtered_snps.vcf.gz --out_vcf file_name.vcf
 # python3 -m unittest -v tests.test_vcf
 
 # https://mbio.asm.org/content/9/5/e01205-18#sec-12
 # https://www.nature.com/articles/s41467-018-04787-4.pdf?origin=ppub
 from optparse import OptionParser
 
 __all__ = []
@@ -56,28 +56,30 @@
 	program_name = os.path.basename(sys.argv[0])
 	program_version = "{}".format(__version__)
 	program_build_date = "%s" % __updated__
 
 	program_version_string = '%%prog %s (%s)' % (program_version, program_build_date)
 	#program_usage = '''usage: spam two eggs''' # optional - will be autogenerated by optparse
 	program_longdesc = '''Identifies heterozygous variations and create three files: 1) valid; 2) heterozygous variants; 3) loss of heterozygous (LOH).
-	It accept 5 mandatory parameters and two optional parameters.
+	It accept 5 mandatory parameters and three optional parameters.
+	It is possible to pass the chain to avoid creation of synchronization. 
 	''' # optional - give further explanation about what the program does
 	program_license = "Copyright 2020 (iBiMED)											\
 				Licensed under the MIT\nhttps://spdx.org/licenses/MIT.html"
 
 	if argv is None:
 		argv = sys.argv[1:]
 	
 		# setup option parser
 		parser = OptionParser(version=program_version_string, epilog=program_longdesc, description=program_license)
 		parser.add_option("--ref1", dest="reference_1", help="[REQUIRED] reference for genome 1", metavar="FILE")
 		parser.add_option("--ref2", dest="reference_2", help="[REQUIRED] reference for genome 2", metavar="FILE")
 		parser.add_option("--vcf1", dest="vcf_1", help="[REQUIRED] vcf of genome 1", metavar="FILE")
 		parser.add_option("--vcf2", dest="vcf_2", help="[REQUIRED] vcf of genome 2", metavar="FILE")
+		parser.add_option("--chain", dest="chain_A_B", help="[Optinal] chain from genome 1 to genome 2", metavar="FILE", default=None)
 		parser.add_option("--out_vcf", dest="outfile_vcf", help="[REQUIRED] file with vcf result file", metavar="FILE")
 		## The reason to use AD is because GATK defines predefine values for AF = 0.5/1 and AC = 1|2. Doesn't reflect the real values of AD  
 		parser.add_option("--threshold_heterozygous_AD", dest="threshold_heterozygous_ad", help="Cutoff ratio of Allelic depths for the alt alleles " +\
 						" in the order listed. If bigger than this level is considered homozygous. If = to -1 it is not going to take it into account", metavar="RATIO", type="float", default=-1.0)
 		parser.add_option("--remove_variants_by_AD_ratio", dest="remove_variants_by_AD_ratio", help="Cutoff ratio of Allelic depths to remove variants. " +\
 						"It will be applied to 'vcf1'. If = to -1 it is not going to take it into account", metavar="RATIO", type="float", default=-1.0)
 
@@ -94,26 +96,28 @@
 		### output directoru		
 		## valid_[A|B]_to_[B|A].vcf”, “removed_[A|B]_to_[B|A].vcf” and “loss_of_heterozygous_[A|B]_to_[B|A].vcf
 		if opts.reference_1: 	print("reference 1                = %s" % opts.reference_1)
 		if opts.reference_2: 	print("reference 2                = %s" % opts.reference_2)
 		if opts.vcf_1: 			print("vcf 1                      = %s" % opts.vcf_1)
 		if opts.vcf_2: 			print("vcf 2                      = %s" % opts.vcf_2)
 		if opts.outfile_vcf: 	print("outfile vcf                = %s" % opts.outfile_vcf)
+		if opts.chain_A_B:		print("chain file                 = %s" % opts.chain_A_B)
 		if (opts.threshold_heterozygous_ad and opts.threshold_heterozygous_ad != -1):
 								print("threshold heterozygous     = {:.2f}".format(opts.threshold_heterozygous_ad))
 		if (opts.remove_variants_by_AD_ratio and opts.remove_variants_by_AD_ratio != -1):
 								print("remove variant by AD ratio = {:.2f}".format(opts.remove_variants_by_AD_ratio))
 
 		if (opts.reference_1 == opts.reference_2): sys.exit("Error: you have the same reference file")
 
 		### test files		
 		utils.test_file_exists(opts.reference_1)
 		utils.test_file_exists(opts.reference_2)
 		utils.test_file_exists(opts.vcf_1)
 		utils.test_file_exists(opts.vcf_2)
+		if opts.chain_A_B: utils.test_file_exists(opts.chain_A_B)
 
 		#### Test reference
 		b_print_results = False
 		threshold_ad = 0.05
 		threshold_remove_variant_ad = 0.05
 		vcf_process_1 = VcfProcess(opts.vcf_1, threshold_ad, threshold_remove_variant_ad, b_print_results)
 		if (vcf_process_1.exist_meta_data_tag('reference')):
@@ -142,15 +146,16 @@
 			
 			if (opts.threshold_heterozygous_ad != -1.0):
 				if (not vcf_process_2.has_format('AD')):
 					print("Warning: Format tag 'AD' is not present in file '{}'. 'threshold_heterozygous_ad' will be disable...".format(opts.vcf_2))  
 					opts.threshold_heterozygous_ad = -1.0
 
 		process_two_genomes = ProcessTwoGenomes(opts.reference_1, opts.reference_2, opts.vcf_1, opts.vcf_2,
-			opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, opts.outfile_vcf)
+			opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, opts.outfile_vcf,
+			opts.chain_A_B)
 		print("outfile report file = %s" % process_two_genomes.get_report_file())
 		print("outfile valid variants = %s" % process_two_genomes.get_vcf_file_name())
 		print("outfile removed variants = %s" % process_two_genomes.get_vcf_removed_file())
 		print("outfile LOH variants = %s" % process_two_genomes.get_vcf_loh_file())
 		
 		### test all software needed to run this script
 		software = Software()
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/synchronize_genomes.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/synchronize_genomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,28 +67,30 @@
 	program_version = "{}".format(__version__)
 	program_build_date = "%s" % __updated__
 
 	program_version_string = '%%prog %s (%s)' % (program_version, program_build_date)
 	#program_usage = '''usage: spam two eggs''' # optional - will be autogenerated by optparse
 	program_longdesc = '''
 	Synchronize two references and add two new fields (StartHit;EndHit) to the VCF/GFF with the positions on hit reference.
-	It accept 4 mandatory parameters and one optional parameters. It is necessary to pass a VCF or a GFF file.
+	It accept 4 mandatory parameters and two optional parameters. It is necessary to pass a VCF or a GFF file.
+	It is possible to pass the chain to avoid creation of synchronization.
 	''' # optional - give further explanation about what the program does
 	program_license = "Copyright 2020 (iBiMED)											\
 				Licensed under the MIT\nhttps://spdx.org/licenses/MIT.html"
 
 	if argv is None:
 		argv = sys.argv[1:]
 	
 		# setup option parser
 		parser = OptionParser(version=program_version_string, epilog=program_longdesc, description=program_license)
-		parser.add_option("--ref1", dest="reference_1", help="[REQUIRED] reference for genome 1", metavar="FILE")
-		parser.add_option("--ref2", dest="reference_2", help="[REQUIRED] reference for genome 2", metavar="FILE")
+		parser.add_option("--ref1", dest="reference_1", help="[REQUIRED] reference for genome A", metavar="FILE")
+		parser.add_option("--ref2", dest="reference_2", help="[REQUIRED] reference for genome B", metavar="FILE")
 		parser.add_option("--gff", dest="gff", help="[Optional] GFF3 file to set new positions of hit genome (gff3)", metavar="FILE")
 		parser.add_option("--vcf", dest="vcf", help="[Optional] VCF file to set new positions of hit genome (vcf)", metavar="FILE")
+		parser.add_option("--chain", dest="chain", help="[Optional] chain from genome A to genome B", metavar="FILE")
 		parser.add_option("--pass_chr", dest="pass_chr", help="[Optional] name of chromosomes to not processed. More than one chr split by comma, example 'chrI,chrII'")
 		parser.add_option("--out", dest="out", help="[REQUIRED] report in tab separated value (tsv)")
 
 		# process options
 		(opts, args) = parser.parse_args(argv)
 		checkRequiredArguments(opts, parser)
 		
@@ -99,24 +101,26 @@
 			print("You must pass one file, a VCF or a GFF3 reference, that belongs to the reference 1")
 			sys.exit(1)
 				
 		if opts.reference_1: print("reference 1         = %s" % opts.reference_1)
 		if opts.reference_2: print("reference 2         = %s" % opts.reference_2)
 		if opts.gff:         print("gff3                = %s" % opts.gff)
 		if opts.vcf:         print("vcf                 = %s" % opts.vcf)
+		if opts.chain:       print("chain               = %s" % opts.chain)
 		if opts.out:         print("out                 = %s" % opts.out)
 		if opts.pass_chr:    print("not processed chr.  = %s" % opts.pass_chr)
 
 		if (opts.reference_1 == opts.reference_2): sys.exit("Error: you have the same reference file")
 
 		utils.test_file_exists(opts.reference_1)
 		utils.test_file_exists(opts.reference_2)
 		if opts.gff: utils.test_file_exists(opts.gff)
 		if opts.vcf: utils.test_file_exists(opts.vcf)
-		process_two_references = ProcessTwoReferences(opts.reference_1, opts.reference_2, opts.out)
+		if opts.chain: utils.test_file_exists(opts.chain)
+		process_two_references = ProcessTwoReferences(opts.reference_1, opts.reference_2, opts.out, opts.chain)
 
 		### test all software needed to run this script
 		software = Software()
 		software.test_softwares()
 
 		### parse pass ref
 		if (opts.pass_chr): opts.pass_chr = [_.lower() for _ in opts.pass_chr.split(',')]
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/install_phasefilter_dependencies.sh` & `PHASEfilter-1.1.0/PHASEfilter/bin/install_phasefilter_dependencies.sh`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/make_alignment.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/make_alignment.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,37 +84,42 @@
 		parser = OptionParser(version=program_version_string, epilog=program_longdesc, description=program_license)
 		parser.add_option("--ref1", dest="reference_1", help="[REQUIRED] reference for genome 1", metavar="FILE")
 		parser.add_option("--ref2", dest="reference_2", help="[REQUIRED] reference for genome 2", metavar="FILE")
 		parser.add_option("--out", dest="outfile", help="[REQUIRED] report in tab separated value (tsv)", metavar="FILE")
 		parser.add_option("--pass_chr", dest="pass_chr", help="[Optional] name of chromosomes to not processed. More than one chr splitted by comma, example 'chrI,chrII'")
 		parser.add_option("--out_alignment", dest="out_alignment", help="[Optional] save the aligments, one for each synchronized chromosome.'", metavar="PATH")
 		parser.add_option("--out_new_reference", dest="out_new_reference", help="[Optional] create new reference for ref1 that has IUPAC codes for bases that are ambiguous between synchronized positions in chromosomes.'", metavar="FILE")
+		parser.add_option("-t", "--threading", dest="threading", type="int", help="[Optional] threading.'", default=1)
 
 		# process options
 		(opts, args) = parser.parse_args(argv)
 		checkRequiredArguments(opts, parser)
 			
 		if opts.reference_1:       print("reference 1          = %s" % opts.reference_1)
 		if opts.reference_2:       print("reference 2          = %s" % opts.reference_2)
 		if opts.outfile:           print("out file             = %s" % opts.outfile)
 		if opts.pass_chr:          print("not processed chr.   = %s" % opts.pass_chr)
 		if opts.out_alignment:     print("out path alignments  = %s" % opts.out_alignment)
 		if opts.out_new_reference:  print("out file new ref.   = %s" % opts.out_new_reference)
+		if opts.threading:         print("threading            = %s" % opts.threading)
 
 		if (opts.reference_1 == opts.reference_2): sys.exit("Error: you have the same reference file")
 		
+		## test reference files
 		utils.test_file_exists(opts.reference_1)
 		utils.test_file_exists(opts.reference_2)
 
 		### create path for out alignments
 		if (opts.out_alignment and not os.path.exists(opts.out_alignment)):
 			os.makedirs(opts.out_alignment, exist_ok=True)
 			
+		chain_name = None		## not need in this case
 		process_two_references = ProcessTwoReferences(opts.reference_1, opts.reference_2, 
-					opts.outfile, opts.out_alignment, opts.out_new_reference)
+					opts.outfile, chain_name, opts.out_alignment, opts.out_new_reference,
+					opts.threading)
 		
 		### test all software needed to run this script
 		software = Software()
 		software.test_softwares()
 		
 		### parse pass ref
 		if (opts.pass_chr): vect_pass_chr = [_.lower() for _ in opts.pass_chr.split(',')]
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/copy_raw_data_example_phasefilter.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/copy_raw_data_example_phasefilter.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 	4) T1_Fluc_7A_snps.vcf.gz.tbi
 	5) T1_Fluc_7B_snps.vcf.gz
 	6) T1_Fluc_7B_snps.vcf.gz.tbi
 	7) T1_Fluc_7A_indels.vcf.gz
 	8) T1_Fluc_7A_indels.vcf.gz.tbi
 	9) T1_Fluc_7B_indels.vcf.gz
 	10) T1_Fluc_7B_indels.vcf.gz.tbi
+	11) Assembly22_hapA_To_Assembly22_hapB.over.chain
+	12) Assembly22_hapB_To_Assembly22_hapA.over.chain
 	''' # optional - give further explanation about what the program does
 	program_license = "Copyright 2020 (iBiMED)											\
 				Licensed under the MIT\nhttps://spdx.org/licenses/MIT.html"
 
 	if argv is None:
 		argv = sys.argv[1:]
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/phasefilter.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/phasefilter.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 # export PYTHONPATH='/home/mmp/git/PHASEfilter'
 # python3 phasefilter.py 
 #   --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta 
 #	--ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta
 #	--vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrA_filtered_snps.vcf.gz
 #	--vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrB_filtered_snps.vcf.gz
 #	--out_dir /home/projects/ua/candida/compare_A_vs_B
-# python3 phasefilter.py --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta --ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta --vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/A-M_S4/A-M_S4_chrB_filtered_snps.vcf.gz --out_dir /home/projects/ua/candida/compare_A_vs_B
+# python3 phasefilter.py --ref1 /home/projects/ua/candida/compare_A_vs_B/ref/genomeA/Ca22chr1A_C_albicans_SC5314.fasta --ref2 /home/projects/ua/candida/compare_A_vs_B/ref/genomeB/Ca22chr1B_C_albicans_SC5314.fasta --vcf1 /home/projects/ua/candida/compare_A_vs_B/vcf/T1_Fluc_5/T1_Fluc_5_chrA_filtered_snps.vcf.gz --vcf2 /home/projects/ua/candida/compare_A_vs_B/vcf/T1_Fluc_5/T1_Fluc_5_chrB_filtered_snps.vcf.gz --out /home/projects/ua/candida/compare_A_vs_B
+
+# --chain_A_B /home/projects/ua/candida/chain/Assembly22_hapA_To_Assembly22_hapB.over.chain --chain_B_A /home/projects/ua/candida/chain/Assembly22_hapB_To_Assembly22_hapA.over.chain
 # python3 -m unittest -v tests.test_vcf
 
 # https://mbio.asm.org/content/9/5/e01205-18#sec-12
 # https://www.nature.com/articles/s41467-018-04787-4.pdf?origin=ppub
 from optparse import OptionParser
 
 __all__ = []
@@ -49,20 +51,21 @@
 		if re.match(r'^\[REQUIRED\]', option.help) and eval('opts.' + option.dest) == None:
 			missing_options.extend(option._long_opts)
 	if len(missing_options) > 0:
 		parser.error('Missing REQUIRED parameters: ' + str(missing_options))
 
 
 def make_ref_from_to_ref_to(reference_1, reference_2, vcf_1, vcf_2,
-					threshold_heterozygous_ad, remove_variants_by_AD_ratio, outfile_vcf):
+					threshold_heterozygous_ad, remove_variants_by_AD_ratio, outfile_vcf, chain_from_to):
 	"""
 	Process from one Ref to Other
 	"""
 	process_two_genomes = ProcessTwoGenomes(reference_1, reference_2, vcf_1, vcf_2,
-				threshold_heterozygous_ad, remove_variants_by_AD_ratio, outfile_vcf)
+				threshold_heterozygous_ad, remove_variants_by_AD_ratio, outfile_vcf,
+				chain_from_to)
 	print("outfile report file = %s" % process_two_genomes.get_report_file())
 	print("outfile valid variants = %s" % process_two_genomes.outfile_vcf)
 	print("outfile removed variants = %s" % process_two_genomes.get_vcf_removed_file())
 	print("outfile LOH variants = %s" % process_two_genomes.get_vcf_loh_file())
 	
 	### test all software needed to run this script
 	software = Software()
@@ -83,29 +86,32 @@
 	program_name = os.path.basename(sys.argv[0])
 	program_version = "{}".format(__version__)
 	program_build_date = "%s" % __updated__
 
 	program_version_string = '%%prog %s (%s)' % (program_version, program_build_date)
 	#program_usage = '''usage: spam two eggs''' # optional - will be autogenerated by optparse
 	program_longdesc = '''Identifies heterozygous variations and create three files: 1) valid; 2) heterozygous variants; 3) loss of heterozygous (LOH).
-	It accept 5 mandatory parameters and two optional parameters.
-	It will work in both directions, from REF1 to REF2 and then from REF2 to REF1
+	It accept 5 mandatory parameters and three optional parameters.
+	It will work in both directions, from REF1 to REF2 and then from REF2 to REF1.
+	It is possible to pass the chain to avoid creation of synchronization
 	''' # optional - give further explanation about what the program does
 	program_license = "Copyright 2020 (iBiMED)											\
 				Licensed under the MIT\nhttps://spdx.org/licenses/MIT.html"
 
 	if argv is None:
 		argv = sys.argv[1:]
 	
 		# setup option parser
 		parser = OptionParser(version=program_version_string, epilog=program_longdesc, description=program_license)
 		parser.add_option("--ref1", dest="reference_1", help="[REQUIRED] reference for genome 1", metavar="FILE")
 		parser.add_option("--ref2", dest="reference_2", help="[REQUIRED] reference for genome 2", metavar="FILE")
 		parser.add_option("--vcf1", dest="vcf_1", help="[REQUIRED] vcf of genome 1", metavar="FILE")
 		parser.add_option("--vcf2", dest="vcf_2", help="[REQUIRED] vcf of genome 2", metavar="FILE")
+		parser.add_option("--chain_A_B", dest="chain_A_B", help="[Optional] chain from genome 1 to genome 2", metavar="FILE", default=None)
+		parser.add_option("--chain_B_A", dest="chain_B_A", help="[Optional] chain from genome 2 to genome 1", metavar="FILE", default=None)
 		parser.add_option("--out", dest="out_dir", help="[REQUIRED] paths to write the VCF files", metavar="PATH")
 		## The reason to use AD is because GATK defines predefine values for AF = 0.5/1 and AC = 1|2. Doesn't reflect the real values of AD  
 		parser.add_option("--threshold_heterozygous_AD", dest="threshold_heterozygous_ad", help="Cutoff ratio of Allelic depths for the alt alleles " +\
 						" in the order listed. If bigger than this level is considered homozygous. If = to -1 it is not going to take it into account", metavar="RATIO", type="float", default=-1.0)
 		parser.add_option("--remove_variants_by_AD_ratio", dest="remove_variants_by_AD_ratio", help="Cutoff ratio of Allelic depths to remove variants. " +\
 						"It will be applied to 'vcf1'. If = to -1 it is not going to take it into account", metavar="RATIO", type="float", default=-1.0)
 
@@ -120,22 +126,26 @@
 		if opts.vcf_1: 			print("vcf 1                      = %s" % opts.vcf_1)
 		if opts.vcf_2: 			print("vcf 2                      = %s" % opts.vcf_2)
 		if opts.out_dir:	 	print("out_dir                    = %s" % opts.out_dir)
 		if (opts.threshold_heterozygous_ad and opts.threshold_heterozygous_ad != -1):
 								print("threshold heterozygous     = {:.2f}".format(opts.threshold_heterozygous_ad))
 		if (opts.remove_variants_by_AD_ratio and opts.remove_variants_by_AD_ratio != -1):
 								print("remove variant by AD ratio = {:.2f}".format(opts.remove_variants_by_AD_ratio))
-
+		if (opts.chain_A_B):    print("Chain from A to B          = {}".format(opts.chain_A_B))
+		if (opts.chain_B_A):    print("Chain from B to A          = {}".format(opts.chain_B_A))
 		if (opts.reference_1 == opts.reference_2): sys.exit("Error: you have the same reference file")
+		if (opts.chain_A_B and opts.chain_B_A and opts.chain_A_B == opts.chain_B_A): sys.exit("Error: you have the same chain file for different directions")
 
-		### test files		
+		### testing files
 		utils.test_file_exists(opts.reference_1)
 		utils.test_file_exists(opts.reference_2)
 		utils.test_file_exists(opts.vcf_1)
 		utils.test_file_exists(opts.vcf_2)
+		if (opts.chain_A_B): utils.test_file_exists(opts.chain_A_B)
+		if (opts.chain_B_A): utils.test_file_exists(opts.chain_B_A)
 
 		#### Test reference
 		b_print_results = False
 		threshold_ad = 0.05
 		threshold_remove_variant_ad = 0.05
 		vcf_process_1 = VcfProcess(opts.vcf_1, threshold_ad, threshold_remove_variant_ad, b_print_results)
 		if (vcf_process_1.exist_meta_data_tag('reference')):
@@ -163,30 +173,35 @@
 				opts.threshold_heterozygous_ad = -1.0
 			
 			if (opts.threshold_heterozygous_ad != -1.0):
 				if (not vcf_process_2.has_format('AD')):
 					print("Warning: Format tag 'AD' is not present in file '{}'. 'threshold_heterozygous_ad' will be disable...".format(opts.vcf_2))  
 					opts.threshold_heterozygous_ad = -1.0
 
+		### test chain file names
+		if (opts.chain_A_B and opts.chain_B_A and opts.chain_A_B == opts.chain_B_A):
+			print("Error: chain file A to B is the same as B to A.")
+			exit(1)
+
 		### make path if not exist
 		utils.make_path(opts.out_dir)
 		
 		## make ref1 to ref2
 		outfile_vcf = os.path.join(opts.out_dir, "{}_TO_{}.vcf.gz".format(
 					utils.get_file_name_without_extension(opts.reference_1),
 					utils.get_file_name_without_extension(opts.reference_2)))
 		make_ref_from_to_ref_to(opts.reference_1, opts.reference_2, opts.vcf_1, opts.vcf_2,
-				opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, outfile_vcf)
+				opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, outfile_vcf, opts.chain_A_B)
 
 		## make ref2 to ref1
 		outfile_vcf = os.path.join(opts.out_dir, "{}_TO_{}.vcf.gz".format(
 					utils.get_file_name_without_extension(opts.reference_2),
 					utils.get_file_name_without_extension(opts.reference_1)))
 		make_ref_from_to_ref_to(opts.reference_2, opts.reference_1, opts.vcf_2, opts.vcf_1,
-				opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, outfile_vcf)
+				opts.threshold_heterozygous_ad, opts.remove_variants_by_AD_ratio, outfile_vcf, opts.chain_B_A)
 
 		print("Done. Outputs in '{}'".format(opts.out_dir))
 
 if __name__ == "__main__":
 
 	sys.exit(main())
```

### Comparing `PHASEfilter-0.3.7/PHASEfilter/bin/reference_statistics.py` & `PHASEfilter-1.1.0/PHASEfilter/bin/reference_statistics.py`

 * *Files identical despite different names*

### Comparing `PHASEfilter-0.3.7/PKG-INFO` & `PHASEfilter-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHASEfilter
-Version: 0.3.7
+Version: 1.1.0
 Summary: Software package to filter variants, SNPs and INDELs, that are present in heterozygous form in phased genomes.
 Home-page: https://github.com/ibigen/PHASEfilter
 Author: Miguel Pinheiro
 Author-email: monsanto@ua.pt
 License: MIT
 Project-URL: Bug Reports, https://github.com/ibigen/PHASEfilter/issues
 Project-URL: Source, https://github.com/ibigen/PHASEfilter
@@ -25,21 +25,21 @@
         ```
         $ pip3 install PHASEfilter
         ```
         
         ### Install with virtualenv
         
         ```
-        $ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 0.3.7) "
+        $ virtualenv PHASEfilter --python=python3 --prompt "(PHASEfilter 1.1.0) "
         $ . PHASEfilter/bin/activate
-        (phasefilter 0.3.7) $ pip install PHASEfilter
+        (phasefilter 1.1.0) $ pip install PHASEfilter
         
         ## install all Software dependencies of PHASEfilter 
-        (phasefilter 0.3.7) $ cd PHASEfilter/bin/
-        (phasefilter 0.3.7) $ ./install_phasefilter_dependencies.sh
+        (phasefilter 1.1.0) $ cd PHASEfilter/bin/
+        (phasefilter 1.1.0) $ ./install_phasefilter_dependencies.sh
         ```
         
         ### Install with conda
         
         ```
         $ wget https://raw.githubusercontent.com/ibigen/PHASEfilter/main/conda/conda_phasefilter_env.yml -O conda_phasefilter_env.yml
         $ conda env create -f conda_phasefilter_env.yml
@@ -64,14 +64,17 @@
         The variant file in analysis it is always the one passed in parameter '--vcf1'.
         
         ```
         $ phasefilter --help
         ## You can can copy some example data to test the commands
         $ copy_raw_data_example_phasefilter --out temp_raw_data
         $ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir
+        
+        ## you can use chain if exists
+        $ phasefilter --ref1 temp_raw_data/Ca22chr7A_C_albicans_SC5314.fasta --ref2 temp_raw_data/Ca22chr7B_C_albicans_SC5314.fasta --vcf1 temp_raw_data/T1_Fluc_7A_snps.vcf.gz --vcf2 temp_raw_data/T1_Fluc_7B_snps.vcf.gz --out output_dir --chain_A_B temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain --chain_B_A temp_raw_data/Assembly22_hapB_To_Assembly22_hapA.over.chain
         ```
         
         Eighth possible files will be created after the commands ends. The outputs are from refrence A (ref1) to reference B (ref2), and from reference B (ref2) to reference A (ref1).
         
         -  report_[A]_to_[B].txt - has the statistics about the analysis;
         -  valid_[A]_to_[B].vcf.gz - has all variants that are not heterozygous between two references;
         -  removed_[A]_to_[B].vcf.gz - has all heterozygous variants;
@@ -102,14 +105,17 @@
         ## Filter variants in phased genomes but only one direction
         
         This tool do as the same of the previous script but only analysis from Reference A (ref1) to Reference B (ref2)
         
         ```
         $ phasefilter_single --help
         $ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz
+        
+        ## with chain
+        $ phasefilter_single --ref1 Ca22chr1A_C_albicans_SC5314.fasta --ref2 Ca22chr1B_C_albicans_SC5314.fasta --vcf1 A-M_S4_chrA_filtered_snps.vcf.gz --vcf2 A-M_S4_chrB_filtered_snps.vcf.gz --out_vcf out_result.vcf.gz --chain temp_raw_data/Assembly22_hapA_To_Assembly22_hapB.over.chain
         ```
         
         ## Synchronize annotation genomes
         
         Synchronize annotations genomes adapting the annotations that are in reference 1 to the reference 2, adding the tags 'StartHit' and 'EndHit' to the result file. In VCF type files only add 'StartHit' tag in Info. The annotations (input file need to be in VCF or GFF3 and belong to the reference 1.
         
         ```
@@ -155,15 +161,15 @@
         ```
         
         # Documentation
         
         PHASEfilter documentation is available in [ReadTheDocs: PHASEfilter](https://phasefilter.readthedocs.io/en/latest/)
         
 Keywords: SNPs INDEL phased genome filtering bioinformatics
-Platform: linux_x86_64
+Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `PHASEfilter-0.3.7/setup.py` & `PHASEfilter-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # encoding: utf-8
 
 import setuptools
 from PHASEfilter.lib.constants import version
 from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 
 ## 
+## cd where setup.py is
+## rm dist/*
 ## python3 setup.py sdist bdist_wheel --plat-name=linux_x86_64
 ## python3 -m twine upload dist/*
 #### and press cancel in all windows
 ### to test in virtual env
 ## python3 -m pip install dist/PHASEfilter-0.1-py3-none-any.whl --install-option test
 
 
@@ -48,15 +50,15 @@
 						'tests/files/software/*',
 						'tests/files/synchronize/*',
 						'tests/files/vcf/*'],
 			},
 	license='MIT',
 	python_requires='>=3.5',
 	include_package_data=True, # include other files
-	platforms='linux_x86_64',
+	platforms=['Linux'],
 	classifiers=[
 		# How mature is this project? Common values are
 		#   Development Status :: 1 - Planning
 		#	Development Status :: 2 - Pre-Alpha
 		#	Development Status :: 3 - Alpha
 		#	Development Status :: 4 - Beta
 		#	Development Status :: 5 - Production/Stable
@@ -76,14 +78,15 @@
 		"Topic :: Scientific/Engineering :: Bio-Informatics",
 	],
 	install_requires=[
 		"pyvcf==0.6.8",
 		"pysam==0.15.2",
 		"biopython==1.78",
 		"gff3tool==2.0.1",
+		"pyliftover==0.4",
 		"wheel",
 	],
 	entry_points={
 		'console_scripts': [
 			'make_alignment = PHASEfilter.bin.make_alignment:main',
 			'reference_statistics = PHASEfilter.bin.reference_statistics:main',
 			'phasefilter = PHASEfilter.bin.phasefilter:main',
```

