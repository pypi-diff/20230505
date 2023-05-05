# Comparing `tmp/aws_cost_optimization-0.3.0.tar.gz` & `tmp/aws_cost_optimization-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cost_optimization-0.3.0.tar", last modified: Tue Apr  4 08:58:49 2023, max compression
+gzip compressed data, was "aws_cost_optimization-0.3.1.tar", last modified: Fri May  5 08:29:10 2023, max compression
```

## Comparing `aws_cost_optimization-0.3.0.tar` & `aws_cost_optimization-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:58:49.622599 aws_cost_optimization-0.3.0/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.0/LICENCE
--rw-rw-rw-   0        0        0      506 2023-04-04 08:58:49.622599 aws_cost_optimization-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      141 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 08:58:49.591332 aws_cost_optimization-0.3.0/aws_cost_optimization/
--rw-rw-rw-   0        0        0     4673 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/__init__.py
--rw-rw-rw-   0        0        0     1440 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_cloudwatch_costing.py
--rw-rw-rw-   0        0        0    11791 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_ec2_costing.py
--rw-rw-rw-   0        0        0     2399 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_elb_costing.py
--rw-rw-rw-   0        0        0     1240 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_kms_costing.py
--rw-rw-rw-   0        0        0     6814 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_rds_costing.py
--rw-rw-rw-   0        0        0     5023 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_ri_recommendations.py
--rw-rw-rw-   0        0        0     5102 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/_savings_plan.py
--rw-rw-rw-   0        0        0     5718 2023-03-29 13:18:38.000000 aws_cost_optimization-0.3.0/aws_cost_optimization/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:58:49.622599 aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/
--rw-rw-rw-   0        0        0      506 2023-04-04 08:58:49.000000 aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-04-04 08:58:49.000000 aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:58:49.000000 aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-04 08:58:49.000000 aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      502 2023-04-04 08:58:19.000000 aws_cost_optimization-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 08:58:49.622599 aws_cost_optimization-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.729882 aws_cost_optimization-0.3.1/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.1/LICENCE
+-rw-rw-rw-   0        0        0      506 2023-05-05 08:29:10.727896 aws_cost_optimization-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.701879 aws_cost_optimization-0.3.1/aws_cost_optimization/
+-rw-rw-rw-   0        0        0     4673 2023-05-05 08:28:27.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/__init__.py
+-rw-rw-rw-   0        0        0     1440 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_cloudwatch_costing.py
+-rw-rw-rw-   0        0        0    11791 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_ec2_costing.py
+-rw-rw-rw-   0        0        0     2399 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_elb_costing.py
+-rw-rw-rw-   0        0        0     1240 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_kms_costing.py
+-rw-rw-rw-   0        0        0     6814 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_rds_costing.py
+-rw-rw-rw-   0        0        0     5023 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_ri_recommendations.py
+-rw-rw-rw-   0        0        0     5102 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_savings_plan.py
+-rw-rw-rw-   0        0        0     5718 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.722880 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      536 2023-05-05 08:28:27.000000 aws_cost_optimization-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:29:10.730884 aws_cost_optimization-0.3.1/setup.cfg
```

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/__init__.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     _cloudwatch_costing, _elb_costing
 from aws_cost_optimization.utils import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = "Dheeraj Banodha"
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 
 class aws_client(_ri_recommendations.ri, _savings_plan.sp, _ec2_costing.ec2, _rds_costing.rds, _kms_costing.kms, _cloudwatch_costing.cw, _elb_costing.elb):
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
```

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_cloudwatch_costing.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_cloudwatch_costing.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_ec2_costing.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_ec2_costing.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_elb_costing.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_elb_costing.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_kms_costing.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_kms_costing.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_rds_costing.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_rds_costing.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_ri_recommendations.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_ri_recommendations.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/_savings_plan.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/_savings_plan.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization/utils.py` & `aws_cost_optimization-0.3.1/aws_cost_optimization/utils.py`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.0/aws_cost_optimization.egg-info/SOURCES.txt` & `aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 aws_cost_optimization/_rds_costing.py
 aws_cost_optimization/_ri_recommendations.py
 aws_cost_optimization/_savings_plan.py
 aws_cost_optimization/utils.py
 aws_cost_optimization.egg-info/PKG-INFO
 aws_cost_optimization.egg-info/SOURCES.txt
 aws_cost_optimization.egg-info/dependency_links.txt
+aws_cost_optimization.egg-info/requires.txt
 aws_cost_optimization.egg-info/top_level.txt
```

