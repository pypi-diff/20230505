# Comparing `tmp/nsloader-1.0.0.tar.gz` & `tmp/nsloader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsloader-1.0.0.tar", last modified: Wed May  3 23:24:55 2023, max compression
+gzip compressed data, was "nsloader-1.1.0.tar", last modified: Fri May  5 14:59:44 2023, max compression
```

## Comparing `nsloader-1.0.0.tar` & `nsloader-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 23:24:37.000000 nsloader-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 23:24:55.612482 nsloader-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-03 23:24:37.000000 nsloader-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/nsloader/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 23:24:37.000000 nsloader-1.0.0/nsloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-03 23:24:37.000000 nsloader-1.0.0/nsloader/wsj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/nsloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:24:55.612482 nsloader-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 23:24:37.000000 nsloader-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:37.000000 nsloader-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-03 23:24:37.000000 nsloader-1.0.0/test/test_wsj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:59:44.721713 nsloader-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 14:59:26.000000 nsloader-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-05 14:59:44.721713 nsloader-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-05 14:59:26.000000 nsloader-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:59:44.721713 nsloader-1.1.0/nsloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 14:59:26.000000 nsloader-1.1.0/nsloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-05 14:59:26.000000 nsloader-1.1.0/nsloader/wsj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:59:44.721713 nsloader-1.1.0/nsloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-05 14:59:44.000000 nsloader-1.1.0/nsloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 14:59:44.000000 nsloader-1.1.0/nsloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:59:44.000000 nsloader-1.1.0/nsloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 14:59:44.000000 nsloader-1.1.0/nsloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 14:59:44.000000 nsloader-1.1.0/nsloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:59:44.721713 nsloader-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 14:59:26.000000 nsloader-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:59:44.721713 nsloader-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:59:26.000000 nsloader-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-05 14:59:26.000000 nsloader-1.1.0/test/test_wsj.py
```

### Comparing `nsloader-1.0.0/LICENSE` & `nsloader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsloader-1.0.0/PKG-INFO` & `nsloader-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsloader
-Version: 1.0.0
+Version: 1.1.0
 Summary: This script collects articles from Wall Street Journal and returns it in dict format.
 Home-page: https://github.com/new-village/nsloader
 Author: new-village
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nsloader  
@@ -18,20 +18,17 @@
 $ python -m pip install nsloader
 ```
 nsloader is tested by Python `3.10`.
   
   
 ### Dependencies
 ----------------------
-- [beautifulsoup4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#)
-- [selenium](https://www.selenium.dev/)
-- [webdriver_manager](https://github.com/SergeyPirogov/webdriver_manager)
-- [chromedriver_binary](https://github.com/danielkaiser/python-chromedriver-binary)
+- [playwright](https://playwright.dev/python/)
   
-Additionaly, you have to install `google-chrome-stable` in your execution environment.  
+Additionaly, you have to execute `install playwright` in your execution environment.  
   
   
 ### Usage
 ----------------------
 To load the [Wall Street Journal](https://www.wsj.com/) articles and parse to dictionay format.
 
 #### Wall Street Journal
```

### Comparing `nsloader-1.0.0/README.md` & `nsloader-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,17 @@
 $ python -m pip install nsloader
 ```
 nsloader is tested by Python `3.10`.
   
   
 ### Dependencies
 ----------------------
-- [beautifulsoup4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#)
-- [selenium](https://www.selenium.dev/)
-- [webdriver_manager](https://github.com/SergeyPirogov/webdriver_manager)
-- [chromedriver_binary](https://github.com/danielkaiser/python-chromedriver-binary)
+- [playwright](https://playwright.dev/python/)
   
-Additionaly, you have to install `google-chrome-stable` in your execution environment.  
+Additionaly, you have to execute `install playwright` in your execution environment.  
   
   
 ### Usage
 ----------------------
 To load the [Wall Street Journal](https://www.wsj.com/) articles and parse to dictionay format.
 
 #### Wall Street Journal
```

### Comparing `nsloader-1.0.0/nsloader.egg-info/PKG-INFO` & `nsloader-1.1.0/nsloader.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsloader
-Version: 1.0.0
+Version: 1.1.0
 Summary: This script collects articles from Wall Street Journal and returns it in dict format.
 Home-page: https://github.com/new-village/nsloader
 Author: new-village
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nsloader  
@@ -18,20 +18,17 @@
 $ python -m pip install nsloader
 ```
 nsloader is tested by Python `3.10`.
   
   
 ### Dependencies
 ----------------------
-- [beautifulsoup4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#)
-- [selenium](https://www.selenium.dev/)
-- [webdriver_manager](https://github.com/SergeyPirogov/webdriver_manager)
-- [chromedriver_binary](https://github.com/danielkaiser/python-chromedriver-binary)
+- [playwright](https://playwright.dev/python/)
   
-Additionaly, you have to install `google-chrome-stable` in your execution environment.  
+Additionaly, you have to execute `install playwright` in your execution environment.  
   
   
 ### Usage
 ----------------------
 To load the [Wall Street Journal](https://www.wsj.com/) articles and parse to dictionay format.
 
 #### Wall Street Journal
```

### Comparing `nsloader-1.0.0/setup.py` & `nsloader-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nsloader',
-    version='1.0.0',
+    version='1.1.0',
     author='new-village',
     url='https://github.com/new-village/nsloader',
     description='This script collects articles from Wall Street Journal and returns it in dict format.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['beautifulsoup4', 'selenium', 'webdriver_manager', 'chromedriver_binary'],
+    install_requires=['playwright'],
     packages=find_packages(),
     package_data={'': ['config/*.json']},
 )
```

### Comparing `nsloader-1.0.0/test/test_wsj.py` & `nsloader-1.1.0/test/test_wsj.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
         # Contents Masking
         result = self.article.to_dict()
         for key in ["profile", "body"]:
             result[key] = len(result[key])
         self.assertDictEqual(result, expect)
 
-
     def test_commentary(self):
         """ testing commentary case
         """
         # Expected result data
         expect = {
             "url": "https://www.wsj.com/articles/ai-needs-guardrails-and-global-cooperation-chatbot-megasystem-intelligence-f7be3a3c",
             "title": "Artificial Intelligence Needs Guardrails and Global Cooperation",
@@ -62,10 +61,9 @@
 
         # Contents Masking
         result = self.article.to_dict()
         for key in ["profile", "body"]:
             result[key] = len(result[key])
         self.assertDictEqual(result, expect)
 
-
 if __name__ == "__main__":
     unittest.main()
```

