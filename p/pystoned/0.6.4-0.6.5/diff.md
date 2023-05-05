# Comparing `tmp/pystoned-0.6.4.tar.gz` & `tmp/pystoned-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystoned-0.6.4.tar", last modified: Fri Apr 14 13:50:02 2023, max compression
+gzip compressed data, was "pystoned-0.6.5.tar", last modified: Fri May  5 11:12:24 2023, max compression
```

## Comparing `pystoned-0.6.4.tar` & `pystoned-0.6.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.637539 pystoned-0.6.4/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    35149 2021-10-05 07:06:23.000000 pystoned-0.6.4/LICENSE
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-14 13:50:02.637539 pystoned-0.6.4/PKG-INFO
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2288 2023-01-28 14:01:26.000000 pystoned-0.6.4/README.md
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    13360 2023-04-14 13:42:03.000000 pystoned-0.6.4/pystoned/CNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8579 2023-04-07 08:10:12.000000 pystoned-0.6.4/pystoned/CNLSDDF.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     9975 2023-04-14 13:44:39.000000 pystoned-0.6.4/pystoned/CNLSG.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    15915 2023-04-14 13:31:50.000000 pystoned-0.6.4/pystoned/CQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8122 2023-04-07 08:10:02.000000 pystoned-0.6.4/pystoned/CQERDDF.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    21756 2023-04-14 13:40:58.000000 pystoned-0.6.4/pystoned/CQERG.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     6908 2023-04-14 13:36:31.000000 pystoned-0.6.4/pystoned/CSVR.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    18111 2023-04-07 08:09:53.000000 pystoned-0.6.4/pystoned/DEA.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     5964 2023-04-07 08:09:49.000000 pystoned-0.6.4/pystoned/FDH.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4816 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/ICNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2861 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/ICQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     9456 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/StoNED.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      800 2023-01-31 11:34:44.000000 pystoned-0.6.4/pystoned/__init__.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1473 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/constant.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned/data/
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1429 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/41Firm.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     7609 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/abatementCost.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3082 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/electricityFirms.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)    33693 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/riceProduction.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4733 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/dataset.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2993 2023-04-08 10:42:52.000000 pystoned-0.6.4/pystoned/pCNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     6357 2023-04-08 10:42:11.000000 pystoned-0.6.4/pystoned/pCQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3250 2023-04-08 10:44:39.000000 pystoned-0.6.4/pystoned/pICQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4701 2023-04-14 13:15:21.000000 pystoned-0.6.4/pystoned/plot.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8256 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/sCQER.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.637539 pystoned-0.6.4/pystoned/utils/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    11736 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    14915 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    12161 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSZG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    15358 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSZG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    13742 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    16930 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    14286 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERZG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    17619 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERZG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      240 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/__init__.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1121 2023-04-14 10:56:02.000000 pystoned-0.6.4/pystoned/utils/interpolation.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      960 2023-02-25 12:37:20.000000 pystoned-0.6.4/pystoned/utils/sweet.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8684 2023-03-04 07:54:35.000000 pystoned-0.6.4/pystoned/utils/tools.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1632 2023-04-07 23:03:08.000000 pystoned-0.6.4/pystoned/wCNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3327 2023-04-07 23:03:03.000000 pystoned-0.6.4/pystoned/wCQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    11886 2023-04-07 23:04:51.000000 pystoned-0.6.4/pystoned/weakCNLS.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned.egg-info/
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/PKG-INFO
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     1075 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/SOURCES.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/dependency_links.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-14 13:49:08.000000 pystoned-0.6.4/pystoned.egg-info/not-zip-safe
--rw-rw-r--   0 dais2     (1000) dais2     (1000)       86 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/requires.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        9 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/top_level.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)       38 2023-04-14 13:50:02.637539 pystoned-0.6.4/setup.cfg
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1345 2023-04-14 12:21:31.000000 pystoned-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.707428 pystoned-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 11:12:09.000000 pystoned-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-05 11:12:24.707428 pystoned-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-05 11:12:09.000000 pystoned-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned/
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLSDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLSG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQERDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQERG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CSVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/FDH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/ICNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/ICQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/StoNED.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/abatementCost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33693 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/riceProduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pCNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pCQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pICQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/sCQER.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.707428 pystoned-0.6.5/pystoned/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/wCNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/wCQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/weakCNLS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:12:24.707428 pystoned-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-05 11:12:10.000000 pystoned-0.6.5/setup.py
```

### Comparing `pystoned-0.6.4/LICENSE` & `pystoned-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/PKG-INFO` & `pystoned-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.4/README.md` & `pystoned-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/CNLS.py` & `pystoned-0.6.5/pystoned/CNLS.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z)
 
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.cet, self.fun, self.rts = cet, fun, rts
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         if type(self.z) != type(None):
             # Initialize the set of z
             self.__model__.K = Set(initialize=range(len(self.z[0])))
@@ -68,16 +66,15 @@
                                                  doc='log-transformed regression equation')
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
@@ -297,15 +294,15 @@
         tools.assert_optimized(self.optimization_status)
         return self.get_residual() - np.amax(self.get_residual())
 
     def get_adjusted_alpha(self):
         """Return the shifted constatnt(alpha) term by CCNLS"""
         tools.assert_optimized(self.optimization_status)
         return self.get_alpha() + np.amax(self.get_residual())
-    
+
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
         if self.rts == RTS_VRS:
             alpha,  beta = self.get_alpha(), self.get_beta()
         elif self.rts == RTS_CRS:
             alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
```

### Comparing `pystoned-0.6.4/pystoned/CNLSDDF.py` & `pystoned-0.6.5/pystoned/CNLSDDF.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,19 @@
             b (float), optional): undesirable output variables. Defaults to None.
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
             gb (list, optional): undesirable output directional vector. Defaults to None.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.y, self.x, self.b, self.gy, self.gx, self.gb = tools.assert_valid_direciontal_data(y,x,b,gy,gx,gb)
-        self.fun = fun
-        self.rts = RTS_VRS
-    
+        self.y, self.x, self.b, self.gy, self.gx, self.gb = tools.assert_valid_direciontal_data(
+            y, x, b, gy, gx, gb)
+        self.fun, self.rts = fun, RTS_VRS
+
+        # Initialize the CNLSDDF model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
         self.__model__.J = Set(initialize=range(len(self.x[0])))
         self.__model__.Q = Set(initialize=range(len(self.y[0])))
 
@@ -62,16 +63,15 @@
                                                      doc='translation property')
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/CNLSG.py` & `pystoned-0.6.5/pystoned/CNLSG.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,23 @@
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.cutactive = sweet.sweet(x)
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z)
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.cet, self.fun, self.rts = cet, fun, rts
 
         # active (added) violated concavity constraint by iterative procedure
         self.active = np.zeros((len(x), len(x)))
         # violated concavity constraint
         self.active2 = np.zeros((len(x), len(x)))
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method"""
         # TODO(error/warning handling): Check problem status after optimization
         self.t0 = time.time()
         if type(self.z) != type(None):
             model1 = CNLSZG1.CNLSZG1(
```

### Comparing `pystoned-0.6.4/pystoned/CQER.py` & `pystoned-0.6.5/pystoned/CQER.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,15 @@
             tau (float): quantile.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z)
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.tau, self.cet, self.fun, self.rts = tau, cet, fun, rts
 
         # Initialize the CQR model
         self.__model__ = ConcreteModel()
 
         if type(self.z) != type(None):
             # Initialize the set of z
             self.__model__.K = Set(initialize=range(len(self.z[0])))
@@ -79,16 +76,15 @@
 
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
@@ -326,15 +322,15 @@
         """Return estimated frontier value by array"""
         tools.assert_optimized(self.optimization_status)
         if self.cet == CET_MULT:
             frontier = np.asarray(list(self.__model__.frontier[:].value)) + 1
         elif self.cet == CET_ADDI:
             frontier = np.asarray(self.y) - self.get_residual()
         return np.asarray(frontier)
-    
+
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
         if self.rts == RTS_VRS:
             alpha,  beta = self.get_alpha(), self.get_beta()
         elif self.rts == RTS_CRS:
             alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
```

### Comparing `pystoned-0.6.4/pystoned/CQERDDF.py` & `pystoned-0.6.5/pystoned/CQERDDF.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,19 @@
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
             gb (list, optional): undesirable output directional vector. Defaults to None.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             tau (float, optional): quantile. Defaults to 0.5.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.y, self.x, self.b, self.gy, self.gx, self.gb = tools.assert_valid_direciontal_data(y,x,b,gy,gx,gb)
-        self.tau = tau
-        self.fun = fun
-        self.rts = RTS_VRS
+        self.y, self.x, self.b, self.gy, self.gx, self.gb = tools.assert_valid_direciontal_data(
+            y, x, b, gy, gx, gb)
+        self.tau, self.fun, self.rts = tau, fun, RTS_VRS
+
+        # Initialize the CQRDDF model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
         self.__model__.J = Set(initialize=range(len(self.x[0])))
         self.__model__.Q = Set(initialize=range(len(self.y[0])))
 
@@ -71,16 +72,15 @@
 
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def __regression_rule(self):
         """Return the proper regression constraint"""
         if type(self.b) == type(None):
             def regression_rule(model, i):
                 return sum(model.gamma[i, q] * self.y[i][q] for q in model.Q) \
                     == model.alpha[i] \
```

### Comparing `pystoned-0.6.4/pystoned/CQERG.py` & `pystoned-0.6.5/pystoned/CQERG.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,23 @@
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.cutactive = sweet.sweet(x)
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z)
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.tau, self.cet, self.fun, self.rts = tau, cet, fun, rts
 
         # active (added) violated concavity constraint by iterative procedure
         self.active = np.zeros((len(x), len(x)))
         # violated concavity constraint
         self.active2 = np.zeros((len(x), len(x)))
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method"""
         # TODO(error/warning handling): Check problem status after optimization
         self.t0 = time.time()
         if type(self.z) != type(None):
             model1 = CQERZG1.CQRZG1(
@@ -258,27 +254,23 @@
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.cutactive = sweet.sweet(x)
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z)
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.tau, self.cet, self.fun, self.rts = tau, cet, fun, rts
 
         # active (added) violated concavity constraint by iterative procedure
         self.active = np.zeros((len(x), len(x)))
         # violated concavity constraint
         self.active2 = np.zeros((len(x), len(x)))
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method"""
         # TODO(error/warning handling): Check problem status after optimization
         self.t0 = time.time()
         if type(self.z) != type(None):
             model1 = CQERZG1.CERZG1(
```

### Comparing `pystoned-0.6.4/pystoned/CSVR.py` & `pystoned-0.6.5/pystoned/CSVR.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,59 +20,55 @@
             x (float): input variables.
             epsilon (float): epsilon-loss function.
             C (float): Regularization parameter.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x, self.z = tools.assert_valid_basic_data(y, x, z=None)
-        self.epsilon = epsilon
-        self.C = C
-        self.cet = CET_ADDI
-        self.fun = fun
+        self.epsilon, self.C, self.cet, self.fun = epsilon, C, CET_ADDI, fun
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
         self.__model__.J = Set(initialize=range(len(self.x[0])))
 
         # Initialize the variables
         self.__model__.alpha = Var(self.__model__.I, doc='alpha')
         self.__model__.beta = Var(self.__model__.I,
                                   self.__model__.J,
                                   doc='beta')
-        self.__model__.ksia = Var(self.__model__.I, 
-                                  bounds=(0.0, None), 
+        self.__model__.ksia = Var(self.__model__.I,
+                                  bounds=(0.0, None),
                                   doc='Ksi a')
-        self.__model__.ksib = Var(self.__model__.I, 
-                                  bounds=(0.0, None), 
+        self.__model__.ksib = Var(self.__model__.I,
+                                  bounds=(0.0, None),
                                   doc='Ksi b')
 
         # Setup the objective function and constraints
         self.__model__.objective = Objective(rule=self.__objective_rule(),
                                              sense=minimize,
                                              doc='objective function')
 
         self.__model__.regression_rule1 = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule1(),
-                                                    doc='regression equation')
+                                                     rule=self.__regression_rule1(),
+                                                     doc='regression equation')
 
         self.__model__.regression_rule2 = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule2(),
-                                                    doc='regression equation')
+                                                     rule=self.__regression_rule2(),
+                                                     doc='regression equation')
 
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
@@ -82,15 +78,15 @@
             self.__model__, email, self.cet, solver)
 
     def __objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return self.C * (sum(model.ksia[i] for i in model.I) + sum(model.ksib[i] for i in model.I)) + \
-                        sum(model.beta[i, j]**2 for i in model.I for j in model.J)
+                sum(model.beta[i, j]**2 for i in model.I for j in model.J)
 
         return objective_rule
 
     def __regression_rule1(self):
         """Return the proper regression constraint"""
 
         def regression_rule1(model, i):
@@ -116,17 +112,17 @@
             __operator = NumericValue.__ge__
 
         def afriat_rule(model, i, h):
             if i == h:
                 return Constraint.Skip
             return __operator(
                 model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                    for j in model.J),
+                                     for j in model.J),
                 model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                    for j in model.J))
+                                     for j in model.J))
 
         return afriat_rule
 
     def display_status(self):
         """Display the status of problem"""
         tools.assert_optimized(self.optimization_status)
         print(self.display_status)
```

### Comparing `pystoned-0.6.4/pystoned/DEA.py` & `pystoned-0.6.5/pystoned/DEA.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,22 @@
             orient (String): ORIENT_IO (input orientation) or ORIENT_OO (output orientation)
             rts (String): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale)
             yref (String, optional): reference output. Defaults to None.
             xref (String, optional): reference inputs. Defaults to None.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x = tools.assert_valid_mupltiple_y_data(y, x)
-        self.orient = orient
-        self.rts = rts
+        self.orient, self.rts = orient, rts
 
         if type(yref) != type(None):
             self.yref, self.xref = tools.assert_valid_reference_data(
                 self.y, self.x, yref, xref)
         else:
             self.yref, self.xref = self.y, self.x
-        
+
         # Initialize DEA model
         self.__model__ = ConcreteModel()
         self.__model__.R = Set(initialize=range(len(self.yref)))
 
         # Initialize sets
         self.__model__.I = Set(initialize=range(len(self.y)))
         self.__model__.J = Set(initialize=range(len(self.x[0])))
@@ -58,16 +57,15 @@
         self.__model__.output = Constraint(
             self.__model__.I, self.__model__.K, rule=self.__output_rule(), doc='output constraint')
         if self.rts == RTS_VRS:
             self.__model__.vrs = Constraint(
                 self.__model__.I, rule=self.__vrs_rule(), doc='variable return to scale rule')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def __objective_rule(self):
         """Return the proper objective function"""
         def objective_rule(model):
             return sum(model.theta[i] for i in model.I)
         return objective_rule
 
@@ -133,15 +131,15 @@
         theta = list(self.__model__.theta[:].value)
         return np.asarray(theta)
 
     def get_lamda(self):
         """Return lamda value by array"""
         tools.assert_optimized(self.optimization_status)
         lamda = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.lamda),
-                                                          list(self.__model__.lamda[:, :].value))])
+                                                           list(self.__model__.lamda[:, :].value))])
         lamda = pd.DataFrame(lamda, columns=['Name', 'Key', 'Value'])
         lamda = lamda.pivot(index='Name', columns='Key', values='Value')
         return lamda.to_numpy()
 
 
 class DDF(DEA):
     def __init__(self,  y, x, b=None, gy=[1], gx=[1], gb=None, rts=RTS_VRS, yref=None, xref=None, bref=None):
@@ -200,16 +198,15 @@
                 self.__model__.I, self.__model__.L, rule=self.__undesirable_output_rule(), doc='undesirable output constraint')
 
         if self.rts == RTS_VRS:
             self.__model__.vrs = Constraint(
                 self.__model__.I, rule=self.__vrs_rule(), doc='various return to scale rule')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def __input_rule(self):
         """Return the proper input constraint"""
         def input_rule(model, o, j):
             return self.x[o][j] - model.theta[o]*self.gx[j] >= sum(model.lamda[o, r] * self.xref[r][j] for r in model.R)
         return input_rule
 
@@ -244,16 +241,15 @@
             yref (String, optional): reference output. Defaults to None.
             xref (String, optional): reference inputs. Defaults to None.
         """
         # Initialize DEA model
         self.__model__ = ConcreteModel()
 
         self.y, self.x = tools.assert_valid_mupltiple_y_data(y, x)
-        self.orient = orient
-        self.rts = rts
+        self.orient, self.rts = orient, rts
 
         if type(yref) != type(None):
             self.yref, self.xref = tools.assert_valid_reference_data(
                 self.y, self.x, yref, xref)
         else:
             self.yref, self.xref = self.y, self.x
         self.__model__.R = Set(initialize=range(len(self.yref)))
@@ -265,69 +261,69 @@
 
         # Initialize variable
         self.__model__.nu = Var(self.__model__.I, self.__model__.J, bounds=(
             0.0, None), doc='multiplier x')
         self.__model__.mu = Var(self.__model__.I, self.__model__.K, bounds=(
             0.0, None), doc='multiplier y')
         if self.rts == RTS_VRS:
-            self.__model__.omega = Var(self.__model__.I, doc='variable return to scale')
+            self.__model__.omega = Var(
+                self.__model__.I, doc='variable return to scale')
 
         # Setup the objective function and constraints
         if self.orient == ORIENT_IO:
             self.__model__.objective = Objective(
                 rule=self.__objective_rule(), sense=maximize, doc='objective function')
         else:
             self.__model__.objective = Objective(
                 rule=self.__objective_rule(), sense=minimize, doc='objective function')
         self.__model__.first = Constraint(
             self.__model__.I, self.__model__.R, rule=self.__first_rule(), doc='technology constraint')
         self.__model__.second = Constraint(
             self.__model__.I, rule=self.__second_rule(), doc='normalization constraint')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def __objective_rule(self):
         """Return the proper objective function"""
         if self.orient == ORIENT_IO:
             def objective_rule(model):
                 if self.rts == RTS_VRS:
                     return sum(sum(model.mu[o, k] * self.y[o][k] for o in model.I) for k in model.K) + sum(model.omega[o] for o in model.I)
-                elif self.rts == RTS_CRS: 
+                elif self.rts == RTS_CRS:
                     return sum(sum(model.mu[o, k] * self.y[o][k] for o in model.I) for k in model.K)
             return objective_rule
         elif self.orient == ORIENT_OO:
             def objective_rule(model):
                 if self.rts == RTS_VRS:
                     return sum(sum(model.nu[o, j] * self.x[o][j] for o in model.I) for j in model.J) + sum(model.omega[o] for o in model.I)
-                elif self.rts == RTS_CRS: 
+                elif self.rts == RTS_CRS:
                     return sum(sum(model.nu[o, j] * self.x[o][j] for o in model.I) for j in model.J)
-            return objective_rule            
- 
+            return objective_rule
+
     def __first_rule(self):
         """Return the proper technology constraint"""
         if self.orient == ORIENT_IO:
             if self.rts == RTS_VRS:
                 def first_rule(model, o, r):
                     return sum(model.mu[o, k] * self.yref[r][k] for k in model.K) - sum(model.nu[o, j] * self.xref[r][j] for j in model.J) + model.omega[o] <= 0
                 return first_rule
             elif self.rts == RTS_CRS:
                 def first_rule(model, o, r):
-                    return sum(model.mu[o, k] * self.yref[r][k] for k in model.K) - sum(model.nu[o, j] * self.xref[r][j] for j in model.J)  <= 0
-                return first_rule         
+                    return sum(model.mu[o, k] * self.yref[r][k] for k in model.K) - sum(model.nu[o, j] * self.xref[r][j] for j in model.J) <= 0
+                return first_rule
         elif self.orient == ORIENT_OO:
             if self.rts == RTS_VRS:
                 def first_rule(model, o, r):
                     return sum(model.nu[o, j] * self.xref[r][j] for j in model.J) - sum(model.mu[o, k] * self.yref[r][k] for k in model.K) + model.omega[o] >= 0
                 return first_rule
             elif self.rts == RTS_CRS:
                 def first_rule(model, o, r):
                     return sum(model.nu[o, j] * self.xref[r][j] for j in model.J) - sum(model.mu[o, k] * self.yref[r][k] for k in model.K) >= 0
-                return first_rule      
+                return first_rule
 
     def __second_rule(self):
         """Return the proper normalization constraint"""
         if self.orient == ORIENT_IO:
             def second_rule(model, o):
                 return sum(model.nu[o, j] * self.x[o][j] for j in model.J) == 1
             return second_rule
@@ -343,33 +339,33 @@
 
     def display_nu(self):
         """Display nu value"""
         tools.assert_optimized(self.optimization_status)
         self.__model__.nu.display()
 
     def display_omega(self):
-         """Display omega value"""
-         tools.assert_optimized(self.optimization_status)
-         tools.assert_various_return_to_scale_omega(self.rts)
-         self.__model__.omega.display()       
+        """Display omega value"""
+        tools.assert_optimized(self.optimization_status)
+        tools.assert_various_return_to_scale_omega(self.rts)
+        self.__model__.omega.display()
 
     def get_mu(self):
         """Return mu value by array"""
         tools.assert_optimized(self.optimization_status)
         mu = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.mu),
-                                                          list(self.__model__.mu[:, :].value))])
+                                                        list(self.__model__.mu[:, :].value))])
         mu = pd.DataFrame(mu, columns=['Name', 'Key', 'Value'])
         mu = mu.pivot(index='Name', columns='Key', values='Value')
         return mu.to_numpy()
 
     def get_nu(self):
         """Return nu value by array"""
         tools.assert_optimized(self.optimization_status)
         nu = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.nu),
-                                                          list(self.__model__.nu[:, :].value))])
+                                                        list(self.__model__.nu[:, :].value))])
         nu = pd.DataFrame(nu, columns=['Name', 'Key', 'Value'])
         nu = nu.pivot(index='Name', columns='Key', values='Value')
         return nu.to_numpy()
 
     def get_omega(self):
         """Return omega value by array"""
         tools.assert_optimized(self.optimization_status)
@@ -386,8 +382,7 @@
             elif self.rts == RTS_VRS:
                 return (np.sum(self.get_mu()*self.y, axis=1)).reshape(len(self.y), 1) + self.get_omega().reshape(len(self.y), 1)
         elif self.orient == ORIENT_OO:
             if self.rts == RTS_CRS:
                 return (np.sum(self.get_nu()*self.x, axis=1)).reshape(len(self.x), 1)
             elif self.rts == RTS_VRS:
                 return (np.sum(self.get_nu()*self.x, axis=1)).reshape(len(self.x), 1) + self.get_omega().reshape(len(self.x), 1)
-
```

### Comparing `pystoned-0.6.4/pystoned/FDH.py` & `pystoned-0.6.5/pystoned/FDH.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             orient (String): ORIENT_IO (input orientation) or ORIENT_OO (output orientation)
             yref (String, optional): reference output. Defaults to None.
             xref (String, optional): reference inputs. Defaults to None.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x = tools.assert_valid_mupltiple_y_data(y, x)
         self.orient = orient
-        
+
         if type(yref) != type(None):
             self.yref, self.xref = tools.assert_valid_reference_data(
                 self.y, self.x, yref, xref)
         else:
             self.yref, self.xref = self.y, self.x
 
         # Initialize FDH model
@@ -55,16 +55,15 @@
             self.__model__.I, self.__model__.J, rule=self.__input_rule(), doc='input constraint')
         self.__model__.output = Constraint(
             self.__model__.I, self.__model__.K, rule=self.__output_rule(), doc='output constraint')
         self.__model__.vrs = Constraint(
             self.__model__.I, rule=self.__vrs_rule(), doc='variable return to scale rule')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def __objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return sum(model.theta[i] for i in model.I)
 
@@ -132,12 +131,11 @@
         theta = list(self.__model__.theta[:].value)
         return np.asarray(theta)
 
     def get_lamda(self):
         """Return lamda value by array"""
         tools.assert_optimized(self.optimization_status)
         lamda = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.lamda),
-                                                          list(self.__model__.lamda[:, :].value))])
+                                                           list(self.__model__.lamda[:, :].value))])
         lamda = pd.DataFrame(lamda, columns=['Name', 'Key', 'Value'])
         lamda = lamda.pivot(index='Name', columns='Key', values='Value')
         return lamda.to_numpy()
-
```

### Comparing `pystoned-0.6.4/pystoned/ICNLS.py` & `pystoned-0.6.5/pystoned/ICNLS.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,15 @@
 
     def __binaryMatrix(self):
         """generating binary matrix P"""
         # transform data
         x = np.array(self.x)
 
         # number of DMUs
-        n = len(x)
-        m = len(x[0])
+        n, m = len(x), len(x[0])
 
         # binary matrix P
         p = np.zeros((n, n))
         for i in range(n):
             pmap = (x[i, 0] <= x[:, 0])
             for j in range(1, m):
                 pmap = pmap & (x[i, j] <= x[:, j])
```

### Comparing `pystoned-0.6.4/pystoned/ICQER.py` & `pystoned-0.6.5/pystoned/ICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/StoNED.py` & `pystoned-0.6.5/pystoned/StoNED.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # import dependencies
 import numpy as np
-import math
+from math import sqrt, pi, log
 import scipy.stats as stats
 import scipy.optimize as opt
 from .utils import tools
 from .constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RED_MOM, RED_QLE, RED_KDE
 
 
 class StoNED:
     """Stochastic nonparametric envelopment of data (StoNED)
     """
 
     def __init__(self, model):
         """StoNED
         model: The input model for residual decomposition
         """
-        self.model = model
-        self.x = model.x
+        self.model, self.x = model, model.x
 
         # If the model is a directional distance based, set cet to CET_ADDI
         if hasattr(self.model, 'gx'):
             self.model.cet = CET_ADDI
             self.y = np.diag(np.tensordot(
                 self.model.y, self.model.get_gamma(), axes=([1], [1])))
         else:
@@ -47,18 +46,18 @@
         Args:
             method (String, optional): RED_MOM (Method of moments) or RED_QLE (Quassi-likelihood estimation). Defaults to RED_MOM.
 
         calculate sigma_u, sigma_v, mu, and epsilon value
         """
         tools.assert_optimized(self.model.optimization_status)
         self.get_unconditional_expected_inefficiency(method)
-        sigma = self.sigma_u * self.sigma_v / math.sqrt(self.sigma_u ** 2 +
-                                                        self.sigma_v ** 2)
+        sigma = self.sigma_u * self.sigma_v / sqrt(self.sigma_u ** 2 +
+                                                   self.sigma_v ** 2)
         mu = self.epsilon * self.sigma_u / (
-            self.sigma_v * math.sqrt(self.sigma_u ** 2 + self.sigma_v ** 2))
+            self.sigma_v * sqrt(self.sigma_u ** 2 + self.sigma_v ** 2))
 
         if self.model.fun == FUN_PROD:
             Eu = sigma * ((stats.norm.pdf(mu) /
                            (1 - stats.norm.cdf(mu) + 0.000001)) - mu)
             if self.model.cet == CET_ADDI:
                 return (self.y - Eu) / self.y
             elif self.model.cet == CET_MULT:
@@ -79,29 +78,29 @@
 
         M2_mean = np.mean(M2, axis=0)
         M3_mean = np.mean(M3, axis=0)
 
         if self.model.fun == FUN_PROD:
             if M3_mean > 0:
                 M3_mean = 0.0
-            self.sigma_u = (M3_mean / ((2 / math.pi) ** (1 / 2) *
-                                       (1 - 4 / math.pi))) ** (1 / 3)
+            self.sigma_u = (M3_mean / ((2 / pi) ** (1 / 2) *
+                                       (1 - 4 / pi))) ** (1 / 3)
 
         elif self.model.fun == FUN_COST:
             if M3_mean < 0:
                 M3_mean = 0.00001
-            self.sigma_u = (-M3_mean / ((2 / math.pi) ** (1 / 2) *
-                                        (1 - 4 / math.pi))) ** (1 / 3)
+            self.sigma_u = (-M3_mean / ((2 / pi) ** (1 / 2) *
+                                        (1 - 4 / pi))) ** (1 / 3)
 
         else:
             raise ValueError("Undefined model parameters.")
 
-        self.sigma_v = (M2_mean -
-                        ((math.pi - 2) / math.pi) * self.sigma_u ** 2) ** (1 / 2)
-        self.mu = (self.sigma_u ** 2 * 2 / math.pi) ** (1 / 2)
+        self.sigma_v = (M2_mean - ((pi - 2) / pi) *
+                        self.sigma_u ** 2) ** (1 / 2)
+        self.mu = (self.sigma_u ** 2 * 2 / pi) ** (1 / 2)
         if self.model.fun == FUN_PROD:
             self.epsilon = residual - self.mu
         else:
             self.epsilon = residual + self.mu
 
     def __quassi_likelihood(self, residual):
         def __quassi_likelihood_estimation(lamda, eps):
@@ -113,28 +112,26 @@
                 eps (list): values of the residual
 
             Returns:
                 float: -logl, negative value of log likelihood
             """
             # sigma Eq. (3.26) in Johnson and Kuosmanen (2015)
             sigma = np.sqrt(
-                np.mean(eps ** 2) / (1 - 2 * lamda ** 2 / (math.pi *
-                                                           (1 + lamda ** 2))))
+                np.mean(eps ** 2) / (1 - 2 * lamda ** 2 / (pi * (1 + lamda ** 2))))
 
             # bias adjusted residuals Eq. (3.25)
             # mean
-            mu = math.sqrt(
-                2 / math.pi) * sigma * lamda / math.sqrt(1 + lamda ** 2)
+            mu = sqrt(2 / pi) * sigma * lamda / sqrt(1 + lamda ** 2)
 
             # adj. res.
             epsilon = eps - mu
 
             # log-likelihood function Eq. (3.24)
             pn = stats.norm.cdf(-epsilon * lamda / sigma)
-            return -(-len(epsilon) * math.log(sigma) + np.sum(np.log(pn)) -
+            return -(-len(epsilon) * log(sigma) + np.sum(np.log(pn)) -
                      0.5 * np.sum(epsilon ** 2) / sigma ** 2)
 
         if self.model.fun == FUN_PROD:
             lamda = opt.minimize(__quassi_likelihood_estimation,
                                  1.0,
                                  residual,
                                  method='BFGS').x[0]
@@ -143,36 +140,34 @@
                                  1.0,
                                  -residual,
                                  method='BFGS').x[0]
         else:
             # TODO(error/warning handling): Raise error while undefined fun
             return False
         # use estimate of lambda to calculate sigma Eq. (3.26) in Johnson and Kuosmanen (2015)
-        sigma = math.sqrt(
-            np.mean(residual ** 2) / (1 - (2 * lamda ** 2) / (math.pi *
-                                                              (1 + lamda ** 2))))
+        sigma = sqrt(np.mean(residual ** 2) /
+                     (1 - (2 * lamda ** 2) / (pi * (1 + lamda ** 2))))
 
         # calculate bias correction
         # (unconditional) mean
-        self.mu = math.sqrt(2) * sigma * lamda / math.sqrt(math.pi *
-                                                           (1 + lamda ** 2))
+        self.mu = sqrt(2) * sigma * lamda / sqrt(pi * (1 + lamda ** 2))
 
         # calculate sigma.u and sigma.v
         self.sigma_v = (sigma ** 2 / (1 + lamda ** 2)) ** (1 / 2)
         self.sigma_u = self.sigma_v * lamda
 
         if self.model.fun == FUN_PROD:
             self.epsilon = residual - self.mu
         elif self.model.fun == FUN_COST:
             self.epsilon = residual + self.mu
 
     def __gaussian_kernel_estimation(self, residual):
         def __gaussian_kernel_estimator(g):
             """Gaussian kernel estimator"""
-            return (1 / math.sqrt(2 * math.pi)) * np.exp(-0.5 * g ** 2)
+            return (1 / sqrt(2 * pi)) * np.exp(-0.5 * g ** 2)
 
         x = np.array(residual)
 
         # choose a bandwidth (rule-of-thumb, Eq. (3.29) in Silverman (1986))
         if np.std(x, ddof=1) < stats.iqr(x, interpolation='midpoint'):
             estimated_sigma = np.std(x, ddof=1)
         else:
@@ -210,17 +205,17 @@
         calculate sigma_u, sigma_v, mu, and epsilon value
         """
         tools.assert_optimized(self.model.optimization_status)
         self.get_unconditional_expected_inefficiency(method)
 
         if self.model.fun == FUN_PROD:
             if self.model.cet == CET_ADDI:
-                return (self.y - self.model.get_residual()) + self.sigma_u * math.sqrt(2 / math.pi)
+                return (self.y - self.model.get_residual()) + self.sigma_u * sqrt(2 / pi)
             elif self.model.cet == CET_MULT:
-                return (self.y / np.exp(self.model.get_residual())) * np.exp(self.sigma_u * math.sqrt(2 / math.pi))
+                return (self.y / np.exp(self.model.get_residual())) * np.exp(self.sigma_u * sqrt(2 / pi))
         elif self.model.fun == FUN_COST:
             if self.model.cet == CET_ADDI:
-                return (self.y - self.model.get_residual()) - self.sigma_u * math.sqrt(2 / math.pi)
+                return (self.y - self.model.get_residual()) - self.sigma_u * sqrt(2 / pi)
             elif self.model.cet == CET_MULT:
-                return (self.y / np.exp(self.model.get_residual())) * np.exp(-self.sigma_u * math.sqrt(2 / math.pi))
+                return (self.y / np.exp(self.model.get_residual())) * np.exp(-self.sigma_u * sqrt(2 / pi))
 
         raise ValueError("Undefined model parameters.")
```

### Comparing `pystoned-0.6.4/pystoned/__init__.py` & `pystoned-0.6.5/pystoned/__init__.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/constant.py` & `pystoned-0.6.5/pystoned/constant.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/data/41Firm.csv` & `pystoned-0.6.5/pystoned/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/data/abatementCost.csv` & `pystoned-0.6.5/pystoned/data/abatementCost.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/data/electricityFirms.csv` & `pystoned-0.6.5/pystoned/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/data/riceProduction.csv` & `pystoned-0.6.5/pystoned/data/riceProduction.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/dataset.py` & `pystoned-0.6.5/pystoned/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,15 @@
             dmu (String): decision making unit.
             x (Numbers): input variables.
             y (Numbers): output variables.
             b (Numbers, optional): bad output variables. Defaults to None.
             z (Numbers, optional): contextual variables. Defaults to None.
         """
         self.decision_making_unit = dmu
-        self.x = x
-        self.y = y
-        self.b = b
-        self.z = z
+        self.x, self.y, self.b, self.z = x, y, b, z
 
 
 def load_GHG_abatement_cost(year=None, x_select=['HRSN', 'CPNK'], y_select=['VALK'], b_select=['GHG']):
     """Loading OECD GHG emissions data
 
     Args:
         year (Numbers, optional): years. Defaults to None.
```

### Comparing `pystoned-0.6.4/pystoned/pCNLS.py` & `pystoned-0.6.5/pystoned/pCNLS.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,48 +21,49 @@
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
             penalty (int, optional): penalty=1 (L1 norm), penalty=2 (L2 norm), and penalty=3 (Lipschitz norm). Defaults to 1.
         """
         self.eta = eta
         CNLS.CNLS.__init__(self, y, x, z, cet, fun, rts)
         if penalty == 1 or penalty == 2:
             self.__model__.objective.deactivate()
-        
+
         if penalty == 1:
             self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 2:
             self.__model__.new_objective = Objective(rule=self.__new_objective_rule2(),
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 3:
-            self.__model__.lipschitz_norm = Constraint(self.__model__.I, 
-                                                        rule=self.__lipschitz_rule(), 
-                                                        doc='Lipschitz norm')
+            self.__model__.lipschitz_norm = Constraint(self.__model__.I,
+                                                       rule=self.__lipschitz_rule(),
+                                                       doc='Lipschitz norm')
         else:
             raise ValueError('Penalty must be 1, 2, or 3.')
 
     def __new_objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return sum(model.epsilon[i] ** 2 for i in model.I) \
-                   + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
+                + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
 
         return objective_rule
 
     def __new_objective_rule2(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return sum(model.epsilon[i] ** 2 for i in model.I) \
-                   + self.eta * sum(model.beta[ij] ** 2 for ij in model.I * model.J)
+                + self.eta * sum(model.beta[ij] **
+                                 2 for ij in model.I * model.J)
 
         return objective_rule
 
     def __lipschitz_rule(self):
         """Lipschitz norm"""
-        
+
         def lipschitz_rule(model, i):
             return sum(model.beta[i, j] ** 2 for j in model.J) <= self.eta**2
-    
+
         return lipschitz_rule
```

### Comparing `pystoned-0.6.4/pystoned/pCQER.py` & `pystoned-0.6.5/pystoned/pCQER.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,48 +32,49 @@
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 2:
             self.__model__.new_objective = Objective(rule=self.__new_objective_rule2(),
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 3:
-            self.__model__.lipschitz_norm = Constraint(self.__model__.I, 
-                                                        rule=self.__lipschitz_rule(), 
-                                                        doc='Lipschitz norm')
+            self.__model__.lipschitz_norm = Constraint(self.__model__.I,
+                                                       rule=self.__lipschitz_rule(),
+                                                       doc='Lipschitz norm')
         else:
             raise ValueError('Penalty must be 1, 2, or 3.')
-                
+
     def __new_objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return self.tau * sum(model.epsilon_plus[i] for i in model.I) \
-                   + (1 - self.tau) * sum(model.epsilon_minus[i] for i in model.I) \
-                   + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
+                + (1 - self.tau) * sum(model.epsilon_minus[i] for i in model.I) \
+                + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
 
         return objective_rule
 
     def __new_objective_rule2(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return self.tau * sum(model.epsilon_plus[i] for i in model.I) \
-                   + (1 - self.tau) * sum(model.epsilon_minus[i] for i in model.I) \
-                   + self.eta * sum(model.beta[ij] ** 2 for ij in model.I * model.J)
+                + (1 - self.tau) * sum(model.epsilon_minus[i] for i in model.I) \
+                + self.eta * sum(model.beta[ij] **
+                                 2 for ij in model.I * model.J)
 
         return objective_rule
 
     def __lipschitz_rule(self):
         """Lipschitz norm"""
-        
+
         def lipschitz_rule(model, i):
             return sum(model.beta[i, j] ** 2 for j in model.J) <= self.eta**2
-    
+
         return lipschitz_rule
-        
+
 
 class pCER(CQER.CER):
     """Penalized convex expectile regression (pCER)
     """
 
     def __init__(self, y, x, tau, eta, z=None, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS, penalty=1):
         """pCER model
@@ -89,50 +90,51 @@
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
             penalty (int, optional): penalty=1 (L1 norm), penalty=2 (L2 norm), and penalty=3 (Lipschitz norm). Defaults to 1.
         """
         self.eta = eta
         CQER.CER.__init__(self, y, x, tau, z, cet, fun, rts)
         if penalty == 1 or penalty == 2:
             self.__model__.squared_objective.deactivate()
-        
+
         if penalty == 1:
             self.__model__.new_objective = Objective(rule=self.__new_squared_objective_rule(),
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 2:
             self.__model__.new_objective = Objective(rule=self.__new_squared_objective_rule2(),
                                                      sense=minimize,
                                                      doc='objective function')
         elif penalty == 3:
-            self.__model__.lipschitz_norm = Constraint(self.__model__.I, 
-                                                        rule=self.__lipschitz_rule(), 
-                                                        doc='Lipschitz norm')
+            self.__model__.lipschitz_norm = Constraint(self.__model__.I,
+                                                       rule=self.__lipschitz_rule(),
+                                                       doc='Lipschitz norm')
         else:
             raise ValueError('Penalty must be 1, 2, or 3.')
-        
+
     def __new_squared_objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return self.tau * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                   + (1 - self.tau) * sum(model.epsilon_minus[i] ** 2 for i in model.I) \
-                   + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
+                + (1 - self.tau) * sum(model.epsilon_minus[i] ** 2 for i in model.I) \
+                + self.eta * sum(model.beta[ij] for ij in model.I * model.J)
 
         return objective_rule
 
     def __new_squared_objective_rule2(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
             return self.tau * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                   + (1 - self.tau) * sum(model.epsilon_minus[i] ** 2 for i in model.I) \
-                   + self.eta * sum(model.beta[ij] ** 2 for ij in model.I * model.J)
+                + (1 - self.tau) * sum(model.epsilon_minus[i] ** 2 for i in model.I) \
+                + self.eta * sum(model.beta[ij] **
+                                 2 for ij in model.I * model.J)
 
         return objective_rule
 
     def __lipschitz_rule(self):
         """Lipschitz norm"""
-        
+
         def lipschitz_rule(model, i):
             return sum(model.beta[i, j] ** 2 for j in model.J) <= self.eta**2
-    
+
         return lipschitz_rule
```

### Comparing `pystoned-0.6.4/pystoned/pICQER.py` & `pystoned-0.6.5/pystoned/pICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/plot.py` & `pystoned-0.6.5/pystoned/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         for j in range(len(XX)):
             ZZ[i, j] = interpolation.interpolation(alpha, beta,
                                                    x=np.array(
                                                        [XX[i, j], YY[i, j]], ndmin=2),
                                                    fun=model.fun)
 
     ax.plot_surface(XX, YY, ZZ, rstride=1, cstride=1, cmap='viridis',
-                         edgecolor='none', alpha=0.5)
+                    edgecolor='none', alpha=0.5)
 
     # add x, y, z label
     ax.set_xlabel("Input $x1$")
     ax.set_ylabel("Input $x2$")
     ax.set_zlabel("Output $y$", rotation=0)
 
     if fig_name == None:
```

### Comparing `pystoned-0.6.4/pystoned/sCQER.py` & `pystoned-0.6.5/pystoned/sCQER.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import dependencies
 from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint
 import numpy as np
 import pandas as pd
 
-from .constant import CET_ADDI,  OPT_LOCAL, OPT_DEFAULT
+from .constant import CET_ADDI, OPT_LOCAL, OPT_DEFAULT
 from .utils import tools
 
 
 class sCQR:
     """Simultaneous estimation of CQR
     """
 
@@ -17,49 +17,53 @@
         Args:
             y (float): output variable. 
             x (float): input variables.
             tau: vector of quantile.
             C: interval (small positive value)
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.y, self.x = tools.to_1d_list(tools.trans_list(y)), tools.to_2d_list(tools.trans_list(x))
+        self.y, self.x = tools.to_1d_list(tools.trans_list(
+            y)), tools.to_2d_list(tools.trans_list(x))
         self.tau = tools.to_1d_list(tools.trans_list(tau))
-        self.C = C
-        self.cet = CET_ADDI
+        self.C, self.cet = C, CET_ADDI
 
         # Initialize the CQR model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
         self.__model__.J = Set(initialize=range(len(self.x[0])))
         self.__model__.K = Set(initialize=range(len(self.tau)))
         self.__model__.W = Set(initialize=range(len(self.tau)-1))
 
         # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.K, self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.K, self.__model__.I, self.__model__.J, bounds=(0.0, None), doc='beta')
-        self.__model__.epsilon_plus = Var(self.__model__.K, self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(self.__model__.K, self.__model__.I, bounds=(0.0, None), doc='negative error term')
-        
+        self.__model__.alpha = Var(
+            self.__model__.K, self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(
+            self.__model__.K, self.__model__.I, self.__model__.J, bounds=(0.0, None), doc='beta')
+        self.__model__.epsilon_plus = Var(self.__model__.K, self.__model__.I, bounds=(
+            0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(self.__model__.K, self.__model__.I, bounds=(
+            0.0, None), doc='negative error term')
+
         # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(), sense=minimize, doc='objective function')
+        self.__model__.objective = Objective(
+            rule=self.__objective_rule(), sense=minimize, doc='objective function')
 
         self.__model__.regression_rule = Constraint(self.__model__.K, self.__model__.I, rule=self.__regression_rule(),
-                                                     doc='regression equation')
-        
+                                                    doc='regression equation')
+
         self.__model__.afriat_rule = Constraint(self.__model__.K, self.__model__.I, self.__model__.I, rule=self.__afriat_rule(),
-                                                 doc='afriat inequality')
+                                                doc='afriat inequality')
 
         self.__model__.noncrossing_rule = Constraint(self.__model__.W, self.__model__.I, rule=self.__noncrossing_rule(),
                                                      doc='non-crossing constraint')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
@@ -68,94 +72,100 @@
         self.problem_status, self.optimization_status = tools.optimize_model(
             self.__model__, email, self.cet, solver)
 
     def __objective_rule(self):
         """Return the proper objective function"""
 
         def objective_rule(model):
-            return sum(self.tau[k] * sum(model.epsilon_plus[k, i] for i in model.I) \
-                   + (1 - self.tau[k]) * sum(model.epsilon_minus[k, i] for i in model.I) for k in model.K)
+            return sum(self.tau[k] * sum(model.epsilon_plus[k, i] for i in model.I)
+                       + (1 - self.tau[k]) * sum(model.epsilon_minus[k, i] for i in model.I) for k in model.K)
 
         return objective_rule
 
     def __regression_rule(self):
         """Return the proper regression constraint"""
 
         def regression_rule(model, k, i):
             return self.y[i] == model.alpha[k, i] + sum(model.beta[k, i, j] * self.x[i][j] for j in model.J) + \
-                   model.epsilon_plus[k, i] - model.epsilon_minus[k, i]
+                model.epsilon_plus[k, i] - model.epsilon_minus[k, i]
 
         return regression_rule
 
     def __afriat_rule(self):
         """Return the proper afriat inequality constraint"""
 
         def afriat_rule(model, k, i, h):
             if i == h:
                 return Constraint.Skip
             return model.alpha[k, i] + sum(model.beta[k, i, j] * self.x[i][j] for j in model.J) \
-                    <= model.alpha[k, h] + sum(model.beta[k, h, j] * self.x[i][j] for j in model.J)
+                <= model.alpha[k, h] + sum(model.beta[k, h, j] * self.x[i][j] for j in model.J)
 
         return afriat_rule
 
     def __noncrossing_rule(self):
         """Return the proper non-crossing constraint"""
 
         def noncrossing_rule(model, w, i):
             return model.alpha[w, i] + sum(model.beta[w, i, j] * self.x[i][j] for j in model.J) + self.C <= \
-                        model.alpha[w+1, i] + sum(model.beta[w+1, i, j] * self.x[i][j] for j in model.J) 
+                model.alpha[w+1, i] + \
+                sum(model.beta[w+1, i, j] * self.x[i][j] for j in model.J)
 
         return noncrossing_rule
 
     def get_alpha(self):
         """Return alpha value by array"""
         tools.assert_optimized(self.optimization_status)
         alpha = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.alpha),
-                                                          list(self.__model__.alpha[:, :].value))])
+                                                           list(self.__model__.alpha[:, :].value))])
         alpha = pd.DataFrame(alpha, columns=['Name', 'Key', 'Value'])
         alpha = alpha.pivot(index='Name', columns='Key', values='Value')
         return alpha.to_numpy().T
 
     def get_beta(self):
         """Return beta value by array"""
         tools.assert_optimized(self.optimization_status)
         beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
                                                           list(self.__model__.beta[:, :, :].value))])
         beta = pd.DataFrame(beta, columns=['tau', 'n', 'd', 'beta'])
         betanew = []
         for i in range(len(self.tau)):
             beta_new = beta.loc[beta['tau'] == i]
             del beta_new["tau"]
-            betanew.append(beta_new.pivot(index='n', columns='d', values='beta').to_numpy())
+            betanew.append(beta_new.pivot(
+                index='n', columns='d', values='beta').to_numpy())
         return np.array(betanew).reshape(len(self.tau)*len(self.y), len(self.x[0]))
 
     def get_positive_residual(self):
         """Return positive residual value by array"""
         tools.assert_optimized(self.optimization_status)
         residual_plus = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.epsilon_plus),
-                                                          list(self.__model__.epsilon_plus[:, :].value))])
-        residual_plus = pd.DataFrame(residual_plus, columns=['Name', 'Key', 'Value'])
-        residual_plus = residual_plus.pivot(index='Name', columns='Key', values='Value')
+                                                                   list(self.__model__.epsilon_plus[:, :].value))])
+        residual_plus = pd.DataFrame(residual_plus, columns=[
+                                     'Name', 'Key', 'Value'])
+        residual_plus = residual_plus.pivot(
+            index='Name', columns='Key', values='Value')
         return residual_plus.to_numpy().T
 
     def get_negative_residual(self):
         """Return negative residual value by array"""
         tools.assert_optimized(self.optimization_status)
         residual_minus = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.epsilon_minus),
-                                                          list(self.__model__.epsilon_minus[:, :].value))])
-        residual_minus = pd.DataFrame(residual_minus, columns=['Name', 'Key', 'Value'])
-        residual_minus = residual_minus.pivot(index='Name', columns='Key', values='Value')
+                                                                    list(self.__model__.epsilon_minus[:, :].value))])
+        residual_minus = pd.DataFrame(residual_minus, columns=[
+                                      'Name', 'Key', 'Value'])
+        residual_minus = residual_minus.pivot(
+            index='Name', columns='Key', values='Value')
         return residual_minus.to_numpy().T
 
     def get_frontier(self):
         """Return estimated frontier value by array"""
         tools.assert_optimized(self.optimization_status)
         frontier = np.tile(np.asarray(self.y).reshape(len(self.y), 1), len(self.tau)) \
-                    - (self.get_positive_residual() - self.get_negative_residual()) 
-        return np.asarray(frontier)       
+            - (self.get_positive_residual() - self.get_negative_residual())
+        return np.asarray(frontier)
 
 
 class sCER(sCQR):
     """Simultaneous estimation of CER
     """
 
     def __init__(self, y, x, tau, C):
@@ -170,11 +180,11 @@
         super().__init__(y, x, tau, C)
         self.__model__.objective.deactivate()
         self.__model__.squared_objective = Objective(
             rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
 
     def __squared_objective_rule(self):
         def squared_objective_rule(model):
-            return sum(self.tau[k] * sum(model.epsilon_plus[k, i] **2 for i in model.I) \
-                   + (1 - self.tau[k]) * sum(model.epsilon_minus[k, i] **2 for i in model.I) for k in model.K)
+            return sum(self.tau[k] * sum(model.epsilon_plus[k, i] ** 2 for i in model.I)
+                       + (1 - self.tau[k]) * sum(model.epsilon_minus[k, i] ** 2 for i in model.I) for k in model.K)
 
-        return squared_objective_rule
+        return squared_objective_rule
```

### Comparing `pystoned-0.6.4/pystoned/utils/CNLSG1.py` & `pystoned-0.6.5/pystoned/utils/CNLSG1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,15 @@
             x (float): input variables.
             cutactive (float): active concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.cet, self.fun, self.rts = x, y, cet, fun, rts
         self.cutactive = cutactive
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
@@ -65,16 +60,15 @@
                                                 doc='elementary Afriat approach')
         self.__model__.sweet_rule = Constraint(self.__model__.I,
                                                self.__model__.I,
                                                rule=self.__sweet_rule(),
                                                doc='sweet spot approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CNLSG2.py` & `pystoned-0.6.5/pystoned/utils/CNLSG2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,15 @@
             cutactive (float): active concavity constraint.
             active (float): violated concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.cet, self.fun, self.rts = x, y, cet, fun, rts
         self.cutactive = cutactive
         self.active = to_2d_list(trans_list(active))
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
@@ -71,16 +66,15 @@
                                                doc='sweet spot approach')
         self.__model__.sweet_rule2 = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__sweet_rule2(),
                                                 doc='sweet spot-2 approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CNLSZG1.py` & `pystoned-0.6.5/pystoned/utils/CNLSZG1.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,15 @@
             z (float, optional): Contextual variable(s). Defaults to None.
             cutactive (float): active concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.z, self.cet, self.fun, self.rts = x, y, z, cet, fun, rts
         self.cutactive = cutactive
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
@@ -69,16 +63,15 @@
                                                 doc='elementary Afriat approach')
         self.__model__.sweet_rule = Constraint(self.__model__.I,
                                                self.__model__.I,
                                                rule=self.__sweet_rule(),
                                                doc='sweet spot approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CNLSZG2.py` & `pystoned-0.6.5/pystoned/utils/CNLSZG2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,15 @@
             cutactive (float): active concavity constraint.
             active (float): violated concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.z, self.cet, self.fun, self.rts = x, y, z, cet, fun, rts
         self.cutactive = cutactive
         self.active = to_2d_list(trans_list(active))
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
@@ -75,16 +69,15 @@
                                                doc='sweet spot approach')
         self.__model__.sweet_rule2 = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__sweet_rule2(),
                                                 doc='sweet spot-2 approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CQERG1.py` & `pystoned-0.6.5/pystoned/utils/CQERG1.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,15 @@
             tau (float): quantile.
             cutactive (float): active concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.tau, self.cet, self.fun, self.rts = x, y, tau, cet, fun, rts
         self.cutactive = cutactive
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
@@ -74,16 +68,15 @@
                                                 doc='elementary Afriat approach')
         self.__model__.sweet_rule = Constraint(self.__model__.I,
                                                self.__model__.I,
                                                rule=self.__sweet_rule(),
                                                doc='sweet spot approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CQERG2.py` & `pystoned-0.6.5/pystoned/utils/CQERG2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,15 @@
             cutactive (float): active concavity constraint.
             active (float): violated concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.tau, self.cet, self.fun, self.rts = x, y, tau, cet, fun, rts
         self.cutactive = cutactive
         self.active = to_2d_list(trans_list(active))
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
@@ -80,16 +74,15 @@
                                                doc='sweet spot approach')
         self.__model__.sweet_rule2 = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__sweet_rule2(),
                                                 doc='sweet spot-2 approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CQERZG1.py` & `pystoned-0.6.5/pystoned/utils/CQERZG1.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,15 @@
             tau (float): quantile.
             cutactive (float): active concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.z, self.tau, self.cet, self.fun, self.rts = x, y, z, tau, cet, fun, rts
         self.cutactive = cutactive
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=range(len(self.y)))
@@ -78,16 +71,15 @@
                                                 doc='elementary Afriat approach')
         self.__model__.sweet_rule = Constraint(self.__model__.I,
                                                self.__model__.I,
                                                rule=self.__sweet_rule(),
                                                doc='sweet spot approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/CQERZG2.py` & `pystoned-0.6.5/pystoned/utils/CQERZG2.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,15 @@
             cutactive (float): active concavity constraint.
             active (float): violated concavity constraint.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
+        self.x, self.y, self.z, self.tau, self.cet, self.fun, self.rts = x, y, z, tau, cet, fun, rts
         self.cutactive = cutactive
         self.active = to_2d_list(trans_list(active))
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
@@ -84,16 +77,15 @@
                                                doc='sweet spot approach')
         self.__model__.sweet_rule2 = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__sweet_rule2(),
                                                 doc='sweet spot-2 approach')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
```

### Comparing `pystoned-0.6.4/pystoned/utils/interpolation.py` & `pystoned-0.6.5/pystoned/utils/interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         x (float): input variables.
         fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
 
     Returns:
         yat: interpolated frontier
     """
     x = np.array(to_2d_list(trans_list(x)))
-    n = len(x)
-    d = len(x[0])
+    n, d = len(x), len(x[0])
 
     if len(beta[0]) != d:
         raise ValueError(
             "The dimensions of x_test must be equal to those of x.")
 
     if fun == FUN_PROD:
         def fun_est(x):
```

### Comparing `pystoned-0.6.4/pystoned/utils/sweet.py` & `pystoned-0.6.5/pystoned/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/pystoned/utils/tools.py` & `pystoned-0.6.5/pystoned/utils/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,17 +276,17 @@
 
     y_shape = np.asarray(y).shape
     x_shape = np.asarray(x).shape
 
     if y_shape[0] != x_shape[0]:
         raise ValueError(
             "Number of DMUs must be the same in x and y.")
-    
+
     if type(z) != type(None):
         z = trans_list(z)
         z = to_2d_list(z)
         z_shape = np.asarray(z).shape
         if y_shape[0] != z_shape[0]:
             raise ValueError(
                 "Number of DMUs must be the same in y and z.")
-        
-    return y, x, z
+
+    return y, x, z
```

### Comparing `pystoned-0.6.4/pystoned/wCNLS.py` & `pystoned-0.6.5/pystoned/wCNLS.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,13 @@
         # TODO(error/warning handling): Check the configuration of the model exist
         super().__init__(y, x, z, cet, fun, rts)
         self.w = tools.trans_list(tools.to_1d_list(w))
 
         self.__model__.objective.deactivate()
         self.__model__.weighted_objective = Objective(
             rule=self.__weighted_objective_rule(), sense=minimize, doc='weighted objective rule')
-        
-        
+
     def __weighted_objective_rule(self):
         def weighted_objective_rule(model):
             return sum(self.w[i] * model.epsilon[i] ** 2 for i in model.I)
 
         return weighted_objective_rule
-
```

### Comparing `pystoned-0.6.4/pystoned/wCQER.py` & `pystoned-0.6.5/pystoned/wCQER.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         self.__model__.objective.deactivate()
         self.__model__.weighted_objective = Objective(
             rule=self.__weighted_objective_rule(), sense=minimize, doc='weighted objective rule')
 
     def __weighted_objective_rule(self):
         def weighted_objective_rule(model):
             return self.tau * sum(self.w[i] * model.epsilon_plus[i] for i in model.I) \
-                + (1 - self.tau) * sum(self.w[i] * model.epsilon_minus[i] for i in model.I)
+                + (1 - self.tau) * \
+                sum(self.w[i] * model.epsilon_minus[i] for i in model.I)
 
         return weighted_objective_rule
 
 
 class wCER(CQER.CQR):
     """Weighted Convex Expectile Regression (wCER)
     """
```

### Comparing `pystoned-0.6.4/pystoned/weakCNLS.py` & `pystoned-0.6.5/pystoned/weakCNLS.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,15 @@
             z (float, optional): Contextual variable(s). Defaults to None.
             cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
         # TODO(error/warning handling): Check the configuration of the model exist
         self.y, self.x, self.b, self.z = tools.assert_valid_wp_data(y, x, b, z)
-
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
+        self.cet, self.fun, self.rts = cet, fun, rts
 
         # Initialize the CNLS model
         self.__model__ = ConcreteModel()
 
         if type(self.z) != type(None):
             # Initialize the set of z
             self.__model__.K = Set(initialize=range(len(self.z[0])))
@@ -49,17 +46,17 @@
 
         # Initialize the variables
         self.__model__.alpha = Var(self.__model__.I, doc='alpha')
         self.__model__.beta = Var(self.__model__.I,
                                   self.__model__.J,
                                   bounds=(0.0, None),
                                   doc='beta')
-        self.__model__.delta = Var(self.__model__.I, 
-                                   self.__model__.L, 
-                                   bounds=(0.0, None), 
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
                                    doc='delta')
         self.__model__.epsilon = Var(self.__model__.I, doc='residual')
         self.__model__.frontier = Var(self.__model__.I,
                                       bounds=(0.0, None),
                                       doc='estimated frontier')
 
         # Setup the objective function and constraints
@@ -74,21 +71,20 @@
                                                  rule=self.__log_rule(),
                                                  doc='log-transformed regression equation')
         self.__model__.afriat_rule = Constraint(self.__model__.I,
                                                 self.__model__.I,
                                                 rule=self.__afriat_rule(),
                                                 doc='afriat inequality')
         self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='weak disposibility')
+                                                       self.__model__.I,
+                                                       rule=self.__disposability_rule(),
+                                                       doc='weak disposibility')
 
         # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+        self.optimization_status, self.problem_status = 0, 0
 
     def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
@@ -100,49 +96,51 @@
     def __regression_rule(self):
         """Return the proper regression constraint"""
         if self.cet == CET_ADDI:
             if self.rts == RTS_VRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
                         return self.y[i] == model.alpha[i] \
-                                + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                                + model.epsilon[i]
+                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                            + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                            + model.epsilon[i]
 
                     return regression_rule
 
                 def regression_rule(model, i):
                     return self.y[i] == model.alpha[i] \
-                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                            + model.epsilon[i]
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon[i]
 
                 return regression_rule
             elif self.rts == RTS_CRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
                         return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                + sum(model.lamda[k] * self.z[i][k] for k in model.K) + model.epsilon[i]
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                            + sum(model.lamda[k] * self.z[i][k]
+                                  for k in model.K) + model.epsilon[i]
 
                     return regression_rule
 
                 def regression_rule(model, i):
                     return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                            + model.epsilon[i]
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon[i]
 
                 return regression_rule
 
         elif self.cet == CET_MULT:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
                     return log(self.y[i]) == log(model.frontier[i] + 1) \
-                            + sum(model.lamda[k] * self.z[i][k] for k in model.K) + model.epsilon[i]
+                        + sum(model.lamda[k] * self.z[i][k]
+                              for k in model.K) + model.epsilon[i]
 
                 return regression_rule
 
             def regression_rule(model, i):
                 return log(self.y[i]) == log(model.frontier[i] + 1) + model.epsilon[i]
 
             return regression_rule
@@ -153,23 +151,25 @@
         """Return the proper log constraint"""
         if self.cet == CET_MULT:
             if self.rts == RTS_VRS:
 
                 def log_rule(model, i):
                     return model.frontier[i] == model.alpha[i] + sum(
                         model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L) - 1
 
                 return log_rule
             elif self.rts == RTS_CRS:
 
                 def log_rule(model, i):
                     return model.frontier[i] == sum(
                         model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L) - 1
 
                 return log_rule
 
         raise ValueError("Undefined model parameters.")
 
     def __afriat_rule(self):
         """Return the proper afriat inequality constraint"""
@@ -181,77 +181,85 @@
         if self.cet == CET_ADDI:
             if self.rts == RTS_VRS:
 
                 def afriat_rule(model, i, h):
                     if i == h:
                         return Constraint.Skip
                     return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j] for j in model.J)
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                        model.alpha[h] + sum(model.beta[h, j] * self.x[i][j] for j in model.J)
-                            + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                        model.alpha[i] + sum(model.beta[i, j]
+                                             * self.x[i][j] for j in model.J)
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L),
+                        model.alpha[h] + sum(model.beta[h, j]
+                                             * self.x[i][j] for j in model.J)
+                        + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
 
                 return afriat_rule
             elif self.rts == RTS_CRS:
 
                 def afriat_rule(model, i, h):
                     if i == h:
                         return Constraint.Skip
                     return __operator(
-                        sum(model.beta[i, j] * self.x[i][j] for j in model.J) 
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                        sum(model.beta[i, j] * self.x[i][j] for j in model.J)
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L),
                         sum(model.beta[h, j] * self.x[i][j] for j in model.J)
-                            + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
+                        + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
 
                 return afriat_rule
         elif self.cet == CET_MULT:
             if self.rts == RTS_VRS:
 
                 def afriat_rule(model, i, h):
                     if i == h:
                         return Constraint.Skip
                     return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j] for j in model.J)
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                        model.alpha[h] + sum(model.beta[h, j] * self.x[i][j] for j in model.J)
-                            + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                        model.alpha[i] + sum(model.beta[i, j]
+                                             * self.x[i][j] for j in model.J)
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L),
+                        model.alpha[h] + sum(model.beta[h, j]
+                                             * self.x[i][j] for j in model.J)
+                        + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
 
                 return afriat_rule
             elif self.rts == RTS_CRS:
 
                 def afriat_rule(model, i, h):
                     if i == h:
                         return Constraint.Skip
                     return __operator(
-                        sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                        sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
+                        sum(model.beta[i, j] * self.x[i][j] for j in model.J)
+                        + sum(model.delta[i, l] * self.b[i][l]
+                              for l in model.L),
+                        sum(model.beta[h, j] * self.x[i][j] for j in model.J)
+                        + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
 
                 return afriat_rule
 
         raise ValueError("Undefined model parameters.")
 
     def __disposability_rule(self):
         """Return the proper weak disposability constraint"""
         def disposability_rule(model, i, h):
             if i == h:
                 return Constraint.Skip
             return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-        
+
         return disposability_rule
-        
+
     def display_delta(self):
         """Display delta value"""
         tools.assert_optimized(self.optimization_status)
         tools.assert_undesirable_output(self.b)
         self.__model__.delta.display()
 
     def get_delta(self):
         """Return delta value by array"""
         tools.assert_optimized(self.optimization_status)
         tools.assert_undesirable_output(self.b)
         delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
                                                            list(self.__model__.delta[:, :].value))])
         delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
         delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
+        return delta.to_numpy()
```

### Comparing `pystoned-0.6.4/pystoned.egg-info/PKG-INFO` & `pystoned-0.6.5/pystoned.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.4/pystoned.egg-info/SOURCES.txt` & `pystoned-0.6.5/pystoned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.4/setup.py` & `pystoned-0.6.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pystoned',
-    version='0.6.4',
+    version='0.6.5',
     description='A Python Package for Convex Regression and Frontier Estimation',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPLv3',
     packages=find_packages(),
     author='Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen',
     author_email='sheng.dai@utu.fi',
```

