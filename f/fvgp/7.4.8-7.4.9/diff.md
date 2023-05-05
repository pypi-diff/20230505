# Comparing `tmp/fvgp-7.4.8.tar.gz` & `tmp/fvgp-7.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvgp-7.4.8.tar", last modified: Thu Mar 23 17:10:22 2023, max compression
+gzip compressed data, was "fvgp-7.4.9.tar", last modified: Fri May  5 00:39:11 2023, max compression
```

## Comparing `fvgp-7.4.8.tar` & `fvgp-7.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.023283 fvgp-7.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-23 17:10:07.000000 fvgp-7.4.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-23 17:10:07.000000 fvgp-7.4.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 17:10:07.000000 fvgp-7.4.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-23 17:10:07.000000 fvgp-7.4.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-23 17:10:07.000000 fvgp-7.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-23 17:10:07.000000 fvgp-7.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-23 17:10:22.023283 fvgp-7.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-23 17:10:07.000000 fvgp-7.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.019283 fvgp-7.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-23 17:10:07.000000 fvgp-7.4.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-23 17:10:07.000000 fvgp-7.4.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.019283 fvgp-7.4.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.019283 fvgp-7.4.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)  2681688 2023-03-23 17:10:07.000000 fvgp-7.4.8/docs/source/_static/landing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2481 2023-03-23 17:10:07.000000 fvgp-7.4.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.023283 fvgp-7.4.8/fvgp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-23 17:10:22.023283 fvgp-7.4.8/fvgp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6647 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/advanced_kernels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11191 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/fvgp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78972 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/gp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27129 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/gp2Scale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4740 2023-03-23 17:10:07.000000 fvgp-7.4.8/fvgp/sparse_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.023283 fvgp-7.4.8/fvgp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-23 17:10:21.000000 fvgp-7.4.8/fvgp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-23 17:10:22.023283 fvgp-7.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-03-23 17:10:07.000000 fvgp-7.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:10:22.023283 fvgp-7.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-23 17:10:07.000000 fvgp-7.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-23 17:10:07.000000 fvgp-7.4.8/tests/latest_hps.npy
--rwxr-xr-x   0 runner    (1001) docker     (123)    10856 2023-03-23 17:10:07.000000 fvgp-7.4.8/tests/test_fvgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-03-23 17:10:07.000000 fvgp-7.4.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.675719 fvgp-7.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 00:38:57.000000 fvgp-7.4.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 00:38:57.000000 fvgp-7.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 00:38:57.000000 fvgp-7.4.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 00:38:57.000000 fvgp-7.4.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 00:38:57.000000 fvgp-7.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 00:38:57.000000 fvgp-7.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-05 00:39:11.675719 fvgp-7.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 00:38:57.000000 fvgp-7.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.667719 fvgp-7.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 00:38:57.000000 fvgp-7.4.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 00:38:57.000000 fvgp-7.4.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.667719 fvgp-7.4.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.667719 fvgp-7.4.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)  2681688 2023-05-05 00:38:57.000000 fvgp-7.4.9/docs/source/_static/landing.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2481 2023-05-05 00:38:57.000000 fvgp-7.4.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.675719 fvgp-7.4.9/fvgp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 00:39:11.675719 fvgp-7.4.9/fvgp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6647 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/advanced_kernels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11191 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/fvgp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78972 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/gp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42804 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/gp2Scale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4902 2023-05-05 00:38:57.000000 fvgp-7.4.9/fvgp/sparse_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.671719 fvgp-7.4.9/fvgp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 00:39:11.000000 fvgp-7.4.9/fvgp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 00:39:11.675719 fvgp-7.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-05-05 00:38:57.000000 fvgp-7.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:39:11.675719 fvgp-7.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 00:38:57.000000 fvgp-7.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 00:38:57.000000 fvgp-7.4.9/tests/latest_hps.npy
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10856 2023-05-05 00:38:57.000000 fvgp-7.4.9/tests/test_fvgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-05 00:38:57.000000 fvgp-7.4.9/versioneer.py
```

### Comparing `fvgp-7.4.8/CONTRIBUTING.rst` & `fvgp-7.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/COPYING` & `fvgp-7.4.9/COPYING`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/LICENSE` & `fvgp-7.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/PKG-INFO` & `fvgp-7.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvgp
-Version: 7.4.8
+Version: 7.4.9
 Summary: Python package for highly flexible function-valued Gaussian processes (fvGP)
 Home-page: https://github.com/MarcusMichaelNoack/fvgp
 Author: Marcus Michael Noack
 Author-email: MarcusNoack@lbl.gov
 License: GNU General Public License v3
 Keywords: fvgp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fvgp-7.4.8/README.md` & `fvgp-7.4.9/README.md`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/docs/Makefile` & `fvgp-7.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/docs/make.bat` & `fvgp-7.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/docs/source/_static/landing.png` & `fvgp-7.4.9/docs/source/_static/landing.png`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/docs/source/conf.py` & `fvgp-7.4.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/fvgp/advanced_kernels.py` & `fvgp-7.4.9/fvgp/advanced_kernels.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/fvgp/fvgp.py` & `fvgp-7.4.9/fvgp/fvgp.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/fvgp/gp.py` & `fvgp-7.4.9/fvgp/gp.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/fvgp/gp2Scale.py` & `fvgp-7.4.9/fvgp/gp2Scale.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import gc
 from scipy.sparse.linalg import splu
 from scipy.sparse.linalg import spilu
 from .mcmc import mcmc
 import torch
 from dask.distributed import Variable
 from .sparse_matrix import gp2ScaleSparseMatrix
-#from .sparse_matrix import UpdateSM
 import gc
 
 
 def sparse_stat_kernel(x1,x2, hps):
     d = 0
     for i in range(len(x1[0])): d += abs(np.subtract.outer(x1[:,i],x2[:,i]))**2
     d = np.sqrt(d)
@@ -58,25 +57,25 @@
     This class allows the user to scale GPs up to millions of datapoints. There is full high-performance-computing
     support through DASK.
     
     Parameters
     ----------
     input_space_dim : int
         Dimensionality of the input space.
-    points : np.ndarray
+    x_data : np.ndarray
         The point positions. Shape (V x D), where D is the `input_space_dim`.
-    values : np.ndarray
+    y_data : np.ndarray
         The values of the data points. Shape (V,output_number).
     init_hyperparameters : np.ndarray
         Vector of hyperparameters used by the GP initially. The class provides methods to train hyperparameters.
     batch_size : int
         The covariance is divided into batches of the defined size for distributed computing.
     variances : np.ndarray, optional
-        An numpy array defining the uncertainties in the data `values`. Shape (V x 1) or (V). Note: if no
-        variances are provided they will be set to `abs(np.mean(values) / 100.0`.
+        An numpy array defining the uncertainties in the data `y_data`. Shape (V x 1) or (V). Note: if no
+        variances are provided they will be set to `abs(np.mean(y_data) / 100.0`.
     limit_workers : int, optional
         If given as integer only the workers up to the limit will be used.
     LUtimeout : int, optional (future release)
         Controls the timeout for the LU decomposition.
     gp_kernel_function : Callable, optional
         A function that calculates the covariance between datapoints. It accepts as input x1 (a V x D array of positions),
         x2 (a U x D array of positions), hyperparameters (a 1-D array of length D+1 for the default kernel), and a
@@ -96,38 +95,38 @@
         These optional arguments will be available as attribute in kernel and mean function definitions.
 
     """
 
     def __init__(
         self,
         input_space_dim,
-        points,
-        values,
+        x_data,
+        y_data,
         init_hyperparameters,
         batch_size,
         variances = None,
         limit_workers = None,
         LUtimeout = 100,
         gp_kernel_function = sparse_stat_kernel,
         gp_mean_function = None,
         covariance_dask_client = None,
         info = False,
         ):
         """
         The constructor for the gp class.
         type help(GP) for more information about attributes, methods and their parameters
         """
-        if input_space_dim != len(points[0]):
+        if input_space_dim != len(x_data[0]):
             raise ValueError("input space dimensions are not in agreement with the point positions given")
-        if np.ndim(values) == 2: values = values[:,0]
+        if np.ndim(y_data) == 2: y_data = y_data[:,0]
 
         self.input_dim = input_space_dim
-        self.x_data = points
+        self.x_data = x_data
         self.point_number = len(self.x_data)
-        self.y_data = values
+        self.y_data = y_data
         self.batch_size = batch_size
         self.num_batches = self.point_number // self.batch_size
         self.limit_workers = limit_workers
         self.info = info
         self.LUtimeout = LUtimeout
         ##########################################
         #######prepare variances##################
@@ -206,17 +205,17 @@
         cov_y = self._compute_covariance_value_product(
                 self.hyperparameters,
                 self.y_data,
                 self.variances,
                 self.prior_mean_vec,client)
         self.covariance_value_prod = cov_y
 
-    def _compute_covariance_value_product(self, hyperparameters,values, variances, mean, client):
+    def _compute_covariance_value_product(self, hyperparameters,y_data, variances, mean, client):
         self.compute_covariance(self.x_data,self.x_data,hyperparameters, variances,client)
-        y = values - mean
+        y = y_data - mean
         #try: success = self.SparsePriorCovariance.compute_LU().result(timeout=self.LUtimeout)
         #except: print("LU failed")
         x = self.SparsePriorCovariance.solve(y).result()
         return x
 
     def total_number_of_batches(self):
         Db = float(self.num_batches)
@@ -339,23 +338,17 @@
     ##################################################################################
     ##################################################################################
     ##################################################################################
     ##################################################################################
     def train(self,
         hyperparameter_bounds,
         init_hyperparameters = None,
-        method = "global",
-        optimization_dict = None,
-        pop_size = 20,
-        tolerance = 0.0001,
         max_iter = 120,
-        local_optimizer = "L-BFGS-B",
-        global_optimizer = "genetic",
-        deflation_radius = None,
-        dask_client = None):
+        dask_client = None
+        ):
         """
         This function finds the maximum of the log_likelihood and therefore trains the fvGP (synchronously).
         This can be done on a remote cluster/computer by specifying the method to be be 'hgdl' and 
         providing a dask client
 
         inputs:
             hyperparameter_bounds (2d numpy array)
@@ -380,41 +373,30 @@
         print("fvGP training started with ",len(self.x_data)," data points")
         ######################
         #####TRAINING#########
         ######################
         self.hyperparameters = self.optimize_log_likelihood(
             init_hyperparameters,
             np.array(hyperparameter_bounds),
-            method,
-            optimization_dict,
             max_iter,
-            pop_size,
-            tolerance,
-            local_optimizer,
-            global_optimizer,
-            deflation_radius,
-            dask_client
             )
         print("computing the prior")
         self.compute_prior_fvGP_pdf(self.covariance_dask_client)
         np.save("latest_hps", self.hyperparameters)
         ######################
         ######################
         ######################
 
 
 
-    def optimize_log_likelihood(self,starting_hps,
-        hp_bounds,method,optimization_dict,max_iter,
-        pop_size,tolerance,
-        local_optimizer,
-        global_optimizer,
-        deflation_radius,
-        constraints = None,
-        dask_client = None):
+    def optimize_log_likelihood(self,
+        starting_hps,
+        hp_bounds,
+        max_iter,
+        ):
 
         #start_log_likelihood = self.log_likelihood(starting_hps, recompute_xK = False)
         print("MCMC started in fvGP")
         print('bounds are',hp_bounds)
         res = mcmc(self.log_likelihood,hp_bounds,max_iter = max_iter, x0 = starting_hps)
         hyperparameters = np.array(res["x"])
         self.mcmc_info = res
@@ -533,14 +515,344 @@
                 np.fill_diagonal(S, v)
 
         return {"x": p,
                 "v(x)": v,
                 "S(x)": S}
 
 
+
+
+
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+class gpm2Scale(gp2Scale):
+    def __init__(self,input_space_dim,
+                 output_space_dim,
+                 x_data, ##data in the original input space
+                 init_hyperparameters,
+                 batch_size,
+                 variances  = None,
+                 init_y_data = None, #initial latent space positions
+                 gp_kernel_function = sparse_stat_kernel,
+                 gp_mean_function = None, covariance_dask_client = None,
+                 info = False):
+
+        if input_space_dim != len(x_data[0]): raise ValueError("input space dimensions are not in agreement with the point positions given")
+        self.input_dim = input_space_dim
+        self.output_dim = output_space_dim
+        self.x_data = x_data
+        self.point_number = len(self.x_data)
+        if init_y_data is None: init_y_data = np.random.rand(len(x_data), self.output_dim)
+        self.y_data = init_y_data
+        self.batch_size = batch_size
+        self.num_batches = self.point_number // self.batch_size
+        self.info = info
+        ##########################################
+        #######prepare variances##################
+        ##########################################
+        if variances is None:
+            self.variances = np.ones((self.x_data.shape[0])) * \
+                    abs(np.mean(self.x_data) / 100.0)
+            print("CAUTION: you have not provided data variances in fvGP,")
+            print("they will be set to 1 percent of the data values!")
+        if len(self.variances[self.variances < 0]) > 0: raise Exception("Negative measurement variances communicated to fvgp.")
+        ##########################################
+        #######define kernel and mean function####
+        ##########################################
+        if gp_kernel_function == "robust": self.kernel = sparse_stat_kernel_robust
+        elif callable(gp_kernel_function): self.kernel = gp_kernel_function
+        else: raise Exception("A kernel callable has to be provided!")
+
+        self.gp_mean_function = gp_mean_function
+        if  callable(gp_mean_function): self.mean_function = gp_mean_function
+        else: self.mean_function = self.default_mean_function
+
+        ##########################################
+        #######prepare hyper parameters###########
+        ##########################################
+        self.hyperparameters = np.array(init_hyperparameters)
+        ##########################################
+        #compute the prior########################
+        ##########################################
+        covariance_dask_client, self.compute_worker_set, self.actor_worker = self._init_dask_client(covariance_dask_client)
+        ###initiate actor that is a future contain the covariance and methods
+        self.SparsePriorCovariance = covariance_dask_client.submit(gp2ScaleSparseMatrix,self.point_number, actor=True, workers=self.actor_worker).result()# Create Actor
+
+        self.covariance_dask_client = covariance_dask_client
+        scatter_data = {"x1_data":self.x_data, "x2_data":self.x_data} ##data that can be scattered
+        self.scatter_future = covariance_dask_client.scatter(scatter_data,workers = self.compute_worker_set)               ##scatter the data
+
+        self.st = time.time()
+        self.compute_covariance(self.y_data,self.y_data,self.hyperparameters,variances,covariance_dask_client)
+        if self.info:
+            sp = self.SparsePriorCovariance.get_result().result()
+            print("gp2Scale successfully initiated, here is some info about the prior covariance matrix:")
+            print("non zero elements: ", sp.count_nonzero())
+            print("Size in GBits:     ", sp.data.nbytes/1e9)
+            print("Sparsity: ",sp.count_nonzero()/float(self.point_number)**2)
+            if self.point_number <= 5000:
+                print("Here is an image:")
+                plt.imshow(sp.toarray())
+                plt.show()
+
+
+
+    def total_number_of_batches(self):
+        Db = float(self.num_batches)
+        return 0.5 * Db * (Db + 1.)
+
+    def compute_covariance(self, x1,x2,hyperparameters, variances,client):
+        """computes the covariance matrix from the kernel on HPC in sparse format"""
+        ###initialize futures
+        futures = []           ### a list of futures
+        actor_futures = []
+        finished_futures = set()
+        ###get workers
+        compute_workers = set(self.compute_worker_set)
+        idle_workers = set(compute_workers)
+        ###future_worker_assignments
+        self.future_worker_assignments = {}
+        ###scatter data
+        start_time = time.time()
+        count = 0
+        num_batches_i = len(x1) // self.batch_size
+        num_batches_j = len(x2) // self.batch_size
+        last_batch_size_i = len(x1) % self.batch_size
+        last_batch_size_j = len(x2) % self.batch_size
+        if last_batch_size_i != 0: num_batches_i += 1
+        if last_batch_size_j != 0: num_batches_j += 1
+
+        for i in range(num_batches_i):
+            beg_i = i * self.batch_size
+            end_i = min((i+1) * self.batch_size, self.point_number)
+            batch1 = self.x_data[beg_i: end_i]
+            for j in range(i,num_batches_j):
+                beg_j = j * self.batch_size
+                end_j = min((j+1) * self.batch_size, self.point_number)
+                batch2 = self.x_data[beg_j : end_j]
+                ##make workers available that are not actively computing
+                while not idle_workers:
+                    idle_workers, futures, finished_futures = self.free_workers(futures, finished_futures)
+                    time.sleep(0.1)
+
+                ####collect finished workers but only if actor is not busy, otherwise do it later
+                if len(finished_futures) >= 1000:
+                    actor_futures.append(self.SparsePriorCovariance.get_future_results(set(finished_futures)))
+                    finished_futures = set()
+
+                #get idle worker and submit work
+                current_worker = self.get_idle_worker(idle_workers)
+                data = {"scattered_data": self.scatter_future,"hps": hyperparameters, "kernel" :self.kernel,  "range_i": (beg_i,end_i), "range_j": (beg_j,end_j), "mode": "prior","gpu": 0}
+                futures.append(client.submit(kernel_function, data, workers = current_worker))
+                self.assign_future_2_worker(futures[-1].key,current_worker)
+                if self.info:
+                    print("    submitted batch. i:", beg_i,end_i,"   j:",beg_j,end_j, "to worker ",current_worker, " Future: ", futures[-1].key)
+                    print("    current time stamp: ", time.time() - start_time," percent finished: ",float(count)/self.total_number_of_batches())
+                    print("")
+                count += 1
+
+        if self.info:
+            print("All tasks submitted after ",time.time() - start_time,flush = True)
+            print("number of computed batches: ", count)
+
+        actor_futures.append(self.SparsePriorCovariance.get_future_results(finished_futures.union(futures)))
+        #actor_futures[-1].result()
+        client.gather(actor_futures)
+        actor_futures.append(self.SparsePriorCovariance.add_to_diag(variances)) ##add to diag on actor
+        actor_futures[-1].result()
+        #clean up
+        #del futures
+        #del actor_futures
+        #del finished_futures
+        #del scatter_future
+
+        #########
+        if self.info: 
+            print("total prior covariance compute time: ", time.time() - start_time, "Non-zero count: ", self.SparsePriorCovariance.get_result().result().count_nonzero())
+            print("Sparsity: ",self.SparsePriorCovariance.get_result().result().count_nonzero()/float(self.point_number)**2)
+
+
+    def free_workers(self, futures, finished_futures):
+        free_workers = set()
+        remaining_futures = []
+        for future in futures:
+            if future.status == "cancelled": print("WARNING: cancelled futures encountered!")
+            if future.status == "finished":
+                finished_futures.add(future)
+                free_workers.add(self.future_worker_assignments[future.key])
+                del self.future_worker_assignments[future.key]
+            else: remaining_futures.append(future)
+        return free_workers, remaining_futures, finished_futures
+
+    def assign_future_2_worker(self, future_key, worker_address):
+        self.future_worker_assignments[future_key] = worker_address
+
+    def get_idle_worker(self,idle_workers):
+        return idle_workers.pop()
+    ##################################################################################
+    ##################################################################################
+    ##################################################################################
+    ##################################################################################
+    ######################DASK########################################################
+    ##################################################################################
+    ##################################################################################
+    ##################################################################################
+    ##################################################################################
+    def _init_dask_client(self,dask_client):
+        if dask_client is None: dask_client = distributed.Client()
+        worker_info = list(dask_client.scheduler_info()["workers"].keys())
+        if not worker_info: raise Exception("No workers available")
+        actor_worker = worker_info[0]
+        compute_worker_set = set(worker_info[1:])
+        print("We have ", len(compute_worker_set)," compute workers ready to go.")
+        print("Actor on", actor_worker)
+        print("Scheduler Address: ", dask_client.scheduler_info()["address"])
+        return dask_client, compute_worker_set,actor_worker
+
+ 
+    def train(self,
+        hyperparameter_bounds,
+        method = "global",
+        init_hyperparameters = None,
+        max_iter = 120,
+        ):
+        """
+        This function finds the maximum of the log_likelihood and therefore trains the fvGP (synchronously).
+        This can be done on a remote cluster/computer by specifying the method to be be 'hgdl' and 
+        providing a dask client
+
+        inputs:
+            hyperparameter_bounds (2d numpy array)
+        optional inputs:
+            init_hyperparameters (1d numpy array):  default = None (= use earlier initialization)
+            method = "global": "global"/"local"/"hgdl"/callable f(obj,optimization_dict)
+            optimization_dict = None: if optimizer is callable, the this will be passed as dict
+            pop_size = 20
+            tolerance = 0.0001
+            max_iter: default = 120
+            local_optimizer = "L-BFGS-B"  important for local and hgdl optimization
+            global_optimizer = "genetic"
+            deflation_radius = None        for hgdl
+            dask_client = None (will use local client, only for hgdl optimization)
+
+        output:
+            None, just updates the class with the new hyperparameters
+        """
+        ############################################
+        if init_hyperparameters is None:
+            init_hyperparameters = np.array(self.hyperparameters)
+        print("fvGP training started with ",len(self.x_data)," data points")
+        ######################
+        #####TRAINING#########
+        ######################
+        self.hyperparameters = self.optimize_log_likelihood(
+            init_hyperparameters,
+            np.array(hyperparameter_bounds),
+            max_iter,
+            method
+            )
+        #print("computing the prior")
+        #self.compute_prior_fvGP_pdf(self.covariance_dask_client)
+        self.y_data = self.hyperparameters[0:-2].reshape(self.point_number, self.output_dim)
+        np.save("output_points", self.y_data)
+        ######################
+        ######################
+        ######################
+
+
+
+    def optimize_log_likelihood(self,
+        starting_hps,
+        hp_bounds,
+        max_iter,
+        method
+        ):
+
+        #start_log_likelihood = self.log_likelihood(starting_hps, recompute_xK = False)
+        if method == "mcmc":
+            print("MCMC started in fvGP")
+            print('bounds are',hp_bounds)
+            res = mcmc(self.log_likelihood,hp_bounds,max_iter = max_iter, x0 = starting_hps)
+            hyperparameters = np.array(res["x"])
+            self.mcmc_info = res
+            print("MCMC has found solution: ", hyperparameters, "with log marginal_likelihood ",res["f(x)"])
+        elif method == "global":
+            res = differential_evolution(self.neg_log_likelihood, hp_bounds)
+        self.hyperparameters = hyperparameters
+        return hyperparameters
+
+    def log_likelihood(self, y):
+        """
+        computes the marginal log-likelihood
+        input:
+            hyper parameters
+        output:
+            negative marginal log-likelihood (scalar)
+        """
+        client = self.covariance_dask_client
+        dim = float(self.input_dim)
+        y1 = y2 = x[0:-2].reshape(self.point_number, self.output_dim)
+        self.SparsePriorCovariance.reset_prior().result()
+        hps = x[-2:]
+        self.compute_covariance(y1,y2,hps, self.variances,client)
+        logdet = self.SparsePriorCovariance.logdet().result()
+        n = len(y)
+        x = self.x_data
+        traceKXX = self.SparsePriorCovariance.traceKXX(x).result()
+        res = -(0.5 * traceKXX) - (dim * 0.5 * logdet) - (0.5 * dim *n * np.log(2.0*np.pi))
+        return res
+
+
+    def neg_log_likelihood(self, y):
+        """
+        computes the marginal log-likelihood
+        input:
+            hyper parameters
+        output:
+            negative marginal log-likelihood (scalar)
+        """
+        client = self.covariance_dask_client
+        dim = float(self.input_dim)
+        y1 = y2 = y[0:-2].reshape(self.point_number, self.output_dim)
+        self.SparsePriorCovariance.reset_prior().result()
+        hps = y[-2:]
+        self.compute_covariance(y1,y2,hps, self.variances,client)
+        logdet = self.SparsePriorCovariance.logdet().result()
+        n = len(y)
+        x = self.x_data
+        traceKXX = self.SparsePriorCovariance.traceKXX(x).result()
+        res = (0.5 * traceKXX) + (dim * 0.5 * logdet) + (0.5 * dim *n * np.log(2.0*np.pi))
+        print("res")
+        print("")
+        return res
+
+
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
+#########################################################################
 def kernel_function(data):
     st = time.time()
     hps= data["hps"]
     mode = data["mode"]
     kernel = data["kernel"]
     worker = distributed.get_worker()
     if mode == "prior":
@@ -553,9 +865,7 @@
         k = kernel(x1,x2,hps)
     else:
         x1 = data["x1_data"]
         x2 = data["x2_data"]
         k = kernel(x1,x2,hps)
     k_sparse = sparse.coo_matrix(k)
     return k_sparse, (data["range_i"][0],data["range_j"][0]), time.time() - st, worker.address
-
-
```

### Comparing `fvgp-7.4.8/fvgp/mcmc.py` & `fvgp-7.4.9/fvgp/mcmc.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/fvgp/sparse_matrix.py` & `fvgp-7.4.9/fvgp/sparse_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import dask.distributed as distributed
 import matplotlib.pyplot as plt
 from scipy.sparse.linalg import spsolve
 from scipy.sparse.linalg import splu
 from scipy.optimize import differential_evolution
 from scipy.sparse import coo_matrix
 import gc
-from scipy.sparse.linalg import splu
 from scipy.sparse.linalg import spilu
 from .mcmc import mcmc
 import torch
 from dask.distributed import Variable
 import math
 #from scikits import umfpack
 #from scikits.umfpack import spsolve, splu
@@ -86,20 +85,20 @@
     def solve(self,x):
         success = True
         try: r = self.LU.solve(x)
         except: success = False
         if success is False:
             try:
                 r,info = sparse.linalg.cg(self.sparse_covariance,x)
-                success = True
+                if info == 0: success = True
             except: pass
         if success is False:
             try:
                 r, info = sparse.linalg.cgs(self.sparse_covariance,x)
-                success = True
+                if info == 0: success = True
             except: pass
         if success is False:
             try:
                 r,info = sparse.linalg.minres(self.sparse_covariance,x)
                 success = True
             except: raise Exception("No solve method was successful. EXIT")
         return r
@@ -132,7 +131,12 @@
             for k in range(1,m):
                 v = C @ v
                 gamma[i,k] = g.T @ v
         s = np.sum(gamma, axis = 0) / float(p)
         s = s / np.arange(1,len(s)+1)
         return N * np.log(alpha) - np.sum(s)
 
+    def traceKXX(self,X):
+        res = np.empty(X.shape)
+        for i in range(X.shape[1]): res[:,i] = self.solve(X[:,i])
+        tr = np.sum(X * res)
+        return tr
```

### Comparing `fvgp-7.4.8/fvgp.egg-info/PKG-INFO` & `fvgp-7.4.9/fvgp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvgp
-Version: 7.4.8
+Version: 7.4.9
 Summary: Python package for highly flexible function-valued Gaussian processes (fvGP)
 Home-page: https://github.com/MarcusMichaelNoack/fvgp
 Author: Marcus Michael Noack
 Author-email: MarcusNoack@lbl.gov
 License: GNU General Public License v3
 Keywords: fvgp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fvgp-7.4.8/fvgp.egg-info/SOURCES.txt` & `fvgp-7.4.9/fvgp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/setup.py` & `fvgp-7.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/tests/test_fvgp.py` & `fvgp-7.4.9/tests/test_fvgp.py`

 * *Files identical despite different names*

### Comparing `fvgp-7.4.8/versioneer.py` & `fvgp-7.4.9/versioneer.py`

 * *Files identical despite different names*

