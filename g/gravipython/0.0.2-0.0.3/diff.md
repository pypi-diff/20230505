# Comparing `tmp/gravipython-0.0.2.tar.gz` & `tmp/gravipython-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravipython-0.0.2.tar", last modified: Fri May  5 13:29:20 2023, max compression
+gzip compressed data, was "gravipython-0.0.3.tar", last modified: Fri May  5 14:15:43 2023, max compression
```

## Comparing `gravipython-0.0.2.tar` & `gravipython-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:29:22.000000 gravipython-0.0.2/
--rw-rw-rw-   0        0        0      174 2023-05-05 13:29:22.000000 gravipython-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1424 2023-05-03 09:36:18.000000 gravipython-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 13:29:22.000000 gravipython-0.0.2/gravipython.egg-info/
--rw-rw-rw-   0        0        0      174 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2023-05-02 13:51:28.000000 gravipython-0.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:29:22.000000 gravipython-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-05-05 13:29:14.000000 gravipython-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/
+-rw-rw-rw-   0        0        0     1721 2023-05-05 14:15:44.000000 gravipython-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-05-05 13:55:16.000000 gravipython-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/
+-rw-rw-rw-   0        0        0     1721 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/
+-rw-rw-rw-   0        0        0     1680 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2023-05-02 13:51:28.000000 gravipython-0.0.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:15:44.000000 gravipython-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-05 14:15:32.000000 gravipython-0.0.3/setup.py
```

### Comparing `gravipython-0.0.2/README.md` & `gravipython-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,46 @@
+Metadata-Version: 2.1
+Name: gravipython
+Version: 0.0.3
+Summary: A python module for simulating planets trajectories in 2D.
+Author: Tom Brandt
+Author-email: latomateultime@gmail.com
+License: MIT license
+Description-Content-Type: text/markdown
+License-File: license.txt
+
 README.md
 
 This python module is a basic module that can be used for small simulations.
 
 v 0.0.1
 
 
-class SolarSystem(width, height, **kwargs):
+``class SolarSystem(width, height, **kwargs)``:
 
-**kwargs :
+``**kwargs`` :
 - collisions=True (Set this to False if you want to deactivate collisions)
 
 Used to create a solar system to add stars in your simulation.
 | 
-| SolarSystem.main():
+| ``SolarSystem.main()``:
 | 
 | Method that does all the work, don't forget otherwise nothing is going to appear.
 | Click on A to spawn an asteroid of 0.000001 solar masses.
 | Click on D to spawn a red dwarf of 0.35 solar masses.
 | Click on B to spawn a brown dwarf of 0.07 solar masses.
 | Click on S to spawn a star of 1 solar mass.
 | Click on P to spawn a planet of 0.0001 solar masses.
 | Click on M to spawn a moon of 0.00001 solar masses.
 | Click on C to spawn a comet of 0.000001 solar masses.
 | Click on W to spawn a white dwarf of 0.9 solar masses.
 | Click on R to reset and remove all stars from the screen.
 
 
-class SolarSystemBody(solar_system, mass, position=(0, 0), velocity=(0, 0), color=(255, 255, 255))
+``class SolarSystemBody(solar_system, mass, position=(0, 0), velocity=(0, 0), color=(255, 255, 255))``
 
 This class allows you to create your own stars.
 | 
 | From this class are created the classes :
 | 
 | - Sun
 | - RedDwarf
@@ -38,8 +48,8 @@
 | - Asteroid
 | - Planet
 | - Moon
 | - Comet
 | - WhiteDwarf
 | 
 | Each of these classes can be initialised with the same parameters as SolaSystemBody, except that they have a default value for the mass and a 
-| different one for the color.
+| different one for the color.
```

### Comparing `gravipython-0.0.2/license.txt` & `gravipython-0.0.3/license.txt`

 * *Files identical despite different names*

