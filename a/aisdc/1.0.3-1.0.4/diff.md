# Comparing `tmp/aisdc-1.0.3.tar.gz` & `tmp/aisdc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.0.3.tar", last modified: Tue May  2 16:13:23 2023, max compression
+gzip compressed data, was "aisdc-1.0.4.tar", last modified: Fri May  5 14:05:25 2023, max compression
```

## Comparing `aisdc-1.0.3.tar` & `aisdc-1.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.3/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-02 16:13:23.828295 aisdc-1.0.3/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-02 15:24:23.000000 aisdc-1.0.3/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      395 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2167 2023-05-02 10:18:16.000000 aisdc-1.0.3/aisdc/attacks/dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22027 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12090 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22656 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/worst_case_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10042 2023-05-02 15:24:23.000000 aisdc-1.0.3/aisdc/generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-02 15:32:15.000000 aisdc-1.0.3/aisdc/metrics.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7595 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7149 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6287 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30719 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1435 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      170 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-05-02 16:13:23.828295 aisdc-1.0.3/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1857 2023-05-02 15:24:23.000000 aisdc-1.0.3/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.3/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attacks_dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6065 2023-05-02 15:24:23.000000 aisdc-1.0.3/tests/test_generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3661 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.3/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15852 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11770 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11146 2023-05-02 10:18:16.000000 aisdc-1.0.3/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.4/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-05 14:05:25.694556 aisdc-1.0.4/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-02 15:24:23.000000 aisdc-1.0.4/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      395 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2167 2023-05-02 10:18:16.000000 aisdc-1.0.4/aisdc/attacks/dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22027 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12090 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22656 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10042 2023-05-02 15:24:23.000000 aisdc-1.0.4/aisdc/generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-02 15:32:15.000000 aisdc-1.0.4/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7595 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7149 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6322 2023-05-05 14:05:12.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30719 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1435 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      170 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-05-05 14:05:25.694556 aisdc-1.0.4/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1857 2023-05-05 14:05:12.000000 aisdc-1.0.4/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.4/tests/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attacks_dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6065 2023-05-02 15:24:23.000000 aisdc-1.0.4/tests/test_generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3661 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_loaders.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.4/tests/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15852 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-05 14:05:12.000000 aisdc-1.0.4/tests/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11146 2023-05-02 10:18:16.000000 aisdc-1.0.4/tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.3/LICENSE` & `aisdc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/PKG-INFO` & `aisdc-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.3/README.md` & `aisdc-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/attacks/attribute_attack.py` & `aisdc-1.0.4/aisdc/attacks/attribute_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/attacks/dataset.py` & `aisdc-1.0.4/aisdc/attacks/dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/attacks/likelihood_attack.py` & `aisdc-1.0.4/aisdc/attacks/likelihood_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/attacks/report.py` & `aisdc-1.0.4/aisdc/attacks/report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/attacks/worst_case_attack.py` & `aisdc-1.0.4/aisdc/attacks/worst_case_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/generate_report.py` & `aisdc-1.0.4/aisdc/generate_report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/metrics.py` & `aisdc-1.0.4/aisdc/metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/preprocessing/loaders.py` & `aisdc-1.0.4/aisdc/preprocessing/loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/safekeras.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 from sklearn.ensemble import RandomForestClassifier
 
 from ..reporting import get_reporting_string
 from ..safemodel import SafeModel
 from .safedecisiontreeclassifier import decision_trees_are_equal
 
-# pylint: disable=too-many-ancestors,too-many-instance-attributes
+# pylint: disable=too-many-ancestors,too-many-instance-attributes, unidiomatic-typecheck
 
 
 class SafeRandomForestClassifier(SafeModel, RandomForestClassifier):
     """Privacy protected Random Forest classifier."""
 
     def __init__(
         self, **kwargs: Any
@@ -68,15 +68,15 @@
         """
         msg = ""
         disclosive = False
         # now the relevant random-forest specific things
         for item in self.examine_seperately_items:
             # template for class of things that make up forest
             if item == "base_estimator":
-                if curr_separate[item] != saved_separate[item]:
+                if type(curr_separate[item]) != type(saved_separate[item]):
                     # msg += get_reporting_string(name="basic_params_differ",length=1)
                     msg += get_reporting_string(
                         name="param_changed_from_to",
                         key="base_estimator",
                         val=saved_separate[item],
                         cur_val=curr_separate[item],
                     )
```

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.0.4/aisdc/safemodel/classifiers/safetf.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/reporting.py` & `aisdc-1.0.4/aisdc/safemodel/reporting.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/rules.json` & `aisdc-1.0.4/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc/safemodel/safemodel.py` & `aisdc-1.0.4/aisdc/safemodel/safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/aisdc.egg-info/PKG-INFO` & `aisdc-1.0.4/aisdc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.3/aisdc.egg-info/SOURCES.txt` & `aisdc-1.0.4/aisdc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/setup.py` & `aisdc-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aisdc",
-    version="1.0.3",
+    version="1.0.4",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="Tools for the statistical disclosure control of machine learning models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/AI-SDC",
```

### Comparing `aisdc-1.0.3/tests/test_attacks.py` & `aisdc-1.0.4/tests/test_attacks.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_attacks_dataset.py` & `aisdc-1.0.4/tests/test_attacks_dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_attacks_via_safemodel.py` & `aisdc-1.0.4/tests/test_attacks_via_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_attribute_inference_attack.py` & `aisdc-1.0.4/tests/test_attribute_inference_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_data_interface.py` & `aisdc-1.0.4/tests/test_data_interface.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_generate_report.py` & `aisdc-1.0.4/tests/test_generate_report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_lira_attack.py` & `aisdc-1.0.4/tests/test_lira_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_loaders.py` & `aisdc-1.0.4/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_metrics.py` & `aisdc-1.0.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.0.4/tests/test_safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_safekeras2.py` & `aisdc-1.0.4/tests/test_safekeras2.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_safemodel.py` & `aisdc-1.0.4/tests/test_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_saferandomforestclassifier.py` & `aisdc-1.0.4/tests/test_saferandomforestclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,20 +147,20 @@
     assert disclosive is False
     # but more detailed analysis says not
     msg2, disclosive2 = model.posthoc_check()
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="bootstrap", val=False, cur_val=True
     )
-    part3 = get_reporting_string(
-        name="param_changed_from_to",
-        key="base_estimator",
-        val="DecisionTreeClassifier()",
-        cur_val="DecisionTreeClassifier()",
-    )
+    part3 = ""  # get_reporting_string(
+    #        name="param_changed_from_to",
+    #        key="base_estimator",
+    #        val="DecisionTreeClassifier()",
+    #        cur_val="DecisionTreeClassifier()",
+    #    )
     correct_msg2 = part1 + part2 + part3
     # print(f'Correct: {correct_msg2}\n Actual: {msg2}')
 
     assert msg2 == correct_msg2, f"{msg2}\n should be {correct_msg2}"
     assert disclosive2 is True
 
 
@@ -263,20 +263,20 @@
     model.posthoc_check()
     msg, disclosive = diffsizemodel.posthoc_check()
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="max_depth", val="None", cur_val="2"
     )
     part3 = get_reporting_string(name="forest_estimators_differ", idx=5)
-    part4 = get_reporting_string(
-        name="param_changed_from_to",
-        key="base_estimator",
-        val="DecisionTreeClassifier()",
-        cur_val="DecisionTreeClassifier()",
-    )
+    part4 = ""  # get_reporting_string(
+    #        name="param_changed_from_to",
+    #        key="base_estimator",
+    #        val="DecisionTreeClassifier()",
+    #        cur_val="DecisionTreeClassifier()",
+    #    )
     correct_msg = part1 + part2 + part3 + part4
     # print(f'Correct:\n{correct_msg} Actual:\n{msg}')
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive, "should be flagged as disclosive"
 
 
 def test_randomforest_hacked_postfit_moretrees():
@@ -294,17 +294,17 @@
     diffsizemodel.saved_model = copy.deepcopy(the_saved_model)
     msg, disclosive = diffsizemodel.posthoc_check()
     part1 = get_reporting_string(name="basic_params_differ", length=1)
     part2 = get_reporting_string(
         name="param_changed_from_to", key="n_estimators", val="5", cur_val="10"
     )
     part3 = get_reporting_string(name="different_num_estimators", num1=10, num2=5)
-    part4 = get_reporting_string(
-        name="param_changed_from_to",
-        key="base_estimator",
-        val="DecisionTreeClassifier()",
-        cur_val="DecisionTreeClassifier()",
-    )
+    part4 = ""  # get_reporting_string(
+    #        name="param_changed_from_to",
+    #        key="base_estimator",
+    #        val="DecisionTreeClassifier()",
+    #        cur_val="DecisionTreeClassifier()",
+    #    )
     correct_msg = part1 + part2 + part3 + part4
     # print(f'Correct:\n{correct_msg} Actual:\n{msg}')
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive, "should be flagged as disclosive"
```

### Comparing `aisdc-1.0.3/tests/test_safesvc.py` & `aisdc-1.0.4/tests/test_safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.3/tests/test_worst_case_attack.py` & `aisdc-1.0.4/tests/test_worst_case_attack.py`

 * *Files identical despite different names*

