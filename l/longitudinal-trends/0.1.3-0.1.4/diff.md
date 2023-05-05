# Comparing `tmp/longitudinal_trends-0.1.3.tar.gz` & `tmp/longitudinal_trends-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.3.tar", last modified: Sun Apr 30 17:14:37 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.4.tar", last modified: Fri May  5 12:39:59 2023, max compression
```

## Comparing `longitudinal_trends-0.1.3.tar` & `longitudinal_trends-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.823988 longitudinal_trends-0.1.3/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.3/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.3/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10037 2023-04-30 17:14:37.808386 longitudinal_trends-0.1.3/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9461 2023-04-29 14:14:41.000000 longitudinal_trends-0.1.3/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.479471 longitudinal_trends-0.1.3/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    18095 2023-04-28 12:55:14.000000 longitudinal_trends-0.1.3/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.730332 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10037 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-30 17:14:37.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-04-29 11:13:53.000000 longitudinal_trends-0.1.3/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.3/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-30 17:14:37.823988 longitudinal_trends-0.1.3/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.4/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.4/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.598758 longitudinal_trends-0.1.4/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17387 2023-05-05 11:45:01.000000 longitudinal_trends-0.1.4/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-05 12:39:59.821368 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-05 12:39:59.000000 longitudinal_trends-0.1.4/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-05 12:17:11.000000 longitudinal_trends-0.1.4/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.4/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-05 12:39:59.887039 longitudinal_trends-0.1.4/setup.cfg
```

### Comparing `longitudinal_trends-0.1.3/LICENSE` & `longitudinal_trends-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.3/PKG-INFO` & `longitudinal_trends-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,15 @@
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
+* Disclaimer
 
 ## Installation
 
 `pip install longitudinal-trends`
 
 ## Requirements
 
@@ -69,15 +70,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
-      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc.
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -183,7 +184,11 @@
 
 On that note, if the search term is not very popular, then the resultant dataset will contain a lot of zeroes that will hugely impact the final outcome.
 
 ## Credits
 
 - `pytrends` library
   - https://github.com/GeneralMills/pytrends/tree/0d6113a3920e7576d4b3459132b5d37fb7ab9bfb
+
+## Disclaimer
+
+This publication was made possible by the generous support of the Qatar Foundation through Carnegie Mellon University in Qatar's Seed Research program. The statements made herein are solely the responsibility of the authors.
```

### Comparing `longitudinal_trends-0.1.3/README.md` & `longitudinal_trends-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
+* Disclaimer
 
 ## Installation
 
 `pip install longitudinal-trends`
 
 ## Requirements
 
@@ -51,15 +52,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
-      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc.
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -165,7 +166,11 @@
 
 On that note, if the search term is not very popular, then the resultant dataset will contain a lot of zeroes that will hugely impact the final outcome.
 
 ## Credits
 
 - `pytrends` library
   - https://github.com/GeneralMills/pytrends/tree/0d6113a3920e7576d4b3459132b5d37fb7ab9bfb
+
+## Disclaimer
+
+This publication was made possible by the generous support of the Qatar Foundation through Carnegie Mellon University in Qatar's Seed Research program. The statements made herein are solely the responsibility of the authors.
```

### Comparing `longitudinal_trends-0.1.3/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.4/longitudinal_trends/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 from rich.logging import RichHandler
 
 from math import ceil
 import random
 
 console = Console()
 
-# session = requests.Session()
-# session.get('https://trends.google.com')
-# cookies_map = session.cookies.get_dict()
-# nid_cookie = cookies_map['NID']
-
 class RequestTrends:
 
     logging.basicConfig(
         level="INFO", format="%(message)s", datefmt="%d-%b-%Y %H:%M:%S", handlers=[RichHandler(rich_tracebacks=True)]
     )
 
 
@@ -58,15 +53,14 @@
         # Validation check for type of data request in addition to valid timeperiod for the requested data format
         if data_format not in ['daily', 'weekly', 'monthly']:
             raise ValueError("data_format should be 'daily'/'weekly'/'monthly'")
         elif data_format == 'monthly':
             self.start_date = dt.datetime(start_date.year, start_date.month, 1)
             if self.__num_of_days < 1890:
                 
-#-------------- TODO: Change the error messages for better understanding-----------------------------------------------------------------------------------------------------------------
                 raise ValueError("Difference Between Start and End date needs to be more than 1889 days to get monthly data. Given only '{}' days".format(self.__num_of_days))
         elif data_format == 'weekly':
             if self.__num_of_days < 270:
                 raise ValueError("Difference Between Start and End date needs to be more than 269 days to get weekly data. Given '{}' days".format(self.__num_of_days))
 
             self.TIME_WINDOW = 1889
             self.__determine_time_periods()
@@ -96,28 +90,28 @@
             fl.write(json.dumps(params, indent=4, sort_keys=True, default=str))
         fl.close()
 
         # Initiaate pytrends request to enquire later
         self.__pytrend = TrendReq(hl='en-US', tz=360)#, requests_args={'headers': {'Cookie': f'NID={nid_cookie}'}})
         self.__logger.info("Pytrend instance have been initiated for longitudinal_trend", extra={"markup": True})
 
+
     def __in_notebook(self):
         try:
             from IPython import get_ipython
             if 'IPKernelApp' not in get_ipython().config:  # pragma: no cover
                 return False                
         except ImportError:
             return False
         except AttributeError:
             return False
         return True
         
 
     # This method is intended to create necessary directories at each discretion
-    # After final upload to PyPI, this behavior might be altered as per requirement
     def __create_required_directory(self, folder):
         if not os.path.exists(folder):
             os.mkdir(folder)
 
     # This method provides list of time periods to fetch data for
     def __determine_time_periods(self):
         timeperiod = ceil(self.__num_of_days/self.TIME_WINDOW)
@@ -352,12 +346,8 @@
 
         # Next Merge/Concatenate over the time data into a single long term trend
         self.concat_time_series(reference_geo_code, zero_replace)
 
         # Finally rescale all across region data by converting them 
         self.convert_cross_section(reference_geo_code, zero_replace)
 
-        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
-
-# day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
-day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2022, 12, 1), dt.datetime(2022,12,31), 'daily') #4017 days
-day_data.cross_section()
+        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
```

### Comparing `longitudinal_trends-0.1.3/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.4/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,15 @@
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
+* Disclaimer
 
 ## Installation
 
 `pip install longitudinal-trends`
 
 ## Requirements
 
@@ -69,15 +70,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
-      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc.
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -183,7 +184,11 @@
 
 On that note, if the search term is not very popular, then the resultant dataset will contain a lot of zeroes that will hugely impact the final outcome.
 
 ## Credits
 
 - `pytrends` library
   - https://github.com/GeneralMills/pytrends/tree/0d6113a3920e7576d4b3459132b5d37fb7ab9bfb
+
+## Disclaimer
+
+This publication was made possible by the generous support of the Qatar Foundation through Carnegie Mellon University in Qatar's Seed Research program. The statements made herein are solely the responsibility of the authors.
```

### Comparing `longitudinal_trends-0.1.3/pyproject.toml` & `longitudinal_trends-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.3'
+version='0.1.4'
 description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.7"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},
```

