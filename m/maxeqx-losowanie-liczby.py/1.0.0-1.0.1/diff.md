# Comparing `tmp/maxeqx-losowanie-liczby.py-1.0.0.tar.gz` & `tmp/maxeqx-losowanie-liczby.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-losowanie-liczby.py-1.0.0.tar", last modified: Fri May  5 15:34:10 2023, max compression
+gzip compressed data, was "maxeqx-losowanie-liczby.py-1.0.1.tar", last modified: Fri May  5 15:36:26 2023, max compression
```

## Comparing `maxeqx-losowanie-liczby.py-1.0.0.tar` & `maxeqx-losowanie-liczby.py-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:34:10.691745 maxeqx-losowanie-liczby.py-1.0.0/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-losowanie-liczby.py-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-losowanie-liczby.py-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-05-05 15:34:10.690745 maxeqx-losowanie-liczby.py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-losowanie-liczby.py-1.0.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 15:34:10.686748 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-05 15:34:10.000000 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-05 15:34:10.000000 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:34:10.000000 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 15:34:10.000000 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 15:34:10.000000 maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 15:34:10.688746 maxeqx-losowanie-liczby.py-1.0.0/maxll/
--rw-rw-rw-   0        0        0      220 2023-05-05 15:33:57.000000 maxeqx-losowanie-liczby.py-1.0.0/maxll/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 15:34:10.691745 maxeqx-losowanie-liczby.py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-05 15:31:30.000000 maxeqx-losowanie-liczby.py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:36:26.128597 maxeqx-losowanie-liczby.py-1.0.1/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-losowanie-liczby.py-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-losowanie-liczby.py-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-05-05 15:36:26.127597 maxeqx-losowanie-liczby.py-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-losowanie-liczby.py-1.0.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:36:26.111597 maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-05 15:36:25.000000 maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-05 15:36:25.000000 maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:36:25.000000 maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 15:36:25.000000 maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:36:26.125597 maxeqx-losowanie-liczby.py-1.0.1/maxll/
+-rw-rw-rw-   0        0        0      220 2023-05-05 15:33:57.000000 maxeqx-losowanie-liczby.py-1.0.1/maxll/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:36:26.128597 maxeqx-losowanie-liczby.py-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-05 15:36:15.000000 maxeqx-losowanie-liczby.py-1.0.1/setup.py
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.0/LICENSE.txt` & `maxeqx-losowanie-liczby.py-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-losowanie-liczby.py-1.0.0/PKG-INFO` & `maxeqx-losowanie-liczby.py-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-losowanie-liczby.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Losuje liczbe.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: losuje liczbe
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.0/README.txt` & `maxeqx-losowanie-liczby.py-1.0.1/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-losowanie-liczby.py-1.0.0/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO` & `maxeqx-losowanie-liczby.py-1.0.1/maxeqx_losowanie_liczby.py.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-losowanie-liczby.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Losuje liczbe.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: losuje liczbe
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-losowanie-liczby.py-1.0.0/setup.py` & `maxeqx-losowanie-liczby.py-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-losowanie-liczby.py',
-  version='1.0.0',
+  version='1.0.1',
   description='Losuje liczbe.',
   long_description="Losuje liczbe.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='losuje liczbe',
   packages=find_packages(),
-  install_requires=['random'] 
+  install_requires=[] 
 )
```

