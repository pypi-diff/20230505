# Comparing `tmp/structuretoolkit-0.0.1.tar.gz` & `tmp/structuretoolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structuretoolkit-0.0.1.tar", last modified: Mon Mar 27 23:13:14 2023, max compression
+gzip compressed data, was "structuretoolkit-0.0.2.tar", last modified: Fri May  5 17:20:04 2023, max compression
```

## Comparing `structuretoolkit-0.0.1.tar` & `structuretoolkit-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/structuretoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/structuretoolkit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.488235 structuretoolkit-0.0.1/structuretoolkit/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/analyse/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.488235 structuretoolkit-0.0.1/structuretoolkit/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/build/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/build/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/build/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/build/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30831 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/structuretoolkit/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.488235 structuretoolkit-0.0.1/structuretoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/structuretoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/structuretoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/structuretoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/structuretoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 23:13:14.000000 structuretoolkit-0.0.1/structuretoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:13:14.492235 structuretoolkit-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_high_index_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-27 23:13:10.000000 structuretoolkit-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/structuretoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/structuretoolkit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/structuretoolkit/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/structuretoolkit/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30831 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.962569 structuretoolkit-0.0.2/structuretoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_high_index_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/versioneer.py
```

### Comparing `structuretoolkit-0.0.1/LICENSE` & `structuretoolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/PKG-INFO` & `structuretoolkit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.1/README.md` & `structuretoolkit-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # structuretoolkit 
+
+[![Unittests](https://github.com/pyiron/structuretoolkit/actions/workflows/unittests.yml/badge.svg)](https://github.com/pyiron/structuretoolkit/actions/workflows/unittests.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pyiron/structuretoolkit/badge.svg?branch=main)](https://coveralls.io/github/pyiron/structuretoolkit?branch=main)
+
 Originally developed as part of the `pyiron_atomistics` module the `structuretoolkit` was release as standalone library
 for analysing, building and visualising atomistic structures. Internally it uses the `ase.atoms.Atoms` class to 
 represent atomistic structures in python. The `structuretoolkit` is integrated inside `pyiron_atomistics`.
 
 ## Disclaimer 
 The `structuretoolkit` is currently under development. 
 
@@ -44,8 +48,8 @@
 * `B2`
 * `C14`
 * `C15`
 * `C36`
 * `D03`
 
 ### Visualize 
-* `plot3d`
+* `plot3d`
```

### Comparing `structuretoolkit-0.0.1/setup.py` & `structuretoolkit-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/__init__.py` & `structuretoolkit-0.0.2/structuretoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/distance.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/distance.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/neighbors.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/phonopy.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/phonopy.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 __version__ = "1.0"
 __maintainer__ = "Osamu Waseda"
 __email__ = "waseda@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
 
-def analyse_phonopy_equivalent_atoms(atoms, symprec=1e-5, angle_tolerance=-1.0):
+def analyse_phonopy_equivalent_atoms(structure, symprec=1e-5, angle_tolerance=-1.0):
     """
     Args: (read phonopy.structure.spglib for more details)
         symprec:
             float: Symmetry search tolerance in the unit of length.
         angle_tolerance:
             float: Symmetry search tolerance in the unit of angle deg.
                 If the value is negative, an internally optimized routine
                 is used to judge symmetry.
 
     """
-    positions = atoms.get_scaled_positions()
-    cell = atoms.cell
-    types = atoms.get_chemical_symbols()
+    positions = structure.get_scaled_positions()
+    cell = structure.cell
+    types = structure.get_chemical_symbols()
     types = list(types)
     natom = len(types)
     positions = np.reshape(np.array(positions), (natom, 3))
     cell = np.reshape(np.array(cell), (3, 3))
     unitcell = PhonopyAtoms(symbols=types, cell=cell, scaled_positions=positions)
     ops = spg.get_symmetry(unitcell, symprec=symprec, angle_tolerance=angle_tolerance)
     return ops["equivalent_atoms"]
```

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/pyscal.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/pyscal.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,38 @@
 __maintainer__ = "Sarath Menon"
 __email__ = "sarath.menon@rub.de"
 __status__ = "development"
 __date__ = "Nov 6, 2019"
 
 
 def get_steinhardt_parameter_structure(
-    atoms,
+    structure,
     neighbor_method="cutoff",
     cutoff=0,
     n_clusters=2,
     q=None,
     averaged=False,
 ):
     """
     Calculate Steinhardts parameters
 
     Args:
-        atoms (Atoms): The structure to analyse.
+        structure (Atoms): The structure to analyse.
         neighbor_method (str) : can be ['cutoff', 'voronoi']. (Default is 'cutoff'.)
         cutoff (float) : Can be 0 for adaptive cutoff or any other value. (Default is 0, adaptive.)
         n_clusters (int/None) : Number of clusters for K means clustering or None to not cluster. (Default is 2.)
         q (list) : Values can be integers from 2-12, the required q values to be calculated. (Default is None, which
             uses (4, 6).)
         averaged (bool) : If True, calculates the averaged versions of the parameter. (Default is False.)
 
     Returns:
         numpy.ndarray: (number of q's, number of atoms) shaped array of q parameters
         numpy.ndarray: If `clustering=True`, an additional per-atom array of cluster ids is also returned
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     q = (4, 6) if q is None else q
 
     sys.find_neighbors(method=neighbor_method, cutoff=cutoff)
 
     sys.calculate_q(q, averaged=averaged)
 
     sysq = np.array(sys.get_qvals(q, averaged=averaged))
@@ -57,47 +57,47 @@
 
         ind = cl.fit(list(zip(*sysq))).labels_
         return sysq, ind
     else:
         return sysq
 
 
-def analyse_centro_symmetry(atoms, num_neighbors=12):
+def analyse_centro_symmetry(structure, num_neighbors=12):
     """
     Analyse centrosymmetry parameter
 
     Args:
-        atoms: Atoms object
+        structure: Atoms object
         num_neighbors (int) : number of neighbors
 
     Returns:
         csm (list) : list of centrosymmetry parameter
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     return np.array(sys.calculate_centrosymmetry(nmax=num_neighbors))
 
 
-def analyse_diamond_structure(atoms, mode="total", ovito_compatibility=False):
+def analyse_diamond_structure(structure, mode="total", ovito_compatibility=False):
     """
     Analyse diamond structure
 
     Args:
-        atoms: Atoms object
+        structure: Atoms object
         mode ("total"/"numeric"/"str"): Controls the style and level
         of detail of the output.
             - total : return number of atoms belonging to each structure
             - numeric : return a per atom list of numbers- 0 for unknown,
                 1 fcc, 2 hcp, 3 bcc and 4 icosa
             - str : return a per atom string of sructures
         ovito_compatibility(bool): use ovito compatiblity mode
 
     Returns:
         (depends on `mode`)
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     diamond_dict = sys.identify_diamond()
 
     ovito_identifiers = [
         "Cubic diamond",
         "Cubic diamond (1st neighbor)",
         "Cubic diamond (2nd neighbor)",
         "Hexagonal diamond",
@@ -174,32 +174,32 @@
             )
     else:
         raise ValueError(
             "Only total, str and numeric mode is imported for analyse_diamond_structure()"
         )
 
 
-def analyse_cna_adaptive(atoms, mode="total", ovito_compatibility=False):
+def analyse_cna_adaptive(structure, mode="total", ovito_compatibility=False):
     """
     Use common neighbor analysis
 
     Args:
-        atoms (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
+        structure (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
         mode ("total"/"numeric"/"str"): Controls the style and level
             of detail of the output.
             - total : return number of atoms belonging to each structure
             - numeric : return a per atom list of numbers- 0 for unknown,
                 1 fcc, 2 hcp, 3 bcc and 4 icosa
             - str : return a per atom string of sructures
         ovito_compatibility(bool): use ovito compatiblity mode
 
     Returns:
         (depends on `mode`)
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     if mode not in ["total", "numeric", "str"]:
         raise ValueError("Unsupported mode")
 
     pyscal_parameter = ["others", "fcc", "hcp", "bcc", "ico"]
     ovito_parameter = [
         "CommonNeighborAnalysis.counts.OTHER",
         "CommonNeighborAnalysis.counts.FCC",
@@ -212,16 +212,16 @@
 
     if mode == "total":
         if not ovito_compatibility:
             return cna
         else:
             return {o: cna[p] for o, p in zip(ovito_parameter, pyscal_parameter)}
     else:
-        atoms = sys.atoms
-        cnalist = np.array([atom.structure for atom in atoms])
+        structure = sys.atoms
+        cnalist = np.array([atom.structure for atom in structure])
         if mode == "numeric":
             return cnalist
         elif mode == "str":
             if not ovito_compatibility:
                 dd = ["others", "fcc", "hcp", "bcc", "ico"]
                 return np.array([dd[int(x)] for x in cnalist])
             else:
@@ -229,48 +229,48 @@
                 return np.array([dd[int(x)] for x in cnalist])
         else:
             raise ValueError(
                 "Only total, str and numeric mode is imported for analyse_cna_adaptive()"
             )
 
 
-def analyse_voronoi_volume(atoms):
+def analyse_voronoi_volume(structure):
     """
     Calculate the Voronoi volume of atoms
 
     Args:
-        atoms : (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
+        structure : (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     sys.find_neighbors(method="voronoi")
-    atoms = sys.atoms
-    return np.array([atom.volume for atom in atoms])
+    structure = sys.atoms
+    return np.array([atom.volume for atom in structure])
 
 
-def pyiron_to_pyscal_system(atoms):
+def pyiron_to_pyscal_system(structure):
     """
     Converts atoms to ase atoms and than to a pyscal system.
     Also adds the pyscal publication.
 
     Args:
-        atoms (pyiron atoms): Structure to convert.
+        structure (pyiron atoms): Structure to convert.
 
     Returns:
         Pyscal system: See the pyscal documentation.
     """
     sys = pc.System()
     sys.read_inputfile(
-        atoms,
+        structure,
         format="ase",
     )
     return sys
 
 
 def analyse_find_solids(
-    atoms,
+    structure,
     neighbor_method="cutoff",
     cutoff=0,
     bonds=0.5,
     threshold=0.5,
     avgthreshold=0.6,
     cluster=False,
     q=6,
@@ -292,23 +292,23 @@
         right (bool, optional): See pyscal documentation. Defaults to True.
         return_sys (bool, optional): Whether to return number of solid atoms or pyscal system. Defaults to False.
 
     Returns:
         int: number of solids,
         pyscal system: pyscal system when return_sys=True
     """
-    sys = pyiron_to_pyscal_system(atoms)
+    sys = pyiron_to_pyscal_system(structure)
     sys.find_neighbors(method=neighbor_method, cutoff=cutoff)
     sys.find_solids(
         bonds=bonds,
         threshold=threshold,
         avgthreshold=avgthreshold,
         q=q,
         cutoff=cutoff,
         cluster=cluster,
         right=right,
     )
     if return_sys:
         return sys
-    atoms = sys.atoms
-    solids = [atom for atom in atoms if atom.solid]
+    structure = sys.atoms
+    solids = [atom for atom in structure if atom.solid]
     return len(solids)
```

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/spatial.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/spatial.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/strain.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/strain.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         distances = np.linalg.norm(
             coords[:, :, None, :] - ref_coord[None, None, :, :], axis=-1
         )
         return np.argmin(distances, axis=-1)
 
     @staticmethod
     def _get_majority_phase(structure):
-        cna = analyse_cna_adaptive(atoms=structure)
+        cna = analyse_cna_adaptive(structure=structure)
         return np.asarray([k for k in cna.keys()])[np.argmax([v for v in cna.values()])]
 
     @staticmethod
     def _get_number_of_neighbors(crystal_phase):
         if crystal_phase == "bcc":
             return 8
         elif crystal_phase == "fcc" or crystal_phase == "hcp":
```

### Comparing `structuretoolkit-0.0.1/structuretoolkit/analyse/symmetry.py` & `structuretoolkit-0.0.2/structuretoolkit/analyse/symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/build/aimsgb.py` & `structuretoolkit-0.0.2/structuretoolkit/build/aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/build/compound.py` & `structuretoolkit-0.0.2/structuretoolkit/build/compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/build/sqs.py` & `structuretoolkit-0.0.2/structuretoolkit/build/sqs.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/build/surface.py` & `structuretoolkit-0.0.2/structuretoolkit/build/surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/helper.py` & `structuretoolkit-0.0.2/structuretoolkit/helper.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit/visualize.py` & `structuretoolkit-0.0.2/structuretoolkit/visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/structuretoolkit.egg-info/PKG-INFO` & `structuretoolkit-0.0.2/structuretoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.1/structuretoolkit.egg-info/SOURCES.txt` & `structuretoolkit-0.0.2/structuretoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_aimsgb.py` & `structuretoolkit-0.0.2/tests/test_aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_analyse.py` & `structuretoolkit-0.0.2/tests/test_analyse.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
         self.assertEqual(len(np.unique(layers[stk.get_layers(structure=structure)[:, 0] == 0, 0])), 1)
 
     def test_pyscal_cna_adaptive(self):
         basis = Atoms(
             "FeFe", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=np.identity(3)
         )
         self.assertTrue(
-            stk.analyse_cna_adaptive(atoms=basis)["bcc"] == 2
+            stk.analyse_cna_adaptive(structure=basis)["bcc"] == 2
         )
 
     def test_pyscal_centro_symmetry(self):
         basis = bulk(name='Fe', a=2.8, crystalstructure='bcc', cubic=True)
         self.assertTrue(
-            all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(atoms=basis, num_neighbors=8)])
+            all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=basis, num_neighbors=8)])
         )
 
     def test_get_voronoi_vertices(self):
         basis = bulk(name='Al', a=4, crystalstructure='fcc', cubic=True)
         self.assertEqual(len(stk.get_voronoi_vertices(structure=basis)), 12)
         self.assertEqual(len(stk.get_voronoi_vertices(structure=basis, distance_threshold=2)), 1)
```

### Comparing `structuretoolkit-0.0.1/tests/test_compound.py` & `structuretoolkit-0.0.2/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_high_index_surface.py` & `structuretoolkit-0.0.2/tests/test_high_index_surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_neighbors.py` & `structuretoolkit-0.0.2/tests/test_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
         self.assertAlmostEqual(cs.max(), 0)
         self.assertAlmostEqual(cs.min(), 0)
         structure.positions += 0.01*(2*np.random.random(structure.positions.shape)-1)
         neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
         self.assertGreater(neigh.centrosymmetry.min(), 0)
         self.assertTrue(
             np.allclose(
-                neigh.centrosymmetry, stk.analyse_centro_symmetry(atoms=structure, num_neighbors=8)
+                neigh.centrosymmetry, stk.analyse_centro_symmetry(structure=structure, num_neighbors=8)
             )
         )
 
     def test_get_all_pairs(self):
         structure = bulk('Fe').repeat(4)
         neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
         for n in [2, 4, 6]:
```

### Comparing `structuretoolkit-0.0.1/tests/test_pyscal.py` & `structuretoolkit-0.0.2/tests/test_pyscal.py`

 * *Files 26% similar despite different names*

```diff
@@ -85,124 +85,124 @@
     def test_steinhardt_parameters(self):
         """ Test the calculation of Steinhardts parameters using the Analyse class. """
         perfect_vals = [0.00, 0.00, 0.190, 0.00, 0.575, 0.00, 0.404, 0.00,
                         0.013, 0.00, 0.600]
 
         qtest = np.random.randint(2, 13, size=2)
 
-        qs, _ = stk.get_steinhardt_parameter_structure(atoms=self.al_fcc_4, cutoff=0, n_clusters=2, q=qtest)
+        qs, _ = stk.get_steinhardt_parameter_structure(structure=self.al_fcc_4, cutoff=0, n_clusters=2, q=qtest)
         for c, q in enumerate(qs):
             self.assertLess(np.abs(np.mean(q) - perfect_vals[qtest[c]-2]), 1E-3)
 
     def test_analyse_pyscal_centro_symmetry(self):
-        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(atoms=self.al_fcc, num_neighbors=12)]))
-        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(atoms=self.fe_bcc, num_neighbors=8)]))
-        self.assertTrue(all([np.isclose(v, 8.7025) for v in stk.analyse_centro_symmetry(atoms=self.ti_hcp, num_neighbors=12)]))
-        self.assertTrue(all([np.isclose(v, 14.742449) for v in stk.analyse_centro_symmetry(atoms=self.si_dia, num_neighbors=4)]))
-        self.assertEqual(len(stk.analyse_centro_symmetry(atoms=self.al_fcc)), len(self.al_fcc))
-        self.assertEqual(len(stk.analyse_centro_symmetry(atoms=self.fe_bcc)), len(self.fe_bcc))
-        self.assertEqual(len(stk.analyse_centro_symmetry(atoms=self.ti_hcp)), len(self.ti_hcp))
-        self.assertEqual(len(stk.analyse_centro_symmetry(atoms=self.si_dia)), len(self.si_dia))
+        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=self.al_fcc, num_neighbors=12)]))
+        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=self.fe_bcc, num_neighbors=8)]))
+        self.assertTrue(all([np.isclose(v, 8.7025) for v in stk.analyse_centro_symmetry(structure=self.ti_hcp, num_neighbors=12)]))
+        self.assertTrue(all([np.isclose(v, 14.742449) for v in stk.analyse_centro_symmetry(structure=self.si_dia, num_neighbors=4)]))
+        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.al_fcc)), len(self.al_fcc))
+        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.fe_bcc)), len(self.fe_bcc))
+        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.ti_hcp)), len(self.ti_hcp))
+        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.si_dia)), len(self.si_dia))
 
     def test_analyse_pyscal_voronoi_volume(self):
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(atoms=self.al_fcc)), 16.60753125)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(atoms=self.fe_bcc)), 11.8199515)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(atoms=self.ti_hcp)), 17.65294557)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(atoms=self.si_dia)), 20.01287587)
-        self.assertEqual(len(stk.analyse_voronoi_volume(atoms=self.al_fcc)), len(self.al_fcc))
-        self.assertEqual(len(stk.analyse_voronoi_volume(atoms=self.fe_bcc)), len(self.fe_bcc))
-        self.assertEqual(len(stk.analyse_voronoi_volume(atoms=self.ti_hcp)), len(self.ti_hcp))
-        self.assertEqual(len(stk.analyse_voronoi_volume(atoms=self.si_dia)), len(self.si_dia))
+        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.al_fcc)), 16.60753125)
+        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.fe_bcc)), 11.8199515)
+        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.ti_hcp)), 17.65294557)
+        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.si_dia)), 20.01287587)
+        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.al_fcc)), len(self.al_fcc))
+        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.fe_bcc)), len(self.fe_bcc))
+        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.ti_hcp)), len(self.ti_hcp))
+        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.si_dia)), len(self.si_dia))
 
     def test_analyse_pyscal_cna_adaptive(self):
         pyscal_keys = [
             'others', 'fcc', 'hcp', 'bcc', 'ico',
         ]
         ovito_keys = [
             'CommonNeighborAnalysis.counts.OTHER',
             'CommonNeighborAnalysis.counts.FCC',
             'CommonNeighborAnalysis.counts.HCP',
             'CommonNeighborAnalysis.counts.BCC',
              'CommonNeighborAnalysis.counts.ICO'
         ]
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[1]], len(self.al_fcc))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[3]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[2]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.si_dia, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 1 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 3 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 2 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'fcc' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'bcc' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'hcp' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_cna_adaptive(structure=self.si_dia, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'others' for v in res_str]))
 
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[1]], len(self.al_fcc))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[3]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[2]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_cna_adaptive(structure=self.si_dia, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 1 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 3 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 2 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_cna_adaptive(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_cna_adaptive(atoms=self.al_fcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'FCC' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.fe_bcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'BCC' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.ti_hcp, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'HCP' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(atoms=self.si_dia, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_cna_adaptive(structure=self.si_dia, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'Other' for v in res_str]))
 
     def test_analyse_pyscal_diamond_structure(self):
         pyscal_keys = [
             'others', 'fcc', 'hcp', 'bcc', 'ico',
             'cubic diamond', 'cubic diamond 1NN', 'cubic diamond 2NN',
@@ -213,88 +213,88 @@
             'IdentifyDiamond.counts.CUBIC_DIAMOND_FIRST_NEIGHBOR',
             'IdentifyDiamond.counts.CUBIC_DIAMOND_SECOND_NEIGHBOR',
             'IdentifyDiamond.counts.HEX_DIAMOND',
             'IdentifyDiamond.counts.HEX_DIAMOND_FIRST_NEIGHBOR',
             'IdentifyDiamond.counts.HEX_DIAMOND_SECOND_NEIGHBOR',
             'IdentifyDiamond.counts.OTHER'
         ]
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.al_fcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.al_fcc))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.si_dia, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.si_dia, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[5]], len(self.si_dia))
 
-        res_numeric = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_diamond_structure(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.si_dia, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse_diamond_structure(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 5 for v in res_numeric]))
 
-        res_str = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_diamond_structure(structure=self.al_fcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.si_dia, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse_diamond_structure(structure=self.si_dia, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'cubic diamond' for v in res_str]))
 
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.al_fcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.al_fcc))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_diamond_structure(atoms=self.si_dia, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse_diamond_structure(structure=self.si_dia, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_diamond_structure(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(atoms=self.si_dia, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse_diamond_structure(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_diamond_structure(atoms=self.al_fcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_diamond_structure(structure=self.al_fcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.fe_bcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.ti_hcp, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(atoms=self.si_dia, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse_diamond_structure(structure=self.si_dia, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'Cubic diamond' for v in res_str]))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `structuretoolkit-0.0.1/tests/test_strain.py` & `structuretoolkit-0.0.2/tests/test_strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_symmetry.py` & `structuretoolkit-0.0.2/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/tests/test_visualize.py` & `structuretoolkit-0.0.2/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.1/versioneer.py` & `structuretoolkit-0.0.2/versioneer.py`

 * *Files identical despite different names*

