# Comparing `tmp/pandasflow-0.4.5.tar.gz` & `tmp/pandasflow-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.5.tar", last modified: Fri May  5 11:46:50 2023, max compression
+gzip compressed data, was "pandasflow-0.4.6.tar", last modified: Fri May  5 12:04:42 2023, max compression
```

## Comparing `pandasflow-0.4.5.tar` & `pandasflow-0.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.870513 pandasflow-0.4.5/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.5/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-05 11:46:50.870513 pandasflow-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.851564 pandasflow-0.4.5/pandasflow/
--rw-rw-rw-   0        0        0      302 2023-05-05 11:46:46.000000 pandasflow-0.4.5/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.856550 pandasflow-0.4.5/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.5/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.5/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.5/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.860543 pandasflow-0.4.5/pandasflow/metrics/
--rw-rw-rw-   0        0        0      282 2023-05-05 11:28:21.000000 pandasflow-0.4.5/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-02 14:28:16.000000 pandasflow-0.4.5/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.5/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.5/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.5/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0     1090 2023-05-05 11:45:57.000000 pandasflow-0.4.5/pandasflow/metrics/precision_recall.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.861546 pandasflow-0.4.5/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.5/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.5/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.861546 pandasflow-0.4.5/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.5/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.863532 pandasflow-0.4.5/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.5/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.4.5/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.4.5/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.855553 pandasflow-0.4.5/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 11:46:50.871511 pandasflow-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.869517 pandasflow-0.4.5/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.5/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.5/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.5/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.5/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.5/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1274 2023-05-05 11:44:42.000000 pandasflow-0.4.5/test/precision_recall_test.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.5/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.5/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.215124 pandasflow-0.4.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.6/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-05 12:04:42.215124 pandasflow-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.199631 pandasflow-0.4.6/pandasflow/
+-rw-rw-rw-   0        0        0      302 2023-05-05 12:04:35.000000 pandasflow-0.4.6/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.202813 pandasflow-0.4.6/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.6/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.6/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.6/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.207059 pandasflow-0.4.6/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      282 2023-05-05 11:28:21.000000 pandasflow-0.4.6/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-02 14:28:16.000000 pandasflow-0.4.6/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.6/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.6/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.6/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0     1110 2023-05-05 12:01:55.000000 pandasflow-0.4.6/pandasflow/metrics/precision_recall.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.207690 pandasflow-0.4.6/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.6/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.6/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.208147 pandasflow-0.4.6/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.6/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.209145 pandasflow-0.4.6/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.6/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.4.6/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.4.6/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.202278 pandasflow-0.4.6/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-05 12:04:42.000000 pandasflow-0.4.6/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2023-05-05 12:04:42.000000 pandasflow-0.4.6/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:04:42.000000 pandasflow-0.4.6/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-05 12:04:42.000000 pandasflow-0.4.6/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 12:04:42.000000 pandasflow-0.4.6/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:04:42.215124 pandasflow-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:04:42.214126 pandasflow-0.4.6/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.6/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.6/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.6/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.6/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.6/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1285 2023-05-05 12:03:43.000000 pandasflow-0.4.6/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.6/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.6/test/split_tvt_test.py
```

### Comparing `pandasflow-0.4.5/LICENCE` & `pandasflow-0.4.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/PKG-INFO` & `pandasflow-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.5
+Version: 0.4.6
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.5/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.6/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/metrics/best_f1.py` & `pandasflow-0.4.6/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/metrics/conf_mat.py` & `pandasflow-0.4.6/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/metrics/lloss_up.py` & `pandasflow-0.4.6/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/reset_mi.py` & `pandasflow-0.4.6/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/split/train_test.py` & `pandasflow-0.4.6/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.6/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.6/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.5
+Version: 0.4.6
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.5/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.6/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/setup.py` & `pandasflow-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/test/best_f1_test.py` & `pandasflow-0.4.6/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/test/conf_mat_test.py` & `pandasflow-0.4.6/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/test/lloss_up_test.py` & `pandasflow-0.4.6/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.5/test/precision_recall_test.py` & `pandasflow-0.4.6/test/precision_recall_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 t['y_score1'] = np.concatenate([np.random.uniform(0, 0.2, size=970),
                                 np.random.uniform(0.8, 1, size=20),
                                 np.random.uniform(0, 0.2, size=5),
                                 np.random.uniform(0.8, 1, size=5)])
 
 t['y_score2'] = np.concatenate([np.random.uniform(0, 0.2, size=900), #TN
-                                np.random.uniform(0.8, 1, size=90), #FP
+                                np.random.uniform(0.8, 1, size=90),  #FP
                                 np.random.uniform(0, 0.2, size=4),   #FN
                                 np.random.uniform(0.8, 1, size=6)])  #TP
 
 t['y_score3'] = np.concatenate([np.random.uniform(0, 0.2, size=850), #TN
                                 np.random.uniform(0.8, 1, size=140), #FP
                                 np.random.uniform(0, 0.2, size=2),   #FN
                                 np.random.uniform(0.8, 1, size=8)])  #TP
 
 
 
-pdf.metrics.precision_recall(t, target='y_true', score=['y_score1'])
+# pdf.metrics.precision_recall(t['y_true'], score=t['y_score1'])
 
-pdf.metrics.precision_recall(t, target='y_true', score=['y_score1', 'y_score2'])
+# pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2']])
 
-pdf.metrics.precision_recall(t, target='y_true', score=['y_score1', 'y_score2', 'y_score3'])
+pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
```

### Comparing `pandasflow-0.4.5/test/split_tvt_test.py` & `pandasflow-0.4.6/test/split_tvt_test.py`

 * *Files identical despite different names*

