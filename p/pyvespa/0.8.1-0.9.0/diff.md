# Comparing `tmp/pyvespa-0.8.1.tar.gz` & `tmp/pyvespa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyvespa-0.8.1.tar", last modified: Fri Aug 27 12:02:46 2021, max compression
+gzip compressed data, was "dist/pyvespa-0.9.0.tar", last modified: Mon Aug 30 08:42:00 2021, max compression
```

## Comparing `pyvespa-0.8.1.tar` & `pyvespa-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-27 12:02:46.000000 pyvespa-0.8.1/
--rw-r--r--   0 tmartins01   (501) staff       (20)       50 2020-09-09 09:21:50.000000 pyvespa-0.8.1/MANIFEST.in
--rw-r--r--   0 tmartins01   (501) staff       (20)      394 2021-08-27 12:02:46.000000 pyvespa-0.8.1/PKG-INFO
--rw-r--r--   0 tmartins01   (501) staff       (20)      765 2021-06-21 11:26:05.000000 pyvespa-0.8.1/README.md
-drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/
--rw-r--r--   0 tmartins01   (501) staff       (20)      394 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/PKG-INFO
--rw-r--r--   0 tmartins01   (501) staff       (20)      773 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/SOURCES.txt
--rw-r--r--   0 tmartins01   (501) staff       (20)        1 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/dependency_links.txt
--rw-r--r--   0 tmartins01   (501) staff       (20)        1 2020-09-09 11:41:54.000000 pyvespa-0.8.1/pyvespa.egg-info/not-zip-safe
--rw-r--r--   0 tmartins01   (501) staff       (20)      124 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/requires.txt
--rw-r--r--   0 tmartins01   (501) staff       (20)        6 2021-08-27 12:02:46.000000 pyvespa-0.8.1/pyvespa.egg-info/top_level.txt
--rw-r--r--   0 tmartins01   (501) staff       (20)       38 2021-08-27 12:02:46.000000 pyvespa-0.8.1/setup.cfg
--rw-r--r--   0 tmartins01   (501) staff       (20)     1329 2021-08-27 12:01:23.000000 pyvespa-0.8.1/setup.py
-drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-27 12:02:46.000000 pyvespa-0.8.1/vespa/
--rw-r--r--   0 tmartins01   (501) staff       (20)      135 2020-09-09 09:21:50.000000 pyvespa-0.8.1/vespa/__init__.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    42193 2021-08-25 16:19:17.000000 pyvespa-0.8.1/vespa/application.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    26430 2021-08-27 10:22:28.000000 pyvespa-0.8.1/vespa/deployment.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     8179 2021-08-20 17:08:40.000000 pyvespa-0.8.1/vespa/evaluation.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     3101 2021-06-21 11:26:05.000000 pyvespa-0.8.1/vespa/gallery.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     2786 2021-08-13 14:00:43.000000 pyvespa-0.8.1/vespa/io.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     2424 2021-06-01 11:15:08.000000 pyvespa-0.8.1/vespa/json_serialization.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    10976 2021-08-25 16:19:17.000000 pyvespa-0.8.1/vespa/ml.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    79142 2021-08-27 10:22:28.000000 pyvespa-0.8.1/vespa/package.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     8455 2021-06-15 09:12:28.000000 pyvespa-0.8.1/vespa/query.py
-drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-27 12:02:46.000000 pyvespa-0.8.1/vespa/templates/
--rw-r--r--   0 tmartins01   (501) staff       (20)      244 2020-09-09 09:21:50.000000 pyvespa-0.8.1/vespa/templates/hosts.xml
--rw-r--r--   0 tmartins01   (501) staff       (20)      157 2021-08-25 16:19:17.000000 pyvespa-0.8.1/vespa/templates/query_profile.xml
--rw-r--r--   0 tmartins01   (501) staff       (20)      153 2021-08-25 16:19:17.000000 pyvespa-0.8.1/vespa/templates/query_profile_type.xml
--rw-r--r--   0 tmartins01   (501) staff       (20)     3149 2021-06-01 11:15:08.000000 pyvespa-0.8.1/vespa/templates/schema.txt
--rw-r--r--   0 tmartins01   (501) staff       (20)      799 2021-08-25 16:19:17.000000 pyvespa-0.8.1/vespa/templates/services.xml
--rw-r--r--   0 tmartins01   (501) staff       (20)    18509 2021-08-20 17:08:40.000000 pyvespa-0.8.1/vespa/test_application.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    23776 2021-08-20 17:08:40.000000 pyvespa-0.8.1/vespa/test_evaluation.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    43494 2021-08-27 10:22:28.000000 pyvespa-0.8.1/vespa/test_integration_docker.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     6872 2021-08-17 13:11:04.000000 pyvespa-0.8.1/vespa/test_integration_running_instance.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    11518 2021-08-27 10:22:28.000000 pyvespa-0.8.1/vespa/test_integration_vespa_cloud.py
--rw-r--r--   0 tmartins01   (501) staff       (20)     5182 2021-06-01 11:15:08.000000 pyvespa-0.8.1/vespa/test_ml.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    62331 2021-08-26 12:58:09.000000 pyvespa-0.8.1/vespa/test_package.py
--rw-r--r--   0 tmartins01   (501) staff       (20)    14188 2021-08-20 17:08:40.000000 pyvespa-0.8.1/vespa/test_query.py
+drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-30 08:42:00.000000 pyvespa-0.9.0/
+-rw-r--r--   0 tmartins01   (501) staff       (20)       50 2020-09-09 09:21:50.000000 pyvespa-0.9.0/MANIFEST.in
+-rw-r--r--   0 tmartins01   (501) staff       (20)      394 2021-08-30 08:42:00.000000 pyvespa-0.9.0/PKG-INFO
+-rw-r--r--   0 tmartins01   (501) staff       (20)      765 2021-06-21 11:26:05.000000 pyvespa-0.9.0/README.md
+drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/
+-rw-r--r--   0 tmartins01   (501) staff       (20)      394 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/PKG-INFO
+-rw-r--r--   0 tmartins01   (501) staff       (20)      773 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/SOURCES.txt
+-rw-r--r--   0 tmartins01   (501) staff       (20)        1 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/dependency_links.txt
+-rw-r--r--   0 tmartins01   (501) staff       (20)        1 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/not-zip-safe
+-rw-r--r--   0 tmartins01   (501) staff       (20)      124 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/requires.txt
+-rw-r--r--   0 tmartins01   (501) staff       (20)        6 2021-08-30 08:42:00.000000 pyvespa-0.9.0/pyvespa.egg-info/top_level.txt
+-rw-r--r--   0 tmartins01   (501) staff       (20)       38 2021-08-30 08:42:00.000000 pyvespa-0.9.0/setup.cfg
+-rw-r--r--   0 tmartins01   (501) staff       (20)     1329 2021-08-30 08:41:17.000000 pyvespa-0.9.0/setup.py
+drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-30 08:42:00.000000 pyvespa-0.9.0/vespa/
+-rw-r--r--   0 tmartins01   (501) staff       (20)      135 2020-09-09 09:21:50.000000 pyvespa-0.9.0/vespa/__init__.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    42193 2021-08-25 16:19:17.000000 pyvespa-0.9.0/vespa/application.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    26430 2021-08-27 10:22:28.000000 pyvespa-0.9.0/vespa/deployment.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     8179 2021-08-20 17:08:40.000000 pyvespa-0.9.0/vespa/evaluation.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     3101 2021-06-21 11:26:05.000000 pyvespa-0.9.0/vespa/gallery.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     2786 2021-08-13 14:00:43.000000 pyvespa-0.9.0/vespa/io.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     2424 2021-06-01 11:15:08.000000 pyvespa-0.9.0/vespa/json_serialization.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    10976 2021-08-25 16:19:17.000000 pyvespa-0.9.0/vespa/ml.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    52901 2021-08-30 08:39:29.000000 pyvespa-0.9.0/vespa/package.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     8455 2021-06-15 09:12:28.000000 pyvespa-0.9.0/vespa/query.py
+drwxr-xr-x   0 tmartins01   (501) staff       (20)        0 2021-08-30 08:42:00.000000 pyvespa-0.9.0/vespa/templates/
+-rw-r--r--   0 tmartins01   (501) staff       (20)      244 2020-09-09 09:21:50.000000 pyvespa-0.9.0/vespa/templates/hosts.xml
+-rw-r--r--   0 tmartins01   (501) staff       (20)      157 2021-08-25 16:19:17.000000 pyvespa-0.9.0/vespa/templates/query_profile.xml
+-rw-r--r--   0 tmartins01   (501) staff       (20)      153 2021-08-25 16:19:17.000000 pyvespa-0.9.0/vespa/templates/query_profile_type.xml
+-rw-r--r--   0 tmartins01   (501) staff       (20)     3149 2021-06-01 11:15:08.000000 pyvespa-0.9.0/vespa/templates/schema.txt
+-rw-r--r--   0 tmartins01   (501) staff       (20)      799 2021-08-25 16:19:17.000000 pyvespa-0.9.0/vespa/templates/services.xml
+-rw-r--r--   0 tmartins01   (501) staff       (20)    18509 2021-08-20 17:08:40.000000 pyvespa-0.9.0/vespa/test_application.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    23776 2021-08-20 17:08:40.000000 pyvespa-0.9.0/vespa/test_evaluation.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    43494 2021-08-27 10:22:28.000000 pyvespa-0.9.0/vespa/test_integration_docker.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     6872 2021-08-17 13:11:04.000000 pyvespa-0.9.0/vespa/test_integration_running_instance.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    11518 2021-08-27 10:22:28.000000 pyvespa-0.9.0/vespa/test_integration_vespa_cloud.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)     5182 2021-06-01 11:15:08.000000 pyvespa-0.9.0/vespa/test_ml.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    62331 2021-08-26 12:58:09.000000 pyvespa-0.9.0/vespa/test_package.py
+-rw-r--r--   0 tmartins01   (501) staff       (20)    14188 2021-08-20 17:08:40.000000 pyvespa-0.9.0/vespa/test_query.py
```

### Comparing `pyvespa-0.8.1/README.md` & `pyvespa-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/pyvespa.egg-info/SOURCES.txt` & `pyvespa-0.9.0/pyvespa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/setup.py` & `pyvespa-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return "{}.{}".format(pyvespa_version, build_nr)
 
 
 min_python = "3.6"
 
 setuptools.setup(
     name="pyvespa",
-    version="0.8.1",
+    version="0.9.0",
     description="Python API for vespa.ai",
     keywords="vespa, search engine, data science",
     author="Thiago G. Martins",
     author_email="tmartins@verizonmedia.com",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
     ],
```

### Comparing `pyvespa-0.8.1/vespa/application.py` & `pyvespa-0.9.0/vespa/application.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/deployment.py` & `pyvespa-0.9.0/vespa/deployment.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/evaluation.py` & `pyvespa-0.9.0/vespa/evaluation.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/gallery.py` & `pyvespa-0.9.0/vespa/gallery.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/io.py` & `pyvespa-0.9.0/vespa/io.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/json_serialization.py` & `pyvespa-0.9.0/vespa/json_serialization.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/ml.py` & `pyvespa-0.9.0/vespa/ml.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/query.py` & `pyvespa-0.9.0/vespa/query.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/templates/schema.txt` & `pyvespa-0.9.0/vespa/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/templates/services.xml` & `pyvespa-0.9.0/vespa/templates/services.xml`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_application.py` & `pyvespa-0.9.0/vespa/test_application.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_evaluation.py` & `pyvespa-0.9.0/vespa/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_integration_docker.py` & `pyvespa-0.9.0/vespa/test_integration_docker.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_integration_running_instance.py` & `pyvespa-0.9.0/vespa/test_integration_running_instance.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_integration_vespa_cloud.py` & `pyvespa-0.9.0/vespa/test_integration_vespa_cloud.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_ml.py` & `pyvespa-0.9.0/vespa/test_ml.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_package.py` & `pyvespa-0.9.0/vespa/test_package.py`

 * *Files identical despite different names*

### Comparing `pyvespa-0.8.1/vespa/test_query.py` & `pyvespa-0.9.0/vespa/test_query.py`

 * *Files identical despite different names*

