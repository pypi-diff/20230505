# Comparing `tmp/pandasflow-0.4.4.tar.gz` & `tmp/pandasflow-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.4.tar", last modified: Tue May  2 12:30:29 2023, max compression
+gzip compressed data, was "pandasflow-0.4.5.tar", last modified: Fri May  5 11:46:50 2023, max compression
```

## Comparing `pandasflow-0.4.4.tar` & `pandasflow-0.4.5.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.457468 pandasflow-0.4.4/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.4/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-02 12:30:29.457468 pandasflow-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.441322 pandasflow-0.4.4/pandasflow/
--rw-rw-rw-   0        0        0      302 2023-05-02 12:30:18.000000 pandasflow-0.4.4/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.444045 pandasflow-0.4.4/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.4/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.4/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.4/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.447909 pandasflow-0.4.4/pandasflow/metrics/
--rw-rw-rw-   0        0        0      216 2023-05-02 11:59:40.000000 pandasflow-0.4.4/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      671 2023-05-02 12:29:16.000000 pandasflow-0.4.4/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.4/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.4/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.4/pandasflow/metrics/mean_error.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.448470 pandasflow-0.4.4/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.4/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.4/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.448914 pandasflow-0.4.4/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.4/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.451062 pandasflow-0.4.4/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.4/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.4/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.4/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.444045 pandasflow-0.4.4/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-02 12:30:29.000000 pandasflow-0.4.4/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 12:30:29.457468 pandasflow-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:30:29.456802 pandasflow-0.4.4/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.4/test/__init__.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.4/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.4/test/test_best_f1.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.4/test/test_conf_mat.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.4/test/test_lloss_up.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.4/test/test_mean_error.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.4/test/test_split_tt.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.870513 pandasflow-0.4.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.5/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-05 11:46:50.870513 pandasflow-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.851564 pandasflow-0.4.5/pandasflow/
+-rw-rw-rw-   0        0        0      302 2023-05-05 11:46:46.000000 pandasflow-0.4.5/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.856550 pandasflow-0.4.5/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.5/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.5/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.5/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.860543 pandasflow-0.4.5/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      282 2023-05-05 11:28:21.000000 pandasflow-0.4.5/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-02 14:28:16.000000 pandasflow-0.4.5/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.5/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.5/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.5/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0     1090 2023-05-05 11:45:57.000000 pandasflow-0.4.5/pandasflow/metrics/precision_recall.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.861546 pandasflow-0.4.5/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.5/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.5/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.861546 pandasflow-0.4.5/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.5/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.863532 pandasflow-0.4.5/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.5/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.4.5/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.4.5/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.855553 pandasflow-0.4.5/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 11:46:50.000000 pandasflow-0.4.5/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:46:50.871511 pandasflow-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:46:50.869517 pandasflow-0.4.5/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.5/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.5/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.5/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.5/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.5/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1274 2023-05-05 11:44:42.000000 pandasflow-0.4.5/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.5/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.5/test/split_tvt_test.py
```

### Comparing `pandasflow-0.4.4/LICENCE` & `pandasflow-0.4.5/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/PKG-INFO` & `pandasflow-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.4
+Version: 0.4.5
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.4/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.5/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/pandasflow/metrics/best_f1.py` & `pandasflow-0.4.5/pandasflow/metrics/best_f1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import pandas as pd
 from sklearn.metrics import f1_score
 from tqdm.notebook import tqdm
 
 
-def best_f1(y_true:pd.Series, score:pd.Series, out=1, tqdm_=True):
+def best_f1(y_true:pd.Series, score:pd.Series, out:int=1, tqdm_:bool=True):
 	thrs = list(score.unique())
-	thrs = [max(min(thrs) - 0.000001, 0)] + thrs
+	thrs = [max(min(thrs) - 0.000001, 0.000001)] + thrs
 	
 	df = pd.concat([y_true, score], axis=1)
 	
 	result = []
 	
 	if tqdm_: thrs = tqdm(thrs)
```

### Comparing `pandasflow-0.4.4/pandasflow/metrics/conf_mat.py` & `pandasflow-0.4.5/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/pandasflow/metrics/lloss_up.py` & `pandasflow-0.4.5/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/pandasflow/reset_mi.py` & `pandasflow-0.4.5/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/pandasflow/split/train_test.py` & `pandasflow-0.4.5/pandasflow/split/train_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,24 +66,24 @@
 	table = pd.DataFrame({
 		'count': [len(train),
 			  len(test),
 			  '',
 			  amount_len,
 			  len(arrays[0])],
 		
-		'prop': [train_pie,
+		'pct': [train_pie,
 			   test_pie,
 			   '',
 			   amount_prop,
 			   '']
 	})
 	
 	table.index = ['train',
 				   'test',
-				   '---',
+				   '',
 				   'Amount',
 				   'InitData']
 	
 	if target != None:
 		try:
 			if type(target) is str:
 				table[target] = [train[target].mean(),
```

### Comparing `pandasflow-0.4.4/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.5/pandasflow/split/train_valid_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 		'count': [len(train),
 				len(valid),
 				len(test),
 				'',
 				amount_len,
 				len(df)],
 		
-		'prop': [train_pie,
+		'pct': [train_pie,
 				 valid_pie,
 				 test_pie,
 				 '',
 				 amount_prop,
 				 ''],
 		
 		
@@ -116,15 +116,15 @@
 									df[col].mean()]
 		except KeyError:
 			raise KeyError(*target)
 	
 	table.index = ['train',
 				   'valid',
 				   'test',
-				   '---',
+				   '',
 				   'Amount',
 				   'InitData']
 	print(table)
 	
 	
 	if amount_prop != 1.0 or len(df) != amount_len:
 		print('---')
```

### Comparing `pandasflow-0.4.4/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.5/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.4
+Version: 0.4.5
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.4/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.5/pandasflow.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
 pandasflow/metrics/__init__.py
 pandasflow/metrics/best_f1.py
 pandasflow/metrics/conf_mat.py
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
+pandasflow/metrics/precision_recall.py
 pandasflow/model/__init__.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
-test/split_tvt_test.py
-test/test_best_f1.py
-test/test_conf_mat.py
-test/test_lloss_up.py
-test/test_mean_error.py
-test/test_split_tt.py
+test/best_f1_test.py
+test/conf_mat_test.py
+test/lloss_up_test.py
+test/mean_error_test.py
+test/precision_recall_test.py
+test/split_tt_test.py
+test/split_tvt_test.py
```

### Comparing `pandasflow-0.4.4/setup.py` & `pandasflow-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/test/split_tvt_test.py` & `pandasflow-0.4.5/test/split_tvt_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/test/test_best_f1.py` & `pandasflow-0.4.5/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/test/test_conf_mat.py` & `pandasflow-0.4.5/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.4/test/test_lloss_up.py` & `pandasflow-0.4.5/test/lloss_up_test.py`

 * *Files identical despite different names*

