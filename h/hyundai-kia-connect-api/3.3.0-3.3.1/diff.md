# Comparing `tmp/hyundai_kia_connect_api-3.3.0.tar.gz` & `tmp/hyundai_kia_connect_api-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.3.0.tar", last modified: Tue May  2 17:24:19 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.3.1.tar", last modified: Fri May  5 12:57:52 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.3.0.tar` & `hyundai_kia_connect_api-3.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.076946 hyundai_kia_connect_api-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51320 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:24:18.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 17:24:03.000000 hyundai_kia_connect_api-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:52.593471 hyundai_kia_connect_api-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-05 12:57:52.593471 hyundai_kia_connect_api-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:52.585471 hyundai_kia_connect_api-3.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:52.589471 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:52.593471 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 12:57:52.000000 hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 12:57:52.593471 hyundai_kia_connect_api-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 12:57:40.000000 hyundai_kia_connect_api-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:52.593471 hyundai_kia_connect_api-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 12:57:15.000000 hyundai_kia_connect_api-3.3.1/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.3.0/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/LICENSE` & `hyundai_kia_connect_api-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/PKG-INFO` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyundai_kia_connect_api
-Version: 3.3.0
+Name: hyundai-kia-connect-api
+Version: 3.3.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -34,15 +34,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.3.0/README.rst` & `hyundai_kia_connect_api-3.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.3.0/docs/Makefile` & `hyundai_kia_connect_api-3.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/docs/conf.py` & `hyundai_kia_connect_api-3.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/docs/installation.rst` & `hyundai_kia_connect_api-3.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/docs/make.bat` & `hyundai_kia_connect_api-3.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         if response["resCode"] in error_code_mapping:
             raise error_code_mapping[response["resCode"]](response["resMsg"])
         else:
             raise APIError(f"Server returned: '{response['resMsg']}'")
 
 
 class KiaUvoApiCN(ApiImpl):
-    data_timezone = tz.gettz("Asia/ShangHai")
+    data_timezone = tz.gettz("Asia/Shanghai")
     temperature_range = [x * 0.5 for x in range(28, 60)]
 
     def __init__(self, region: int, brand: int, language: str) -> None:
         self.stamps = None
 
         if BRANDS[brand] == BRAND_KIA:
             self.BASE_DOMAIN: str = "prd.cn-ccapi.kia.com"
@@ -288,19 +288,19 @@
             vehicle.last_updated_at = self.get_last_updated_at(
                 get_child_value(state, "status.time")
             )
         else:
             vehicle.last_updated_at = dt.datetime.now(self.data_timezone)
 
         vehicle.odometer = (
-            get_child_value(state, "odometer.value"),
+            get_child_value(state, "status.odometer.value"),
             DISTANCE_UNITS[
                 get_child_value(
                     state,
-                    "odometer.unit",
+                    "status.odometer.unit",
                 )
             ],
         )
         vehicle.car_battery_percentage = get_child_value(state, "status.battery.batSoc")
         vehicle.engine_is_running = get_child_value(state, "status.engine")
 
         # Converts temp to usable number. Currently only support celsius.
@@ -648,28 +648,28 @@
         url = self.SPA_API_URL + "vehicles/" + vehicle.id + "/status/latest"
 
         response = requests.get(
             url, headers=self._get_authenticated_headers(token)
         ).json()
         _LOGGER.debug(f"{DOMAIN} - get_cached_vehicle_status response: {response}")
         _check_response_for_errors(response)
-        response = response["resMsg"]["status"]
+        response = response["resMsg"]
 
         return response
 
     def _get_location(self, token: Token, vehicle: Vehicle) -> dict:
         url = self.SPA_API_URL + "vehicles/" + vehicle.id + "/location"
 
         try:
             response = requests.get(
                 url, headers=self._get_authenticated_headers(token)
             ).json()
             _LOGGER.debug(f"{DOMAIN} - _get_location response: {response}")
             _check_response_for_errors(response)
-            return response["resMsg"]["gpsDetail"]
+            return response["resMsg"]
         except:
             _LOGGER.debug(f"{DOMAIN} - _get_location failed")
             return None
 
     def _get_forced_vehicle_state(self, token: Token, vehicle: Vehicle) -> dict:
         url = self.SPA_API_URL + "vehicles/" + vehicle.id + "/status"
         response = requests.get(
```

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyundai-kia-connect-api
-Version: 3.3.0
+Name: hyundai_kia_connect_api
+Version: 3.3.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -34,15 +34,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.3.1/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/setup.py` & `hyundai_kia_connect_api-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.3.0",
+    version="3.3.1",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.3.0/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.3.1/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.0/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.3.1/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

