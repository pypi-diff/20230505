# Comparing `tmp/pysearchconsole-1.0.3.tar.gz` & `tmp/pysearchconsole-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysearchconsole-1.0.3.tar", last modified: Fri May  5 07:20:56 2023, max compression
+gzip compressed data, was "pysearchconsole-1.0.4.tar", last modified: Fri May  5 09:10:20 2023, max compression
```

## Comparing `pysearchconsole-1.0.3.tar` & `pysearchconsole-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4631 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     3748 2023-05-05 07:20:09.000000 pysearchconsole-1.0.3/README.md
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/setup.cfg
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1325 2023-05-05 07:20:15.000000 pysearchconsole-1.0.3/setup.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/credential/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.3/src/credential/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.3/src/credential/credential.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4631 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       57 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/requires.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/top_level.txt
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/searchconsole/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.3/src/searchconsole/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.3/src/searchconsole/searchconsole.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4074 2023-05-05 08:58:27.000000 pysearchconsole-1.0.4/README.md
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/setup.cfg
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1516 2023-05-05 09:09:58.000000 pysearchconsole-1.0.4/setup.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/credential/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.4/src/credential/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.4/src/credential/credential.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       57 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/requires.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/top_level.txt
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/searchconsole/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.4/src/searchconsole/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.4/src/searchconsole/searchconsole.py
```

### Comparing `pysearchconsole-1.0.3/PKG-INFO` & `pysearchconsole-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.3
-Summary: A Python wrapper for the Google Search Console API
+Version: 1.0.4
+Summary: PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
 Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
-Keywords: search console api google seo
+Keywords: search console api google seo python libraries API integration web traffic analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -46,14 +46,20 @@
 ```
  After enter the Authorization you will get the credenial.json then after comment the Credential(client_id=client_id, client_secret=client_secret)
  
  
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
+
+
+Make sure that you have obtained the credentials.json file. Please note that the refresh token for this library expires after 6 months of inactivity. If you use the library before the expiration date, the expiration time gets extended to another 6 months.
+
+So you don't need to generate the credential.json again and again
+
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
 from searchconsole.searchconsole import Searchconsole
 
 domain = "https://www.example.com/"
```

### Comparing `pysearchconsole-1.0.3/README.md` & `pysearchconsole-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 ```
  After enter the Authorization you will get the credenial.json then after comment the Credential(client_id=client_id, client_secret=client_secret)
  
  
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
+
+
+Make sure that you have obtained the credentials.json file. Please note that the refresh token for this library expires after 6 months of inactivity. If you use the library before the expiration date, the expiration time gets extended to another 6 months.
+
+So you don't need to generate the credential.json again and again
+
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
 from searchconsole.searchconsole import Searchconsole
 
 domain = "https://www.example.com/"
```

### Comparing `pysearchconsole-1.0.3/setup.py` & `pysearchconsole-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
-
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pysearchconsole',
-    version='1.0.3',
-    description='A Python wrapper for the Google Search Console API',
+    version='1.0.4',
+    description="PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Rahul Katoch, Harish kumar',
     author_email='rahulkatoch99@gmail.com',
     maintainer_email='rahulkatoch99@gmail.com, echkayweb@gmail.com',
     url='https://github.com/Rahulkatoch99/py_searchconsole',
     packages=find_packages(where='src'),
@@ -29,11 +28,11 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
-    keywords='search console api google seo',
+    keywords='search console api google seo python libraries API integration web traffic analysis',
     python_requires='>=3.6',
     license='MIT',
 )
```

### Comparing `pysearchconsole-1.0.3/src/credential/credential.py` & `pysearchconsole-1.0.4/src/credential/credential.py`

 * *Files identical despite different names*

### Comparing `pysearchconsole-1.0.3/src/pysearchconsole.egg-info/PKG-INFO` & `pysearchconsole-1.0.4/src/pysearchconsole.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.3
-Summary: A Python wrapper for the Google Search Console API
+Version: 1.0.4
+Summary: PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
 Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
-Keywords: search console api google seo
+Keywords: search console api google seo python libraries API integration web traffic analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -46,14 +46,20 @@
 ```
  After enter the Authorization you will get the credenial.json then after comment the Credential(client_id=client_id, client_secret=client_secret)
  
  
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
+
+
+Make sure that you have obtained the credentials.json file. Please note that the refresh token for this library expires after 6 months of inactivity. If you use the library before the expiration date, the expiration time gets extended to another 6 months.
+
+So you don't need to generate the credential.json again and again
+
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
 from searchconsole.searchconsole import Searchconsole
 
 domain = "https://www.example.com/"
```

### Comparing `pysearchconsole-1.0.3/src/searchconsole/searchconsole.py` & `pysearchconsole-1.0.4/src/searchconsole/searchconsole.py`

 * *Files identical despite different names*

