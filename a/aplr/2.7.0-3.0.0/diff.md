# Comparing `tmp/aplr-2.7.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-3.0.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 293690 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   323072 b- defN 23-May-04 15:05 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   335360 b- defN 23-May-04 15:09 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-04 15:01 aplr/__init__.py
--rw-rw-rw-  2.0 fat     6214 b- defN 23-May-04 15:01 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      626 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      690 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/RECORD
-9 files, 667236 bytes uncompressed, 292518 bytes compressed:  56.2%
+Zip file size: 297251 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   327680 b- defN 23-May-05 15:24 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   340992 b- defN 23-May-05 15:29 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-05 15:20 aplr/__init__.py
+-rw-rw-rw-  2.0 fat     6307 b- defN 23-May-05 15:20 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-May-05 15:29 aplr-3.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      626 b- defN 23-May-05 15:29 aplr-3.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-05 15:29 aplr-3.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-05 15:29 aplr-3.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      690 b- defN 23-May-05 15:29 aplr-3.0.0.dist-info/RECORD
+9 files, 677569 bytes uncompressed, 296079 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-2.7.0.dist-info/LICENSE
+Filename: aplr-3.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-2.7.0.dist-info/METADATA
+Filename: aplr-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-2.7.0.dist-info/WHEEL
+Filename: aplr-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-2.7.0.dist-info/top_level.txt
+Filename: aplr-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-2.7.0.dist-info/RECORD
+Filename: aplr-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -1,56 +1,56 @@
 import numpy as np
 import numpy.typing as npt
 from typing import List
 import aplr_cpp
 
 
 class APLRRegressor():
-    def __init__(self, m:int=1000, v:float=0.1, random_state:int=0, family:str="gaussian", link_function:str="identity", n_jobs:int=0, validation_ratio:float=0.2, intercept:float=np.nan, bins:int=300, max_interaction_level:int=1, max_interactions:int=100000, min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5, verbosity:int=0, tweedie_power:float=1.5, validation_tuning_metric:str="default", quantile:float=0.5):
+    def __init__(self, m:int=1000, v:float=0.1, random_state:int=0, loss_function:str="mse", link_function:str="identity", n_jobs:int=0, validation_ratio:float=0.2, intercept:float=np.nan, bins:int=300, max_interaction_level:int=1, max_interactions:int=100000, min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5, verbosity:int=0, dispersion_parameter:float=1.5, validation_tuning_metric:str="default", quantile:float=0.5):
         self.m=m
         self.v=v
         self.random_state=random_state
-        self.family=family
+        self.loss_function=loss_function
         self.link_function=link_function
         self.n_jobs=n_jobs
         self.validation_ratio=validation_ratio
         self.intercept=intercept
         self.bins=bins
         self.max_interaction_level=max_interaction_level
         self.max_interactions=max_interactions
         self.min_observations_in_split=min_observations_in_split
         self.ineligible_boosting_steps_added=ineligible_boosting_steps_added
         self.max_eligible_terms=max_eligible_terms
         self.verbosity=verbosity
-        self.tweedie_power=tweedie_power
+        self.dispersion_parameter=dispersion_parameter
         self.validation_tuning_metric=validation_tuning_metric
         self.quantile=quantile
 
         #Creating aplr_cpp and setting parameters
         self.APLRRegressor=aplr_cpp.APLRRegressor()
         self.__set_params_cpp()
 
     #Sets parameters for aplr_cpp.APLRRegressor cpp object
     def __set_params_cpp(self):
         self.APLRRegressor.m=self.m
         self.APLRRegressor.v=self.v
         self.APLRRegressor.random_state=self.random_state
-        self.APLRRegressor.family=self.family
+        self.APLRRegressor.loss_function=self.loss_function
         self.APLRRegressor.link_function=self.link_function
         self.APLRRegressor.n_jobs=self.n_jobs
         self.APLRRegressor.validation_ratio=self.validation_ratio
         self.APLRRegressor.intercept=self.intercept
         self.APLRRegressor.bins=self.bins
         self.APLRRegressor.max_interaction_level=self.max_interaction_level
         self.APLRRegressor.max_interactions=self.max_interactions
         self.APLRRegressor.min_observations_in_split=self.min_observations_in_split
         self.APLRRegressor.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
         self.APLRRegressor.max_eligible_terms=self.max_eligible_terms
         self.APLRRegressor.verbosity=self.verbosity
-        self.APLRRegressor.tweedie_power=self.tweedie_power
+        self.APLRRegressor.dispersion_parameter=self.dispersion_parameter
         self.APLRRegressor.validation_tuning_metric=self.validation_tuning_metric
         self.APLRRegressor.quantile=self.quantile
 
     def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[], group:npt.ArrayLike = np.empty(0), interaction_constraints:List[int]=[]):
         self.__set_params_cpp()
         self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group,interaction_constraints)
 
@@ -101,27 +101,27 @@
 
     #For sklearn
     def get_params(self, deep=True):
         return {
             "m": self.m,
             "v": self.v,
             "random_state":self.random_state,
-            "family":self.family,
+            "loss_function":self.loss_function,
             "link_function":self.link_function,
             "n_jobs":self.n_jobs,
             "validation_ratio":self.validation_ratio,
             "intercept":self.intercept,
             "bins":self.bins,
             "max_interaction_level":self.max_interaction_level,
             "max_interactions":self.max_interactions,
             "verbosity":self.verbosity,
             "min_observations_in_split":self.min_observations_in_split,
             "ineligible_boosting_steps_added":self.ineligible_boosting_steps_added,
             "max_eligible_terms":self.max_eligible_terms,
-            "tweedie_power":self.tweedie_power,
+            "dispersion_parameter":self.dispersion_parameter,
             "validation_tuning_metric":self.validation_tuning_metric,
             "quantile":self.quantile
         }
 
     #For sklearn
     def set_params(self, **parameters):
         for parameter, value in parameters.items():
```

## Comparing `aplr-2.7.0.dist-info/LICENSE` & `aplr-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-2.7.0.dist-info/METADATA` & `aplr-3.0.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 2.7.0
+Version: 3.0.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

