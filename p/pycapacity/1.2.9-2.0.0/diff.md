# Comparing `tmp/pycapacity-1.2.9.tar.gz` & `tmp/pycapacity-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycapacity-1.2.9.tar", last modified: Fri May 13 14:44:54 2022, max compression
+gzip compressed data, was "dist/pycapacity-2.0.0.tar", last modified: Fri May  5 15:39:59 2023, max compression
```

## Comparing `pycapacity-1.2.9.tar` & `pycapacity-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/
--rwxr-xr-x   0 antun     (1000) antun     (1000)     1069 2021-08-06 14:07:42.000000 pycapacity-1.2.9/LICENSE
--rwxr-xr-x   0 antun     (1000) antun     (1000)    16247 2021-12-07 14:52:25.000000 pycapacity-1.2.9/README.md
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity/
--rwxr-xr-x   0 antun     (1000) antun     (1000)    13379 2022-03-24 17:38:23.000000 pycapacity-1.2.9/pycapacity/robot.py
--rwxr-xr-x   0 antun     (1000) antun     (1000)    10074 2022-04-04 15:06:52.000000 pycapacity-1.2.9/pycapacity/visual.py
--rwxr-xr-x   0 antun     (1000) antun     (1000)    19233 2022-05-13 14:40:04.000000 pycapacity-1.2.9/pycapacity/algorithms.py
--rwxr-xr-x   0 antun     (1000) antun     (1000)     7983 2022-04-12 15:12:45.000000 pycapacity-1.2.9/pycapacity/human.py
--rw-rw-r--   0 antun     (1000) antun     (1000)      102 2022-04-12 14:47:05.000000 pycapacity-1.2.9/pycapacity/polytope.py
--rwxr-xr-x   0 antun     (1000) antun     (1000)        0 2021-10-27 17:41:22.000000 pycapacity-1.2.9/pycapacity/__init__.py
--rw-rw-r--   0 antun     (1000) antun     (1000)    16937 2022-05-13 14:44:54.000000 pycapacity-1.2.9/PKG-INFO
--rwxr-xr-x   0 antun     (1000) antun     (1000)     1028 2022-05-13 14:44:04.000000 pycapacity-1.2.9/setup.py
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/
--rw-rw-r--   0 antun     (1000) antun     (1000)      327 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/SOURCES.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)       11 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/top_level.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)        1 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/dependency_links.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)    16937 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/PKG-INFO
--rw-rw-r--   0 antun     (1000) antun     (1000)       44 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/requires.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)       38 2022-05-13 14:44:54.000000 pycapacity-1.2.9/setup.cfg
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2023-05-05 15:39:59.000000 pycapacity-2.0.0/
+-rw-rw-r--   0 antun     (1000) antun     (1000)     1069 2022-05-16 11:41:12.000000 pycapacity-2.0.0/LICENSE
+-rw-rw-r--   0 antun     (1000) antun     (1000)    17818 2023-05-05 15:34:53.000000 pycapacity-2.0.0/README.md
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2023-05-05 15:39:59.000000 pycapacity-2.0.0/pycapacity/
+-rwxrwxr-x   0 antun     (1000) antun     (1000)    17662 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/robot.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)    17887 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/visual.py
+-rwxrwxr-x   0 antun     (1000) antun     (1000)    24406 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/algorithms.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)     5629 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/objects.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)    10447 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/human.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)      127 2023-05-05 15:34:53.000000 pycapacity-2.0.0/pycapacity/__init__.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)    18484 2023-05-05 15:39:59.000000 pycapacity-2.0.0/PKG-INFO
+-rwxrwxr-x   0 antun     (1000) antun     (1000)      995 2023-05-05 15:38:51.000000 pycapacity-2.0.0/setup.py
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2023-05-05 15:39:59.000000 pycapacity-2.0.0/tests/
+-rw-rw-r--   0 antun     (1000) antun     (1000)     1827 2023-04-16 11:39:23.000000 pycapacity-2.0.0/tests/testing_human.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)    15920 2023-05-03 15:18:06.000000 pycapacity-2.0.0/tests/testing_algos.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)     3820 2023-05-05 15:34:53.000000 pycapacity-2.0.0/tests/testing_robot.py
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2023-05-05 15:39:59.000000 pycapacity-2.0.0/pycapacity.egg-info/
+-rw-rw-r--   0 antun     (1000) antun     (1000)      395 2023-05-05 15:39:58.000000 pycapacity-2.0.0/pycapacity.egg-info/SOURCES.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)       11 2023-05-05 15:39:58.000000 pycapacity-2.0.0/pycapacity.egg-info/top_level.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)        1 2023-05-05 15:39:58.000000 pycapacity-2.0.0/pycapacity.egg-info/dependency_links.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)    18484 2023-05-05 15:39:58.000000 pycapacity-2.0.0/pycapacity.egg-info/PKG-INFO
+-rw-rw-r--   0 antun     (1000) antun     (1000)       37 2023-05-05 15:39:58.000000 pycapacity-2.0.0/pycapacity.egg-info/requires.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)       38 2023-05-05 15:39:59.000000 pycapacity-2.0.0/setup.cfg
```

### Comparing `pycapacity-1.2.9/LICENSE` & `pycapacity-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycapacity-1.2.9/README.md` & `pycapacity-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,96 @@
+Metadata-Version: 2.1
+Name: pycapacity
+Version: 2.0.0
+Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
+Home-page: https://github.com/auctus-team/pycapacity
+Author: Antun Skuric
+Author-email: antun.skuric@inria.fr
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Framework :: Robot Framework :: Tool
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Real-time capable task-space capacity calculation python pip package
 
-# Real-time capable task-space capacity calculation python module
 
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
+
+> 📢 New version of the pycapacity package is out - version v2.0!
+> 🚨 Beware beacause there are some breaking changes in the API, please check the changelog for more details.
+
+### changelog v2.0 (05-2023)
+
+
+- polyope and ellipsoid algorithms now return `Polytope`  and `Ellipsoid`  objects (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.polytope.html))
+  - `Polytope`  class can be used as a standalone class to find  vertex, halfplane and face representation of a polytope
+- Visualisation tools improved: (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.visual.html))
+  - new `plot_polytope` function for plotting polytopes
+  - functions `plot_polytope_vertex` and `plot_polytope_faces` now can receive a polyope object
+  - function `plot_ellipsoid` now can receive a ellipsoid object
+  - better management of the `matplotlib` figures and axes, now user can provide an `ax`, `plt` or `figure` to the plotting functions
+- Added support for robot reachable workspace approximation using convex polytopes (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.reachable_space_approximation))
+- Added unit testing + continuous integration
+- improved docs with sphinx
+
+## About 
+[![PyPI package](https://img.shields.io/pypi/v/pycapacity)](https://pypi.org/project/pycapacity/) [![Tests](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml) ![](https://img.shields.io/pypi/dm/pycapacity?color=blue&label=pip%20downloads)  [![Docs](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml)
+
+<img src="https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/comparison.gif" height="250px"><img src="https://github.com/auctus-team/pycapacity/blob/master/images/human_poly.gif?raw=true" height="250px">
 
 The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
 - Robotic serial manipulators - `pycapacity.robot`
 - Human musculoskeletal models - `pycapacity.human`
 
 This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
 
 Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
 
-See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See [full API documentation and docs.](https://auctus-team.github.io/pycapacity/)
 
 ## Robotic manipulator capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/robot.png' height='300px'>
 
 For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
 - Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
 - Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
 - Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
 
 And polytopes: 
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
 - Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
+- **NEW** 📢: Reachable space of the robot with the horizon `T`  <br> `P_x = {x | x = JM(-1)tT^2/2, t_min < t < t_max,   dq_min < M^(-1)tT < dq_max,   q_min < M^(-1)tT^2/2 < q_max}`
 - Force polytopes *Minkowski sum and intersection*
 
 Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
 
+Reachable space polytope approximation is based on this paper: <br>
+[**Approximating robot reachable space using convex polytopes**](https://arxiv.org/pdf/2211.17054.pdf)<br> by Skuric, Antun, Vincent Padois, and David Daney. <br> In: Human-Friendly Robotics 2022: HFR: 15th International Workshop on Human-Friendly Robotics. Cham: Springer International Publishing, 2023.
+
+The force polytope functions have been implemented according to the paper:<br>
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
 The force polytope functions have been implemented according to the paper:<br>
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 ## Human musculoskeletal models capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/force.png' height='200px'>
 
 For the human musculoskeletal models this package implements the polytope metrics:
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
 - Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
 
 Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
@@ -59,54 +106,54 @@
 ## Polytope evaluation algorithms
 
 There are three methods implemented in this paper to resolve all the polytope calculations:
 - Hyper-plane shifting method
 - Iterative convex hull method
 - Vertex enumeration auctus
 
-All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
+All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#). 
 
 ### Hyper-plane shifting method
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 This method finds the half-space representation of the polytope of a class:
 ```
 P = {x | x = By, y_min <= y <= y_max }
 ```
 To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
+The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.hyper_plane_shift_method). 
 
 ### Iterative convex-hull method
 [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
 by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
 
 This method finds both vertex and half-space representation of the class of polytopes:
 ```
 P = {x | Ax = By, y_min <= y <= y_max }
 ``` 
 And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
 ```
 P = {x | x= Pz, Az = By, y_min <= y <= y_max }
 ``` 
 
-The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
+The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.iterative_convex_hull_method)
 
 ### Vertex enumeration auctus
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 This method finds vertex representation of the class of polytopes:
 ```
 P = {x | Ax = y, y_min <= y <= y_max }
 ``` 
 To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
+The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.vertex_enumeration_auctus)
 
 ## Installation
 
 All you need to do to install it is:
 ```
 pip install pycapacity
 ```
@@ -119,66 +166,66 @@
 import pycapacity.algorithms 
 #and/or
 import pycapacity.visual 
 ```
 
 Other way to install the code is by installing it directly from the git repo:
 ```
-pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
+pip install git+https://github.com/auctus-team/pycapacity.git
 ```
 
 ## Package API docs
 
-See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See full docs at the [link](https://auctus-team.github.io/pycapacity/)
 
 ### Modules
 
-- [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
-- [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
-- [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
-- [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
+- [`human`](https://auctus-team.github.io/pycapacity/pycapacity.human.html#module-pycapacity.human)
+- [`robot`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
+- [`algorithms`](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
+- [`visual`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
 
 ### Functions
 
 Robot metrics
-- [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
-- [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
-- [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
-- [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
-- [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
-- [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
-- [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
-- [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
-- [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
+- [`robot.acceleration_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
+- [`robot.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
+- [`robot.acceleration_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
+- [`robot.force_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
+- [`robot.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
+- [`robot.force_polytope_intersection`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_sum_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
+- [`robot.velocity_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
+- [`robot.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
+- [`robot.velocity_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
 
 Human metrics
-- [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
-- [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
-- [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
-- [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
-- [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
+- [`human.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
+- [`human.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
+- [`human.joint_torques_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
+- [`human.torque_to_muscle_force`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
+- [`human.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
 
 
 Algorithms
-- [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
-- [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
-- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
+- [`algorithms.hyper_plane_shift_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
+- [`algorithms.iterative_convex_hull_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
+- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
 
 
 Visualisation tools
-- [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
-- [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
+- [`visual.plot_polytope_faces`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
+- [`visual.plot_polytope_vertex`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
 ---
 
 ## Code examples
 
-See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
+See [`demo_notebook.ipynb`](https://github.com/auctus-team/pycapacity/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
 
 ### Randomised serial robot example
 ```python
 """
 A simple example program for 3d force polytope 
 evaluation of a randomised 6dof robot 
 """
@@ -248,8 +295,10 @@
 ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
 plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
 
 plt.tight_layout()
 plt.legend()
 plt.show()
 
-```
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycapacity-1.2.9/pycapacity/algorithms.py` & `pycapacity-2.0.0/pycapacity/algorithms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,84 @@
-from math import sin, cos 
+"""
+Overview
+---------
+
+There are three main polytope evaluation algorithms implemented:
+
+* `hyper_plane_shift_method <#pycapacity\.algorithms\.hyper_plane_shift_method>`_: Hyper plane shifting method implementation used to find half-space representaiton of problems of a form 
+
+.. math:: P = \{x~ |~ y = Ax,\quad x_{min} <= x <= x_{max}\}
+
+* `vertex_enumeration_auctus  <#pycapacity\.algorithms\.vertex_enumeration_auctus>`_: Efficient vertex enumeration algorithm for a problem of a form: 
+
+.. math:: P = \{x~ |~ Ax = b,\quad b_{min} \leq b \leq b_{max}\}
+
+* `iterative_convex_hull_method <#pycapacity\.algorithms\.iterative_convex_hull_method>`_: A function calculating the polytopes given by the equations form: 
+
+.. math:: P = \{x~ |~ Ax = By,\quad y_{min} \leq y \leq y_{max}\}
+
+Additionally this module implements different helping functions to half-plane and vertex representation manipulaitons of the polytopes:
+
+* `hspace_to_vertex <#pycapacity\.algorithms\.hspace_to_vertex>`_: Function transforming H-representation to V-representation
+* `vertex_to_hspace <#pycapacity\.algorithms\.vertex_to_hspace>`_: Function transforming V-representation to H-representation
+* `vertex_to_faces <#pycapacity\.algorithms\.vertex_to_faces>`_: Helping function transforming vertices of the polytope to a triangulated faces
+
+"""
+
 import numpy as np
-import numpy.matlib 
 import itertools
 from scipy.spatial import ConvexHull, HalfspaceIntersection
 from cvxopt import matrix
 import cvxopt.glpk
-from scipy.optimize import linprog
 
 
-def iterative_convex_hull_method(A, B, y_min, y_max, tol, P = None, bias = None,  G_in = None, h_in = None, G_eq = None, h_eq = None):
+def iterative_convex_hull_method(A, B, y_min, y_max, tol, P = None, bias = None,  G_in = None, h_in = None, G_eq = None, h_eq = None, max_iter=1000, verbose=False):
     """
     A function calculating the polytopes of achievable x for equations form:
 
-    .. math:: z = By, \quad Ax = z
-    .. math:: y_{min} \leq y \leq y_{max}
-    
-    or
-    
-    .. math:: Ax = By
-    .. math:: y_{min} \leq y \leq y_{max}
+    .. math:: P_x = \{x~ |~ Ax = By,\quad y_{min} \leq y \leq y_{max}\}
 
     (optionally - additional projection matrix)
 
-    .. math:: Az = By, \quad Pz = x
-    .. math:: y_{min} \leq y \leq y_{max}
+    .. math:: P_x = \{x~ |~Pz = x,~~ Az = By,\quad y_{min} \leq y \leq y_{max}\}
 
-    (optionally - additional bias)
+    (optionally - additional bias :math:`b`)
 
-    .. math:: Az = By + bias
-    .. math:: y_{min} \leq y \leq y_{max}
+    .. math:: P_x = \{x~ |~Ax = By + b, \quad y_{min} \leq y \leq y_{max}\}
 
     (optionally - additional inequality constaints)
 
-    .. math:: G_{in} x \leq h_{in}    
+    .. math:: G_{in} y \leq h_{in}    
     
     (optionally - additional equality constaints)
 
-    .. math:: G_{eq} x = h_{eq}
+    .. math:: G_{eq} y = h_{eq}
+
+    Finally, the most general equation supported is
+
+    .. math:: P_x = \{x~ |~Pz = x,~~ Az = By,~~ G_{in} y \leq h_{in} ,~~ G_{eq} y = h_{eq}, ~~ y_{min} \leq y \leq y_{max}\}
 
     Note:
         On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method
         A.Skuric,V.Padois,N.Rezzoug,D.Daney 
 
     Args:
         A: matrix
         B: matrix
         y_min: minimal values
         y_max: maximal values
         tol: tolerance for the polytope calculation
         P: an additional projection matrix 
         bias: bias in the intermediate space 
-        G_in: matrix - inegality constraint G_in x < h_in
-        h_in: vector - inegality constraint G_in x < h_in
-        G_eq: matrix - equality constraint G_eq x = h_eq
-        h_eq: vector - equality constraint G_eq x = h_eq
+        G_in: matrix - inegality constraint G_in y < h_in
+        h_in: vector - inegality constraint G_in y < h_in
+        G_eq: matrix - equality constraint G_eq y = h_eq
+        h_eq: vector - equality constraint G_eq y = h_eq
+        max_iter: maximum number of iterations (number of linera programmes solved) - default 1000
+        verbose: verbose program output - showing execution warnings - default False
     
     Returns
     ---------
         x_vert(list):  
             list of vertices
         H(list):  
             matrix of half-space representation `Hx<d`
@@ -66,43 +87,53 @@
         faces(list):   
             list of vertex indexes forming polytope faces  
         y_vert(list):
             list of y values producing x_vert
         z_vert(list):
             list of z values producing x_vert
         
+            
+    :raises ValueError: if the dimensions of the input matrices are not valid
+    :raises ValueError: if the limits dimensions are not valid
+    :raises ValueError: if the limits min and max are not valid
+    :raises ValueError: if the inequality/equality constraints dimensions are not valid
+    :raises ValueError: if the the projection matrix dimensions are not valid
+    
     """
     # svd of jacobian
     n, m = A.shape
     nB,L = B.shape
     #L = len(y_min)
     if n != nB:
-        raise ValueError('Matrix A and B must have same number fo rows. In your case A: {}, B: {} '.format(A.shape,B.shape))
+        raise ValueError('ICHM: Matrix A and B must have same number fo rows. In your case A: {}, B: {} '.format(A.shape,B.shape))
 
     if m > n or n > L :
-        raise ValueError('Matrix A and B dimensions must be colB >= rowB = rowA >= colA. In your case A: {}, B: {} '.format(A.shape,B.shape))
+        raise ValueError('ICHM: Matrix A and B dimensions must be colB >= rowB = rowA >= colA. In your case A: {}, B: {} '.format(A.shape,B.shape))
 
     if L!= len(y_max) or L!= len(y_min):
-        raise ValueError('Limits dimensios are not valid, should have {:d} entries. In your case y_min:{} and y_max:{}'.format(L,len(y_min),len(y_max)))
+        raise ValueError('ICHM: Limits dimensios are not valid, should have {:d} entries. In your case y_min:{} and y_max:{}'.format(L,len(y_min),len(y_max)))
 
 
     y_min = np.array(y_min).reshape((-1,))
     y_max = np.array(y_max).reshape((-1,))
 
+    if np.min(y_max - y_min) < 0:
+        raise ValueError('ICHM: Limits not valid, minimal value is higher than maximal value.')
+
     u, s, v = np.linalg.svd(A.T)
     r = len(s)
     V1 = np.array(v.transpose()[:,:r])
     V2 = np.array(v.transpose()[:,r:])
 
     # if bias not defiend set it to zero
     if bias is None:
         bias = np.zeros((n,1))  
     else:
         bias = np.array(bias).reshape((n,1))  
-
+    
     # optimisation setup
     if n > m:
         # for redundant case
         M = np.linalg.pinv(A).dot(B)
         x_bias = -np.linalg.pinv(A).dot(bias)
         # - intersection with the image of the J^T 
         Aeq = matrix(V2.T.dot(B)) 
@@ -126,100 +157,113 @@
             u = np.array([[1]])
 
     # if optional projection defined
     if P is not None:
         # check the size
         nP, mP = P.shape
         if mP != m or nP > mP:
-            raise ValueError('Matrix P dimensions error - (rows,cols) = P.shape should be: rows > cols and cols = {:d}. In your case P.shape = {}.'.format(m,P.shape))
+            raise ValueError('ICHM: Matrix P dimensions error - (rows,cols) = P.shape should be: rows > cols and cols = {:d}. In your case P.shape = {}.'.format(m,P.shape))
         M = P.dot(M)
         x_bias = P.dot(x_bias)
         u = P.dot(u)  
 
     if G_in is not None:
         # check the size
         nG, mG = G_in.shape
+        h_in = np.array(h_in).reshape((-1,))
         if mG != L:
-            raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case G_in.shape = {}.'.format(L,G_in.shape))
+            raise ValueError('ICHM: Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case G_in.shape = {}.'.format(L,G_in.shape))
         if nG != len(h_in):
-            raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case h_in.shape = {}.'.format(nG,len(h_in)))    
+            raise ValueError('ICHM: Vector h_in dimensions error - should have {:d} entries. In your case h_in.shape = {}.'.format(nG,len(h_in)))    
 
         G = matrix(np.vstack((-np.identity(L),np.identity(L),G_in)))
         h = matrix(np.hstack((list(-np.array(y_min)),y_max, h_in)))
     else:
         G = matrix(np.vstack((-np.identity(L),np.identity(L))))
         h = matrix(np.hstack((list(-np.array(y_min)),y_max)))
 
     if G_eq is not None:
         # check the size
         nG, mG = G_eq.shape
-        if mG != L:
+        h_eq = np.array(h_eq).reshape((-1,1))
+        if mG != L: 
             raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case Geq.shape = {}.'.format(L,G_eq.shape))
         if nG != len(h_eq):
             raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case h_eq.shape = {}.'.format(nG,len(h_eq)))    
         if Aeq is not None:
             Aeq = matrix(np.vstack((Aeq,G_eq)))
-            beq = matrix(np.hstack((beq,h_eq)))
+            beq = matrix(np.vstack((beq,h_eq)))
         else:
             Aeq = matrix(G_eq)
             beq = matrix(h_eq)
 
     #solvers.options['show_progress'] = False
     solvers_opt = ""#"glpk"
     #solvers.options['glpk'] = dict(msg_lev='GLP_MSG_OFF')
     # solvers_opt.options['solver'] = 'mosek' # 'glpk'
 
+    linprog_count = 0
+
     solvers_opt={'tm_lim': 100000, 'msg_lev': 'GLP_MSG_OFF', 'it_lim':10000}
 
     y_vert, x_p = [],[]
     for i in range(m):
+        linprog_count = linprog_count + 2
         c = matrix((u[:,i].T).dot(M))
         res = cvxopt.glpk.lp(c=-c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
-        if res[1]:
+        if res[1] is not None:
             y_vert = stack(y_vert, res[1],'h')
         res = cvxopt.glpk.lp(c=c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
-        if res[1]:
+        if res[1] is not None:
             y_vert = stack(y_vert, res[1],'h')
     x_p  = M.dot(y_vert) + x_bias
     z_vert = B.dot(y_vert) + bias
 
     # if one directin only
     if m == 1:
         return x_p, np.array([[1],[-1]]), np.array([[np.max(x_p)],[-np.max(x_p)]]), [], y_vert, z_vert
 
 
     try:
         hull = ConvexHull(x_p.T, incremental=True)
     except:
+        if(verbose): print("ICHM: Convex hull issue at init - continuing with a QJ option!")
         try:
             hull = ConvexHull(x_p.T, incremental=True, qhull_options="QJ")
         except:
+            if(verbose): print("ICHM: Search stopped prematurely - inital convex hull not found!")
             z_vert = B.dot(y_vert) + bias
             x_vert  = M.dot(y_vert) + x_bias
             return x_vert, [], [], [], [], []
 
-    n_faces, n_faces_old,  = len(hull.simplices), 0
-    face_final, cnt = {}, 2*m
-
-    while n_faces > n_faces_old:
-        n_faces_old = n_faces
+    # dictionary of face normals
+    face_final = {}
+    # set the initial max delta to some random value higher than the tolerance
+    max_delta = tol*100 
+    # iterate until the maxima
+    # insteadl distance between the target and 
+    # the aproximated polytope is under tol value
+    while max_delta > tol and linprog_count <= max_iter:
         
         x_center = np.mean(x_p,axis=1)
         
         y_vert_new = []
-
+        max_delta = 0
         for face, equation in zip(hull.simplices,hull.equations):
             
             # create a string index of the face 
             # this value is used as a hash map index
             # to store dyamically the faces that have been found as final
-            face_key = str(np.sort(face))
+            face_key = str(np.sort(equation))
             # check if this face (face index) has been found as final
             if face_key in face_final.keys():
-                continue; 
+                continue
+            
+            # update linprog counter
+            linprog_count = linprog_count + 1
 
             # calculate the normal vector to the face
             face_normal = equation[:-1]
 
             # calculate the projection of the centroid on the normal of the face
             # to figure out the direction of the LP
             dir = np.mean(face_normal.dot(x_p[:,face[0]] - x_center)) > 0
@@ -227,51 +271,58 @@
             c = matrix((face_normal).dot(M))
             if dir:
                 res = cvxopt.glpk.lp(c=-c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
             else:
                 res = cvxopt.glpk.lp(c=c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
                 
             res = np.array(res[1])
-            # a simple counter of linprog execuitions
-            cnt = cnt+1
 
             # vertex distance from the face
             distance = np.abs( face_normal.dot( M.dot(res) + x_bias) -face_normal.dot( x_p[:,face[0]] ))
+
             if distance > tol:
                 # new vertex found
                 y_vert_new = stack(y_vert_new, res, 'h')
             else:
                 face_final[face_key] = 1
+            
+            if distance > max_delta:
+                max_delta = distance
 
         if len(y_vert_new):
             x_p_new = M.dot(y_vert_new) + x_bias
+
+            x_p  = stack(x_p, x_p_new,'h')
+            y_vert = stack(y_vert, y_vert_new,'h')
+
+            z_new = B.dot(y_vert_new) + bias
+            z_vert = stack(z_vert, z_new,'h')
+
             try:
                 hull.add_points(x_p_new.T)
             except:
+                if(verbose): print("ICHM: Convex hull issue - continuing with a QJ option!")
                 hull = ConvexHull(x_p.T, incremental=True, qhull_options="QJ")
             
-            y_vert = stack(y_vert, y_vert_new,'h')
-            x_p  = stack(x_p, x_p_new,'h')
+        elif max_delta > tol: 
+            if(verbose): print("ICHM: Search stopped prematurely - search stuck at precision: {}!".format(max_delta))
+            # raise error here instead
+            break 
 
-            z_new = B.dot(y_vert_new) + bias
-            z_vert = stack(z_vert, z_new,'h')
- 
-        n_faces = len(hull.simplices)
-  
+    if linprog_count >= max_iter:
+        if(verbose): print("ICHM: Max iteration number reached: {}".format(max_iter))
 
-    return x_p, hull.equations[:,:-1], hull.equations[:,-1], hull.simplices, y_vert, z_vert
+    return hull.points.T, hull.equations[:,:-1], -hull.equations[:,-1], hull.simplices, y_vert, z_vert
 
 
 def hyper_plane_shift_method(A, x_min, x_max, tol = 1e-15):
     """
     Hyper plane shifting method implementation used to solve problems of a form:
 
-    .. math:: y = Ax
-    .. math:: x_min <= x <= x_max
-
+    .. math:: P = \{y~ |~y = Ax, \quad x_{min} \leq x \leq x_{max}\}
 
     Note:
         *Gouttefarde M., Krut S. (2010) Characterization of Parallel Manipulator Available Wrench Set Facets. In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht*
 
 
     This algorithm can be used to calcualte acceleration polytope, velocity polytoe and even 
     polytope of the joint achievable joint torques based on the muscle forces
@@ -283,19 +334,32 @@
         
     Returns
     --------
         H(list):  
             matrix of half-space representation `Hx<d`
         d(list): 
             vector of half-space representation `Hx<d`
+
+    
+    :raises ValueError: if the limits are not of the same size as the projection matrix
+    :raises ValueError: if the limits are not of the same size
+
     """
 
     H = []
     d = []
 
+    # check if the limits are the same size
+    if len(x_min) != len(x_max):
+        raise ValueError("x_min and x_max must be of the same size {} != {}".format(len(x_min),len(x_max)))
+    # check if the limits are the same size as the projection matrix
+    if len(x_min) != A.shape[1]:
+        raise ValueError("x_min and x_max must be of the same size as the projection matrix {} != {}".format(len(x_min),A.shape[1]))
+    
+
     x_min = np.array(x_min).reshape((-1,1))
     x_max = np.array(x_max).reshape((-1,1))
     A = np.array(A)
     # Combination of n x n-1 columns of A
     #C = nchoosek(1:size(A,2),size(A,1)-1)
     C = np.array(list(itertools.combinations(range(A.shape[1]),A.shape[0]-1)))
     for comb in C:
@@ -330,21 +394,19 @@
     return H, d
 
 # maximal end effector force
 def vertex_enumeration_auctus(A, b_max, b_min, b_bias = None):
     """
     Efficient vertex enumeration algorithm for a problem of a form:
     
-    .. math:: Ax = b
-    .. math:: b_{min} \leq b \leq b_{max}
+    .. math:: P = \{x~ |~Ax = b, \quad b_{min} \leq b \leq b_{max}\}
 
-    Optional (if b_bias added): 
+    Optional (bias :math:`b_{bias}` can be added): 
     
-    .. math:: Ax = b - b_{bias}
-    .. math:: b_{min} \leq b \leq b_{max}
+    .. math:: P = \{x~ |~Ax = b - b_{bias}, \quad b_{min} \leq b \leq b_{max}\}
 
     Note:
         On-line force capability evaluation based on efficient polytope vertex search
         by A. Skuric, V. Padois, D. Daney
 
     Args:
         A:      system matrix A
@@ -352,14 +414,19 @@
         b_min:  minimal b  
         b_bias: b bias vector ( offset from 0 )
 
     Returns
     --------
         x_vertex(list): vertices of the polytope
         b_vartex(list): b values producing x_vertex
+
+    :raises ValueError: if the A matrix dimensions are not valid  
+    :raises ValueError: if the b_min and b_max are not of the same size as the A matrix
+    :raises ValueError: if the b_bias is not of the same size as the A matrix
+
     """ 
     # Size calculation
     n, m = A.shape
     if m > n:
         raise ValueError('Matrix dimensions must be n >= m.  In your case n:'+str(n)+' m:'+str(m))
 
     if n!= len(b_max) or n!= len(b_min):
@@ -382,15 +449,15 @@
     V2 = np.array(V.transpose()[:,m:])
 
     # A matrix pseudo inverse
     A_inv = np.linalg.pinv(A)
 
     # matrix of axis vectors - for polytope search
     T_vec = np.diagflat(b_max-b_min)
-    T_min = np.matlib.repmat(b_min - b_bias,1,2**m)
+    T_min = np.tile(b_min - b_bias,(1,2**m))
     b_max_bias = b_max - b_bias
 
     # all the face origin vector combiantions
     fixed_vectors_combinations = np.array(list(itertools.combinations(range(n),m)))
     permutations = np.array(list(itertools.product([0, 1], repeat=m))).T
 
     x_vertex = []
@@ -443,16 +510,42 @@
     
     # only unique vertices
     b_vertex = np.unique(np.around(b_vertex,7), axis=1)
     # calculate the forces based on the vertex torques
     x_vertex = A_inv.dot( b_vertex )
     return x_vertex, b_vertex
 
+def chebyshev_center(A,b):
+    """
+    Calculating chebyshev center of a polytope given the half-space representation
 
-def hsapce_to_vertex(H,d):
+    https://pageperso.lis-lab.fr/~francois.denis/IAAM1/scipy-html-1.0.0/generated/scipy.spatial.HalfspaceIntersection.html
+
+    Args:
+        A(list):  
+            matrix of half-space representation `Ax<b`
+        b(list): 
+            vector of half-space representation `Ax<b`
+    Returns:
+        center(array): returns a chebyshev center of the polytope
+    """
+    # calculate the certices
+    Ab_mat = np.hstack((np.array(A),-np.array(b)))
+
+    # calculating chebyshev center
+    norm_vector = np.reshape(np.linalg.norm(Ab_mat[:, :-1], axis=1), (A.shape[0], 1))
+    c = np.zeros((Ab_mat.shape[1],))
+    c[-1] = -1
+    G = matrix(np.hstack((Ab_mat[:, :-1], norm_vector)))
+    h = matrix(- Ab_mat[:, -1:])
+    solvers_opt={'tm_lim': 100000, 'msg_lev': 'GLP_MSG_OFF', 'it_lim':10000}
+    res = cvxopt.glpk.lp(c=c,  G=G, h=h, options=solvers_opt)
+    return np.array(res[1][:-1]).reshape((-1,))
+
+def hspace_to_vertex(H,d):
     """
     From half-space representaiton to the vertex representation
 
     Args:
         H(list):  
             matrix of half-space representation `Hx<d`
         d(list): 
@@ -460,36 +553,62 @@
     Returns
     --------
         vertices(list)  : vertices of the polytope
         face_indexes(list) : indexes of verteices forming triangulated faces of the polytope
 
     """
     if len(H):
-        # calculate the certices
+        d = d.reshape(-1,1)
         hd_mat = np.hstack((np.array(H),-np.array(d)))
-
-        # calculating chebyshev center
-        # https://pageperso.lis-lab.fr/~francois.denis/IAAM1/scipy-html-1.0.0/generated/scipy.spatial.HalfspaceIntersection.html
-        norm_vector = np.reshape(np.linalg.norm(H[:, :-1], axis=1), (H.shape[0], 1))
-        c = np.zeros((hd_mat.shape[1],))
-        c[-1] = -1
-        A = np.hstack((hd_mat[:, :-1], norm_vector))
-        b = - hd_mat[:, -1:]
-        G = matrix(A)
-        h = matrix(b)
-        solvers_opt={'tm_lim': 100000, 'msg_lev': 'GLP_MSG_OFF', 'it_lim':10000}
-        res = cvxopt.glpk.lp(c=c,  G=G, h=h, options=solvers_opt)
-        feasible_point = np.array(res[1][:-1]).reshape((-1,))
-
+        # calculate a feasible point inside the polytope
+        feasible_point = chebyshev_center(H,d)
         # calculate the convex hull
-        hd = HalfspaceIntersection(hd_mat,feasible_point,'QJ')
-        hull = ConvexHull(hd.intersections)
+        try:
+            hd = HalfspaceIntersection(hd_mat,feasible_point)
+            hull = ConvexHull(hd.intersections)
+        except:
+            print("H2V: Convex hull issue: using QJ option! ")
+            try:
+                hd = HalfspaceIntersection(hd_mat,feasible_point,qhull_options='QJ')
+                hull = ConvexHull(hd.intersections)
+            except:
+                print("H2V: Convex hull issue: using Q0 option! ")
+                hd = HalfspaceIntersection(hd_mat,feasible_point,qhull_options='Q0')
+                hull = ConvexHull(hd.intersections)
         return hd.intersections.T, hull.simplices
 
+
+def vertex_to_hspace(vertex):
+    """
+    Function transforming vertice to half-sapoce representation using a ConvexHull algorithm
+
+    Args:
+        vertex(array):  list of verteices
+
+    Returns
+    -------
+        H(list): matrix of half-space representation `Hx<d`
+        d(list): vector of half-space representation `Hx<d`
+    """
+    hull = ConvexHull(vertex.T, qhull_options='QJ')
+    return  hull.equations[:,:-1], -hull.equations[:,-1]
+
+
+
 def vertex_to_faces(vertex):
+    """
+    Function grouping the vertices to faces using a ConvexHull algorithm
+
+
+    Args:
+        vertex(array):  list of verteices
+
+    Returns:
+        faces(array) : list of triangle faces with vertex indexes which form them
+    """
     if vertex.shape[0] == 1:
         faces = [0, 1]
     else:        
         hull = ConvexHull(vertex.T, qhull_options='QJ')
         faces = hull.simplices
     return faces
 
@@ -530,37 +649,16 @@
     else:
         return [vertices[:,face] for face in indexes]
 
 def stack(A, B, dir='v'):
     """
     Helping function enabling vertical and horisontal stacking of numpy arrays
     """
-    if not len(A):
+    if A is None or not len(A):
         return B
-    elif not len(B):
+    elif B is None or not len(B):
         return A
     elif dir == 'v':
         return  np.vstack((A, B))
     else:
         return  np.hstack((A, B))
-         
-# definition of the four_link_solver module
-if __name__ == '__main__':
-    L = 10
-    n = 5 
-    m = 3 
-    B = (np.random.rand(n,L)*2 -1)
-    A = (np.random.rand(n,m)*2 -1)
-    y_min = np.zeros(L)
-    y_max = np.ones(L)
-
-    # Ax = By
-    # s.t. y in [y_min, y_max]
-    iterative_convex_hull_method(A, B, y_min, y_max,0.1)
-    # x = By
-    # s.t. y in [y_min, y_max]
-    hyper_plane_shift_method(B, y_min, y_max)
-    # Ax = y
-    # s.t. y in [y_min, y_max]
-    y_min = np.zeros(n)
-    y_max = np.ones(n)
-    vertex_enumeration_auctus(A, y_min, y_max)
+
```

### Comparing `pycapacity-1.2.9/PKG-INFO` & `pycapacity-2.0.0/pycapacity.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,96 @@
 Metadata-Version: 2.1
 Name: pycapacity
-Version: 1.2.9
+Version: 2.0.0
 Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
-Home-page: https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity
+Home-page: https://github.com/auctus-team/pycapacity
 Author: Antun Skuric
 Author-email: antun.skuric@inria.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Framework :: Robot Framework :: Tool
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Real-time capable task-space capacity calculation python module
+# Real-time capable task-space capacity calculation python pip package
 
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
+
+
+> 📢 New version of the pycapacity package is out - version v2.0!
+> 🚨 Beware beacause there are some breaking changes in the API, please check the changelog for more details.
+
+### changelog v2.0 (05-2023)
+
+
+- polyope and ellipsoid algorithms now return `Polytope`  and `Ellipsoid`  objects (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.polytope.html))
+  - `Polytope`  class can be used as a standalone class to find  vertex, halfplane and face representation of a polytope
+- Visualisation tools improved: (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.visual.html))
+  - new `plot_polytope` function for plotting polytopes
+  - functions `plot_polytope_vertex` and `plot_polytope_faces` now can receive a polyope object
+  - function `plot_ellipsoid` now can receive a ellipsoid object
+  - better management of the `matplotlib` figures and axes, now user can provide an `ax`, `plt` or `figure` to the plotting functions
+- Added support for robot reachable workspace approximation using convex polytopes (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.reachable_space_approximation))
+- Added unit testing + continuous integration
+- improved docs with sphinx
+
+## About 
+[![PyPI package](https://img.shields.io/pypi/v/pycapacity)](https://pypi.org/project/pycapacity/) [![Tests](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml) ![](https://img.shields.io/pypi/dm/pycapacity?color=blue&label=pip%20downloads)  [![Docs](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml)
+
+<img src="https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/comparison.gif" height="250px"><img src="https://github.com/auctus-team/pycapacity/blob/master/images/human_poly.gif?raw=true" height="250px">
 
 The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
 - Robotic serial manipulators - `pycapacity.robot`
 - Human musculoskeletal models - `pycapacity.human`
 
 This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
 
 Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
 
-See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See [full API documentation and docs.](https://auctus-team.github.io/pycapacity/)
 
 ## Robotic manipulator capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/robot.png' height='300px'>
 
 For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
 - Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
 - Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
 - Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
 
 And polytopes: 
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
 - Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
+- **NEW** 📢: Reachable space of the robot with the horizon `T`  <br> `P_x = {x | x = JM(-1)tT^2/2, t_min < t < t_max,   dq_min < M^(-1)tT < dq_max,   q_min < M^(-1)tT^2/2 < q_max}`
 - Force polytopes *Minkowski sum and intersection*
 
 Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
 
+Reachable space polytope approximation is based on this paper: <br>
+[**Approximating robot reachable space using convex polytopes**](https://arxiv.org/pdf/2211.17054.pdf)<br> by Skuric, Antun, Vincent Padois, and David Daney. <br> In: Human-Friendly Robotics 2022: HFR: 15th International Workshop on Human-Friendly Robotics. Cham: Springer International Publishing, 2023.
+
+The force polytope functions have been implemented according to the paper:<br>
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
 The force polytope functions have been implemented according to the paper:<br>
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 ## Human musculoskeletal models capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/force.png' height='200px'>
 
 For the human musculoskeletal models this package implements the polytope metrics:
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
 - Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
 
 Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
@@ -77,54 +106,54 @@
 ## Polytope evaluation algorithms
 
 There are three methods implemented in this paper to resolve all the polytope calculations:
 - Hyper-plane shifting method
 - Iterative convex hull method
 - Vertex enumeration auctus
 
-All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
+All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#). 
 
 ### Hyper-plane shifting method
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 This method finds the half-space representation of the polytope of a class:
 ```
 P = {x | x = By, y_min <= y <= y_max }
 ```
 To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
+The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.hyper_plane_shift_method). 
 
 ### Iterative convex-hull method
 [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
 by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
 
 This method finds both vertex and half-space representation of the class of polytopes:
 ```
 P = {x | Ax = By, y_min <= y <= y_max }
 ``` 
 And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
 ```
 P = {x | x= Pz, Az = By, y_min <= y <= y_max }
 ``` 
 
-The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
+The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.iterative_convex_hull_method)
 
 ### Vertex enumeration auctus
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 This method finds vertex representation of the class of polytopes:
 ```
 P = {x | Ax = y, y_min <= y <= y_max }
 ``` 
 To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
+The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.vertex_enumeration_auctus)
 
 ## Installation
 
 All you need to do to install it is:
 ```
 pip install pycapacity
 ```
@@ -137,66 +166,66 @@
 import pycapacity.algorithms 
 #and/or
 import pycapacity.visual 
 ```
 
 Other way to install the code is by installing it directly from the git repo:
 ```
-pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
+pip install git+https://github.com/auctus-team/pycapacity.git
 ```
 
 ## Package API docs
 
-See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See full docs at the [link](https://auctus-team.github.io/pycapacity/)
 
 ### Modules
 
-- [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
-- [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
-- [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
-- [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
+- [`human`](https://auctus-team.github.io/pycapacity/pycapacity.human.html#module-pycapacity.human)
+- [`robot`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
+- [`algorithms`](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
+- [`visual`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
 
 ### Functions
 
 Robot metrics
-- [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
-- [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
-- [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
-- [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
-- [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
-- [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
-- [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
-- [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
-- [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
+- [`robot.acceleration_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
+- [`robot.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
+- [`robot.acceleration_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
+- [`robot.force_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
+- [`robot.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
+- [`robot.force_polytope_intersection`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_sum_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
+- [`robot.velocity_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
+- [`robot.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
+- [`robot.velocity_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
 
 Human metrics
-- [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
-- [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
-- [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
-- [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
-- [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
+- [`human.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
+- [`human.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
+- [`human.joint_torques_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
+- [`human.torque_to_muscle_force`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
+- [`human.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
 
 
 Algorithms
-- [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
-- [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
-- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
+- [`algorithms.hyper_plane_shift_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
+- [`algorithms.iterative_convex_hull_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
+- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
 
 
 Visualisation tools
-- [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
-- [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
+- [`visual.plot_polytope_faces`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
+- [`visual.plot_polytope_vertex`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
 ---
 
 ## Code examples
 
-See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
+See [`demo_notebook.ipynb`](https://github.com/auctus-team/pycapacity/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
 
 ### Randomised serial robot example
 ```python
 """
 A simple example program for 3d force polytope 
 evaluation of a randomised 6dof robot 
 """
@@ -268,7 +297,8 @@
 
 plt.tight_layout()
 plt.legend()
 plt.show()
 
 ```
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycapacity-1.2.9/setup.py` & `pycapacity-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pycapacity',
-    version='1.2.9',
+    version='2.0.0',
     author='Antun Skuric',
     author_email='antun.skuric@inria.fr',
     description='A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models',
     long_description=long_description, #'A Real-time capable robot capacity calculation module', 
     long_description_content_type="text/markdown",
-    url='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity',
+    url='https://github.com/auctus-team/pycapacity',
     license='MIT',
     packages = ['pycapacity'],
-    install_requires=['numpy','scipy','cvxopt>=1.2.6','matplotlib','plotly'],
+    install_requires=['numpy','scipy','cvxopt>=1.2.6','matplotlib'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Framework :: Robot Framework",
         "Framework :: Robot Framework :: Library",
         "Framework :: Robot Framework :: Tool"
```

### Comparing `pycapacity-1.2.9/pycapacity.egg-info/PKG-INFO` & `pycapacity-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,78 @@
-Metadata-Version: 2.1
-Name: pycapacity
-Version: 1.2.9
-Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
-Home-page: https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity
-Author: Antun Skuric
-Author-email: antun.skuric@inria.fr
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Framework :: Robot Framework :: Tool
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
+# Real-time capable task-space capacity calculation python pip package
 
-# Real-time capable task-space capacity calculation python module
 
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
-<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
+
+> 📢 New version of the pycapacity package is out - version v2.0!
+> 🚨 Beware beacause there are some breaking changes in the API, please check the changelog for more details.
+
+### changelog v2.0 (05-2023)
+
+
+- polyope and ellipsoid algorithms now return `Polytope`  and `Ellipsoid`  objects (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.polytope.html))
+  - `Polytope`  class can be used as a standalone class to find  vertex, halfplane and face representation of a polytope
+- Visualisation tools improved: (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.visual.html))
+  - new `plot_polytope` function for plotting polytopes
+  - functions `plot_polytope_vertex` and `plot_polytope_faces` now can receive a polyope object
+  - function `plot_ellipsoid` now can receive a ellipsoid object
+  - better management of the `matplotlib` figures and axes, now user can provide an `ax`, `plt` or `figure` to the plotting functions
+- Added support for robot reachable workspace approximation using convex polytopes (see [api docs](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.reachable_space_approximation))
+- Added unit testing + continuous integration
+- improved docs with sphinx
+
+## About 
+[![PyPI package](https://img.shields.io/pypi/v/pycapacity)](https://pypi.org/project/pycapacity/) [![Tests](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/python-app.yml) ![](https://img.shields.io/pypi/dm/pycapacity?color=blue&label=pip%20downloads)  [![Docs](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml/badge.svg)](https://github.com/auctus-team/pycapacity/actions/workflows/main.yml)
+
+<img src="https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/comparison.gif" height="250px"><img src="https://github.com/auctus-team/pycapacity/blob/master/images/human_poly.gif?raw=true" height="250px">
 
 The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
 - Robotic serial manipulators - `pycapacity.robot`
 - Human musculoskeletal models - `pycapacity.human`
 
 This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
 
 Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
 
-See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See [full API documentation and docs.](https://auctus-team.github.io/pycapacity/)
 
 ## Robotic manipulator capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/robot.png' height='300px'>
 
 For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
 - Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
 - Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
 - Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
 
 And polytopes: 
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
 - Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
+- **NEW** 📢: Reachable space of the robot with the horizon `T`  <br> `P_x = {x | x = JM(-1)tT^2/2, t_min < t < t_max,   dq_min < M^(-1)tT < dq_max,   q_min < M^(-1)tT^2/2 < q_max}`
 - Force polytopes *Minkowski sum and intersection*
 
 Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
 
+Reachable space polytope approximation is based on this paper: <br>
+[**Approximating robot reachable space using convex polytopes**](https://arxiv.org/pdf/2211.17054.pdf)<br> by Skuric, Antun, Vincent Padois, and David Daney. <br> In: Human-Friendly Robotics 2022: HFR: 15th International Workshop on Human-Friendly Robotics. Cham: Springer International Publishing, 2023.
+
+The force polytope functions have been implemented according to the paper:<br>
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
 The force polytope functions have been implemented according to the paper:<br>
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 ## Human musculoskeletal models capacity metrics
-<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
+<img src='https://raw.githubusercontent.com/auctus-team/pycapacity/master/images/force.png' height='200px'>
 
 For the human musculoskeletal models this package implements the polytope metrics:
 - Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
 - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
 - Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
 
 Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
@@ -77,54 +88,54 @@
 ## Polytope evaluation algorithms
 
 There are three methods implemented in this paper to resolve all the polytope calculations:
 - Hyper-plane shifting method
 - Iterative convex hull method
 - Vertex enumeration auctus
 
-All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
+All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#). 
 
 ### Hyper-plane shifting method
 [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
 by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
 
 This method finds the half-space representation of the polytope of a class:
 ```
 P = {x | x = By, y_min <= y <= y_max }
 ```
 To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
+The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.hyper_plane_shift_method). 
 
 ### Iterative convex-hull method
 [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
 by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
 
 This method finds both vertex and half-space representation of the class of polytopes:
 ```
 P = {x | Ax = By, y_min <= y <= y_max }
 ``` 
 And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
 ```
 P = {x | x= Pz, Az = By, y_min <= y <= y_max }
 ``` 
 
-The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
+The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.iterative_convex_hull_method)
 
 ### Vertex enumeration auctus
 [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
 by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
 
 This method finds vertex representation of the class of polytopes:
 ```
 P = {x | Ax = y, y_min <= y <= y_max }
 ``` 
 To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
 
-The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
+The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#pycapacity.algorithms.vertex_enumeration_auctus)
 
 ## Installation
 
 All you need to do to install it is:
 ```
 pip install pycapacity
 ```
@@ -137,66 +148,66 @@
 import pycapacity.algorithms 
 #and/or
 import pycapacity.visual 
 ```
 
 Other way to install the code is by installing it directly from the git repo:
 ```
-pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
+pip install git+https://github.com/auctus-team/pycapacity.git
 ```
 
 ## Package API docs
 
-See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+See full docs at the [link](https://auctus-team.github.io/pycapacity/)
 
 ### Modules
 
-- [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
-- [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
-- [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
-- [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
+- [`human`](https://auctus-team.github.io/pycapacity/pycapacity.human.html#module-pycapacity.human)
+- [`robot`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
+- [`algorithms`](https://auctus-team.github.io/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
+- [`visual`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
 
 ### Functions
 
 Robot metrics
-- [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
-- [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
-- [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
-- [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
-- [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
-- [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
-- [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
-- [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
-- [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
-- [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
+- [`robot.acceleration_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
+- [`robot.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
+- [`robot.acceleration_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
+- [`robot.force_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
+- [`robot.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
+- [`robot.force_polytope_intersection`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_sum_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
+- [`robot.velocity_ellipsoid`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
+- [`robot.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
+- [`robot.velocity_polytope_withfaces`](https://auctus-team.github.io/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
 
 Human metrics
-- [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
-- [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
-- [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
-- [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
-- [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
+- [`human.acceleration_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
+- [`human.force_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
+- [`human.joint_torques_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
+- [`human.torque_to_muscle_force`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
+- [`human.velocity_polytope`](https://auctus-team.github.io/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
 
 
 Algorithms
-- [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
-- [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
-- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
+- [`algorithms.hyper_plane_shift_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
+- [`algorithms.iterative_convex_hull_method`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
+- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.github.io/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
 
 
 Visualisation tools
-- [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
-- [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
+- [`visual.plot_polytope_faces`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
+- [`visual.plot_polytope_vertex`](https://auctus-team.github.io/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
 ---
 
 ## Code examples
 
-See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
+See [`demo_notebook.ipynb`](https://github.com/auctus-team/pycapacity/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
 
 ### Randomised serial robot example
 ```python
 """
 A simple example program for 3d force polytope 
 evaluation of a randomised 6dof robot 
 """
@@ -267,8 +278,7 @@
 plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
 
 plt.tight_layout()
 plt.legend()
 plt.show()
 
 ```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

