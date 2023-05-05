# Comparing `tmp/twity-0.0.2.tar.gz` & `tmp/twity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twity-0.0.2.tar", last modified: Fri May  5 09:56:49 2023, max compression
+gzip compressed data, was "twity-0.0.3.tar", last modified: Fri May  5 10:26:26 2023, max compression
```

## Comparing `twity-0.0.2.tar` & `twity-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 methmal    (501) staff       (20)        0 2023-05-05 09:56:49.646110 twity-0.0.2/
--rw-r--r--   0 methmal    (501) staff       (20)      726 2023-05-05 09:56:49.645994 twity-0.0.2/PKG-INFO
--rw-r--r--   0 methmal    (501) staff       (20)      279 2023-05-05 09:45:43.000000 twity-0.0.2/README.md
--rw-r--r--   0 methmal    (501) staff       (20)       38 2023-05-05 09:56:49.646142 twity-0.0.2/setup.cfg
--rw-r--r--   0 methmal    (501) staff       (20)      916 2023-05-05 09:56:37.000000 twity-0.0.2/setup.py
-drwxr-xr-x   0 methmal    (501) staff       (20)        0 2023-05-05 09:56:49.644982 twity-0.0.2/twity/
--rw-r--r--   0 methmal    (501) staff       (20)        0 2023-05-02 16:55:42.000000 twity-0.0.2/twity/__init__.py
--rw-r--r--   0 methmal    (501) staff       (20)      797 2023-05-05 08:49:41.000000 twity-0.0.2/twity/auth.py
--rw-r--r--   0 methmal    (501) staff       (20)      631 2023-05-03 11:21:32.000000 twity-0.0.2/twity/config.py
--rw-r--r--   0 methmal    (501) staff       (20)      721 2023-05-05 08:49:51.000000 twity-0.0.2/twity/create.py
--rw-r--r--   0 methmal    (501) staff       (20)      184 2023-05-05 08:49:46.000000 twity-0.0.2/twity/delete.py
--rw-r--r--   0 methmal    (501) staff       (20)      210 2023-05-05 08:49:37.000000 twity-0.0.2/twity/twity.py
-drwxr-xr-x   0 methmal    (501) staff       (20)        0 2023-05-05 09:56:49.645793 twity-0.0.2/twity.egg-info/
--rw-r--r--   0 methmal    (501) staff       (20)      726 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/PKG-INFO
--rw-r--r--   0 methmal    (501) staff       (20)      289 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/SOURCES.txt
--rw-r--r--   0 methmal    (501) staff       (20)        1 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/dependency_links.txt
--rw-r--r--   0 methmal    (501) staff       (20)       47 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/entry_points.txt
--rw-r--r--   0 methmal    (501) staff       (20)      245 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/requires.txt
--rw-r--r--   0 methmal    (501) staff       (20)        6 2023-05-05 09:56:49.000000 twity-0.0.2/twity.egg-info/top_level.txt
+drwxr-xr-x   0 methmal    (501) staff       (20)        0 2023-05-05 10:26:26.665664 twity-0.0.3/
+-rw-r--r--   0 methmal    (501) staff       (20)      726 2023-05-05 10:26:26.665552 twity-0.0.3/PKG-INFO
+-rw-r--r--   0 methmal    (501) staff       (20)      279 2023-05-05 09:45:43.000000 twity-0.0.3/README.md
+-rw-r--r--   0 methmal    (501) staff       (20)       38 2023-05-05 10:26:26.665699 twity-0.0.3/setup.cfg
+-rw-r--r--   0 methmal    (501) staff       (20)      910 2023-05-05 10:25:34.000000 twity-0.0.3/setup.py
+drwxr-xr-x   0 methmal    (501) staff       (20)        0 2023-05-05 10:26:26.665398 twity-0.0.3/twity.egg-info/
+-rw-r--r--   0 methmal    (501) staff       (20)      726 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/PKG-INFO
+-rw-r--r--   0 methmal    (501) staff       (20)      194 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/SOURCES.txt
+-rw-r--r--   0 methmal    (501) staff       (20)        1 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/dependency_links.txt
+-rw-r--r--   0 methmal    (501) staff       (20)       41 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/entry_points.txt
+-rw-r--r--   0 methmal    (501) staff       (20)      245 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/requires.txt
+-rw-r--r--   0 methmal    (501) staff       (20)        1 2023-05-05 10:26:26.000000 twity-0.0.3/twity.egg-info/top_level.txt
```

### Comparing `twity-0.0.2/PKG-INFO` & `twity-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twity
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple twitter bot to create and delete your tweets from the terminal
 Home-page: https://github.com/methmal66/twity.git
 Author: Sanuja Methmal
 Author-email: methmal66@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twity-0.0.2/setup.py` & `twity-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required_packages = f.read().splitlines()
 
 setup(
     name='twity',
-    version='0.0.2',
+    version='0.0.3',
     author='Sanuja Methmal',
     author_email='methmal66@gmail.com',
     url='https://github.com/methmal66/twity.git',
     description='A simple twitter bot to create and delete your tweets from the terminal',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=required_packages,
     python_requires='>=3.6',
     entry_points={
         'console_scripts':[
-            'twity=twity.twity:__main__'
+            'twity=twity:__main__'
         ]
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `twity-0.0.2/twity.egg-info/PKG-INFO` & `twity-0.0.3/twity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twity
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple twitter bot to create and delete your tweets from the terminal
 Home-page: https://github.com/methmal66/twity.git
 Author: Sanuja Methmal
 Author-email: methmal66@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

