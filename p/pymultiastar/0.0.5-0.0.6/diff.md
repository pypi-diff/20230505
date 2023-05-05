# Comparing `tmp/pymultiastar-0.0.5.tar.gz` & `tmp/pymultiastar-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultiastar-0.0.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pymultiastar-0.0.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pymultiastar-0.0.5.tar` & `pymultiastar-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,59 @@
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.gitignore
--rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/CMakeLists.txt
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/LICENSE
--rw-r--r--   0        0        0     3429 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/README.md
--rw-r--r--   0        0        0    99021 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/assets/imgs/tradeoff.png
--rw-r--r--   0        0        0     7688 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/Makefile
--rw-r--r--   0        0        0     9488 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/conf.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/index.rst
--rw-r--r--   0        0        0     7265 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/make.bat
--rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/python_example.rst
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/__init__.py
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/log.py
--rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_maze_2d.py
--rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_scenarios.py
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_simple_demo.py
--rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_simple_world_3d.py
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/noxfile.py
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/output/.gitignore
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/scripts/upload.sh
--rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/include/pymultiastar.hpp
--rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/main.cpp
--rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/__init__.py
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/_core.pyi
--rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/__init__.py
--rw-r--r--   0        0        0     8307 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/geoplanner.py
--rw-r--r--   0        0        0     4844 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/helper.py
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/log.py
--rw-r--r--   0        0        0     2626 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/types.py
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/types.py
--rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/img2d_helpers.py
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/log.py
--rw-r--r--   0        0        0     5375 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/vis3d_helpers.py
--rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar.cpp
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/.gitignore
--rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/maze_large.png
--rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/maze_small.png
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/.gitignore
--rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/annarbor/plan.json
--rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/annarbor/voxel_map.npy
--rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/newyork/plan.json
--rw-r--r--   0        0        0 68625128 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/newyork/voxel_map.npy
--rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/test_basic.py
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/test_geo_helper.py
--rw-r--r--   0        0        0     4488 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/CMakeLists.txt
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3873 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/README.md
+-rw-r--r--   0        0        0   585757 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/assets/imgs/newyork_map.png
+-rw-r--r--   0        0        0   578063 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/assets/imgs/newyork_solved_1.png
+-rw-r--r--   0        0        0   543823 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/assets/imgs/newyork_solved_2.png
+-rw-r--r--   0        0        0    99021 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/assets/imgs/tradeoff.png
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/contributing.md
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/contributing.md
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/css/material.css
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/css/style.css
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/index.md
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/license.md
+-rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/tutorials/geoplanner.md
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/docs/tutorials/simple.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/__init__.py
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/log.py
+-rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/run_maze_2d.py
+-rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/run_scenarios.py
+-rw-r--r--   0        0        0     1202 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/run_simple_demo.py
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/examples/run_simple_world_3d.py
+-rw-r--r--   0        0        0     1854 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/noxfile.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/output/.gitignore
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/scripts/upload.sh
+-rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/include/pymultiastar.hpp
+-rw-r--r--   0        0        0     3063 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/main.cpp
+-rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/__init__.py
+-rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/_core.pyi
+-rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/geoplanner/__init__.py
+-rw-r--r--   0        0        0     8307 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/geoplanner/geoplanner.py
+-rw-r--r--   0        0        0     4970 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/geoplanner/helper.py
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/geoplanner/log.py
+-rw-r--r--   0        0        0     2626 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/geoplanner/types.py
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/types.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/visualization/__init__.py
+-rw-r--r--   0        0        0     1727 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/visualization/img2d_helpers.py
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/visualization/log.py
+-rw-r--r--   0        0        0     6549 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar/visualization/vis3d_helpers.py
+-rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/src/pymultiastar.cpp
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/.gitignore
+-rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/maze_large.png
+-rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/maze_small.png
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/world/.gitignore
+-rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/world/annarbor/plan.json
+-rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/world/annarbor/voxel_map.npy
+-rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/world/newyork/plan.json
+-rw-r--r--   0        0        0 68625128 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/fixtures/world/newyork/voxel_map.npy
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/test_basic.py
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/tests/test_geo_helper.py
+-rw-r--r--   0        0        0     5601 2022-11-09 12:37:21.000000 pymultiastar-0.0.6/PKG-INFO
```

### Comparing `pymultiastar-0.0.5/.github/workflows/pip.yml` & `pymultiastar-0.0.6/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/.github/workflows/wheels.yml` & `pymultiastar-0.0.6/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/.gitignore` & `pymultiastar-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/.pre-commit-config.yaml` & `pymultiastar-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/LICENSE` & `pymultiastar-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/README.md` & `pymultiastar-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Multi-Goal A-star
 
-This repo contains code to search for **multiple** goals with **heterogenous** values using a 3D A* **discrete** planner. The majority of the code is written in C++ with Python bindings. This planner was used in the paper [Map-Based Planning for Small Unmanned Aircraft Rooftop Landing](https://drive.google.com/file/d/1Sy0I8I8nsuy1xv1tFh_W6_Gazcp7pW9M/view?usp=share_link)
+This repo contains code to search for **multiple** goals with **heterogenous** values using a 3D A-star **discrete** planner. The majority of the code is written in C++ with Python bindings. This planner was used in the paper [Map-Based Planning for Small Unmanned Aircraft Rooftop Landing](https://drive.google.com/file/d/1Sy0I8I8nsuy1xv1tFh_W6_Gazcp7pW9M/view?usp=share_link)
 
 **What do you mean by discrete?**
 
-The map provided should be a 3D voxel grid(i, j, k), which the planner searches. This grid is a 3D Numpy array. A cell with the value 0.0 is considered free space. A cell with the value 1.0 is considered an obstacle and cannot be traversed (this value is configurable). Values between 0.0 and 1.0 can be traversed but with a penalty (penalty weight is configurable).
+The map provided should be a 3D voxel grid(i, j, k), a 3D NumPy array, which the planner searches. A cell with the value 0.0 is considered free space. A cell with the value 1.0 is considered an obstacle and cannot be traversed (this value is configurable). Values between 0.0 and 1.0 can be traversed but with a penalty (penalty weight is configurable).
 
 **What do you mean by multiple goals with heterogenous values?**
 
-A normal A* planner has a start location and one goal. This Multi-Goal planner allows you to provide multiple goal cells each having different values. Goals with lower values are more desirable. This planner will try to find the optimal **goal** *and* **path** which minimizes an objective function. It must be understood that the planner doesn't just find a path. It finds the goal and the corresponding optimal path that minimizes some larger objective function. 
+A normal A-star planner has a start location and one goal. This Multi-Goal planner allows you to provide multiple goal cells each having different values. Goals with lower values are more desirable. This planner will try to find the optimal **goal** *and* **path** which minimizes an objective function. It must be understood that the planner doesn't just find a path. It finds the goal and the corresponding optimal path that minimizes some larger objective function. 
 
 **What is the objective function?**
 
 The objective function is the minimization of total risk ($r_t$), which is the combination of path risk ($r_p$) and goal risk $r_g$. In my research the goals were landing sites, therefore I called the latter landing site risk $r_l$. 
 Below is an excerpt from my paper that discusses this trade-off between objectives:
 
     The figure below shows an example Pareto frontier that minimizes two objectives: landing
@@ -24,15 +24,15 @@
     each objective must be constructed to select a final choice. A linear weighting scheme
     is used for these purposes
 
 $$
 r_t = w_l \cdot r_l + w_p · r_p
 $$
 
-![Tradeoff](./assets/imgs/tradeoff.png)
+![Tradeoff](https://raw.githubusercontent.com/JeremyBYU/pymultiastar/master/assets/imgs/tradeoff.png)
 
 **What precisely are these two objectives and how do they relate to the planner?**
 
 See the following sections in the paper linked above: 
 
 - Definition of Path **Cost**: Section 1.3.2, Equations 1.6-1.8
 - Definition of Path **Risk**: Section 1.5, Equation 1.17
@@ -47,12 +47,16 @@
     1. This planner only knows about Voxel Grid to traverse.
 2. Geographically Aware Planner - `pip install pymultiastar[geo]` - This also exposes the class `GeoPlanner`
     1. This is a geographically aware wrapper around `PyMultiAStar`. You give a georeferenced voxel map and start conditions in GPS and landing sites in GPS and it will do the conversions between GPS to voxel cell for you. 
 
 
 ## How to use
 
-TBD
+Below are some examples:
+
+1. `run_simple_world_3d.py`. Shows a very simple example of a small 3D world with multiple goals.
+2. `run_maze_2d.py` - Demonstrates that 2D A-star path planning is a subset of the Multi-Goal Planner. It loads a 2D image of a maze as a single slice in a 3D world and has only 1 goal. 
+3. `run_scenarios.py` - Shows how to use the GeoPlanner and plan in a 3D world.
 
 ## Notes
 
 inside pymultiastar map data - (i,j,k) is the row, column, depth
```

### Comparing `pymultiastar-0.0.5/assets/imgs/tradeoff.png` & `pymultiastar-0.0.6/assets/imgs/tradeoff.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/examples/run_maze_2d.py` & `pymultiastar-0.0.6/examples/run_maze_2d.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/examples/run_scenarios.py` & `pymultiastar-0.0.6/examples/run_scenarios.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/examples/run_simple_demo.py` & `pymultiastar-0.0.6/examples/run_simple_demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import pymultiastar as pmstar
 
 
 def main():
     # create our map
     # pymultiastar expects a three dimensional map in f32
     map_3d = np.zeros(shape=(3,3,3), dtype='f4') 
-    start_cell = [0,0,0]
-    goal_cells = [([0,0,1], 6), ([2,2,2], 1), ([2,2,1], 4)]
+    start_cell = (0,0,0)
+    goal_cells = [((0,0,1), 6), ((2,2,2), 1), ((2,2,1), 4)]
 
     # parameters to initialize multi goal a-star search
     params = dict(
-        map_res=1.0,
-        obstacle_value=1.0, # map ranges from 0-1 values. An obstacle will be the value 1.0
+        allow_diag=True, # allow diagonal movement
+        map_res=1.0, # the length of a voxel cell in meters
+        obstacle_value=1.0, # map ranges from 0.0-1.0 values. An obstacle will be the value 1.0
         normalizing_path_cost = 3.0, # normalize path distance by dividing by this number
-        goal_weight = 0.5, 
-        path_weight = 0.5,
+        goal_weight = 0.5, # weighting between path goal risk and path risk
+        path_weight = 0.5, # weighting between path goal risk and path risk
+        keep_nodes=False, # optimization strategy to prevent more dynamic memory allocation
+        path_w0=1.0 # weighting for potential field in the maze
     )
     planner = pmstar.PyMultiAStar(map_3d, **params)
 
     path, meta = planner.search_multiple(start_cell, goal_cells)
     print(f"path: {path}, meta: {meta}")
 
 if __name__ == "__main__":
```

### Comparing `pymultiastar-0.0.5/examples/run_simple_world_3d.py` & `pymultiastar-0.0.6/examples/run_simple_world_3d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-import open3d as o3d
-import matplotlib as mpl
 import numpy as np
 
 import pymultiastar as pmstar
-from pymultiastar.visualization.vis3d_helpers import create_map, create_pcd_map
+from pymultiastar.visualization.vis3d_helpers import create_map, create_pcd_map, visualize_world
 
 
 def main():
     map_3d = create_map()
-    geoms = create_pcd_map(map_3d) 
 
-    def init(vis):
-        vis.show_ground = True
-        vis.ground_plane = o3d.visualization.rendering.Scene.GroundPlane.XY
-
-    start_cell = [0,0,1]
+    start_cell = (0,0,1)
     goal_cells = [([9, 9, 3], 2), ([5,9,2], 4)]
 
     # this is the diagonal from the origin of the map to the top right (opposite corners of a cube)
     normalizing_path_cost = np.sqrt(10**2 + 10**2 + 5**2)
 
     params = dict(
         map_res=1.0,
         obstacle_value=1.0, # map ranges from 0-1 values. An obstacle will be the value 1.0
         normalizing_path_cost = normalizing_path_cost, # normalize path distance by dividing by this number
         goal_weight = 0.5, 
         path_weight = 0.5,
     )
     planner = pmstar.PyMultiAStar(map_3d, **params)
     path, meta = planner.search_multiple(start_cell, goal_cells)
-
-
     print(f"path: {path}, meta: {meta}")
-
-    o3d.visualization.draw([*geoms], lookat=[0, 0, 0], eye=[0, -20, 30], up=[0, 0, 1], title="World Viewer", on_init=init, show_ui=True)
+    
+    geoms = create_pcd_map(map_3d, ds_voxel_size=1.0)
+    visualize_world(geoms, point_size=25)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pymultiastar-0.0.5/pyproject.toml` & `pymultiastar-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymultiastar"
-version = "0.0.5"
+version = "0.0.6"
 description="Multi-goal A* with cpp bindings to python"
 readme = "README.md"
 authors = [
   { name = "Jeremy Castagno", email = "jeremybyu@gmail.com" },
 ]
 requires-python = ">=3.9"
 classifiers = [
@@ -21,24 +21,34 @@
 [build-system]
 requires = ["scikit-build-core>=0.3.3", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project.optional-dependencies]
 geo = ["pyproj>=3.0"]
 test = ["pytest", "Pillow", "pyproj>=3.0"]
+docs = ["mkdocstrings[python]", "mkdocs-autorefs>=0.3.1",
+      "pymdown-extensions>=6.3", "mkdocs>=1.3",
+      "mkdocs-coverage>=0.2", "mkdocs-gen-files>=0.3",
+      "mkdocs-literate-nav>=0.4","mkdocs-material>=7.3",
+      "mkdocs-section-index>=0.3", "mkdocstrings-python>=0.5.1",
+      "markdown-callouts>=0.2","markdown-exec>=0.5"]
+
 dev = ["black", "open3d>=0.17", "matplotlib", 
       "rich", "typer", "ipdb", "Pillow", 
       "pymultiastar[geo,test]"]
 
+
 [tool.scikit-build]
 wheel.expand-macos-universal-tags = true
 
 [tool.cibuildwheel]
 test-command = "pytest {project}/tests"
 test-extras = ["test"]
 test-skip = ["*universal2:arm64"]
 build-verbosity = 1
 
+[tool.setuptools]
+package-dir = {"" = "src"}
 
 [tool.ruff]
 line-length = 100
 target-version = "py310"
```

### Comparing `pymultiastar-0.0.5/src/include/pymultiastar.hpp` & `pymultiastar-0.0.6/src/include/pymultiastar.hpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/src/pymultiastar/geoplanner/geoplanner.py` & `pymultiastar-0.0.6/src/pymultiastar/geoplanner/geoplanner.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/src/pymultiastar/geoplanner/helper.py` & `pymultiastar-0.0.6/src/pymultiastar/geoplanner/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,127 +4,144 @@
 import numpy as np
 from pyproj import Transformer
 
 from ..types import Cell
 from .types import GPS, ArrayFloatMxNxK, Coord, CoordPath, LandingSite, VoxelMeta
 from .log import logger
 
-def convert_cost_map_to_float(cost_map, reverse_yaxis=True, normalize=True, set_max_value_to_inf=True):
+
+def convert_cost_map_to_float(
+    cost_map, reverse_yaxis=True, normalize=True, set_max_value_to_inf=True
+) -> np.ndarray:
     """Will convert a uint8 cost map to a float32
 
 
     Note, the normal expectation is that the dimension are like so [y, x, z]
     Also the y-axis is growing DOWN, like an image, if this was generated from https://bitbucket.org/umich_a2sys/create-voxel/src/master/
 
 
     Args:
-        cost_map (np.ndarray): Three dimenstional cost map
+        cost_map (np.ndarray): Three dimensional cost map
         reverse_yaxis (bool, optional): Will reverse y axes of the map. Defaults to True.
         normalize (bool, optional): Will normalize cost from 0 to 1.0. Defaults to True.
         set_max_value_to_inf (bool, optional): All max values will be mapped to np.inf. Defaults True.
 
     Returns:
         np.ndarray: Your 3D cost map in float32
     """
     cost_map = cost_map.astype(np.float32)
     if reverse_yaxis:
-        cost_map = np.flip(cost_map, 0) # reverses the y-axis
+        cost_map = np.flip(cost_map, 0)  # reverses the y-axis
     if normalize:
         max_value = np.max(cost_map)
-        cost_map = cost_map / max_value # convert to float32
+        cost_map = cost_map / max_value  # convert to float32
     if set_max_value_to_inf:
         cost_map[cost_map == 1.0] = np.inf
     return cost_map
 
 
-def prepare_planning_args_optimized(start_position:GPS, ls_list:List[LandingSite], transformer:Transformer):
+def prepare_planning_args_optimized(
+    start_position: GPS, ls_list: List[LandingSite], transformer: Transformer
+):
     """Prepares a list of landing sites formatted as a dictionary to be sent to a Path Planner
     Data is in x, y, height all in meters"""
-    projected_position:Tuple[float, float, float] = transformer.transform(*start_position.to_array())
-    projected_goal_positions:List[Tuple[Tuple[float, float, float], float]] = [(transformer.transform(*ls.centroid.to_array()), ls.landing_site_risk)
-                        for ls in ls_list]
+    projected_position: Tuple[float, float, float] = transformer.transform(
+        *start_position.to_array()
+    )
+    projected_goal_positions: List[Tuple[Tuple[float, float, float], float]] = [
+        (transformer.transform(*ls.centroid.to_array()), ls.landing_site_risk)
+        for ls in ls_list
+    ]
 
     return projected_position, projected_goal_positions
 
 
-def voxel_projected_to_cell(coord:Coord, voxel_meta:VoxelMeta) -> Cell:
-
-    x_meters = coord[0] - voxel_meta['xmin']
-    y_meters = coord[1] - voxel_meta['ymin']
-    z_meters = coord[2] - voxel_meta['zmin']
-
-    j = max(min(int(round(
-        (x_meters - voxel_meta['xres'] / 2) / voxel_meta['xres'])), voxel_meta['ncols'] - 1), 0)  # cols
-    i = max(min(int(round(
-        (y_meters - voxel_meta['yres'] / 2) / voxel_meta['yres'])), voxel_meta['nrows'] - 1), 0)  # rows
-
-    k = max(min(
-        int(round((z_meters) / voxel_meta['zres'])), voxel_meta['nslices'] - 1), 0)  # depth
+def voxel_projected_to_cell(coord: Coord, voxel_meta: VoxelMeta) -> Cell:
+    x_meters = coord[0] - voxel_meta["xmin"]
+    y_meters = coord[1] - voxel_meta["ymin"]
+    z_meters = coord[2] - voxel_meta["zmin"]
+
+    j = max(
+        min(
+            int(round((x_meters - voxel_meta["xres"] / 2) / voxel_meta["xres"])),
+            voxel_meta["ncols"] - 1,
+        ),
+        0,
+    )  # cols
+    i = max(
+        min(
+            int(round((y_meters - voxel_meta["yres"] / 2) / voxel_meta["yres"])),
+            voxel_meta["nrows"] - 1,
+        ),
+        0,
+    )  # rows
+
+    k = max(
+        min(int(round((z_meters) / voxel_meta["zres"])), voxel_meta["nslices"] - 1), 0
+    )  # depth
 
     return (i, j, k)
 
 
-def voxel_cell_to_projected(coord:Cell, voxel_meta:VoxelMeta) -> Coord:
-    x_meters:float = float(coord[1] * voxel_meta['xres'] + \
-        voxel_meta['xmin'])
-    y_meters:float = float(coord[0] * voxel_meta['yres'] + \
-        voxel_meta['ymin'])
-    z_meters:float = float(coord[2] * voxel_meta['zres'] + \
-        voxel_meta['zmin'])
+def voxel_cell_to_projected(coord: Cell, voxel_meta: VoxelMeta) -> Coord:
+    x_meters: float = float(coord[1] * voxel_meta["xres"] + voxel_meta["xmin"])
+    y_meters: float = float(coord[0] * voxel_meta["yres"] + voxel_meta["ymin"])
+    z_meters: float = float(coord[2] * voxel_meta["zres"] + voxel_meta["zmin"])
 
     return (x_meters, y_meters, z_meters)
 
-def voxel_cell_to_projected_zero_origin(coord:Cell, voxel_meta:VoxelMeta) -> Coord:
-    x_meters:float = float(coord[1] * voxel_meta['xres'])
-    y_meters:float = float(coord[0] * voxel_meta['yres'])
-    z_meters:float = float(coord[2] * voxel_meta['zres'])
+
+def voxel_cell_to_projected_zero_origin(coord: Cell, voxel_meta: VoxelMeta) -> Coord:
+    x_meters: float = float(coord[1] * voxel_meta["xres"])
+    y_meters: float = float(coord[0] * voxel_meta["yres"])
+    z_meters: float = float(coord[2] * voxel_meta["zres"])
 
     return (x_meters, y_meters, z_meters)
 
 
-def get_free_neighbor_cell(cell:Cell, cost_map:ArrayFloatMxNxK):
+def get_free_neighbor_cell(cell: Cell, cost_map: ArrayFloatMxNxK):
     neighbors = [
-        (cell[0], cell[1], cell[2] + 1), # z-up
-        (cell[0] + 1, cell[1], cell[2]), # y-up
-        (cell[0] - 1, cell[1], cell[2]), # y-down
-        (cell[0], cell[1] + 1, cell[2]), # x-right
-        (cell[0], cell[1] - 1, cell[2]), # x-left
-        (cell[0] + 1, cell[1], cell[2] + 1), # y-up, z-up
-        (cell[0] - 1, cell[1], cell[2] + 1), # y-down, z-up
-        (cell[0], cell[1] + 1, cell[2] + 1), # x-right, z-up
-        (cell[0], cell[1] - 1, cell[2] + 1), # x-left, z-up
+        (cell[0], cell[1], cell[2] + 1),  # z-up
+        (cell[0] + 1, cell[1], cell[2]),  # y-up
+        (cell[0] - 1, cell[1], cell[2]),  # y-down
+        (cell[0], cell[1] + 1, cell[2]),  # x-right
+        (cell[0], cell[1] - 1, cell[2]),  # x-left
+        (cell[0] + 1, cell[1], cell[2] + 1),  # y-up, z-up
+        (cell[0] - 1, cell[1], cell[2] + 1),  # y-down, z-up
+        (cell[0], cell[1] + 1, cell[2] + 1),  # x-right, z-up
+        (cell[0], cell[1] - 1, cell[2] + 1),  # x-left, z-up
     ]
     for n in neighbors:
         try:
             if cost_map[n[0], n[1], n[2]] != np.inf:
                 return n
         except Exception as e:
             continue
     return None
 
-def get_first_free_cell_up(cell:Cell, voxel_meta:VoxelMeta, cost_map:ArrayFloatMxNxK):
-    for i in range(cell[2], voxel_meta['nslices']):
+
+def get_first_free_cell_up(
+    cell: Cell, voxel_meta: VoxelMeta, cost_map: ArrayFloatMxNxK
+):
+    for i in range(cell[2], voxel_meta["nslices"]):
         val = cost_map[cell[0], cell[1], i]
         if val != np.inf:
             return (cell[0], cell[1], i)
     return None
 
-def get_path_dist(path:CoordPath) -> float:
-    dist:float = 0.0
+
+def get_path_dist(path: CoordPath) -> float:
+    dist: float = 0.0
     for i in range(len(path) - 1):
         a = np.array(path[i], dtype=np.float32)
         b = np.array(path[i + 1], dtype=np.float32)
         dist += float(np.linalg.norm(a - b))
     return dist
 
 
-
 class EnhancedJSONEncoder(json.JSONEncoder):
-        def default(self, o):
-            if dataclasses.is_dataclass(o):
-                return dataclasses.asdict(o)
-            if isinstance(o, np.ndarray):
-                return o.tolist()
-            return super().default(o)
-
-
-
+    def default(self, o):
+        if dataclasses.is_dataclass(o):
+            return dataclasses.asdict(o)
+        if isinstance(o, np.ndarray):
+            return o.tolist()
+        return super().default(o)
```

### Comparing `pymultiastar-0.0.5/src/pymultiastar/geoplanner/types.py` & `pymultiastar-0.0.6/src/pymultiastar/geoplanner/types.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/src/pymultiastar/types.py` & `pymultiastar-0.0.6/src/pymultiastar/types.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/src/pymultiastar/visualization/img2d_helpers.py` & `pymultiastar-0.0.6/src/pymultiastar/visualization/img2d_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
 from pathlib import Path
 from PIL import Image, ImageDraw
 import shutil
+from .log import logger
 
 def get_maze(img_path: Path, offset=3):
     """This will load an image of maze into a 3D numpy array
 
     Args:
         img_path (Path): Path to img holding maze
         offset (int, optional): Where to offset to start and finish. Defaults to 3.
 
     Returns:
         dict: Returns a dictionary of maze data
     """
     img = np.asarray(Image.open(img_path))
-    print(f"Maze name: {img_path.name}, Shape: {img.shape}")
-    print(f"Unique values: {np.unique(img)}")
+    logger.debug(f"Maze name: {img_path.name}, Shape: {img.shape}")
+    logger.debug(f"Unique values: {np.unique(img)}")
     # convert to float and an empty third dimension
     img_f = np.expand_dims((img / np.max(img)).astype(np.float32), axis=2)
     # Best case scenario is a diagonal path, lets guess it will be 50% bigger
     normalizing_path_cost = 1.5 * np.sqrt(img.shape[0] ** 2 + img.shape[1] ** 2)
 
     return dict(
         img=img,
```

### Comparing `pymultiastar-0.0.5/src/pymultiastar/visualization/vis3d_helpers.py` & `pymultiastar-0.0.6/src/pymultiastar/visualization/vis3d_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 from ..geoplanner.types import GPS, LandingSite, Coord, GeoMultiPlannerResult
 from ..geoplanner import GeoPlanner
 from ..geoplanner.helper import convert_cost_map_to_float
 from typing import List
 from .log import logger
 
 default_buildings = [
-    [(1, 3), (3, 10), (0, 3), 255],
-    [(4, 8), (3, 5), (0, 5), 255],
-    [(6, 8), (6, 10), (0, 3), 255],
+    [(7, 12), (7, 12), (0, 12 ), 255],
 ]
 
-
 def create_map(
-    shape=(10, 10, 5), buildings=default_buildings, dtype=np.float32, normalize=True
+    shape=(20, 30, 15), buildings=default_buildings, dtype=np.float32, normalize=True
 ):
     data = np.zeros(shape, dtype=dtype)
     for x, y, z, value in buildings:
         data[x[0] : x[1], y[0] : y[1], z[0] : z[1]] = value
     if normalize:
         data = data / np.max(data)
     return data
@@ -52,37 +49,47 @@
     pcd = o3d.geometry.PointCloud()
     pcd.points = o3d.utility.Vector3dVector(points)
     pcd.colors = o3d.utility.Vector3dVector(colors)
 
     return pcd
 
 
-def create_pcd_map(map, obstacle_value=1.0, **kwargs):
+def create_pcd_map(map, obstacle_value=1.0, ds_voxel_size=4.0, **kwargs):
     obstacle_mask = map == obstacle_value
     # pf_mask = (~obstacle_mask) & (map > 0)
     pcd_obstacle = convert_to_point_cloud(
         map, mask=obstacle_mask, color_by_height=True, **kwargs
     )
     # only way to make work better....
-    pcd_obstacle = pcd_obstacle.voxel_down_sample(voxel_size=4.0)
+    pcd_obstacle = pcd_obstacle.voxel_down_sample(voxel_size=ds_voxel_size)
     obstacle = dict(name="Obstacles", geometry=pcd_obstacle)
 
+    xres = kwargs.get('xres', 1.0)
+    i, j, k = map.shape
+    map_bounds = np.array([
+        [0, 0, 0],
+        [0, i * xres, 0],
+        [j*xres, i*xres, 0],
+        [j*xres, 0, 0],
+        [0, 0, 0],
+    ])
+    line_set = dict(name="Map Bounds", geometry=create_line(map_bounds))
     # when the point cloud is bigger than 7_000_000 points it will reappear if deselected
     # this was just a test to prove it
     # print(pcd_obstacle)
     # pcd = o3d.geometry.PointCloud()
     # colors = mpl.colormaps.get_cmap('viridis')(np.random.rand(10_000_000))[:, :3]
     # pcd.points = o3d.utility.Vector3dVector(np.random.randn(10_000_000, 3) * 10)
     # pcd.colors = o3d.utility.Vector3dVector(colors)
     # pcd_pf = convert_to_point_cloud(map, mask=pf_mask, **kwargs)
     # obstacle = dict(name="Obstacles", geometry=pcd)
 
     # pf = dict(name="Potential Field", geometry=pcd_pf)
     # geoms = [obstacle, pf] if np.any(pf_mask) else [obstacle]
-    geoms = [obstacle]
+    geoms = [line_set, obstacle]
 
     return geoms
 
 
 def create_landing_objects(
     start_gps: GPS,
     ls_list: List[LandingSite],
@@ -134,34 +141,62 @@
     line_set = o3d.geometry.LineSet(
         points=o3d.utility.Vector3dVector(points),
         lines=o3d.utility.Vector2iVector(lines),
     )
     line_set.paint_uniform_color(color)
     return line_set
 
-def visualize_plan(planner_data, plan_result, xres=2.0):
-    logger.info("Loading Map for Visualization ...")
-
-    landing_objects = create_landing_objects(**plan_result)  # type: ignore
-    map_3d = np.load(planner_data["cost_map_fp"])
-    map_3d = convert_cost_map_to_float(
-        map_3d, reverse_yaxis=True, set_max_value_to_inf=False
-    )
-    world_geoms = create_pcd_map(map_3d, obstacle_value=1.0, xres=xres)
-    logger.info("Finished Loaded Map!")
+def visualize_world(all_geoms, look_at=None, eye=None, point_size=7):
 
     def init(vis):
         vis.show_ground = True
         vis.ground_plane = o3d.visualization.rendering.Scene.GroundPlane.XY  # type: ignore
-        vis.point_size = 7
+        vis.point_size = point_size
         vis.show_axes = True
 
+    if eye is None or look_at is None:
+        boundary = all_geoms[0]['geometry'].get_axis_aligned_bounding_box()
+        look_at = boundary.get_center()
+        extent = boundary.get_extent()
+        eye = [extent[0]/2, -extent[1]/1.5, extent[1]]
+
     logger.info("Please exit by closing the 3D Visualization Window!")
     o3d.visualization.draw(  # type: ignore
-        [*world_geoms, *landing_objects],
-        lookat=[375, 375, 0],
-        eye=[375, -100, 100],
+        all_geoms,
+        lookat=look_at,
+        eye=eye,
         up=[0, 0, 1],
         title="World Viewer",
         on_init=init,
         show_ui=True,
-    )
+    )
+
+def visualize_plan(planner_data, plan_result, xres=2.0):
+    logger.info("Loading Map for Visualization ...")
+
+    landing_objects = create_landing_objects(**plan_result)  # type: ignore
+    map_3d = np.load(planner_data["cost_map_fp"])
+    map_3d = convert_cost_map_to_float(
+        map_3d, reverse_yaxis=True, set_max_value_to_inf=False
+    )
+    world_geoms = create_pcd_map(map_3d, obstacle_value=1.0, xres=xres)
+    logger.info("Finished Loaded Map!")
+
+    all_geoms = [*world_geoms, *landing_objects,]
+    visualize_world(all_geoms)
+
+    # def init(vis):
+    #     vis.show_ground = True
+    #     vis.ground_plane = o3d.visualization.rendering.Scene.GroundPlane.XY  # type: ignore
+    #     vis.point_size = 7
+    #     vis.show_axes = True
+
+    # logger.info("Please exit by closing the 3D Visualization Window!")
+    # o3d.visualization.draw(  # type: ignore
+    #     [*world_geoms, *landing_objects],
+    #     lookat=[375, 375, 0],
+    #     eye=[375, -100, 100],
+    #     up=[0, 0, 1],
+    #     title="World Viewer",
+    #     on_init=init,
+    #     show_ui=True,
+    # )
```

### Comparing `pymultiastar-0.0.5/src/pymultiastar.cpp` & `pymultiastar-0.0.6/src/pymultiastar.cpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/maze_large.png` & `pymultiastar-0.0.6/tests/fixtures/maze_large.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/maze_small.png` & `pymultiastar-0.0.6/tests/fixtures/maze_small.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/world/annarbor/plan.json` & `pymultiastar-0.0.6/tests/fixtures/world/annarbor/plan.json`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/world/annarbor/voxel_map.npy` & `pymultiastar-0.0.6/tests/fixtures/world/annarbor/voxel_map.npy`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/world/newyork/plan.json` & `pymultiastar-0.0.6/tests/fixtures/world/newyork/plan.json`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/fixtures/world/newyork/voxel_map.npy` & `pymultiastar-0.0.6/tests/fixtures/world/newyork/voxel_map.npy`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/test_basic.py` & `pymultiastar-0.0.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/tests/test_geo_helper.py` & `pymultiastar-0.0.6/tests/test_geo_helper.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.5/PKG-INFO` & `pymultiastar-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 Metadata-Version: 2.1
 Name: pymultiastar
-Version: 0.0.5
+Version: 0.0.6
 Summary: Multi-goal A* with cpp bindings to python
 Author-Email: Jeremy Castagno <jeremybyu@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.15
 Requires-Dist: pyproj>=3.0; extra == "geo"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: Pillow; extra == "test"
 Requires-Dist: pyproj>=3.0; extra == "test"
+Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: mkdocs-autorefs>=0.3.1; extra == "docs"
+Requires-Dist: pymdown-extensions>=6.3; extra == "docs"
+Requires-Dist: mkdocs>=1.3; extra == "docs"
+Requires-Dist: mkdocs-coverage>=0.2; extra == "docs"
+Requires-Dist: mkdocs-gen-files>=0.3; extra == "docs"
+Requires-Dist: mkdocs-literate-nav>=0.4; extra == "docs"
+Requires-Dist: mkdocs-material>=7.3; extra == "docs"
+Requires-Dist: mkdocs-section-index>=0.3; extra == "docs"
+Requires-Dist: mkdocstrings-python>=0.5.1; extra == "docs"
+Requires-Dist: markdown-callouts>=0.2; extra == "docs"
+Requires-Dist: markdown-exec>=0.5; extra == "docs"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: open3d>=0.17; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: rich; extra == "dev"
 Requires-Dist: typer; extra == "dev"
 Requires-Dist: ipdb; extra == "dev"
 Requires-Dist: Pillow; extra == "dev"
 Requires-Dist: pymultiastar[geo,test]; extra == "dev"
 Provides-Extra: geo
 Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # Multi-Goal A-star
 
-This repo contains code to search for **multiple** goals with **heterogenous** values using a 3D A* **discrete** planner. The majority of the code is written in C++ with Python bindings. This planner was used in the paper [Map-Based Planning for Small Unmanned Aircraft Rooftop Landing](https://drive.google.com/file/d/1Sy0I8I8nsuy1xv1tFh_W6_Gazcp7pW9M/view?usp=share_link)
+This repo contains code to search for **multiple** goals with **heterogenous** values using a 3D A-star **discrete** planner. The majority of the code is written in C++ with Python bindings. This planner was used in the paper [Map-Based Planning for Small Unmanned Aircraft Rooftop Landing](https://drive.google.com/file/d/1Sy0I8I8nsuy1xv1tFh_W6_Gazcp7pW9M/view?usp=share_link)
 
 **What do you mean by discrete?**
 
-The map provided should be a 3D voxel grid(i, j, k), which the planner searches. This grid is a 3D Numpy array. A cell with the value 0.0 is considered free space. A cell with the value 1.0 is considered an obstacle and cannot be traversed (this value is configurable). Values between 0.0 and 1.0 can be traversed but with a penalty (penalty weight is configurable).
+The map provided should be a 3D voxel grid(i, j, k), a 3D NumPy array, which the planner searches. A cell with the value 0.0 is considered free space. A cell with the value 1.0 is considered an obstacle and cannot be traversed (this value is configurable). Values between 0.0 and 1.0 can be traversed but with a penalty (penalty weight is configurable).
 
 **What do you mean by multiple goals with heterogenous values?**
 
-A normal A* planner has a start location and one goal. This Multi-Goal planner allows you to provide multiple goal cells each having different values. Goals with lower values are more desirable. This planner will try to find the optimal **goal** *and* **path** which minimizes an objective function. It must be understood that the planner doesn't just find a path. It finds the goal and the corresponding optimal path that minimizes some larger objective function. 
+A normal A-star planner has a start location and one goal. This Multi-Goal planner allows you to provide multiple goal cells each having different values. Goals with lower values are more desirable. This planner will try to find the optimal **goal** *and* **path** which minimizes an objective function. It must be understood that the planner doesn't just find a path. It finds the goal and the corresponding optimal path that minimizes some larger objective function. 
 
 **What is the objective function?**
 
 The objective function is the minimization of total risk ($r_t$), which is the combination of path risk ($r_p$) and goal risk $r_g$. In my research the goals were landing sites, therefore I called the latter landing site risk $r_l$. 
 Below is an excerpt from my paper that discusses this trade-off between objectives:
 
     The figure below shows an example Pareto frontier that minimizes two objectives: landing
@@ -53,15 +66,15 @@
     each objective must be constructed to select a final choice. A linear weighting scheme
     is used for these purposes
 
 $$
 r_t = w_l \cdot r_l + w_p · r_p
 $$
 
-![Tradeoff](./assets/imgs/tradeoff.png)
+![Tradeoff](https://raw.githubusercontent.com/JeremyBYU/pymultiastar/master/assets/imgs/tradeoff.png)
 
 **What precisely are these two objectives and how do they relate to the planner?**
 
 See the following sections in the paper linked above: 
 
 - Definition of Path **Cost**: Section 1.3.2, Equations 1.6-1.8
 - Definition of Path **Risk**: Section 1.5, Equation 1.17
@@ -76,12 +89,16 @@
     1. This planner only knows about Voxel Grid to traverse.
 2. Geographically Aware Planner - `pip install pymultiastar[geo]` - This also exposes the class `GeoPlanner`
     1. This is a geographically aware wrapper around `PyMultiAStar`. You give a georeferenced voxel map and start conditions in GPS and landing sites in GPS and it will do the conversions between GPS to voxel cell for you. 
 
 
 ## How to use
 
-TBD
+Below are some examples:
+
+1. `run_simple_world_3d.py`. Shows a very simple example of a small 3D world with multiple goals.
+2. `run_maze_2d.py` - Demonstrates that 2D A-star path planning is a subset of the Multi-Goal Planner. It loads a 2D image of a maze as a single slice in a 3D world and has only 1 goal. 
+3. `run_scenarios.py` - Shows how to use the GeoPlanner and plan in a 3D world.
 
 ## Notes
 
 inside pymultiastar map data - (i,j,k) is the row, column, depth
```

