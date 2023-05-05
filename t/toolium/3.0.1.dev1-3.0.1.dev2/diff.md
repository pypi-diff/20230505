# Comparing `tmp/toolium-3.0.1.dev1.tar.gz` & `tmp/toolium-3.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.1.dev1.tar", last modified: Fri May  5 08:35:24 2023, max compression
+gzip compressed data, was "toolium-3.0.1.dev2.tar", last modified: Fri May  5 14:58:07 2023, max compression
```

## Comparing `toolium-3.0.1.dev1.tar` & `toolium-3.0.1.dev2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.579561 toolium-3.0.1.dev1/
--rw-rw-rw-   0        0        0    29882 2023-05-05 08:33:04.000000 toolium-3.0.1.dev1/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.1.dev1/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.1.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0     5526 2023-05-05 08:35:24.580561 toolium-3.0.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/README.rst
--rw-rw-rw-   0        0        0       12 2023-05-05 08:34:57.000000 toolium-3.0.1.dev1/VERSION
--rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/requirements.txt
--rw-rw-rw-   0        0        0      205 2023-05-05 08:33:04.000000 toolium-3.0.1.dev1/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 08:35:24.581564 toolium-3.0.1.dev1/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.397605 toolium-3.0.1.dev1/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev1/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.428606 toolium-3.0.1.dev1/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev1/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12432 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    10954 2023-05-04 10:43:56.000000 toolium-3.0.1.dev1/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    21012 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/config_parser.py
--rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.499604 toolium-3.0.1.dev1/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.522604 toolium-3.0.1.dev1/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev1/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.536198 toolium-3.0.1.dev1/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.1.dev1/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.1.dev1/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.1.dev1/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8668 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.577562 toolium-3.0.1.dev1/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.1.dev1/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.1.dev1/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:35:24.410606 toolium-3.0.1.dev1/toolium.egg-info/
--rw-rw-rw-   0        0        0     5526 2023-05-05 08:35:24.000000 toolium-3.0.1.dev1/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-05-05 08:35:24.000000 toolium-3.0.1.dev1/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:35:24.000000 toolium-3.0.1.dev1/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-05-05 08:35:24.000000 toolium-3.0.1.dev1/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 08:35:24.000000 toolium-3.0.1.dev1/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.252834 toolium-3.0.1.dev2/
+-rw-rw-rw-   0        0        0    29956 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.1.dev2/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.1.dev2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5526 2023-05-05 14:58:07.252834 toolium-3.0.1.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/README.rst
+-rw-rw-rw-   0        0        0       12 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/VERSION
+-rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/requirements.txt
+-rw-rw-rw-   0        0        0      205 2023-05-05 08:33:04.000000 toolium-3.0.1.dev2/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-05-05 14:58:07.253833 toolium-3.0.1.dev2/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.119833 toolium-3.0.1.dev2/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.135837 toolium-3.0.1.dev2/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12432 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    10973 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21012 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.188834 toolium-3.0.1.dev2/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.203874 toolium-3.0.1.dev2/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.212835 toolium-3.0.1.dev2/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8668 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.250835 toolium-3.0.1.dev2/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.1.dev2/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.126835 toolium-3.0.1.dev2/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5526 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.1.dev1/CHANGELOG.rst` & `toolium-3.0.1.dev2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ------
 
 *Release date: In development*
 
 - Allow to search in `context.storage` using `[CONTEXT:a.b.c]` replacement when `before_feature` method is not used
 - Execute after scenario methods also when a scenario is skipped to assure that scenario preconditions are cleaned
 - Fix `[LANG:key]` replacement bug when it contains carriage returns
+- `context.storage` must be initialized before dynamic environment steps
 
 v3.0.0
 ------
 
 *Release date: 2023-05-03*
 
 - Add support for Python 3.11
```

### Comparing `toolium-3.0.1.dev1/LICENSE` & `toolium-3.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/PKG-INFO` & `toolium-3.0.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.1.dev1
+Version: 3.0.1.dev2
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.1.dev1/README.rst` & `toolium-3.0.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/setup.py` & `toolium-3.0.1.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/behave/env_utils.py` & `toolium-3.0.1.dev2/toolium/behave/env_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/behave/environment.py` & `toolium-3.0.1.dev2/toolium/behave/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,18 +124,19 @@
     add_assert_screenshot_methods(context, scenario)
 
     # Configure Jira properties
     save_jira_conf()
 
     context.logger.info("Running new scenario: %s", scenario.name)
 
+    # Make sure storage dict are empty in each scenario
+    context.storage = dict()
+
     # Behave dynamic environment
     context.dyn_env.execute_before_scenario_steps(context)
-    # Make sure storage dict are empty
-    context.storage = dict()
 
 
 def create_and_configure_wrapper(context):
     """Create and configure driver wrapper in behave tests
 
     :param context: behave context
     """
```

### Comparing `toolium-3.0.1.dev1/toolium/config_driver.py` & `toolium-3.0.1.dev2/toolium/config_driver.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/config_files.py` & `toolium-3.0.1.dev2/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/config_parser.py` & `toolium-3.0.1.dev2/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/driver_wrapper.py` & `toolium-3.0.1.dev2/toolium/driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/driver_wrappers_pool.py` & `toolium-3.0.1.dev2/toolium/driver_wrappers_pool.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/jira.py` & `toolium-3.0.1.dev2/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/__init__.py` & `toolium-3.0.1.dev2/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/button_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/checkbox_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/group_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/input_radio_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/input_text_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/link_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/page_elements.py` & `toolium-3.0.1.dev2/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/select_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageelements/text_page_element.py` & `toolium-3.0.1.dev2/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageobjects/common_object.py` & `toolium-3.0.1.dev2/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageobjects/mobile_page_object.py` & `toolium-3.0.1.dev2/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pageobjects/page_object.py` & `toolium-3.0.1.dev2/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/pytest_fixtures.py` & `toolium-3.0.1.dev2/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/resources/VisualTests.css` & `toolium-3.0.1.dev2/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/resources/VisualTests.js` & `toolium-3.0.1.dev2/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/resources/VisualTestsTemplate.html` & `toolium-3.0.1.dev2/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/selenoid.py` & `toolium-3.0.1.dev2/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/test_cases.py` & `toolium-3.0.1.dev2/toolium/test_cases.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/data_generator.py` & `toolium-3.0.1.dev2/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/dataset.py` & `toolium-3.0.1.dev2/toolium/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/download_files.py` & `toolium-3.0.1.dev2/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/driver_utils.py` & `toolium-3.0.1.dev2/toolium/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/driver_wait_utils.py` & `toolium-3.0.1.dev2/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/path_utils.py` & `toolium-3.0.1.dev2/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/utils/poeditor.py` & `toolium-3.0.1.dev2/toolium/utils/poeditor.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium/visual_test.py` & `toolium-3.0.1.dev2/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev1/toolium.egg-info/PKG-INFO` & `toolium-3.0.1.dev2/toolium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.1.dev1
+Version: 3.0.1.dev2
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.1.dev1/toolium.egg-info/SOURCES.txt` & `toolium-3.0.1.dev2/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

