# Comparing `tmp/wildboottest-0.1.5.tar.gz` & `tmp/wildboottest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildboottest-0.1.5.tar", max compression
+gzip compressed data, was "wildboottest-0.1.6.tar", max compression
```

## Comparing `wildboottest-0.1.5.tar` & `wildboottest-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1093 2022-12-15 18:51:39.427307 wildboottest-0.1.5/LICENSE
--rw-r--r--   0        0        0     4045 2022-12-15 18:51:39.428116 wildboottest-0.1.5/README.md
--rw-r--r--   0        0        0     1480 2022-12-15 19:10:04.440089 wildboottest-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2022-12-15 19:10:04.441535 wildboottest-0.1.5/wildboottest/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-14 20:19:32.512004 wildboottest-0.1.5/wildboottest/weights.py
--rw-r--r--   0        0        0    19406 2022-12-15 19:08:51.312810 wildboottest-0.1.5/wildboottest/wildboottest.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 wildboottest-0.1.5/setup.py
--rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 wildboottest-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-12-15 18:51:39.427307 wildboottest-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4045 2022-12-15 18:51:39.428116 wildboottest-0.1.6/README.md
+-rw-r--r--   0        0        0     1480 2022-12-15 20:58:10.755439 wildboottest-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-12-15 20:58:10.756859 wildboottest-0.1.6/wildboottest/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-14 20:19:32.512004 wildboottest-0.1.6/wildboottest/weights.py
+-rw-r--r--   0        0        0    19776 2022-12-15 20:22:21.827447 wildboottest-0.1.6/wildboottest/wildboottest.py
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 wildboottest-0.1.6/setup.py
+-rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 wildboottest-0.1.6/PKG-INFO
```

### Comparing `wildboottest-0.1.5/LICENSE` & `wildboottest-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wildboottest-0.1.5/README.md` & `wildboottest-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wildboottest-0.1.5/pyproject.toml` & `wildboottest-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wildboottest"
-version = "0.1.5"
+version = "0.1.6"
 description = "Wild Cluster Bootstrap Inference for Linear Models in Python"
 authors = [
   "Alexander Fischer <alexander-fischer1801@t-online.de>",
   "Aleksandr Michuda <amichuda@gmail.com>"
 ]
 maintainers= [
   "Aleksandr Michuda <amichuda@gmail.com>",
```

### Comparing `wildboottest-0.1.5/wildboottest/weights.py` & `wildboottest-0.1.6/wildboottest/weights.py`

 * *Files identical despite different names*

### Comparing `wildboottest-0.1.5/wildboottest/wildboottest.py` & `wildboottest-0.1.6/wildboottest/wildboottest.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,39 +144,40 @@
     self.tXgyg_list = tXgyg_list
     self.tXX = tXX
     self.tXy = tXy
       
     self.tXXinv = np.linalg.inv(tXX)
     self.RtXXinv = np.matmul(R, self.tXXinv)
       
-  def get_weights(self, weights_type: Union[str, Callable]) -> Tuple[np.ndarray, int]:
+  def get_weights(self, weights_type: Union[str, Callable]) -> Tuple[np.ndarray, int, bool]:
     """Function for getting weights for bootstrapping.
 
     Args:
         weights_type (Tuple[str, Callable]): The distribution to be used. Accepts Either 'rademacher', 'mammen', 'norm' or 'webb'. Optionally accepts a callable of one argument, `n`, the number of bootstraps iterations.
 
     Returns:
         Tuple[np.ndarray, int]: Returns the arrays of weights and the number of bootstrap iterations
     """    
     self.weights_type = weights_type 
     
     if 2**self.N_G_bootcluster < self.B and weights_type=='rademacher':
       self.full_enumeration = True
-      warnings.warn("2^G < the number of boot iterations, setting full_enumeration to True.")
+      full_enumeration_warn=True
     else: 
       self.full_enumeration = False
+      full_enumeration_warn=False
       
     self.v, self.B = draw_weights(
       t = self.weights_type, 
       full_enumeration = self.full_enumeration, 
       N_G_bootcluster = self.N_G_bootcluster,
       boot_iter = self.B
     )  
     
-    return self.v, self.B
+    return self.v, self.B, full_enumeration_warn
     
   def get_scores(self, bootstrap_type : str, 
                  impose_null : bool, adj: bool = True, 
                  cluster_adj: bool = True) -> np.ndarray:
     """Run bootstrap and get scores for each variable
 
     Args:
@@ -188,17 +189,17 @@
     Returns:
         np.ndarray: The output array of scores of shape kxG
     """    
     
     if bootstrap_type[1:2] == '1':
       self.crv_type = "crv1"
       self.ssc = 1
-      if(adj == True):
+      if adj:
         self.ssc = self.ssc * (self.N - 1) / (self.N - self.k)
-      if(cluster_adj == True):
+      if cluster_adj:
         self.ssc = self.ssc * self.G / (self.G - 1)
     elif bootstrap_type[1:2] == '3':
       self.crv_type = "crv3"
       self.ssc = (self.G - 1) / self.G
 
     bootstrap_type_x = bootstrap_type[0:1] + 'x'
 
@@ -415,15 +416,18 @@
 def wildboottest(model : 'OLS', 
                  cluster : Union[np.ndarray, pd.Series, pd.DataFrame], 
                  B:int, 
                  param : Union[str, None] = None, 
                  weights_type: str = 'rademacher',
                  impose_null: bool = True, 
                  bootstrap_type: str = '11', 
-                 seed: Union[str, None] = None) -> float:
+                 seed: Union[str, None] = None,
+                 adj: bool = True,
+                 cluster_adj: bool = True,
+                 show=True) -> pd.DataFrame:
   """Run a wild cluster bootstrap based on an object of class 'statsmodels.regression.linear_model.OLS'
 
   Args:
       model (OLS):  A statsmodels regression object
       cluster (Union[np.ndarray, pd.Series, pd.DataFrame]): A numpy array of dimension one, containing the clustering variable.
       B (int): The number of bootstrap iterations to run
       param (Union[str, None], optional): A string of length one, containing the test parameter of interest. Defaults to None.
@@ -486,46 +490,50 @@
     
     # is it possible to fetch the clustering variables from the pre-processed data 
     # frame, e.g. with 'excluding' observations with missings etc
     # cluster = ...
         
     boot = Wildboottest(X = X, Y = Y, cluster = cluster, 
                         R = R, B = B, seed = seed)
-    boot.get_scores(bootstrap_type = bootstrap_type, impose_null = impose_null)
-    boot.get_weights(weights_type = weights_type)
+    boot.get_scores(bootstrap_type = bootstrap_type, impose_null = impose_null, adj=adj, cluster_adj=cluster_adj)
+    _, _, full_enumeration_warn = boot.get_weights(weights_type = weights_type)
     boot.get_numer()
     boot.get_denom()
     boot.get_tboot()
     boot.get_vcov()
     boot.get_tstat()
     boot.get_pvalue(pval_type = "two-tailed")
     
     pvalues.append(boot.pvalue)
     tstats.append(boot.t_stat[0])
-  
-    return pvalues, tstats
+      
+    return pvalues, tstats, full_enumeration_warn
     
   if param is None:
     for x in xnames:
-      pvalues, tstats = generate_stats(x)
+      pvalues, tstats, full_enumeration_warn = generate_stats(x)
     param = xnames
   elif isinstance(param, str):
-    pvalues, tstats = generate_stats(param)
+    pvalues, tstats, full_enumeration_warn = generate_stats(param)
   else:
     raise Exception("`param` not correctly specified")
   
+  if full_enumeration_warn:
+    warnings.warn("2^G < the number of boot iterations, setting full_enumeration to True.")
+  
   res = {
     'param': param,
     'statistic': tstats,
     'p-value': pvalues
   }
   
   res_df = pd.DataFrame(res).set_index('param')
   
-  print(res_df.to_markdown(floatfmt=".3f"))
+  if show:
+    print(res_df.to_markdown(floatfmt=".3f"))
   
   return res_df
   
 if __name__ == '__main__':
     import statsmodels.api as sm
     import numpy as np
```

### Comparing `wildboottest-0.1.5/setup.py` & `wildboottest-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pandas>=1.4,<2.0',
  'pytest>=3.0,<4.0',
  'statsmodels>=0.13,<0.14',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'wildboottest',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Wild Cluster Bootstrap Inference for Linear Models in Python',
     'long_description': '## wildboottest\n\n![PyPI](https://img.shields.io/pypi/v/wildboottest?label=pypi%20package)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/wildboottest)\n\n`wildboottest` implements multiple fast wild cluster\nbootstrap algorithms as developed in [Roodman et al\n(2019)](https://econpapers.repec.org/paper/qedwpaper/1406.htm) and\n[MacKinnon, Nielsen & Webb\n(2022)](https://www.econ.queensu.ca/sites/econ.queensu.ca/files/wpaper/qed_wp_1485.pdf).\n\nIt has similar, but more limited functionality than Stata\'s [boottest](https://github.com/droodman/boottest), R\'s [fwildcusterboot](https://github.com/s3alfisc/fwildclusterboot) or Julia\'s [WildBootTests.jl](https://github.com/droodman/WildBootTests.jl). It supports\n\n-   The wild cluster bootstrap for OLS ([Cameron, Gelbach & Miller 2008](https://direct.mit.edu/rest/article-abstract/90/3/414/57731/Bootstrap-Based-Improvements-for-Inference-with),\n    [Roodman et al (2019)](https://econpapers.repec.org/paper/qedwpaper/1406.htm)).\n-   Multiple new versions of the wild cluster bootstrap as described in\n    [MacKinnon, Nielsen & Webb (2022)](https://www.econ.queensu.ca/sites/econ.queensu.ca/files/wpaper/qed_wp_1485.pdf), including the WCR13, WCR31, WCR33,\n    WCU13, WCU31 and WCU33.\n-   CRV1 and CRV3 robust variance estimation, including the CRV3-Jackknife as \n    described in [MacKinnon, Nielsen & Webb (2022)](https://arxiv.org/pdf/2205.03288.pdf).\n    \nAt the moment, `wildboottest` only computes wild cluster bootstrapped *p-values*, and no confidence intervals. \n\nOther features that are currently not supported: \n\n- The (non-clustered) wild bootstrap for OLS ([Wu, 1986](https://projecteuclid.org/journals/annals-of-statistics/volume-14/issue-4/Jackknife-Bootstrap-and-Other-Resampling-Methods-in-Regression-Analysis/10.1214/aos/1176350142.full)).\n-   The subcluster bootstrap ([MacKinnon and Webb 2018](https://academic.oup.com/ectj/article-abstract/21/2/114/5078969?login=false)).\n-   Confidence intervals formed by inverting the test and iteratively\n    searching for bounds.\n-   Multiway clustering.\n\n\nDirect support for [statsmodels](https://github.com/statsmodels/statsmodels) and \n[linearmodels](https://github.com/bashtage/linearmodels) is work in progress.\n\nIf you\'d like to cooperate, either send us an \n[email](alexander-fischer1801@t-online.de) or comment in the issues section!\n\n## Installation \n\nYou can install `wildboottest` from [PyPi](https://pypi.org/project/wildboottest/) by running \n\n```\npip install wildboottest\n```\n\n## Example \n\n```python\nfrom wildboottest.wildboottest import wildboottest\nimport statsmodels.api as sm\nimport numpy as np\nimport pandas as pd\n\n# create data\nnp.random.seed(12312312)\nN = 1000\nk = 10\nG = 25\nX = np.random.normal(0, 1, N * k).reshape((N,k))\nX = pd.DataFrame(X)\nX.rename(columns = {0:"X1"}, inplace = True)\nbeta = np.random.normal(0,1,k)\nbeta[0] = 0.005\nu = np.random.normal(0,1,N)\nY = 1 + X @ beta + u\ncluster = np.random.choice(list(range(0,G)), N)\n\n# estimation\nmodel = sm.OLS(Y, X)\n\nwildboottest(model, param = "X1", cluster = cluster, B = 9999, bootstrap_type = "11")\n#   param              statistic   p-value\n# 0    X1  [-1.0530803154504016]  0.308831\n\nwildboottest(model, param = "X1", cluster = cluster, B = 9999, bootstrap_type = "31")\n#   param              statistic   p-value\n# 0    X1  [-1.0530803154504016]  0.307631\n\nwildboottest(model, param = "X1", cluster = cluster, B = 9999, bootstrap_type = "33")\n#   param              statistic   p-value\n# 0    X1  [-1.0394791020434824]  0.294286\n\n\nwildboottest(model, cluster = cluster, B = 9999)\n#   param              statistic   p-value\n# 0    X1  [-1.0530803154504016]  0.315132\n# 1     1    [-18.5149486170657]  0.000000\n# 2     2    [7.831855813581191]  0.000000\n# 3     3   [-16.85188951397906]  0.000000\n# 4     4  [-12.721095348008182]  0.000000\n# 5     5    [1.200524160940055]  0.243624\n# 6     6    [6.870946666836135]  0.000000\n# 7     7   [-31.31653422266621]  0.000000\n# 8     8    [10.26443257212472]  0.000000\n# 9     9  [-20.650361366939535]  0.000000\n```\n',
     'author': 'Alexander Fischer',
     'author_email': 'alexander-fischer1801@t-online.de',
     'maintainer': 'Aleksandr Michuda',
     'maintainer_email': 'amichuda@gmail.com',
     'url': 'https://github.com/s3alfisc/wildboottest',
```

### Comparing `wildboottest-0.1.5/PKG-INFO` & `wildboottest-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildboottest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wild Cluster Bootstrap Inference for Linear Models in Python
 Home-page: https://github.com/s3alfisc/wildboottest
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Maintainer: Aleksandr Michuda
 Maintainer-email: amichuda@gmail.com
```

