# Comparing `tmp/maxeqx-losowanie-liczby.py-1.0.2.tar.gz` & `tmp/maxeqx-losowanie-liczby.py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-losowanie-liczby.py-1.0.2.tar", last modified: Fri May  5 15:39:31 2023, max compression
+gzip compressed data, was "maxeqx-losowanie-liczby.py-1.0.3.tar", last modified: Fri May  5 15:43:19 2023, max compression
```

## Comparing `maxeqx-losowanie-liczby.py-1.0.2.tar` & `maxeqx-losowanie-liczby.py-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:39:31.968745 maxeqx-losowanie-liczby.py-1.0.2/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-losowanie-liczby.py-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-losowanie-liczby.py-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-05-05 15:39:31.956744 maxeqx-losowanie-liczby.py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-losowanie-liczby.py-1.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 15:39:31.939746 maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-05 15:39:31.000000 maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-05 15:39:31.000000 maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:39:31.000000 maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 15:39:31.000000 maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 15:39:31.942745 maxeqx-losowanie-liczby.py-1.0.2/maxll/
--rw-rw-rw-   0        0        0      210 2023-05-05 15:39:24.000000 maxeqx-losowanie-liczby.py-1.0.2/maxll/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 15:39:31.968745 maxeqx-losowanie-liczby.py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-05 15:39:03.000000 maxeqx-losowanie-liczby.py-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:43:19.584392 maxeqx-losowanie-liczby.py-1.0.3/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-losowanie-liczby.py-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-losowanie-liczby.py-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-05-05 15:43:19.583393 maxeqx-losowanie-liczby.py-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-losowanie-liczby.py-1.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:43:19.576390 maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-05 15:43:19.000000 maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-05 15:43:19.000000 maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:43:19.000000 maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 15:43:19.000000 maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:43:19.579391 maxeqx-losowanie-liczby.py-1.0.3/maxll/
+-rw-rw-rw-   0        0        0      230 2023-05-05 15:43:05.000000 maxeqx-losowanie-liczby.py-1.0.3/maxll/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:43:19.585391 maxeqx-losowanie-liczby.py-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-05 15:43:13.000000 maxeqx-losowanie-liczby.py-1.0.3/setup.py
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.2/LICENSE.txt` & `maxeqx-losowanie-liczby.py-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-losowanie-liczby.py-1.0.2/PKG-INFO` & `maxeqx-losowanie-liczby.py-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-losowanie-liczby.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Losuje liczbe.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: losuje liczbe
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.2/README.txt` & `maxeqx-losowanie-liczby.py-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-losowanie-liczby.py-1.0.2/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO` & `maxeqx-losowanie-liczby.py-1.0.3/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-losowanie-liczby.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Losuje liczbe.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: losuje liczbe
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.2/setup.py` & `maxeqx-losowanie-liczby.py-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-losowanie-liczby.py',
-  version='1.0.2',
+  version='1.0.3',
   description='Losuje liczbe.',
   long_description="Losuje liczbe.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

