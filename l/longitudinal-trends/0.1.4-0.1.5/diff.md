# Comparing `tmp/longitudinal_trends-0.1.4.tar.gz` & `tmp/longitudinal_trends-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.4.tar", last modified: Fri May  5 12:39:59 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.5.tar", last modified: Fri May  5 12:48:29 2023, max compression
```

## Comparing `longitudinal_trends-0.1.4.tar` & `longitudinal_trends-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.4/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.4/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.4/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.598758 longitudinal_trends-0.1.4/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17387 2023-05-05 11:45:01.000000 longitudinal_trends-0.1.4/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.821368 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-05 12:17:11.000000 longitudinal_trends-0.1.4/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.4/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:48:29.638960 longitudinal_trends-0.1.5/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.5/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.5/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:48:29.638960 longitudinal_trends-0.1.5/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.5/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:48:29.328949 longitudinal_trends-0.1.5/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17391 2023-05-05 12:47:53.000000 longitudinal_trends-0.1.5/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:48:29.576063 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:48:28.000000 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-05 12:48:29.000000 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-05 12:48:28.000000 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-05 12:48:28.000000 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-05 12:48:28.000000 longitudinal_trends-0.1.5/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-05 12:48:06.000000 longitudinal_trends-0.1.5/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.5/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-05 12:48:29.638960 longitudinal_trends-0.1.5/setup.cfg
```

### Comparing `longitudinal_trends-0.1.4/LICENSE` & `longitudinal_trends-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.4/PKG-INFO` & `longitudinal_trends-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `longitudinal_trends-0.1.4/README.md` & `longitudinal_trends-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.4/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.5/longitudinal_trends/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                             quit()
                         else:
                             self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
                             self.__logger.error("[bold red]Don't worry about 'Assertion Error'. [/]", extra={"markup": True})
                             assert False
                         
                     time.sleep(5)
-                    df.to_csv("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.keyword, self.data_format,  form, i, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
+                    df.to_csv("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
 
                     current_time += chng_delta
 
             self.__logger.info("[bold green]Successfully Collected Required Data![/]", extra={"markup": True})
 
 
     # Time Series Data collection method for 'monthly'
```

### Comparing `longitudinal_trends-0.1.4/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.5/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `longitudinal_trends-0.1.4/pyproject.toml` & `longitudinal_trends-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.4'
+version='0.1.5'
 description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.7"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},
```

