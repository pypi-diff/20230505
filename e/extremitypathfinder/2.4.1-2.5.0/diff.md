# Comparing `tmp/extremitypathfinder-2.4.1.tar.gz` & `tmp/extremitypathfinder-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extremitypathfinder-2.4.1.tar", max compression
+gzip compressed data, was "extremitypathfinder-2.5.0.tar", max compression
```

## Comparing `extremitypathfinder-2.4.1.tar` & `extremitypathfinder-2.5.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0      200 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/.editorconfig
--rw-r--r--   0        0        0     2048 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     3927 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/CHANGELOG.rst
--rw-r--r--   0        0        0     3091 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1056 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/LICENSE
--rw-r--r--   0        0        0      688 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/Makefile
--rw-r--r--   0        0        0     2311 2022-08-21 23:14:28.572798 extremitypathfinder-2.4.1/README.rst
--rw-r--r--   0        0        0      574 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/example.json
--rw-r--r--   0        0        0      132 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/__init__.py
--rw-r--r--   0        0        0     2260 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/command_line.py
--rw-r--r--   0        0        0      151 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/configs.py
--rw-r--r--   0        0        0    16294 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/extremitypathfinder.py
--rw-r--r--   0        0        0     6892 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/plotting.py
--rw-r--r--   0        0        0      379 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/types.py
--rw-r--r--   0        0        0    39693 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/extremitypathfinder/utils.py
--rw-r--r--   0        0        0     1880 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/__init__.py
--rw-r--r--   0        0        0      580 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/cli_test.py
--rwxr-xr-x   0        0        0     6871 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/helper_fcts_test.py
--rwxr-xr-x   0        0        0      838 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/helpers.py
--rwxr-xr-x   0        0        0     7485 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/main_test.py
--rw-r--r--   0        0        0    10758 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tests/test_cases.py
--rwxr-xr-x   0        0        0      298 2022-08-21 23:14:28.584798 extremitypathfinder-2.4.1/tox.ini
--rw-r--r--   0        0        0     3325 2022-08-21 23:14:38.326223 extremitypathfinder-2.4.1/setup.py
--rw-r--r--   0        0        0     3846 2022-08-21 23:14:38.326750 extremitypathfinder-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/.editorconfig
+-rw-r--r--   0        0        0     2043 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     4071 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     3091 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1056 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/LICENSE
+-rw-r--r--   0        0        0      759 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/Makefile
+-rw-r--r--   0        0        0     2447 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/README.rst
+-rw-r--r--   0        0        0      574 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/example.json
+-rw-r--r--   0        0        0      132 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/__init__.py
+-rw-r--r--   0        0        0     2234 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/command_line.py
+-rw-r--r--   0        0        0      151 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/configs.py
+-rw-r--r--   0        0        0    14688 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/extremitypathfinder.py
+-rw-r--r--   0        0        0     6866 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/plotting.py
+-rw-r--r--   0        0        0      379 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/types.py
+-rw-r--r--   0        0        0    41506 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/utils.py
+-rw-r--r--   0        0        0     1906 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/cli_test.py
+-rwxr-xr-x   0        0        0     6871 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/helper_fcts_test.py
+-rwxr-xr-x   0        0        0      838 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/helpers.py
+-rwxr-xr-x   0        0        0     7352 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/main_test.py
+-rw-r--r--   0        0        0    10758 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/test_cases.py
+-rwxr-xr-x   0        0        0      318 2023-05-05 11:43:19.743766 extremitypathfinder-2.5.0/tox.ini
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 extremitypathfinder-2.5.0/PKG-INFO
```

### Comparing `extremitypathfinder-2.4.1/.pre-commit-config.yaml` & `extremitypathfinder-2.5.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-ast  # Is it valid Python?
       - id: debug-statements # no debbuging statements used
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
@@ -16,56 +16,56 @@
       - id: check-merge-conflict
       - id: check-docstring-first
       - id: requirements-txt-fixer
       #            -   id: detect-aws-credentials
       - id: detect-private-key
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args: [ "--profile", "black", "--filter-files" ]
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
         args:
           - --line-length=120
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [ black ]
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         exclude: ^(docs|scripts|tests)/
         # E203 whitespace before ':'
         args:
           - --max-line-length=120
           - --ignore=E203
         additional_dependencies:
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-tidy-imports
 
   - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.48"
+    rev: "0.49"
     hooks:
       - id: check-manifest
         args: [ "--no-build-isolation", "--ignore",  "*.png,docs/*,publish.py,readthedocs.yml,poetry.lock,setup.py,scripts/*" ]
-        additional_dependencies: [ numpy, poetry==1.1.11 ]
+        additional_dependencies: [ numpy, poetry>=1.4 ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.37.3
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
 
 # TODO enable for very detailed linting:
 #    -   repo: https://github.com/pycqa/pylint
 #        rev: pylint-2.6.0
 #        hooks:
```

### Comparing `extremitypathfinder-2.4.1/CHANGELOG.rst` & `extremitypathfinder-2.5.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Changelog
 =========
 
-TODOs
 
-* pending major release: remove separate prepare step?! initialise in one step during initialisation
-* Numba JIT compilation of utils. line speed profiling for highest impact of refactoring
-* allow input of complex geometries: input coords, and edges separately (polygons are special case)
-* drop simplify parameter
+2.5.0 (2023-05-05)
+-------------------
+
+* removed need for separate ``.prepare()`` call. Storing environment boundary data automatically triggers the preparation of the visibility graph. This is a non-breaking change. The ``.prepare()`` method is still available, but it is not needed anymore.
+
+internal:
+
+* updated dependency specification: networkx>=3, relaxed development dependency version requirements
+* included tests for python 3.11
+* minor code refactoring
+
 
 2.4.1 (2022-08-22)
 -------------------
 
 * bugfix: catch the case where no path is possible in the graph in the ``networkx`` A* implementation
 * added speed benchmarks and performance section in the documentation with benchmark results
```

### Comparing `extremitypathfinder-2.4.1/CONTRIBUTING.rst` & `extremitypathfinder-2.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/LICENSE` & `extremitypathfinder-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/Makefile` & `extremitypathfinder-2.5.0/Makefile`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-pin:
-	@echo "pinning the dependencies specified in 'pyproject.toml':"
-	@poetry update -vv
-	#poetry export -f requirements.txt --output docs/requirements.txt --without-hashes
-
-req:
+install:
 	@echo "installing the development dependencies..."
 	@poetry install
 	@#poetry install --no-dev
 
 
-update: pin req
+update:
+	@echo "updating the dependencies pinned in 'pyproject.toml':"
+	@poetry update -vvv
+	#poetry export -f requirements.txt --output docs/requirements.txt --without-hashes
+
+lock:
+	@echo "pinning the dependencies in 'pyproject.toml':"
+	@poetry lock -vvv
+
 
 test:
-	@tox
 	#pytest
+	@tox
 
 hook:
 	@pre-commit install
 	@pre-commit run --all-files
 
 hook2:
 	@pre-commit autoupdate
```

### Comparing `extremitypathfinder-2.4.1/README.rst` & `extremitypathfinder-2.5.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ===================
 extremitypathfinder
 ===================
 
+..
+    Note: can't include the badges file from the docs here, as it won't render on PyPI -> sync manually
 
-.. image:: https://api.travis-ci.org/jannikmi/extremitypathfinder.svg?branch=master
-    :target: https://travis-ci.org/jannikmi/extremitypathfinder
+
+.. image:: https://github.com/jannikmi/extremitypathfinder/actions/workflows/build.yml/badge.svg?branch=master
+    :target: https://github.com/jannikmi/extremitypathfinder/actions?query=branch%3Amaster
 
 .. image:: https://readthedocs.org/projects/extremitypathfinder/badge/?version=latest
     :alt: documentation status
     :target: https://extremitypathfinder.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/pypi/wheel/extremitypathfinder.svg
     :target: https://pypi.python.org/pypi/extremitypathfinder
@@ -54,15 +57,14 @@
             (3.0, 7.0),
             (5.0, 9.0),
             (4.5, 7.0),
             (5.0, 4.0),
         ],
     ]
     environment.store(boundary_coordinates, list_of_holes, validate=False)
-    environment.prepare()
     start_coordinates = (4.5, 1.0)
     goal_coordinates = (4.0, 8.5)
     path, length = environment.find_shortest_path(start_coordinates, goal_coordinates)
 
 
 For more refer to the `documentation <https://extremitypathfinder.readthedocs.io/en/latest/>`__.
```

### Comparing `extremitypathfinder-2.4.1/example.json` & `extremitypathfinder-2.5.0/example.json`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/extremitypathfinder/command_line.py` & `extremitypathfinder-2.5.0/extremitypathfinder/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,9 @@
 
     # Parse tuples from the input arguments (interpreted as lists):
     start_coordinates = tuple(parsed_args.start)
     goal_coordinates = tuple(parsed_args.goal)
 
     # Execute search for the given parameters
     environment.store(boundary_coordinates, list_of_holes, validate=False)
-    environment.prepare()
     path, distance = environment.find_shortest_path(start_coordinates, goal_coordinates)
     print(path, distance)
```

### Comparing `extremitypathfinder-2.4.1/extremitypathfinder/extremitypathfinder.py` & `extremitypathfinder-2.5.0/extremitypathfinder/extremitypathfinder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import pickle
+import warnings
 from typing import Dict, Iterable, List, Optional, Set, Tuple
 
 import networkx as nx
 import numpy as np
 
 from extremitypathfinder import types as t
+from extremitypathfinder import utils
 from extremitypathfinder.configs import DEFAULT_PICKLE_NAME
 from extremitypathfinder.types import InputCoord, InputCoordList, Length, ObstacleIterator, Path
-from extremitypathfinder.utils import (
-    check_data_requirements,
-    cmp_reps_n_distances,
-    compute_extremity_idxs,
-    compute_graph,
-    convert_gridworld,
-    find_identical_single,
-    find_visible,
-    get_distance,
-    is_within_map,
-)
 
 
 class PolygonEnvironment:
     """Class allowing to use polygons to represent "2D environments" and use them for path finding.
 
     Keeps a "loaded" and prepared environment for consecutive path queries.
     Internally uses a visibility graph optimised for shortest path finding.
@@ -85,70 +76,37 @@
         :raises AssertionError: when validate=True and the input is invalid.
         """
         self.prepared = False
         # loading the map
         boundary_coordinates = np.array(boundary_coordinates, dtype=float)
         list_of_hole_coordinates = [np.array(hole_coords, dtype=float) for hole_coords in list_of_hole_coordinates]
         if validate:
-            check_data_requirements(boundary_coordinates, list_of_hole_coordinates)
+            utils.check_data_requirements(boundary_coordinates, list_of_hole_coordinates)
 
-        self.boundary_polygon = boundary_coordinates
-
-        # IMPORTANT: make a copy of the list instead of linking to the same list (python!)
+        # Note: independent copy!
         self.holes = list_of_hole_coordinates
+        self.boundary_polygon = boundary_coordinates
 
-        list_of_polygons = [boundary_coordinates] + list_of_hole_coordinates
-        nr_total_pts = sum(map(len, list_of_polygons))
-        vertex_edge_idxs = np.empty((nr_total_pts, 2), dtype=int)
-        # TODO required? inverse of the other. get_neighbours function
-        edge_vertex_idxs = np.empty((nr_total_pts, 2), dtype=int)
-        edge_idx = 0
-        offset = 0
-        extremity_idxs = set()
-        for poly in list_of_polygons:
-            poly_extr_idxs = compute_extremity_idxs(poly)
-            poly_extr_idxs = {i + offset for i in poly_extr_idxs}
-            extremity_idxs |= poly_extr_idxs
-
-            nr_coords = len(poly)
-            v1 = -1 % nr_coords
-            # TODO col 1 is just np.arange?!
-            for v2 in range(nr_coords):
-                v1_idx = v1 + offset
-                v2_idx = v2 + offset
-                edge_vertex_idxs[edge_idx, 0] = v1_idx
-                edge_vertex_idxs[edge_idx, 1] = v2_idx
-                vertex_edge_idxs[v1_idx, 1] = edge_idx
-                vertex_edge_idxs[v2_idx, 0] = edge_idx
-                # move to the next vertex/edge
-                v1 = v2
-                edge_idx += 1
-
-            offset = edge_idx
-
-        # assert edge_idx == nr_total_pts
-
-        coords = np.concatenate(list_of_polygons, axis=0)
-        # Attention: only consider extremities that are actually within the map
-        extremity_idxs = [i for i in extremity_idxs if self.within_map(coords[i])]
-
-        mask = np.full(nr_total_pts, False, dtype=bool)
-        for i in extremity_idxs:
-            mask[i] = True
+        (
+            self.coords,
+            self.extremity_indices,
+            self.extremity_mask,
+            self.vertex_edge_idxs,
+            self.edge_vertex_idxs,
+        ) = utils.compile_boundary_data_fr_polys(boundary_coordinates, list_of_hole_coordinates)
 
+        nr_total_pts = self.edge_vertex_idxs.shape[0]
         self.nr_vertices = nr_total_pts
+        self.reprs_n_distances = {i: utils.cmp_reps_n_distances(i, self.coords) for i in self.extremity_indices}
+
         # start and goal points will be stored after all polygon coordinates
         self.idx_start = nr_total_pts
         self.idx_goal = nr_total_pts + 1
-        self.edge_vertex_idxs = edge_vertex_idxs
-        self.vertex_edge_idxs = vertex_edge_idxs
-        self.coords = coords
-        self.extremity_indices = extremity_idxs
-        self.extremity_mask = mask
-        self.reprs_n_distances = {i: cmp_reps_n_distances(i, coords) for i in extremity_idxs}
+
+        self.prepare()
 
     def store_grid_world(
         self,
         size_x: int,
         size_y: int,
         obstacle_iter: ObstacleIterator,
         simplify: bool = True,
@@ -161,15 +119,17 @@
 
         :param size_x: the horizontal grid world size
         :param size_y: the vertical grid world size
         :param obstacle_iter: an iterable of coordinate pairs (x,y) representing blocked grid cells (obstacles)
         :param validate: whether the input should be validated
         :param simplify: whether the polygons should be simplified or not. reduces edge amount, allow diagonal edges
         """
-        boundary_coordinates, list_of_hole_coordinates = convert_gridworld(size_x, size_y, obstacle_iter, simplify)
+        boundary_coordinates, list_of_hole_coordinates = utils.convert_gridworld(
+            size_x, size_y, obstacle_iter, simplify
+        )
         self.store(boundary_coordinates, list_of_hole_coordinates, validate)
 
     def export_pickle(self, path: str = DEFAULT_PICKLE_NAME):
         print("storing map class in:", path)
         with open(path, "wb") as f:
             pickle.dump(self, f)
         print("done.\n")
@@ -191,18 +151,19 @@
             In the created graph however, these nodes must be merged at the end to avoid ambiguities!
 
         .. note::
             Pre computing the shortest paths between all directly reachable extremities
             and storing them in the graph would not be an advantage, because then the graph is fully connected.
             A* would visit every node in the graph at least once (-> disadvantage!).
         """
-        if self.prepared:
-            raise ValueError("this environment is already prepared. load new polygons first.")
+        if self.prepared:  # idempotent
+            warnings.warn("called .prepare() on already prepared map. skipping...", stacklevel=1)
+            return
 
-        self.graph = compute_graph(
+        self.graph = utils.compute_graph(
             self.nr_edges,
             self.extremity_indices,
             self.reprs_n_distances,
             self.coords,
             self.edge_vertex_idxs,
             self.extremity_mask,
             self.vertex_edge_idxs,
@@ -211,28 +172,28 @@
 
     def within_map(self, coords: np.ndarray) -> bool:
         """checks if the given coordinates lie within the boundary polygon and outside of all holes
 
         :param coords: numerical tuple representing coordinates
         :return: whether the given coordinate is a valid query point
         """
-        return is_within_map(coords, self.boundary_polygon, self.holes)
+        return utils.is_within_map(coords, self.boundary_polygon, self.holes)
 
     def get_visible_idxs(
         self,
         origin: int,
         candidates: Iterable[int],
         coords: np.ndarray,
         vert_idx2repr: np.ndarray,
         vert_idx2dist: np.ndarray,
     ) -> Set[int]:
         # Note: points with equal coordinates should not be considered visible (will be merged later)
         candidates = {i for i in candidates if not vert_idx2dist[i] == 0.0}
         edge_idxs2check = set(range(self.nr_edges))
-        return find_visible(
+        return utils.find_visible(
             origin,
             candidates,
             edge_idxs2check,
             coords,
             vert_idx2repr,
             vert_idx2dist,
             self.extremity_mask,
@@ -257,16 +218,14 @@
          if points close to or on polygon edges should be accepted as valid input, set this to ``False``.
         :return: a tuple of shortest path and its length. ([], None) if there is no possible path.
         """
         # path planning query:
         # make sure the map has been loaded and prepared
         if self.boundary_polygon is None:
             raise ValueError("No Polygons have been loaded into the map yet.")
-        if not self.prepared:
-            self.prepare()
 
         coords_start = np.array(start_coordinates, dtype=float)
         coords_goal = np.array(goal_coordinates, dtype=float)
         if verify and not self.within_map(coords_start):
             raise ValueError("start point does not lie within the map")
         if verify and not self.within_map(coords_goal):
             raise ValueError("goal point does not lie within the map")
@@ -285,15 +244,15 @@
 
         # check the goal node first (earlier termination possible)
         origin = goal
         # the visibility of only the graph nodes has to be checked (not all extremities!)
         # IMPORTANT: also check if the start node is visible from the goal node!
         candidate_idxs: Set[int] = set(self.graph.nodes)
         candidate_idxs.add(start)
-        repr_n_dists = cmp_reps_n_distances(origin, coords)
+        repr_n_dists = utils.cmp_reps_n_distances(origin, coords)
         self.reprs_n_distances[origin] = repr_n_dists
         vert_idx2repr, vert_idx2dist = repr_n_dists
         visibles_goal = self.get_visible_idxs(origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist)
         if len(visibles_goal) == 0:
             # The goal node does not have any neighbours. Hence there is not possible path to the goal.
             return [], None
 
@@ -318,40 +277,40 @@
         # as the graph is only being used for a single query
         for i in visibles_goal:
             graph.add_edge(i, goal, weight=vert_idx2dist[i])
 
         origin = start
         # the visibility of only the graphs nodes have to be checked
         # the goal node does not have to be considered, because of the earlier check
-        repr_n_dists = cmp_reps_n_distances(origin, coords)
+        repr_n_dists = utils.cmp_reps_n_distances(origin, coords)
         self.reprs_n_distances[origin] = repr_n_dists
         vert_idx2repr, vert_idx2dist = repr_n_dists
         visibles_start = self.get_visible_idxs(origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist)
 
         if len(visibles_start) == 0:
             # The start node does not have any neighbours. Hence there is no possible path to the goal.
             return [], None
 
         # add edges: start <-> extremity (i)
         for i in visibles_start:
             graph.add_edge(start, i, weight=vert_idx2dist[i])
 
         # apply mapping to start and goal index as well
-        start_mapped = find_identical_single(start, graph.nodes, self.reprs_n_distances)
+        start_mapped = utils.find_identical_single(start, graph.nodes, self.reprs_n_distances)
         if start_mapped != start:
             nx.relabel_nodes(graph, {start: start_mapped}, copy=False)
 
-        goal_mapped = find_identical_single(goal, graph.nodes, self.reprs_n_distances)
+        goal_mapped = utils.find_identical_single(goal, graph.nodes, self.reprs_n_distances)
         if goal_mapped != goal_mapped:
             nx.relabel_nodes(graph, {goal: goal_mapped}, copy=False)
 
         self._idx_start_tmp, self._idx_goal_tmp = start_mapped, goal_mapped  # for plotting
 
         def l2_distance(n1, n2):
-            return get_distance(n1, n2, self.reprs_n_distances)
+            return utils.get_distance(n1, n2, self.reprs_n_distances)
 
         try:
             id_path = nx.astar_path(graph, start_mapped, goal_mapped, heuristic=l2_distance, weight="weight")
         except nx.exception.NetworkXNoPath:
             return [], None
 
         # clean up
```

### Comparing `extremitypathfinder-2.4.1/extremitypathfinder/plotting.py` & `extremitypathfinder-2.5.0/extremitypathfinder/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,14 @@
     def store(self, *args, **kwargs):
         """In addition to storing, also plots a graph of the input polygons."""
         super().store(*args, **kwargs)
         draw_loaded_map(self)
 
     def prepare(self):
         """Also draws a prepared map with the computed visibility graph."""
-        super().prepare()
         draw_prepared_map(self)
 
     def find_shortest_path(self, start_coordinates, goal_coordinates, *args, **kwargs):
         """Also draws the computed shortest path."""
         # important to not delete the temp graph! for plotting
         vertex_path, distance = super().find_shortest_path(
             start_coordinates, goal_coordinates, *args, free_space_after=False, **kwargs
```

### Comparing `extremitypathfinder-2.4.1/extremitypathfinder/utils.py` & `extremitypathfinder-2.5.0/extremitypathfinder/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -691,15 +691,14 @@
     extremity_indices: Iterable[int],
     reprs_n_distances: Dict[int, np.ndarray],
     coords: np.ndarray,
     edge_vertex_idxs: np.ndarray,
     extremity_mask: np.ndarray,
     vertex_edge_idxs: np.ndarray,
 ) -> t.Graph:
-
     graph = t.Graph()
     # IMPORTANT: add all extremities (even if they turn out to be dangling in the end),
     # adding start and goal nodes at query time might connect them!
     graph.add_nodes_from(extremity_indices)
 
     # optimisation: no not check the last extremity as no other candidates will remain (cf. below)
     for extr_ptr, origin_idx in enumerate(extremity_indices[:-1]):
@@ -759,15 +758,15 @@
     Parse data from a JSON file and save as lists of tuples for both boundary and holes.
     NOTE: The format of the JSON file is explained in the command line script (argparse definition)
 
     :param path2json_file: The path to the input json file
     :return: The parsed lists of boundaries and holes
     """
     # parse data from the input file
-    with open(path2json_file, "r") as json_file:
+    with open(path2json_file) as json_file:
         json_data = json_file.read()
     json_loaded = json.loads(json_data)
     boundary_data = try_extraction(json_loaded, BOUNDARY_JSON_KEY)
     holes_data = try_extraction(json_loaded, HOLES_JSON_KEY)
     boundary_coordinates = convert2polygon(boundary_data)
     list_of_holes = [convert2polygon(hole_data) for hole_data in holes_data]
     return boundary_coordinates, list_of_holes
@@ -984,7 +983,51 @@
     return extr_idxs
 
 
 def load_pickle(path=DEFAULT_PICKLE_NAME):
     print("loading map from:", path)
     with open(path, "rb") as f:
         return pickle.load(f)
+
+
+def compile_boundary_data_fr_polys(boundary_coordinates, list_of_hole_coordinates):
+    def within_map(coord):
+        return is_within_map(coord, boundary_coordinates, list_of_hole_coordinates)
+
+    list_of_polygons = [boundary_coordinates] + list_of_hole_coordinates
+    nr_total_pts = sum(map(len, list_of_polygons))
+
+    # compute edge and vertex indices from polygon data structure
+    vertex_edge_idxs = np.empty((nr_total_pts, 2), dtype=int)
+    # TODO required? inverse of the other. get_neighbours function
+    edge_vertex_idxs = np.empty((nr_total_pts, 2), dtype=int)
+    edge_idx = 0
+    offset = 0
+    extremity_indices = set()
+    for poly in list_of_polygons:
+        poly_extr_idxs = compute_extremity_idxs(poly)
+        poly_extr_idxs = {i + offset for i in poly_extr_idxs}
+        extremity_indices |= poly_extr_idxs
+
+        nr_coords = len(poly)
+        v1 = -1 % nr_coords
+        # TODO col 1 is just np.arange?!
+        for v2 in range(nr_coords):
+            v1_idx = v1 + offset
+            v2_idx = v2 + offset
+            edge_vertex_idxs[edge_idx, 0] = v1_idx
+            edge_vertex_idxs[edge_idx, 1] = v2_idx
+            vertex_edge_idxs[v1_idx, 1] = edge_idx
+            vertex_edge_idxs[v2_idx, 0] = edge_idx
+            # move to the next vertex/edge
+            v1 = v2
+            edge_idx += 1
+
+        offset = edge_idx
+
+    coords = np.concatenate(list_of_polygons, axis=0)
+    # Attention: only consider extremities that are actually within the map (polygons are allowed to overlap)
+    extremity_indices = [i for i in extremity_indices if within_map(coords[i])]
+    extremity_mask = np.full(nr_total_pts, False, dtype=bool)
+    for i in extremity_indices:
+        extremity_mask[i] = True
+    return coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs
```

### Comparing `extremitypathfinder-2.4.1/pyproject.toml` & `extremitypathfinder-2.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extremitypathfinder"
-version = "2.4.1"
+version = "2.5.0"
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/jannikmi/extremitypathfinder"
 homepage = "https://extremitypathfinder.readthedocs.io/en/latest/"
 documentation = "https://extremitypathfinder.readthedocs.io/en/latest/"
 keywords = ["path-planning", "path-finding", "shortest-path", "visibility", "graph", "polygon", "grid", "map", "robotics", "navigation", "offline"]
 classifiers = [
@@ -15,15 +15,15 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Education",
     "Topic :: Games/Entertainment"
 ]
-description = "python package implementing a multivariate Horner scheme for efficiently evaluating multivariate polynomials"
+description = "python package for fast shortest path computation on 2D polygon or grid maps"
 authors = ["jannikmi <github@michelfe.it>"]
 include = [
     "LICENSE",
     ".editorconfig",
     ".pre-commit-config.yaml",
     "CHANGELOG.rst",
     "CONTRIBUTING.rst",
@@ -37,27 +37,32 @@
 
 [tool.poetry.scripts]
 extremitypathfinder = "extremitypathfinder.command_line:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22"
-networkx = "^2.8.5"
+networkx = "^3"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "*"
+
+[tool.poetry.group.plot.dependencies]
+matplotlib = "*"
+
+[tool.poetry.group.test.dependencies]
+pytest = "*"
+tox = "*"
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "*"
+sphinx-rtd-theme = "*"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-tox = "^3.24.4"
-pre-commit = "^2.15.0"
-# docs
-Sphinx = "^4.3.1"
-sphinx-rtd-theme = "^1.0.0"
-matplotlib = "^3.5.2"
 
 [tool.poetry.extras]
-numba = ["numba"]
 plot = ["matplotlib"]
 test = ["pytest", "tox"]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [build-system]
-requires = ["poetry-core>=1.0.7", "poetry==1.1.11"]
+requires = ["poetry-core>=1.5", "poetry>=1.4"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `extremitypathfinder-2.4.1/tests/cli_test.py` & `extremitypathfinder-2.5.0/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/tests/helper_fcts_test.py` & `extremitypathfinder-2.5.0/tests/helper_fcts_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/tests/helpers.py` & `extremitypathfinder-2.5.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/tests/main_test.py` & `extremitypathfinder-2.5.0/tests/main_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,29 +49,28 @@
             status_str = "OK"
         else:
             status_str = "XX"
         print(f"{status_str} input: {(start_coordinates, goal_coordinates)} ")
         assert correct_result, f"unexpected result (path, length): got {output} instead of {expected_output} "
 
     print("testing if path and distance are correct:")
-    for ((start_coordinates, goal_coordinates), expected_output) in test_cases:
+    for (start_coordinates, goal_coordinates), expected_output in test_cases:
         validate(start_coordinates, goal_coordinates, expected_output)
         # automatically test reversed!
         path, length = expected_output
         expected_output_reversed = list(reversed(path)), length
         validate(goal_coordinates, start_coordinates, expected_output_reversed)
 
 
 def test_grid_env():
     grid_env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
 
     grid_env.store_grid_world(*GRID_ENV_PARAMS, simplify=False, validate=False)
     nr_extremities = len(grid_env.all_extremities)
     assert nr_extremities == 17, "extremities do not get detected correctly!"
-    grid_env.prepare()
     nr_graph_nodes = len(grid_env.graph.nodes)
     assert nr_graph_nodes == 16, "identical nodes should get joined in the graph!"
 
     # test if points outside the map are being rejected
     for start_coordinates, goal_coordinates in INVALID_DESTINATION_DATA:
         with pytest.raises(ValueError):
             grid_env.find_shortest_path(start_coordinates, goal_coordinates)
@@ -92,15 +91,14 @@
 def test_poly_env():
     poly_env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
     poly_env.store(*POLY_ENV_PARAMS, validate=True)
     nr_exp_extremities = 4
     assert (
         len(list(poly_env.all_extremities)) == nr_exp_extremities
     ), f"the environment should detect all {nr_exp_extremities} extremities!"
-    poly_env.prepare()
     nr_nodes_env2 = len(poly_env.graph.nodes)
     # TODO
     # assert nr_nodes_env2 == nr_exp_extremities, (
     #     f"the visibility graph should store all {nr_exp_extremities} extremities {list(poly_env.all_extremities)}!"
     #     f"\n found: {poly_env.graph.nodes}"
     # )
 
@@ -124,23 +122,21 @@
     # test if property 1 is being properly exploited
     # (extremities lying in front of each other need not be connected)
 
 
 def test_overlapping_polygon():
     overlap_poly_env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
     overlap_poly_env.store(*OVERLAP_POLY_ENV_PARAMS)
-    overlap_poly_env.prepare()
     print("\ntesting polygon environment with overlapping polygons")
     try_test_cases(overlap_poly_env, TEST_DATA_OVERLAP_POLY_ENV)
 
 
 def test_separated_environment():
     env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
     env.store(*SEPARATED_ENV)
-    env.prepare()
     print("\ntesting polygon environment with two separated areas")
     try_test_cases(env, TEST_DATA_SEPARATE_ENV)
 
 
 @pytest.mark.parametrize(
     "env_data",
     POLYGON_ENVS,
@@ -148,15 +144,14 @@
 def test_extremity_neighbour_connection(env_data):
     # if two extremities are direct neighbours in a polygon, they also must be connected in the prepared graph
     # exception: there is another polygon edge intersecting that
     print("\ntesting if all two direct extremity neighbour are connected")
     env = PolygonEnvironment()
     env.store(*env_data)
     coords = env.coords
-    env.prepare()
     graph = env.graph
     extremities = env.extremity_indices
     edge_vertex_idxs = env.edge_vertex_idxs
 
     def connection_as_expected(i1: int, i2: int):
         if i2 not in extremities:
             return
@@ -179,15 +174,14 @@
     # if two extremities are direct neighbours in a polygon, they also must be connected in the prepared graph
     # exception: there is another polygon edge intersecting that
     print("\ntesting if all two direct extremity neighbour are connected")
     env = PolygonEnvironment()
     env.store(*env_data)
     coords = env.coords
     nr_vertices = env.nr_vertices
-    env.prepare()
 
     for start, goal in itertools.product(range(nr_vertices), repeat=2):
         coords_start = coords[start]
         coords_goal = coords[goal]
 
         if not env.within_map(coords_start):
             continue
```

### Comparing `extremitypathfinder-2.4.1/tests/test_cases.py` & `extremitypathfinder-2.5.0/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.4.1/PKG-INFO` & `extremitypathfinder-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: extremitypathfinder
-Version: 2.4.1
-Summary: python package implementing a multivariate Horner scheme for efficiently evaluating multivariate polynomials
+Version: 2.5.0
+Summary: python package for fast shortest path computation on 2D polygon or grid maps
 Home-page: https://extremitypathfinder.readthedocs.io/en/latest/
 License: MIT
 Keywords: path-planning,path-finding,shortest-path,visibility,graph,polygon,grid,map,robotics,navigation,offline
 Author: jannikmi
 Author-email: github@michelfe.it
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: docs
-Provides-Extra: numba
 Provides-Extra: plot
 Provides-Extra: test
-Requires-Dist: networkx (>=2.8.5,<3.0.0)
+Requires-Dist: networkx (>=3,<4)
 Requires-Dist: numpy (>=1.22,<2.0)
 Project-URL: Documentation, https://extremitypathfinder.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jannikmi/extremitypathfinder
 Description-Content-Type: text/x-rst
 
 ===================
 extremitypathfinder
 ===================
 
+..
+    Note: can't include the badges file from the docs here, as it won't render on PyPI -> sync manually
+
 
-.. image:: https://api.travis-ci.org/jannikmi/extremitypathfinder.svg?branch=master
-    :target: https://travis-ci.org/jannikmi/extremitypathfinder
+.. image:: https://github.com/jannikmi/extremitypathfinder/actions/workflows/build.yml/badge.svg?branch=master
+    :target: https://github.com/jannikmi/extremitypathfinder/actions?query=branch%3Amaster
 
 .. image:: https://readthedocs.org/projects/extremitypathfinder/badge/?version=latest
     :alt: documentation status
     :target: https://extremitypathfinder.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/pypi/wheel/extremitypathfinder.svg
     :target: https://pypi.python.org/pypi/extremitypathfinder
@@ -89,15 +92,14 @@
             (3.0, 7.0),
             (5.0, 9.0),
             (4.5, 7.0),
             (5.0, 4.0),
         ],
     ]
     environment.store(boundary_coordinates, list_of_holes, validate=False)
-    environment.prepare()
     start_coordinates = (4.5, 1.0)
     goal_coordinates = (4.0, 8.5)
     path, length = environment.find_shortest_path(start_coordinates, goal_coordinates)
 
 
 For more refer to the `documentation <https://extremitypathfinder.readthedocs.io/en/latest/>`__.
```

