# Comparing `tmp/cefeste-1.0.3.tar.gz` & `tmp/cefeste-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.0.3.tar", last modified: Mon Apr  3 12:25:22 2023, max compression
+gzip compressed data, was "cefeste-1.1.0.tar", last modified: Fri May  5 08:29:51 2023, max compression
```

## Comparing `cefeste-1.0.3.tar` & `cefeste-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.471492 cefeste-1.0.3/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-03-27 17:15:12.000000 cefeste-1.0.3/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-04-03 12:25:22.471492 cefeste-1.0.3/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1558 2023-03-27 17:15:12.000000 cefeste-1.0.3/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-04-03 12:24:52.000000 cefeste-1.0.3/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-04-03 12:25:22.471492 cefeste-1.0.3/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-04-03 12:25:01.000000 cefeste-1.0.3/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    13889 2023-03-31 13:12:22.000000 cefeste-1.0.3/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    29692 2023-04-03 12:23:48.000000 cefeste-1.0.3/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2369 2023-03-27 17:15:12.000000 cefeste-1.0.3/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-04-03 12:25:22.467492 cefeste-1.0.3/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-04-03 12:25:22.000000 cefeste-1.0.3/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-04-03 12:25:22.000000 cefeste-1.0.3/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-04-03 12:25:22.000000 cefeste-1.0.3/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-04-03 12:25:22.000000 cefeste-1.0.3/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-04-03 12:25:22.000000 cefeste-1.0.3/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.014606 cefeste-1.1.0/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.0/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-05 08:29:51.010606 cefeste-1.1.0/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1558 2023-05-05 08:25:33.000000 cefeste-1.1.0/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-05 08:25:52.000000 cefeste-1.1.0/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-05 08:29:51.014606 cefeste-1.1.0/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-05 08:25:52.000000 cefeste-1.1.0/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.002606 cefeste-1.1.0/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.006605 cefeste-1.1.0/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    13908 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25190 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-05 08:29:51.000000 cefeste-1.1.0/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.0.3/LICENCE` & `cefeste-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/PKG-INFO` & `cefeste-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.0.3
+Version: 1.1.0
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.0.3/README.md` & `cefeste-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/pyproject.toml` & `cefeste-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.0.3/setup.py` & `cefeste-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.0.3",
+    version="1.1.0",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.0.3/src/cefeste/__init__.py` & `cefeste-1.1.0/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/elimination/__init__.py` & `cefeste-1.1.0/src/cefeste/elimination/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         # Hyperparameters Tuning / Cross Validation Fold
         cv_funct=RandomizedSearchCV,
         cv_scoring="auto",
         n_iter=20,
         manage_groups=False,
         groups=None,
         cv_type=StratifiedKFold(5, random_state=42, shuffle=True),
-        manage_cats=False,
+        use_ohe=False,
         # Reporting
         step_size=0.1,
         min_n_feat_step=5,
         final_n_feature=1,
         verbose=True,
         write_final=False,
         write_substep=False,
@@ -52,15 +52,15 @@
             cv_funct: function or class for the Cross Validation. Defaults to RandomizedSearchCV
             cv_scoring: scoring argument of the cv_functs. Defaults to "auto" selects "roc_auc" fo classification, "r2" for regression 
                 and "balanced accuracy" for multiclass.
             n_iter (int, optional): number of iteration, i.e. set of hyperparams tested in Cross Validation. Defaults to 20.
             manage_groups (bool, optional): determines if there is a feature whose groups have to be kept joined in CV. Defaults to False.
             groups (pd.Series, optional): feature whose groups have to be kept joined in CV. Defaults to None.
             cv_type : function or class for defining the CV sets. Defaults to StratifiedKFold(5, random_state=42, shuffle=True).
-            manage_cats (bool, optional): determines if there are categorical features to be preprocessed. Defaults to False.
+            use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to False.
             step_size (int or float, optional): determines how many features to remove at each step.
                 Fixed int or percentage of total features. Defaults to 0.1.
             min_n_feat_step (int, optional): min number of feature to remove at each step. Defaults to 5.
             final_n_feature (int, optional): number of features of the last model. Defaults to 1.
             verbose (bool, optional): If True print a log of information. Defaults to True.
             write_final (bool, optional): If True it saves in the current directory the final report that can be used for quick start. Defaults to False.
             write_substep (bool, optional): If True it saves in the current directory the report after SHAP_RFE that can be used for quick start. Defaults to False.
@@ -122,15 +122,15 @@
         self.grid = grid
         self.cv_funct = cv_funct
         self.cv_scoring = cv_scoring
         self.n_iter = n_iter
         self.manage_groups = manage_groups
         self.groups = groups
         self.cv_type = cv_type
-        self.manage_cats = manage_cats
+        self.use_ohe = use_ohe
         self.step_size = step_size
         self.min_n_feat_step = min_n_feat_step
         self.final_n_feature = final_n_feature
         self.verbose = verbose
         self.write_final = write_final
         self.write_substep = write_substep
         self.dim_cat_threshold = dim_cat_threshold
@@ -179,19 +179,19 @@
             elif not self.groups.index.equals(self.db.index):
                 raise ValueError("Groups Series index do not match with DataFrame index in input!")
             else:
                 self.groups = self.groups.reset_index(drop=True).iloc[X_train.index]
         else:
             self.groups = None
 
-        # Categorical Features
-        if self.manage_cats:
-            self.categorical_features_list = get_categorical_features(X_train)
+        # Categorical Features for One Hot Encoding
+        if self.use_ohe:
+            self.categorical_features_list_ohe = get_categorical_features(X_train)
         else:
-            self.categorical_features_list = []
+            self.categorical_features_list_ohe = []
 
         shap_report = Shap_RFE_full(
             X_train,
             y_train,
             model=self.model,
             grid=self.grid,
             cv_funct=self.cv_funct,
@@ -203,16 +203,16 @@
             algo_type=self.algo_type,
             step_size=self.step_size,
             min_n_feat_step=self.min_n_feat_step,
             final_n_feature=self.final_n_feature,
             verbose=self.verbose,
             write_final=self.write_final,
             write_substep=self.write_substep,
-            manage_cats=self.manage_cats,
-            categorical_features_list=self.categorical_features_list,
+            use_ohe=self.use_ohe,
+            categorical_features_list_ohe=self.categorical_features_list_ohe,
             dim_cat_threshold=self.dim_cat_threshold,
         )
 
         self.report = shap_report
 
         return self.report
```

### Comparing `cefeste-1.0.3/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.0/src/cefeste/elimination/shap_rfe.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     algo_type="classification",
     step_size=0.1,
     min_n_feat_step=5,
     final_n_feature=1,
     verbose=True,
     write_final=False,
     write_substep=False,
-    manage_cats=True,
-    categorical_features_list=None,
+    use_ohe=True,
+    categorical_features_list_ohe=None,
     dim_cat_threshold=10,
 ):
     """Recursive Feature Elimination Process with Hyperparameters grid search.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
@@ -50,16 +50,16 @@
         step_size (int or float, optional): determines how many features to remove at each step.
             Fixed int or percentage of total features. Defaults to 0.1.
         min_n_feat_step (int, optional): min number of feature to remove at each step. Defaults to 5.
         final_n_feature (int, optional): number of features of the last model. Defaults to 1.
         verbose (bool, optional): If True print a log of information. Defaults to True.
         write_final (bool, optional): If True it saves in the current directory the final report that can be used for quick start. Defaults to False.
         write_substep (bool, optional): If True it saves in the current directory the report after SHAP_RFE that can be used for quick start. Defaults to False.
-        manage_cats (bool, optional): determines if there are categorical features to be preprocessed. Defaults to True.
-        categorical_features_list (list, optional): list of categorical features. Defaults to None.
+        use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to True.
+        categorical_features_list_ohe (list, optional): list of categorical features for One Hot Encoding. Defaults to None.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
 
     Return:
     pd.DataFrame: Report of the detail and result of each step of FE and Grid Search.
     """
     if groups is None:
@@ -94,100 +94,69 @@
                 )
             )
         number_splits = cv_type.n_splits
         CVSel_algo.cv = GroupKFold(number_splits).split(X_train, y_train, groups)
     else:
         number_splits = None
 
-    # Check categorical features
-    if not manage_cats:
-        if len(get_categorical_features(X_train)) > 0:
-            raise ValueError("dataset contains categorical features")
-
     # Perform Shap Recursive Feature Elimination
     report = Shap_RFE(
         X_train,
         y_train,
         CVSel_algo,
         algo_type=algo_type,
         step_size=step_size,
         min_n_feat_step=min_n_feat_step,
         final_n_feature=final_n_feature,
         verbose=verbose,
         write=write_substep,
-        manage_cats=manage_cats,
-        categorical_features_list=categorical_features_list,
+        use_ohe=use_ohe,
+        categorical_features_list_ohe=categorical_features_list_ohe,
         number_splits=number_splits,
         dim_cat_threshold=dim_cat_threshold,
     )
     # Train the final model
     X_train = X_train[report["feat_select"].iloc[-1]]
     initial_feat_n = X_train.shape[1]
     if manage_groups:
         CVSel_algo.cv = GroupKFold(number_splits).split(X_train, y_train, groups)
-    if manage_cats:
-        cats_feat = list(set(categorical_features_list) & set(X_train.columns))
-        if str(CVSel_algo.estimator.__class__()).startswith("LGBM"):
-            # Categorical Preprocessing with LGBM - Label-Encoder
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OrdinalEncoder(handle_unknown="error"), cats_feat),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train), columns=feat_names)
-
-            CVSel_algo.fit(X_train_tsf, y_train, categorical_feature=cats_feat)
-        # Categorical Preprocessing without LGBM - Hot-One-Encoder
-        else:
-            X_train_tsf = X_train.copy()
-            for col in cats_feat:
-                if X_train_tsf[col].nunique() > dim_cat_threshold:
-                    values_cat = list(
-                        X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                    )[:dim_cat_threshold]
-                    for val in values_cat:
-                        X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
-                    X_train_tsf = X_train_tsf.drop(columns=col)
-                    cats_feat.remove(col)
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train_tsf)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
-
-            CVSel_algo.fit(X_train_tsf, y_train)
+    X_train_tsf = X_train.copy()
+    if use_ohe:
+        cats_feat = list(set(categorical_features_list_ohe) & set(X_train.columns))   
+        for col in cats_feat:
+            if X_train_tsf[col].nunique() > dim_cat_threshold:
+                values_cat = list(
+                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
+                )[:dim_cat_threshold]
+                for val in values_cat:
+                    X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
+                X_train_tsf = X_train_tsf.drop(columns=col)
+                cats_feat.remove(col)
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
+            ],
+            remainder="passthrough",
+        )
+        preprocessor.fit(X_train_tsf)
+        feat_names = preprocessor.get_feature_names_out()
+        feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
+        X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
     else:
-        CVSel_algo.fit(X_train, y_train)
+        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+    CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
     # Get measure
     if algo_type == "classification":
-        if manage_cats:
-            train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
-        else:
-            train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train)[:, 1])
+        train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
     elif algo_type == "regression":
-        if manage_cats:
-            train_model_score = r2_score(y_train, CVSel_algo.predict(X_train_tsf))
-        else:
-            train_model_score = r2_score(y_train, CVSel_algo.predict(X_train))
+        train_model_score = r2_score(y_train, CVSel_algo.predict(X_train_tsf))
     elif algo_type == "multiclass":
-        if manage_cats:
-            train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
-        else:
-            train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train))
+        train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
 
     valid_model_score = CVSel_algo.best_score_
     report_step = pd.DataFrame(
         {
             "n_feat": [initial_feat_n],
             "train_score": [train_model_score],
             "valid_score": [valid_model_score],
@@ -213,16 +182,16 @@
     CVSel_algo,
     algo_type="classification",
     step_size=0.1,
     min_n_feat_step=5,
     final_n_feature=1,
     verbose=True,
     write=True,
-    manage_cats=False,
-    categorical_features_list=None,
+    use_ohe=False,
+    categorical_features_list_ohe=None,
     manage_groups=False,
     groups=None,
     number_splits=5,
     dim_cat_threshold=10,
 ):
     """Recursive Feature Elimination Process with Hyperparameters grid search.
 
@@ -233,29 +202,29 @@
         algo_type: "classification", "regression" or "multiclass", describes the problem type. Defaults to "classification".
         step_size (int or float): determines how many features to remove at each step.
             Fixed int or percentage of total features. Defaults to 0.1.
         min_n_feat_step (int): min number of feature to remove at each step. Defaults to 5.
         final_n_feature (int): number of features of the last model. Defaults to 1.
         verbose (bool): If True print a log of information. Defaults to True.
         write (bool): If True it saves in the current directory the report that can be used for quick start. Defaults to True.
-        manage_cats (bool, optional): determines if there are categorical features to be preprocessed. Defaults to False.
-        categorical_features_list (list, optional): list of categorical features. Defaults to None.
+        use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to False.
+        categorical_features_list_ohe (list, optional): list of categorical features for One Hot Encoding. Defaults to None.
         manage_groups (bool, optional): determines if there is a feature whose groups have to be kept joined in CV. Defaults to False.
         groups (pd.Series, optional): feature whose groups have to be kept joined in CV. Defaults to None.
         number_splits (int, optional): number of splits in CV for GroupFold. Defaults to 5.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
 
 
     Return:
     pd.DataFrame: Report of the detail and result of each step of FE and Grid Search.
     """
     initial_feat_n = X_train.shape[1]
-    if manage_cats:
-        cats_feat = list(set(X_train.columns) & set(categorical_features_list))
+    if use_ohe:
+        cats_feat = list(set(X_train.columns) & set(categorical_features_list_ohe))
 
         if algo_type == "classification":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_AUC(
                 X_train, y_train, CVSel_algo, categorical_feature=cats_feat, dim_cat_threshold=dim_cat_threshold
             )
         elif algo_type == "regression":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_R2(
@@ -311,16 +280,16 @@
             CVSel_algo,
             algo_type,
             step_size,
             min_n_feat_step,
             final_n_feature,
             verbose,
             write,
-            manage_cats,
-            categorical_features_list,
+            use_ohe,
+            categorical_features_list_ohe,
             manage_groups,
             groups,
             number_splits=number_splits,
             dim_cat_threshold=dim_cat_threshold,
         )
         report = pd.concat([report, report_step])
 
@@ -391,163 +360,124 @@
 def get_Shap_AUC(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
     """Get the AUC of the model and Features' Shapley Value.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
         CVSel_algo: class that include the classifier, grid search and detail of CV selection.
-        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to [].
+        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
     Returns:
         (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid AUC.
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Estimate
     categorical_shap_ohe = False
+    X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
-        if str(CVSel_algo.estimator.__class__()).startswith("LGBM"):
-            # Categorical Preprocessing with LGBM - Label-Encoder
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OrdinalEncoder(handle_unknown="error"), categorical_feature),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train), columns=feat_names)
-
-            CVSel_algo.fit(X_train_tsf, y_train, categorical_feature=categorical_feature)
-        # Categorical Preprocessing without LGBM - Hot-One-Encoder
-        else:
-            cats_feat = categorical_feature.copy()
-            X_train_tsf = X_train.copy()
-            for col in cats_feat:
-                if X_train_tsf[col].nunique() > dim_cat_threshold:
-                    values_cat = list(
-                        X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                    )[:dim_cat_threshold]
-                    for val in values_cat:
-                        X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
-                    X_train_tsf = X_train_tsf.drop(columns=col)
-                    cats_feat.remove(col)
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train_tsf)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
-            categorical_shap_ohe = True
+        # Categorical Preprocessing Hot-One-Encoder
+        cats_feat = categorical_feature.copy()
+        for col in cats_feat:
+            if X_train_tsf[col].nunique() > dim_cat_threshold:
+                values_cat = list(
+                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
+                )[:dim_cat_threshold]
+                for val in values_cat:
+                    X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
+                X_train_tsf = X_train_tsf.drop(columns=col)
+                cats_feat.remove(col)
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
+            ],
+            remainder="passthrough",
+        )
+        preprocessor.fit(X_train_tsf)
+        feat_names = preprocessor.get_feature_names_out()
+        feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
+        X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
+        categorical_shap_ohe = True
 
-            CVSel_algo.fit(X_train_tsf, y_train)
     else:
-        CVSel_algo.fit(X_train, y_train)
+        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+    
+    CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
 
     # Get AUC
-    if len(categorical_feature) > 0:
-        train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
-    else:
-        train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train)[:, 1])
+    train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    if len(categorical_feature) > 0:
-        shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
-    else:
-        shap_importance = get_Shap(X_train, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
 def get_Shap_R2(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
     """Get the R squared of the model and Features' Shapley Value.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
         CVSel_algo: class that include the regressor, grid search and detail of CV selection.
-        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to [].
+        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
     Returns:
         (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid R2.
 
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Estimate
     categorical_shap_ohe = False
+    X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
-        if str(CVSel_algo.estimator.__class__()).startswith("LGBM"):
-            # Categorical Preprocessing with LGBM - Label-Encoder
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OrdinalEncoder(handle_unknown="error"), categorical_feature),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train), columns=feat_names)
-
-            CVSel_algo.fit(X_train_tsf, y_train, categorical_feature=categorical_feature)
-        # Categorical Preprocessing without LGBM - Hot-One-Encoder
-        else:
-            cats_feat = categorical_feature.copy()
-            X_train_tsf = X_train.copy()
-            for col in cats_feat:
-                if X_train_tsf[col].nunique() > dim_cat_threshold:
-                    values_cat = list(
-                        X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                    )[:dim_cat_threshold]
-                    for val in values_cat:
-                        X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
-                    X_train_tsf = X_train_tsf.drop(columns=col)
-                    cats_feat.remove(col)
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train_tsf)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
-            categorical_shap_ohe = True
+        # Categorical Preprocessing Hot-One-Encoder
+        cats_feat = categorical_feature.copy()
+        for col in cats_feat:
+            if X_train_tsf[col].nunique() > dim_cat_threshold:
+                values_cat = list(
+                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
+                )[:dim_cat_threshold]
+                for val in values_cat:
+                    X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
+                X_train_tsf = X_train_tsf.drop(columns=col)
+                cats_feat.remove(col)
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
+            ],
+            remainder="passthrough",
+        )
+        preprocessor.fit(X_train_tsf)
+        feat_names = preprocessor.get_feature_names_out()
+        feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
+        X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
+        categorical_shap_ohe = True
 
-            CVSel_algo.fit(X_train_tsf, y_train)
     else:
-        CVSel_algo.fit(X_train, y_train)
+        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+
+    CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
+
     # Get R2
-    if len(categorical_feature) > 0:
-        train_model_score = r2_score(y_train, CVSel_algo.predict(X_train_tsf))
-    else:
-        train_model_score = r2_score(y_train, CVSel_algo.predict(X_train))
+    train_model_score = r2_score(y_train, CVSel_algo.predict(X_train_tsf))
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    if len(categorical_feature) > 0:
-        shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
-    else:
-        shap_importance = get_Shap(X_train, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
 def get_Shap_BalAcc(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
     """Get the Balanced Accuracy of the model and Features' Shapley Value.
 
@@ -563,71 +493,51 @@
 
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Estimate
     categorical_shap_ohe = False
+    X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
-        if str(CVSel_algo.estimator.__class__()).startswith("LGBM"):
-            # Categorical Preprocessing with LGBM - Label-Encoder
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OrdinalEncoder(handle_unknown="error"), categorical_feature),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train), columns=feat_names)
-
-            CVSel_algo.fit(X_train_tsf, y_train, categorical_feature=categorical_feature)
-        # Categorical Preprocessing without LGBM - Hot-One-Encoder
-        else:
-            cats_feat = categorical_feature.copy()
-            X_train_tsf = X_train.copy()
-            for col in cats_feat:
-                if X_train_tsf[col].nunique() > dim_cat_threshold:
-                    values_cat = list(
-                        X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                    )[:dim_cat_threshold]
-                    for val in values_cat:
-                        X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
-                    X_train_tsf = X_train_tsf.drop(columns=col)
-                    cats_feat.remove(col)
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
-                ],
-                remainder="passthrough",
-            )
-            preprocessor.fit(X_train_tsf)
-            feat_names = preprocessor.get_feature_names_out()
-            feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
-            X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
-            categorical_shap_ohe = True
+        # Categorical Preprocessing Hot-One-Encoder
+        cats_feat = categorical_feature.copy()
+        for col in cats_feat:
+            if X_train_tsf[col].nunique() > dim_cat_threshold:
+                values_cat = list(
+                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
+                )[:dim_cat_threshold]
+                for val in values_cat:
+                    X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
+                X_train_tsf = X_train_tsf.drop(columns=col)
+                cats_feat.remove(col)
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
+            ],
+            remainder="passthrough",
+        )
+        preprocessor.fit(X_train_tsf)
+        feat_names = preprocessor.get_feature_names_out()
+        feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
+        X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
+        categorical_shap_ohe = True
 
-            CVSel_algo.fit(X_train_tsf, y_train)
     else:
-        CVSel_algo.fit(X_train, y_train)
+        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+
+        CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
     # Get Balanced Accuracy
-    if len(categorical_feature) > 0:
-        train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
-    else:
-        train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train))
+    train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    if len(categorical_feature) > 0:
-        shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
-    else:
-        shap_importance = get_Shap(X_train, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
 def get_new_X(X_train, shap_importance, step_size=0.1, min_n_feat_step=5, final_n_feature=1):
     """Determines the reduced DataFrame excluding the shap-useless features.
```

### Comparing `cefeste-1.0.3/src/cefeste/selection/__init__.py` & `cefeste-1.1.0/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/selection/explanatory.py` & `cefeste-1.1.0/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/selection/multivariate.py` & `cefeste-1.1.0/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/selection/univariate.py` & `cefeste-1.1.0/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/transform/__init__.py` & `cefeste-1.1.0/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.0.3/src/cefeste/utils.py` & `cefeste-1.1.0/src/cefeste/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Returns:
         list: the list of numerical feature names
     """
     if feature_filter is None:
         feature_filter = []
 
-    return [var for var in df.columns if (df[var].dtype != "O") and (var not in feature_filter)]
+    return [var for var in df.columns if (df[var].dtype != "O" and df[var].dtype != "category") and (var not in feature_filter)]
 
 
 def get_categorical_features(df, feature_filter=None):
     """It gets a list of categorical features' names from a DataFrame excluding unwanted features' names.
 
     Args:
 
@@ -31,15 +31,15 @@
 
     Returns:
         list: the list of categorical feature names
     """
     if feature_filter is None:
         feature_filter = []
 
-    categorical_feat = [var for var in df.columns if df[var].dtype == "O" and var not in feature_filter]
+    categorical_feat = [var for var in df.columns if (df[var].dtype == "O" or df[var].dtype == "category") and var not in feature_filter]
 
     return categorical_feat
 
 
 def remove_features(df, features_to_remove):
     """Remove a list of features from the dataframe.
```

### Comparing `cefeste-1.0.3/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.0/src/cefeste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.0.3
+Version: 1.1.0
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.0.3/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.0/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

