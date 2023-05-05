# Comparing `tmp/pdcscore-1.0.9.tar.gz` & `tmp/pdcscore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.0.9.tar", last modified: Thu May  4 16:47:51 2023, max compression
+gzip compressed data, was "pdcscore-1.1.0.tar", last modified: Fri May  5 20:35:08 2023, max compression
```

## Comparing `pdcscore-1.0.9.tar` & `pdcscore-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.758205 pdcscore-1.0.9/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     4931 2023-05-04 16:47:51.758205 pdcscore-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3687 2023-05-04 16:46:18.000000 pdcscore-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.737174 pdcscore-1.0.9/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.9/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.9/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.756207 pdcscore-1.0.9/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4931 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 16:47:51.759212 pdcscore-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1608 2023-05-04 16:46:13.000000 pdcscore-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.147213 pdcscore-1.1.0/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4963 2023-05-05 20:35:08.146213 pdcscore-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-05-04 17:21:47.000000 pdcscore-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.122213 pdcscore-1.1.0/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.1.0/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3524 2023-05-05 20:23:41.000000 pdcscore-1.1.0/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.144212 pdcscore-1.1.0/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     4963 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:35:08.147213 pdcscore-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-05-05 20:32:31.000000 pdcscore-1.1.0/setup.py
```

### Comparing `pdcscore-1.0.9/LICENSE` & `pdcscore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.9/PKG-INFO` & `pdcscore-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
-Home-page: UNKNOWN
+Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -87,15 +87,15 @@
                                        '2022-03-31', '2022-03-31', '2022-03-31'])
 })
 
 # Inspect sample data
 df.head(n=len(df))
 
 # calculate PDC scores on the input DataFrame
-calcfunc= pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
+calcfunc = pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
                                          , filldate_col='RX_FILLED_DT', supply_days_col='DAYS_SPLY_NBR'
                                          , mbr_elig_start_dt_col='START_DT', mbr_elig_end_dt_col='END_DT')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
```

### Comparing `pdcscore-1.0.9/README.md` & `pdcscore-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,14 @@
                                        '2022-03-31', '2022-03-31', '2022-03-31'])
 })
 
 # Inspect sample data
 df.head(n=len(df))
 
 # calculate PDC scores on the input DataFrame
-calcfunc= pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
+calcfunc = pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
                                          , filldate_col='RX_FILLED_DT', supply_days_col='DAYS_SPLY_NBR'
                                          , mbr_elig_start_dt_col='START_DT', mbr_elig_end_dt_col='END_DT')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
```

### Comparing `pdcscore-1.0.9/pdcscore/pdcscore.py` & `pdcscore-1.1.0/pdcscore/pdcscore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-       
-"""
-Author: Daniel Famutimi
-Package Name: pdcscore
-Usage:
-    A package to faciliate efficent calculation of the medication adherence metric
-        "Proportion of Days Covered" or "PDC".
-    Currently contains a single public function (calculate_pdc) to calculate PDC at either the
-        member level or the member-drug level as desired. 
-"""
-
 import numpy as np
 import pandas as pd
 from multiprocessing import Pool, cpu_count
 
 class pdccalc:
     def __init__(self, dataframe, patient_id_col, drugname_col, filldate_col,
                           supply_days_col, mbr_elig_start_dt_col,
@@ -28,19 +17,28 @@
         self.drugs = set(dataframe[drugname_col])
         self.pdc_scores_df = pd.DataFrame(columns=[patient_id_col, drugname_col, 'DAYSCOVERED', 'TOTALDAYS', 'PDC_SCORE'])
         
     def calculate_pdc_for_patient_drug(self, patient_id, drug):
         subset = self.dataframe[(self.dataframe[self.patient_id_col] == patient_id) & (self.dataframe[self.drugname_col] == drug)]
         if subset.empty:
             return None
+        
+        # determine if the first fill date precedes mbr_elig_start_dt_col by <=6 months
+        first_fill_date = subset[self.filldate_col].min()
+        mbr_elig_start_dt = subset[self.mbr_elig_start_dt_col].iloc[0]
+        if (first_fill_date - mbr_elig_start_dt) <= pd.Timedelta(days=6*30):
+            start_date = mbr_elig_start_dt
+        else:
+            start_date = max(first_fill_date, mbr_elig_start_dt)
+        
         dates = []
         for i, row in subset.iterrows():
-            start_date = max(row[self.filldate_col], row[self.mbr_elig_start_dt_col])
             end_date = min(row[self.filldate_col] + pd.Timedelta(days=row[self.supply_days_col]), row[self.mbr_elig_end_dt_col])
-            dates.append((start_date, end_date))
+            if end_date >= start_date:
+                dates.append((start_date, end_date))
         dates.sort()
         merged_dates = [dates[0]]
         for date_range in dates[1:]:
             if date_range[0] <= merged_dates[-1][1]:
                 merged_dates[-1] = (merged_dates[-1][0], max(date_range[1], merged_dates[-1][1]))
             else:
                 merged_dates.append(date_range)
@@ -68,8 +66,8 @@
         
         for result in results:
             data = result.get()
             if data is not None:
                 self.pdc_scores_df = pd.concat([self.pdc_scores_df, pd.DataFrame.from_records([data])])
                 
         self.pdc_scores_dataframe = self.pdc_scores_df.sort_values(by=[self.patient_id_col, self.drugname_col]).reset_index(drop=True)
-        return self.pdc_scores_dataframe
+        return self.pdc_scores_dataframe
```

### Comparing `pdcscore-1.0.9/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.1.0/pdcscore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
-Home-page: UNKNOWN
+Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -87,15 +87,15 @@
                                        '2022-03-31', '2022-03-31', '2022-03-31'])
 })
 
 # Inspect sample data
 df.head(n=len(df))
 
 # calculate PDC scores on the input DataFrame
-calcfunc= pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
+calcfunc = pdccalc(dataframe=df, patient_id_col='MCID', drugname_col='DRUGNAME'
                                          , filldate_col='RX_FILLED_DT', supply_days_col='DAYS_SPLY_NBR'
                                          , mbr_elig_start_dt_col='START_DT', mbr_elig_end_dt_col='END_DT')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
```

### Comparing `pdcscore-1.0.9/setup.py` & `pdcscore-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.0.9',
+    version='1.1.0',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    # url='https://github.com/<username>/<repository>',
+    url='https://github.com/famutimine/pdcscore',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Healthcare Industry',
```

