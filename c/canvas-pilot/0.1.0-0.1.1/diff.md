# Comparing `tmp/canvas-pilot-0.1.0.tar.gz` & `tmp/canvas-pilot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas-pilot-0.1.0.tar", last modified: Fri May  5 00:48:43 2023, max compression
+gzip compressed data, was "canvas-pilot-0.1.1.tar", last modified: Fri May  5 00:59:31 2023, max compression
```

## Comparing `canvas-pilot-0.1.0.tar` & `canvas-pilot-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:48:43.572253 canvas-pilot-0.1.0/
--rw-r--r--   0 ziang      (501) staff       (20)     2388 2023-05-05 00:48:43.572134 canvas-pilot-0.1.0/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)     1642 2023-05-05 00:43:54.000000 canvas-pilot-0.1.0/README.md
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:48:43.571612 canvas-pilot-0.1.0/canvas_pilot.egg-info/
--rw-r--r--   0 ziang      (501) staff       (20)     2388 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)      284 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/entry_points.txt
--rw-r--r--   0 ziang      (501) staff       (20)       25 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/requires.txt
--rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-05 00:48:43.000000 canvas-pilot-0.1.0/canvas_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:48:43.571831 canvas-pilot-0.1.0/canvas_tools/
--rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.0/canvas_tools/__init__.py
--rw-r--r--   0 ziang      (501) staff       (20)     5958 2023-05-05 00:40:42.000000 canvas-pilot-0.1.0/canvas_tools/canvas.py
--rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-05 00:48:43.572292 canvas-pilot-0.1.0/setup.cfg
--rw-r--r--   0 ziang      (501) staff       (20)     1287 2023-05-05 00:45:05.000000 canvas-pilot-0.1.0/setup.py
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102842 canvas-pilot-0.1.1/
+-rw-r--r--   0 ziang      (501) staff       (20)    35148 2023-05-05 00:58:23.000000 canvas-pilot-0.1.1/LICENSE
+-rw-r--r--   0 ziang      (501) staff       (20)     2447 2023-05-05 00:59:31.102714 canvas-pilot-0.1.1/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)     1640 2023-05-05 00:56:46.000000 canvas-pilot-0.1.1/README.md
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102181 canvas-pilot-0.1.1/canvas_pilot.egg-info/
+-rw-r--r--   0 ziang      (501) staff       (20)     2447 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)      292 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       25 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/requires.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102415 canvas-pilot-0.1.1/canvas_tools/
+-rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.1/canvas_tools/__init__.py
+-rw-r--r--   0 ziang      (501) staff       (20)     5958 2023-05-05 00:40:42.000000 canvas-pilot-0.1.1/canvas_tools/canvas.py
+-rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-05 00:59:31.102881 canvas-pilot-0.1.1/setup.cfg
+-rw-r--r--   0 ziang      (501) staff       (20)     1326 2023-05-05 00:57:02.000000 canvas-pilot-0.1.1/setup.py
```

### Comparing `canvas-pilot-0.1.0/PKG-INFO` & `canvas-pilot-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
-License: MIT
+License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Canvas Pilot
 
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
@@ -96,10 +97,8 @@
 
 ## Contributing
 
 Contributions are welcome! If you find a bug, have a feature request, or want to improve the Canvas CLI, please open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
-```
-
+This project is licensed under the GPLv3+ License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `canvas-pilot-0.1.0/README.md` & `canvas-pilot-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -76,10 +76,8 @@
 
 ## Contributing
 
 Contributions are welcome! If you find a bug, have a feature request, or want to improve the Canvas CLI, please open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
-```
-
+This project is licensed under the GPLv3+ License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `canvas-pilot-0.1.0/canvas_pilot.egg-info/PKG-INFO` & `canvas-pilot-0.1.1/canvas_pilot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
-License: MIT
+License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Canvas Pilot
 
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
@@ -96,10 +97,8 @@
 
 ## Contributing
 
 Contributions are welcome! If you find a bug, have a feature request, or want to improve the Canvas CLI, please open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
-```
-
+This project is licensed under the GPLv3+ License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `canvas-pilot-0.1.0/canvas_tools/canvas.py` & `canvas-pilot-0.1.1/canvas_tools/canvas.py`

 * *Files identical despite different names*

### Comparing `canvas-pilot-0.1.0/setup.py` & `canvas-pilot-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the README.md content
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="canvas-pilot",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "requests",
         "icalendar",
         "click",
     ],
     entry_points={
@@ -20,21 +20,21 @@
         ],
     },
     author="Ziang Zhou",
     author_email="ziang.zhou518@gmail.com",
     description="A command-line tool for managing Canvas courses, fetching assignments, and grades.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    license="MIT",
+    license="GPLv3+",
     keywords="canvas api cli",
     url="https://github.com/realzza/canvas-cli",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6, <4",
```

