# Comparing `tmp/Nimbus Splash-0.9.2.tar.gz` & `tmp/Nimbus Splash-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nimbus Splash-0.9.2.tar", last modified: Thu Mar 16 18:45:17 2023, max compression
+gzip compressed data, was "Nimbus Splash-0.9.3.tar", last modified: Mon Mar 20 12:05:04 2023, max compression
```

## Comparing `Nimbus Splash-0.9.2.tar` & `Nimbus Splash-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 18:45:17.786128 Nimbus Splash-0.9.2/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 18:45:17.786128 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/
--rw-r--r--   0 root         (0) root         (0)      512 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-16 18:45:17.000000 Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      512 2023-03-16 18:45:17.786128 Nimbus Splash-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 18:45:17.786128 Nimbus Splash-0.9.2/nimbus_splash/
--rw-r--r--   0 root         (0) root         (0)      108 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/nimbus_splash/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-16 18:45:15.000000 Nimbus Splash-0.9.2/nimbus_splash/__version__.py
--rw-r--r--   0 root         (0) root         (0)     6520 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/nimbus_splash/cli.py
--rw-r--r--   0 root         (0) root         (0)    11692 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/nimbus_splash/job.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/nimbus_splash/utils.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-03-16 18:45:14.000000 Nimbus Splash-0.9.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 18:45:17.786128 Nimbus Splash-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1145 2023-03-16 18:45:15.000000 Nimbus Splash-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 12:05:04.371563 Nimbus Splash-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 12:05:04.371563 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-03-20 12:05:04.000000 Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      512 2023-03-20 12:05:04.371563 Nimbus Splash-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 12:05:04.371563 Nimbus Splash-0.9.3/nimbus_splash/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/nimbus_splash/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/nimbus_splash/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/nimbus_splash/cli.py
+-rw-r--r--   0 root         (0) root         (0)    11692 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/nimbus_splash/job.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/nimbus_splash/utils.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 12:05:04.371563 Nimbus Splash-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-03-20 12:05:01.000000 Nimbus Splash-0.9.3/setup.py
```

### Comparing `Nimbus Splash-0.9.2/LICENSE` & `Nimbus Splash-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Nimbus Splash-0.9.2/Nimbus_Splash.egg-info/PKG-INFO` & `Nimbus Splash-0.9.3/Nimbus_Splash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nimbus-Splash
-Version: 0.9.2
+Version: 0.9.3
 Summary: A package to make life easier when using the University of         Bath's cloud computing suite for Orca calculations.
 Home-page: https://github.com/jonkragskow/nimbus_splash
 Author: Jon Kragskow
 Author-email: jgck20@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Nimbus Splash-0.9.2/PKG-INFO` & `Nimbus Splash-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nimbus Splash
-Version: 0.9.2
+Version: 0.9.3
 Summary: A package to make life easier when using the University of         Bath's cloud computing suite for Orca calculations.
 Home-page: https://github.com/jonkragskow/nimbus_splash
 Author: Jon Kragskow
 Author-email: jgck20@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Nimbus Splash-0.9.2/README.md` & `Nimbus Splash-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `Nimbus Splash-0.9.2/nimbus_splash/cli.py` & `Nimbus Splash-0.9.3/nimbus_splash/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     # Create -rst xyz file
     new_xyz = os.path.join(new_folder, "{}-rst.xyz".format(head))
     xyzp.save_xyz(new_xyz, labels, coords, verbose=False)
 
     # Edit xyz file name in input_info
     input_info = re.sub(
-        r"[a-z0-9A-Z_]+\.xyz",
+        r"[\-a-z0-9A-Z_]+\.xyz",
         "{}-rst.xyz".format(head),
         input_info
     )
 
     # Create -rst input file
     new_input = os.path.join(new_folder, "{}-rst.inp".format(head))
     with open(new_input, 'w') as f:
```

### Comparing `Nimbus Splash-0.9.2/nimbus_splash/job.py` & `Nimbus Splash-0.9.3/nimbus_splash/job.py`

 * *Files identical despite different names*

### Comparing `Nimbus Splash-0.9.2/nimbus_splash/utils.py` & `Nimbus Splash-0.9.3/nimbus_splash/utils.py`

 * *Files identical despite different names*

### Comparing `Nimbus Splash-0.9.2/setup.py` & `Nimbus Splash-0.9.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 setuptools.setup(
     name="Nimbus Splash",
     version=__version__,
     author="Jon Kragskow",
     author_email="jgck20@bath.ac.uk",
     description="A package to make life easier when using the University of \
```

