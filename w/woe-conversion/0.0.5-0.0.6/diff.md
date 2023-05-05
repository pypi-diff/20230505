# Comparing `tmp/woe_conversion-0.0.5.tar.gz` & `tmp/woe_conversion-0.0.6.tar.gz`

## Comparing `woe_conversion-0.0.5.tar` & `woe_conversion-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/README.md~
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/pyproject.toml~
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/src/woe_conversion/__init__.py
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/src/woe_conversion/woe.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/LICENSE~
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/README.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 woe_conversion-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/README.md~
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/pyproject.toml~
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/src/woe_conversion/__init__.py
+-rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/src/woe_conversion/woe.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/src/woe_conversion/woe.py~
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/LICENSE~
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 woe_conversion-0.0.6/PKG-INFO
```

### Comparing `woe_conversion-0.0.5/pyproject.toml~` & `woe_conversion-0.0.6/pyproject.toml~`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","pandas","numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "woe_conversion"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Bertrand Brelier", email="bertrand.brelier@gmail.com" },
 ]
 description = "woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `woe_conversion-0.0.5/src/woe_conversion/woe.py` & `woe_conversion-0.0.6/src/woe_conversion/woe.py~`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.5/LICENSE` & `woe_conversion-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.5/README.md` & `woe_conversion-0.0.6/README.md~`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.5/pyproject.toml` & `woe_conversion-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","pandas","numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "woe_conversion"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Bertrand Brelier", email="bertrand.brelier@gmail.com" },
 ]
 description = "woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `woe_conversion-0.0.5/PKG-INFO` & `woe_conversion-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woe_conversion
-Version: 0.0.5
+Version: 0.0.6
 Summary: woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects.
 Project-URL: Homepage, https://github.com/BertrandBrelier/woe
 Project-URL: Bug Tracker, https://github.com/BertrandBrelier/woe
 Author-email: Bertrand Brelier <bertrand.brelier@gmail.com>
 License-File: LICENSE
 License-File: LICENSE~
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,18 @@
 ## usage
 ```
 from woe_conversion.woe import *
 
 # create an instance of the WoeConversion class
 woemodel = WoeConversion(binarytarget='survived', features=['categorical_variable_1','categorical_variable_2','continuous_variable_3'])
 
-# fit the model using training data
+# fit the model using training data (train is a pandas dataframe)
 woemodel.fit(train)
 
-# transform the training and test data using the fitted model
+# transform the training and test data using the fitted model (train and test are pandas dataframes)
 transformedtrain = woemodel.transform(train)
 transformedtest = woemodel.transform(test)
 ```
 
 In the above code, WoeConversion is the class that is used to perform the conversion of variables to weight of evidence. The binarytarget parameter is the name of the binary target column in your dataset, and features is a list of the columns that you want to convert to weight of evidence.
 
 Once the model has been created, it is fit to the training data using the fit method. This method calculates the weight of evidence for each category in the specified columns, and stores the results in the model object.
```

