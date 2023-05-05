# Comparing `tmp/statinf-1.2.4.tar.gz` & `tmp/statinf-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.4.tar", last modified: Tue May  2 11:44:34 2023, max compression
+gzip compressed data, was "statinf-1.2.5.tar", last modified: Fri May  5 14:18:57 2023, max compression
```

## Comparing `statinf-1.2.4.tar` & `statinf-1.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.114357 statinf-1.2.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.4/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-02 11:44:34.114357 statinf-1.2.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.4/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-02 11:44:34.114357 statinf-1.2.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.4/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-05-02 11:44:33.000000 statinf-1.2.4/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.071023 statinf-1.2.4/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-05-02 11:44:33.000000 statinf-1.2.4/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.4/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.4/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.4/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    20390 2023-05-02 09:53:55.000000 statinf-1.2.4/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.4/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.4/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.092690 statinf-1.2.4/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.4/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.4/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.4/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.4/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.4/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.4/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.4/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.092690 statinf-1.2.4/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.4/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.4/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.103523 statinf-1.2.4/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.4/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.4/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.4/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.114357 statinf-1.2.4/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.4/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.4/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.4/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.4/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.4/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.5/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-05 14:18:57.601566 statinf-1.2.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.5/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-05 14:18:57.601566 statinf-1.2.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.5/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-05-05 14:18:57.000000 statinf-1.2.5/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.5/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.5/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.5/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    25196 2023-05-05 14:18:00.000000 statinf-1.2.5/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.5/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.5/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.5/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.5/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.5/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.5/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.5/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.5/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.5/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.5/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.5/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.5/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.5/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.5/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2023-05-05 13:38:11.000000 statinf-1.2.5/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.5/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.5/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.5/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.5/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.4/LICENSE` & `statinf-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/PKG-INFO` & `statinf-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.4
+Version: 1.2.5
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.4/README.md` & `statinf-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/setup.py` & `statinf-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/setup_new.py` & `statinf-1.2.5/setup_new.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statinf",
-    version="1.2.4",
+    version="1.2.5",
     author="Florian Felice",
     author_email="florian.felice@outlook.com",
     description="A library for statistics and causal inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/statinf",
     packages=setuptools.find_packages(),
```

### Comparing `statinf-1.2.4/statinf/data/GenerateData.py` & `statinf-1.2.5/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/data/ProcessData.py` & `statinf-1.2.5/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/distributions/discrete.py` & `statinf-1.2.5/statinf/distributions/discrete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import math
 from decimal import Decimal
 
 import datetime
 
 import scipy
+from scipy.special import factorial, gamma, gammaln
 from scipy import optimize
 import warnings
 
 
 scipy_methods = ['BFGS', 'L-BFGS-B', 'Newton-CG', 'CG', 'Powell', 'Nelder-Mead']
 
 # Empty object with future attributes
@@ -85,22 +86,24 @@
                 fun=self.nll_fun,
                 x0=init_params,
                 args=nll_args,
                 method=method,
                 bounds=bounds
             )
             self.nll = res.fun
+            self.ll = -self.nll
 
             if verbose:
                 print(res)
         else:
             raise ValueError(f"The selected method is not valid, should be on of {', '.join(scipy_methods)}")
 
         return res
 
+
 class Poisson(Discrete):
     def __init__(self, lambda_=None, *args, **kwargs) -> None:
         """Poisson distribution.
 
         The Poisson distribution is the most common probability distribution for count data.
 
         :formula: The probability mass function is defined by
@@ -237,15 +240,15 @@
 
         res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, **kwargs)
         self.lambda_ = res.x[0]
 
         out = {'lambda_': self.lambda_}
 
         if method in scipy_methods:
-            out.update({'nll': self.nll})
+            out.update({'loglikelihood': self.ll})
 
         return out
 
 
 class CMPoisson(Discrete):
     def __init__(self, lambda_=None, nu_=None, j=500, *args, **kwargs) -> None:
         """Conway-Maxwell Poisson distribution.
@@ -437,34 +440,149 @@
             There is no close form to estimate the parameters nor a direct relation between the empirical moments (:math:`\\bar{X}`) and the theoretical ones.
             Therefore, only MLE is available (no fast method).
 
         :param data: Data to fit and estimate parameters from.
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param method: Optimization method to estimate the parameters, defaults to 'L-BFGS-B'
         :type method: :obj:`str`, optional
-        :param init_params: Initial parameters for the optimization method, defaults to obj:`np.array([1., 1.])`
+        :param init_params: Initial parameters for the optimization method, defaults to :obj:`np.array([1., 0.5])`
         :type init_params: :obj:`numpy.array`, optional
 
         :return: Estimated parameters
         :rtype: :obj:`dict`
         """
         # We transform warnings as error (for overflow) to handle in try / except: https://stackoverflow.com/questions/5644836/
         j = j if j else self.j
+        data = np.asarray(data)
         if bounds is None:
             bounds = [(self.eps, None), (self.eps, None)]
         if init_params == 'auto':
-            _disp = data.var() / data.mean()
+            _disp = data.mean() / data.var()
             init_params = np.array([data.mean(), _disp])
 
         res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
         warnings.filterwarnings("error")
         self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j)
         warnings.resetwarnings()
 
         out = {'lambda_': self.lambda_, 'nu_': self.nu_, 'convergence': res.success}
 
         if method in scipy_methods:
-            out.update({'loglikelihood': -self.nll})
+            out.update({'loglikelihood': self.ll})
+
+        return out
+
+
+class NegativeBinomial(Discrete):
+    def __init__(self, r_=None, p_=None, *args, **kwargs) -> None:
+        """Negative Binomial distribution.
+
+        :formulae: The probability mass function (pmf) is defined by
+
+            .. math:: \\mathbb{P}(X = x | r, p) = \\dfrac{(x + r - 1)!}{(r - 1)! x!} (1 - p)^{k} p^{r}
+
+        :example:
+
+        >>> from statinf.distributions import NegativeBinomial
+        >>> # Let us generate a random sample of size 1000
+        >>> x = NegativeBinomial(n_=5, p_=0.15).sample(size=1000)
+        >>> # We can also estimate the parameters from the generated sample
+        >>> # We just need to initialize the class...
+        >>> nb = NegativeBinomial()
+        >>> # ... and we can fit from the generated sample. The function returns a dictionary
+        >>> nb.fit(x)
+        ... {'r_': 5, 'p_': 0.15069905301345346, 'convergence': True, 'loglikelihood': -3972.2726626530775}
+        >>> # The class stores the value of the estimated parameters
+        >>> print(nb.p_)
+        ... 0.15069905301345346
+        >>> # So we can generate more samples using the fitted parameters
+        >>> y = nb.sample(200)
+
+
+        :reference: * DeGroot, M. H., & Schervish, M. J. (2012). Probability and statistics. Pearson Education.
+        """
+        super(NegativeBinomial, self).__init__(*args, **kwargs)
+        self.r_ = r_
+        self.p_ = p_
+
+    def pmf(self, x) -> float:
+        """Computes the probability mass function for selected value :obj:`x`.
+
+        :formula: The probability mass function (pmf) is computed by
+
+            .. math:: \\mathbb{P}(X = x | r, p) = \\dfrac{(x + r - 1)!}{(r - 1)! x!} (1 - p)^{k} p^{r}
+
+        :param x: Value to be evaluated
+        :type x: :obj:`int`
+
+        :return: Probability :math:`\\mathbb{P}(X = x | r, p)`
+        :rtype: :obj:`float`
+        """
+        x = [x] if type(x) in [float, int] else x
+
+        _comb = np.array([scipy.special.comb(_x + self.r_ - 1, _x, exact=True) for _x in x])
+
+        # _comb = np.array([_a / _b for _a, _b in zip(_num, _denom)])
+        _m1 = np.array([pow(1 - self.p_, _x) for _x in x])
+        _m2 = pow(self.p_, self.r_)
+        return _comb * _m1 * _m2
+
+    @staticmethod
+    def nloglike(params, data, eps=10e-4) -> float:
+        """Static method to estumate the negative likelihood (used in :meth:`statinf.distributions.discrete.NegativeBinomial.fit` method).
+
+        :formula: The log-likelihood function :math:`l` is defined by
+
+            .. math:: \\mathcal{l}(x_1, ..., x_n | r, p) &= \\sum_{i=1}^{n} {\\log(\\Gamma(x_i + r))} \\sum_{i=1}^{n} {\\log(x_i!)} - N \\log(\\Gamma(r)) \\\\ &+ \\sum_{i=1}^{n} {x_i \\log(1-p)} + N r \\log(p)
+
+        :param params: List of parameters :math:`r` and :math:`p`
+        :type params: :obj:`list`
+        :param data: Data to evaluate the netative log-likelihood on
+        :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
+
+        :return: Negative log-likelihood
+        :rtype: :obj:`float`
+        """
+        r_ = params[0]
+        p_ = params[1]
+        X = np.asarray(data)
+        n = len(X)
+
+        ll = np.sum(gammaln(X + r_))
+        ll += - np.sum(np.log(factorial(X)))
+        ll += - n * (gammaln(r_))
+        ll += n * r_ * np.log(p_)
+        ll += np.sum(X * np.log(1 - (p_ if p_ < 1 else 1 - eps)))
+        return -ll
+
+    def fit(self, data, method='L-BFGS-B', init_params=[1, 0.5], bounds=None, **kwargs) -> dict:
+        """Estimates the parameters :math:`\\lambda` and :math:`\\nu` of the distribution from empirical data based on Maximum Likelihood Estimation.
+
+        .. note::
+
+            There is no close form to estimate the parameters. Therefore, only MLE is available (no fast method).
+
+        :param data: Data to fit and estimate parameters from.
+        :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
+        :param method: Optimization method to estimate the parameters, defaults to 'L-BFGS-B'
+        :type method: :obj:`str`, optional
+        :param init_params: Initial parameters for the optimization method, defaults to :obj:`np.array([1., 1.])`
+        :type init_params: :obj:`numpy.array`, optional
+
+        :return: Estimated parameters
+        :rtype: :obj:`dict`
+        """
+        if bounds is None:
+            bounds = [(self.eps, None), (self.eps, 1)]
+
+        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, **kwargs)
+        self.r_ = int(round(res.x[0], 0))
+        self.p_ = res.x[1]
+
+        out = {'r_': self.r_, 'p_': self.p_, 'convergence': res.success}
+
+        if method in scipy_methods:
+            out.update({'loglikelihood': self.ll})
 
         return out
```

### Comparing `statinf-1.2.4/statinf/misc.py` & `statinf-1.2.5/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/activations.py` & `statinf-1.2.5/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/initializations.py` & `statinf-1.2.5/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/losses.py` & `statinf-1.2.5/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/neuralnetwork.py` & `statinf-1.2.5/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/optimizers.py` & `statinf-1.2.5/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/ml/performance.py` & `statinf-1.2.5/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/nonparametrics/kernels.py` & `statinf-1.2.5/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/regressions/LinearModels.py` & `statinf-1.2.5/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/regressions/glm.py` & `statinf-1.2.5/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/regressions/glm_test.py` & `statinf-1.2.5/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/stats/bayesian.py` & `statinf-1.2.5/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/stats/descriptive.py` & `statinf-1.2.5/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/stats/tests.py` & `statinf-1.2.5/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/stats/timeseries.py` & `statinf-1.2.5/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf/stats/unsupervised.py` & `statinf-1.2.5/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.4/statinf.egg-info/PKG-INFO` & `statinf-1.2.5/statinf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.4
+Version: 1.2.5
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.4/statinf.egg-info/SOURCES.txt` & `statinf-1.2.5/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

