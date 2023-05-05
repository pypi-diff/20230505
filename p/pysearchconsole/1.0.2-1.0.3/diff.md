# Comparing `tmp/pysearchconsole-1.0.2.tar.gz` & `tmp/pysearchconsole-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysearchconsole-1.0.2.tar", last modified: Fri May  5 06:53:47 2023, max compression
+gzip compressed data, was "pysearchconsole-1.0.3.tar", last modified: Fri May  5 07:20:56 2023, max compression
```

## Comparing `pysearchconsole-1.0.2.tar` & `pysearchconsole-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 06:53:47.885538 pysearchconsole-1.0.2/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4536 2023-05-05 06:53:47.881538 pysearchconsole-1.0.2/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     3647 2023-05-05 06:03:16.000000 pysearchconsole-1.0.2/README.md
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-05 06:53:47.885538 pysearchconsole-1.0.2/setup.cfg
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1328 2023-05-05 06:53:19.000000 pysearchconsole-1.0.2/setup.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 06:53:47.881538 pysearchconsole-1.0.2/src/
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 06:53:47.881538 pysearchconsole-1.0.2/src/credential/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.2/src/credential/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.2/src/credential/credential.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 06:53:47.881538 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4536 2023-05-05 06:53:47.000000 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-05 06:53:47.000000 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-05 06:53:47.000000 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       57 2023-05-05 06:53:47.000000 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/requires.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-05 06:53:47.000000 pysearchconsole-1.0.2/src/pysearchconsole.egg-info/top_level.txt
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 06:53:47.881538 pysearchconsole-1.0.2/src/searchconsole/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.2/src/searchconsole/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.2/src/searchconsole/searchconsole.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4631 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     3748 2023-05-05 07:20:09.000000 pysearchconsole-1.0.3/README.md
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/setup.cfg
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1325 2023-05-05 07:20:15.000000 pysearchconsole-1.0.3/setup.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/credential/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.3/src/credential/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.3/src/credential/credential.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4631 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       57 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/requires.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-05 07:20:56.000000 pysearchconsole-1.0.3/src/pysearchconsole.egg-info/top_level.txt
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 07:20:56.175598 pysearchconsole-1.0.3/src/searchconsole/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.3/src/searchconsole/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.3/src/searchconsole/searchconsole.py
```

### Comparing `pysearchconsole-1.0.2/PKG-INFO` & `pysearchconsole-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the Google Search Console API
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
-Author: ['Rahul Katoch', 'Harish kumar']
+Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
 Keywords: search console api google seo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 searchconsole is a Python library that provides an easy-to-use interface for working with the Google Search Console API. With this library, you can fetch data from your Search Console account and use it to analyze your website's performance in search results.
 
 # Getting Started
 
 Before you can use the searchconsole library, you need to generate a credentials.json file that will allow you to authenticate with the Google Search Console API. To generate this file, you can use the Credential class provided by the library.
 ```python
-from searchconsole.credential import Credential
+from credential.credential import Crediential
 
 client_id = "kjahfdnjkeahfnulkjbn38294u2389"
 client_secret = "32u4393kjbjjk3b4bk331094i3jb"
 
 # create the credentials.json file in your home directory
 
 Credential(client_id=client_id, client_secret=client_secret)
@@ -50,23 +50,25 @@
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
-from searchconsole import SearchConsole
+from searchconsole.searchconsole import Searchconsole
 
-domain = "example.com"
+domain = "https://www.example.com/"
 start_date = "2022-01-01"
-end_date = "2022-01-31"
+
+
+# dont write end date they will automatically update as date.today()
 
 authenticate with the API using credentials.json
 
-auth_response = SearchConsole(domain, credentials='credentials.json')
+auth_response = SearchConsole(domain=domain,start_date=start_date, credentials='credentials.json')
 
 # print the data
 
 # print(auth_response)
 
 report_dict = []
 for i in auth_response['rows']:
```

### Comparing `pysearchconsole-1.0.2/README.md` & `pysearchconsole-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 searchconsole is a Python library that provides an easy-to-use interface for working with the Google Search Console API. With this library, you can fetch data from your Search Console account and use it to analyze your website's performance in search results.
 
 # Getting Started
 
 Before you can use the searchconsole library, you need to generate a credentials.json file that will allow you to authenticate with the Google Search Console API. To generate this file, you can use the Credential class provided by the library.
 ```python
-from searchconsole.credential import Credential
+from credential.credential import Crediential
 
 client_id = "kjahfdnjkeahfnulkjbn38294u2389"
 client_secret = "32u4393kjbjjk3b4bk331094i3jb"
 
 # create the credentials.json file in your home directory
 
 Credential(client_id=client_id, client_secret=client_secret)
@@ -28,23 +28,25 @@
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
-from searchconsole import SearchConsole
+from searchconsole.searchconsole import Searchconsole
 
-domain = "example.com"
+domain = "https://www.example.com/"
 start_date = "2022-01-01"
-end_date = "2022-01-31"
+
+
+# dont write end date they will automatically update as date.today()
 
 authenticate with the API using credentials.json
 
-auth_response = SearchConsole(domain, credentials='credentials.json')
+auth_response = SearchConsole(domain=domain,start_date=start_date, credentials='credentials.json')
 
 # print the data
 
 # print(auth_response)
 
 report_dict = []
 for i in auth_response['rows']:
```

### Comparing `pysearchconsole-1.0.2/setup.py` & `pysearchconsole-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pysearchconsole',
-    version='1.0.2',
+    version='1.0.3',
     description='A Python wrapper for the Google Search Console API',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author=['Rahul Katoch','Harish kumar'],
+    author='Rahul Katoch, Harish kumar',
     author_email='rahulkatoch99@gmail.com',
     maintainer_email='rahulkatoch99@gmail.com, echkayweb@gmail.com',
     url='https://github.com/Rahulkatoch99/py_searchconsole',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'apiclient',
```

### Comparing `pysearchconsole-1.0.2/src/credential/credential.py` & `pysearchconsole-1.0.3/src/credential/credential.py`

 * *Files identical despite different names*

### Comparing `pysearchconsole-1.0.2/src/pysearchconsole.egg-info/PKG-INFO` & `pysearchconsole-1.0.3/src/pysearchconsole.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the Google Search Console API
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
-Author: ['Rahul Katoch', 'Harish kumar']
+Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
 Keywords: search console api google seo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 searchconsole is a Python library that provides an easy-to-use interface for working with the Google Search Console API. With this library, you can fetch data from your Search Console account and use it to analyze your website's performance in search results.
 
 # Getting Started
 
 Before you can use the searchconsole library, you need to generate a credentials.json file that will allow you to authenticate with the Google Search Console API. To generate this file, you can use the Credential class provided by the library.
 ```python
-from searchconsole.credential import Credential
+from credential.credential import Crediential
 
 client_id = "kjahfdnjkeahfnulkjbn38294u2389"
 client_secret = "32u4393kjbjjk3b4bk331094i3jb"
 
 # create the credentials.json file in your home directory
 
 Credential(client_id=client_id, client_secret=client_secret)
@@ -50,23 +50,25 @@
 
 This will create a credentials.json file in your home directory that you can use to authenticate with the API.
 
 # Fetching Data
 
 Once you have generated your credentials.json file, you can use the searchconsole library to fetch data from your Search Console account. Here is an example of how to fetch search analytics data for a given domain:
 ```python
-from searchconsole import SearchConsole
+from searchconsole.searchconsole import Searchconsole
 
-domain = "example.com"
+domain = "https://www.example.com/"
 start_date = "2022-01-01"
-end_date = "2022-01-31"
+
+
+# dont write end date they will automatically update as date.today()
 
 authenticate with the API using credentials.json
 
-auth_response = SearchConsole(domain, credentials='credentials.json')
+auth_response = SearchConsole(domain=domain,start_date=start_date, credentials='credentials.json')
 
 # print the data
 
 # print(auth_response)
 
 report_dict = []
 for i in auth_response['rows']:
```

### Comparing `pysearchconsole-1.0.2/src/searchconsole/searchconsole.py` & `pysearchconsole-1.0.3/src/searchconsole/searchconsole.py`

 * *Files identical despite different names*

