# Comparing `tmp/checkQC-3.7.0.tar.gz` & `tmp/checkQC-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkQC-3.7.0.tar", last modified: Wed Nov 23 14:13:30 2022, max compression
+gzip compressed data, was "checkQC-3.8.0.tar", last modified: Fri May  5 06:05:07 2023, max compression
```

## Comparing `checkQC-3.7.0.tar` & `checkQC-3.8.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.504071 checkQC-3.7.0/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    35141 2022-03-09 14:47:52.000000 checkQC-3.7.0/LICENSE
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      146 2022-03-09 14:47:52.000000 checkQC-3.7.0/MANIFEST.in
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2022-11-23 14:13:30.504071 checkQC-3.7.0/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    11317 2022-10-25 10:40:55.000000 checkQC-3.7.0/README.md
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.500071 checkQC-3.7.0/checkQC/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       23 2022-11-23 13:27:21.000000 checkQC-3.7.0/checkQC/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     5028 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/app.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     9538 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/config.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.500071 checkQC-3.7.0/checkQC/default_config/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    11826 2022-11-23 13:27:21.000000 checkQC-3.7.0/checkQC/default_config/config.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      576 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/default_config/logger.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      836 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/exceptions.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.504071 checkQC-3.7.0/checkQC/handlers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1857 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/cluster_pf_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3646 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/error_rate_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2240 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/q30_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     7911 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/qc_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1545 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/qc_handler_factory.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3248 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/reads_per_sample_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4146 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/undetermined_percentage_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    15665 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/handlers/unidentified_index_handler.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.504071 checkQC-3.7.0/checkQC/parsers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3958 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/demux_summary_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3532 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/interop_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2245 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2098 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/samplesheet_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3189 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/parsers/stats_json_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4378 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/qc_engine.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     7991 2022-11-23 13:27:21.000000 checkQC-3.7.0/checkQC/run_type_recognizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1498 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/run_type_summarizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2937 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/runfolder_reader.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4221 2022-03-09 14:47:52.000000 checkQC-3.7.0/checkQC/web_app.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2022-11-23 14:13:30.500071 checkQC-3.7.0/checkQC.egg-info/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1067 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/SOURCES.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        1 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/dependency_links.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       81 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/entry_points.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       65 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/requires.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        8 2022-11-23 14:13:30.000000 checkQC-3.7.0/checkQC.egg-info/top_level.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       79 2022-11-23 14:13:30.504071 checkQC-3.7.0/setup.cfg
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1180 2022-10-25 10:40:55.000000 checkQC-3.7.0/setup.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    35141 2022-03-09 14:47:52.000000 checkQC-3.8.0/LICENSE
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      146 2022-03-09 14:47:52.000000 checkQC-3.8.0/MANIFEST.in
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2023-05-05 06:05:07.512037 checkQC-3.8.0/PKG-INFO
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    11335 2023-05-04 09:28:20.000000 checkQC-3.8.0/README.md
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       23 2023-05-04 11:01:05.000000 checkQC-3.8.0/checkQC/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     5028 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/app.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     9538 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/config.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC/default_config/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    14396 2023-05-04 09:28:20.000000 checkQC-3.8.0/checkQC/default_config/config.yaml
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      576 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/default_config/logger.yaml
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      836 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/exceptions.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/checkQC/handlers/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1857 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/cluster_pf_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3646 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/error_rate_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2240 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/q30_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     7911 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/qc_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1545 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/qc_handler_factory.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3248 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/reads_per_sample_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4146 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/undetermined_percentage_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    15665 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/unidentified_index_handler.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/checkQC/parsers/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3958 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/demux_summary_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3532 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/interop_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2245 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2098 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/samplesheet_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3189 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/stats_json_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4378 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/qc_engine.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     7802 2023-05-04 09:28:20.000000 checkQC-3.8.0/checkQC/run_type_recognizer.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1498 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/run_type_summarizer.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2937 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/runfolder_reader.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4221 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/web_app.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC.egg-info/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/PKG-INFO
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1067 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/SOURCES.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        1 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/dependency_links.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       81 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/entry_points.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       65 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/requires.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        8 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/top_level.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       79 2023-05-05 06:05:07.512037 checkQC-3.8.0/setup.cfg
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1180 2022-10-25 10:40:55.000000 checkQC-3.8.0/setup.py
```

### Comparing `checkQC-3.7.0/LICENSE` & `checkQC-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/PKG-INFO` & `checkQC-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 3.7.0
+Version: 3.8.0
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/3.7.0.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/3.8.0.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 License-File: LICENSE
 
 A simple program to parse Illumina NGS data and check it for quality criteria.
```

### Comparing `checkQC-3.7.0/README.md` & `checkQC-3.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 Instrument types supported in checkQC are the following:
  - HiSeqX
  - HiSeq2500
  - iSeq
  - MiSeq
  - NovaSeq
+ - NovaSeq X Plus
 
 Install instructions
 --------------------
 CheckQC **requires Python 3.6** (or higher to run). CheckQC can be installed with pip.
 
 ```
 pip install checkqc
```

### Comparing `checkQC-3.7.0/checkQC/app.py` & `checkQC-3.8.0/checkQC/app.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/config.py` & `checkQC-3.8.0/checkQC/config.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/default_config/config.yaml` & `checkQC-3.8.0/checkQC/default_config/config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -319,14 +319,125 @@
         allow_missing_error_rate: False
         warning: 5
         error: unknown
       - name: ReadsPerSampleHandler
         warning: unknown
         error: 1500
 
+novaseqxplus_1.5B:
+  51:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 800
+        error: unknown
+      - name: Q30Handler
+        warning: 90 
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 1
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 600
+  101:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 800
+        error: unknown
+      - name: Q30Handler
+        warning: 85
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 2
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 600
+  151:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 800
+        error: unknown
+      - name: Q30Handler
+        warning: 85
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 5
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 600
+
+novaseqxplus_10B:
+  51:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 1250
+        error: unknown
+      - name: Q30Handler
+        warning: 90
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 1
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 937.5
+  101:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 1250
+        error: unknown
+      - name: Q30Handler
+        warning: 85
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 2
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 937.5
+  151:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 1250
+        error: unknown
+      - name: Q30Handler
+        warning: 85
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False 
+        warning: 5
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 937.5
+
+novaseqxplus_25B:
+  151:
+    handlers:
+      - name: ClusterPFHandler
+        warning: 3250
+        error: unknown
+      - name: Q30Handler
+        warning: 85
+        error: unknown
+      - name: ErrorRateHandler
+        allow_missing_error_rate: False
+        warning: 5
+        error: unknown
+      - name: ReadsPerSampleHandler
+        warning: unknown
+        error: 2437.5
+
 miseq_nano_v2:
   151:
     handlers:
       - name: ClusterPFHandler
         warning: 1
         error: unknown
       - name: Q30Handler
```

### Comparing `checkQC-3.7.0/checkQC/default_config/logger.yaml` & `checkQC-3.8.0/checkQC/default_config/logger.yaml`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/exceptions.py` & `checkQC-3.8.0/checkQC/exceptions.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/cluster_pf_handler.py` & `checkQC-3.8.0/checkQC/handlers/cluster_pf_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/error_rate_handler.py` & `checkQC-3.8.0/checkQC/handlers/error_rate_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/q30_handler.py` & `checkQC-3.8.0/checkQC/handlers/q30_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/qc_handler.py` & `checkQC-3.8.0/checkQC/handlers/qc_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/qc_handler_factory.py` & `checkQC-3.8.0/checkQC/handlers/qc_handler_factory.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/reads_per_sample_handler.py` & `checkQC-3.8.0/checkQC/handlers/reads_per_sample_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/undetermined_percentage_handler.py` & `checkQC-3.8.0/checkQC/handlers/undetermined_percentage_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/handlers/unidentified_index_handler.py` & `checkQC-3.8.0/checkQC/handlers/unidentified_index_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/parsers/demux_summary_parser.py` & `checkQC-3.8.0/checkQC/parsers/demux_summary_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/parsers/interop_parser.py` & `checkQC-3.8.0/checkQC/parsers/interop_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/parsers/parser.py` & `checkQC-3.8.0/checkQC/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/parsers/samplesheet_parser.py` & `checkQC-3.8.0/checkQC/parsers/samplesheet_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/parsers/stats_json_parser.py` & `checkQC-3.8.0/checkQC/parsers/stats_json_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/qc_engine.py` & `checkQC-3.8.0/checkQC/qc_engine.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/run_type_recognizer.py` & `checkQC-3.8.0/checkQC/run_type_recognizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,45 +10,21 @@
 class IlluminaInstrument(object):
     """
     Base class representing an Illumina instrument. The `name` and `reagent_version` needs to be implemented
     by the specific subclasses.
     """
 
     @staticmethod
-    def get_subclasses():
-        """
-        Get all subclasses which extends this class (which should be all supported Illumina instruments)
-
-        :returns: a list of IlluminaInstrument subclasses
-        """
-        return IlluminaInstrument.__subclasses__()
-
-    @staticmethod
-    def create_instrument_instance(instrument_name):
-        """
-        Get the instrument instance corresponding to the given instrument name
-
-        :param instrument_name: name of instrument to get the implementing class for
-        :returns: a instance of the corresponding IlluminaInstrument
-        """
-        subclasses = IlluminaInstrument.get_subclasses()
-        for subclass in subclasses:
-            if instrument_name == subclass.name():
-                return subclass()
-        raise InstrumentTypeUnknown
-
-    @staticmethod
     def name():
         """
         Name of the instrument, e.g. 'nova_seq'
 
         :returns: name of instrument as string
         """
         raise NotImplementedError
-
     @staticmethod
     def reagent_version(runtype_recognizer):
         """
         Reagent version, e.g. `v1`
         Can used the provided runtype_recognizer to determined the exact reagent version
 
         :param runtype_recognizer: A instance of RuntypeRecognizer
@@ -77,14 +53,34 @@
         try:
             reagent_version = runtype_recognizer.run_parameters["RunParameters"]["RfidsInfo"]["FlowCellMode"]
             return reagent_version
         except KeyError:
             raise ReagentVersionUnknown("Could not identify flowcell mode for Novaseq")
 
 
+class NovaSeqXPlus(IlluminaInstrument):
+
+    @staticmethod
+    def name():
+        return "novaseqxplus"
+
+    @staticmethod
+    def reagent_version(runtype_recognizer):
+        try:
+            run_parameters = runtype_recognizer.run_parameters['RunParameters']
+            consumables = run_parameters["ConsumableInfo"]["ConsumableInfo"]
+            reagent_version = next(
+                consumable for consumable in consumables
+                if consumable['Type'] == 'FlowCell'
+            )['Mode']
+            return reagent_version
+        except (KeyError, StopIteration):
+            raise ReagentVersionUnknown("Could not identify flowcell mode for NovaSeqXPlus")
+
+
 class HiSeqX(IlluminaInstrument):
 
     @staticmethod
     def name():
         return "hiseqx"
 
     @staticmethod
@@ -190,23 +186,26 @@
         This will look in the RunInfo.xml and determine the run type, based on the
         mappings from instrument names to instrument types
 
         :raises: InstrumentTypeUnknown
         :returns: the instrument type of the runfolder
         """
         instrument_name = self.run_info["RunInfo"]["Run"]["Instrument"]
-        machine_type_mappings = {"M": "miseq",
-                                 "D": "hiseq2500",
-                                 "ST": "hiseqx",
-                                 "A": "novaseq",
-                                 "FS": "iseq"}
-
-        for key, value in machine_type_mappings.items():
-            if instrument_name.startswith(key):
-                return IlluminaInstrument.create_instrument_instance(value)
+        machine_type_mappings = {
+            "M": MiSeq,
+            "D": HiSeq2500,
+            "ST": HiSeqX,
+            "A": NovaSeq,
+            "FS": ISeq,
+            "LH": NovaSeqXPlus,
+        }
+
+        for instrument_code, instrument_class in machine_type_mappings.items():
+            if instrument_name.startswith(instrument_code):
+                return instrument_class()
 
         raise InstrumentTypeUnknown("Did not recognize instrument type of: {}".format(instrument_name))
 
     def instrument_and_reagent_version(self):
         """
         Get the instrument and reagent version associated with this runfolder.
```

### Comparing `checkQC-3.7.0/checkQC/run_type_summarizer.py` & `checkQC-3.8.0/checkQC/run_type_summarizer.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/runfolder_reader.py` & `checkQC-3.8.0/checkQC/runfolder_reader.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC/web_app.py` & `checkQC-3.8.0/checkQC/web_app.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/checkQC.egg-info/PKG-INFO` & `checkQC-3.8.0/checkQC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 3.7.0
+Version: 3.8.0
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/3.7.0.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/3.8.0.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 License-File: LICENSE
 
 A simple program to parse Illumina NGS data and check it for quality criteria.
```

### Comparing `checkQC-3.7.0/checkQC.egg-info/SOURCES.txt` & `checkQC-3.8.0/checkQC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `checkQC-3.7.0/setup.py` & `checkQC-3.8.0/setup.py`

 * *Files identical despite different names*

