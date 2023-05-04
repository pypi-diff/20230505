# Comparing `tmp/pymatgen-analysis-defects-2023.4.5.tar.gz` & `tmp/pymatgen-analysis-defects-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.4.5.tar", last modified: Wed Apr  5 20:08:09 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.5.4.tar", last modified: Thu May  4 22:57:36 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.4.5.tar` & `pymatgen-analysis-defects-2023.5.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.314755 pymatgen-analysis-defects-2023.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-05 20:08:09.314755 pymatgen-analysis-defects-2023.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.310754 pymatgen-analysis-defects-2023.4.5/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.310754 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.310754 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.310754 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    39008 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.310754 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-05 20:08:09.000000 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-05 20:08:09.000000 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:08:09.000000 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-05 20:08:09.000000 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-05 20:08:09.000000 pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 20:08:09.314755 pymatgen-analysis-defects-2023.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:08:09.314755 pymatgen-analysis-defects-2023.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-05 20:07:48.000000 pymatgen-analysis-defects-2023.4.5/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-05 20:07:49.000000 pymatgen-analysis-defects-2023.4.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 22:57:36.127658 pymatgen-analysis-defects-2023.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.119658 pymatgen-analysis-defects-2023.5.4/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.119658 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42384 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:57:36.127658 pymatgen-analysis-defects-2023.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.4.5/LICENSE` & `pymatgen-analysis-defects-2023.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/PKG-INFO` & `pymatgen-analysis-defects-2023.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.4.5
+Version: 2023.5.4
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.4.5/README.rst` & `pymatgen-analysis-defects-2023.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import numpy as np
 from monty.json import MSONable
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core import Element, PeriodicSite, Species, Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.symmetry.structure import SymmetrizedStructure
+from pyrho.utils import get_plane_spacing
 
 from pymatgen.analysis.defects.supercells import get_sc_fromstruct
 
 # TODO Possible redesign idea: ``DefectSite`` class defined with a defect object.
 # This makes some of the accounting logic a bit harder since we will probably
 # just have one concrete ``Defect`` class so you can write custom multiplicity functions
 # but it makes the implementation of defect complexes trivial.
@@ -158,24 +159,26 @@
         self,
         sc_mat: np.ndarray | None = None,
         dummy_species: str | None = None,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10.0,
         force_diagonal: bool = False,
+        relax_radius: float | str | None = None,
     ) -> Structure:
         """Generate the supercell for a defect.
 
         Args:
             sc_mat: supercell matrix if None, the supercell will be determined by `CubicSupercellAnalyzer`.
             dummy_species: Dummy species to highlight the defect position (for visualizing vacancies).
             max_atoms: Maximum number of atoms allowed in the supercell.
             min_atoms: Minimum number of atoms allowed in the supercell.
             min_length: Minimum length of the smallest supercell lattice vector.
             force_diagonal: If True, return a transformation with a diagonal transformation matrix.
+            relax_radius: Relax the supercell atoms to a sphere of this radius around the defect site.
 
         Returns:
             Structure: The supercell structure.
         """
         if sc_mat is None:
             sc_mat = get_sc_fromstruct(
                 self.structure,
@@ -191,19 +194,25 @@
         sc_site = PeriodicSite(self.site.specie, sc_pos, sc_structure.lattice)
 
         sc_defect = self.__class__(
             structure=sc_structure, site=sc_site, oxi_state=self.oxi_state
         )
         sc_defect_struct = sc_defect.defect_structure
         sc_defect_struct.remove_oxidation_states()
+
         if dummy_species is not None:
             dummy_pos = np.dot(self.site.frac_coords, sc_mat_inv)
             dummy_pos = np.mod(dummy_pos, 1)
             sc_defect_struct.insert(len(sc_structure), dummy_species, dummy_pos)
 
+        _set_selective_dynamics(
+            structure=sc_defect_struct,
+            site_pos=sc_pos,
+            relax_radius=relax_radius,
+        )
         return sc_defect_struct
 
     @property
     def symmetrized_structure(self) -> SymmetrizedStructure:
         """Returns the multiplicity of a defect site within the structure.
 
         This is required for concentration analysis and confirms that defect_site is a
@@ -565,14 +574,15 @@
         self,
         sc_mat: np.ndarray | None = None,
         dummy_species: Species | None = None,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10.0,
         force_diagonal: bool = False,
+        relax_radius: float | str | None = None,
     ) -> Structure:
         """Generate the supercell for a defect.
 
         Args:
             sc_mat: supercell matrix if None, the supercell will be determined by `CubicSupercellAnalyzer`.
             dummy_species: Dummy species used for visualization. Will be placed at the average
                 position of the defect sites.
@@ -588,30 +598,35 @@
             sc_mat = get_sc_fromstruct(
                 self.structure,
                 min_atoms=min_atoms,
                 max_atoms=max_atoms,
                 min_length=min_length,
                 force_diagonal=force_diagonal,
             )
-        sc_structure = self.structure * sc_mat
+        sc_defect_struct = self.structure * sc_mat
         sc_mat_inv = np.linalg.inv(sc_mat)
         complex_pos = np.zeros(3)
         for defect in self.defects:
             sc_pos = np.dot(defect.site.frac_coords, sc_mat_inv)
             complex_pos += sc_pos
-            sc_site = PeriodicSite(defect.site.specie, sc_pos, sc_structure.lattice)
-            update_structure(sc_structure, sc_site, defect_type=defect.defect_type)
-        complex_pos /= len(self.defects)
+            sc_site = PeriodicSite(defect.site.specie, sc_pos, sc_defect_struct.lattice)
+            update_structure(sc_defect_struct, sc_site, defect_type=defect.defect_type)
+        complex_pos /= float(len(self.defects))
         if dummy_species is not None:
             for defect in self.defects:
                 dummy_pos = np.dot(defect.site.frac_coords, sc_mat_inv)
                 dummy_pos = np.mod(dummy_pos, 1)
-                sc_structure.insert(len(sc_structure), dummy_species, dummy_pos)
+                sc_defect_struct.insert(len(sc_defect_struct), dummy_species, dummy_pos)
 
-        return sc_structure
+        _set_selective_dynamics(
+            structure=sc_defect_struct,
+            site_pos=sc_pos,
+            relax_radius=relax_radius,
+        )
+        return sc_defect_struct
 
 
 def update_structure(structure, site, defect_type):
     """Update the structure with the defect site.
 
     Types of operations:
         1. Vacancy: remove the site.
@@ -697,12 +712,31 @@
         isite: The site index of the vacancy.
         **kwargs: Keyword arguments to pass to Vacancy constructor.
     """
     site = structure[isite]
     return Vacancy(structure=structure, site=site, **kwargs)
 
 
+def _set_selective_dynamics(structure, site_pos, relax_radius):
+    if relax_radius is None:
+        return
+    if relax_radius == "auto":
+        relax_radius = min(get_plane_spacing(structure.lattice.matrix)) / 2.0
+    if not isinstance(relax_radius, float):
+        raise ValueError("relax_radius must be a float or 'auto' or None")
+
+    structure.get_sites_in_sphere(site_pos, relax_radius)
+    relax_sites = structure.get_sites_in_sphere(
+        [0, 0, 0], relax_radius, include_index=True
+    )
+    relax_indices = [site.index for site in relax_sites]
+    relax_mask = [[False, False, False]] * len(structure)
+    for i in relax_indices:
+        relax_mask[i] = [True, True, True]
+    structure.add_site_property("selective_dynamics", relax_mask)
+
+
 # TODO: matching defect complexes might be done with some kind of CoM site to fix the periodicity
 # Get this by taking the periodic average of all the provided sites.
 # class DefectComplex(DummySpecies):
 #     def __init__(self, oxidation_state: float = 0, properties: dict | None = None):
 #         super().__init__("Vac", oxidation_state, properties)
```

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,53 +6,58 @@
 
 from __future__ import annotations
 
 import logging
 import math
 from pathlib import Path
 
+from pymatgen.core import Structure
+from pymatgen.io.vasp import Outcar, Vasprun
+
 from pymatgen.analysis.defects.utils import CorrectionResult, get_zfile
 
-# check that pydefect is installed
 try:
     from vise import user_settings
 
     # Disable messages from pydefect import
     user_settings.logger.setLevel(logging.CRITICAL)
     from pydefect.analyzer.calc_results import CalcResults
     from pydefect.cli.vasp.make_efnv_correction import make_efnv_correction
 
+    __has_pydefect__ = True
 except ImportError:  # pragma: no cover
-    raise ModuleNotFoundError(
-        "vise/pydefect is not installed. Please install it first."
-    )
-
-
-from pymatgen.core import Structure
-from pymatgen.io.vasp import Outcar, Vasprun
+    __has_pydefect__ = False
 
 __author__ = "Jimmy-Xuan Shen"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy-Xuan Shen"
 __email__ = "jmmshn@gmail.com"
-
 _logger = logging.getLogger(__name__)
 # suppress pydefect INFO messages
 logging.getLogger("pydefect").setLevel(logging.WARNING)
 
 
+def _check_import_pydefect():
+    """Import pydefect if it is installed."""
+    if __has_pydefect__:
+        raise ModuleNotFoundError(
+            "vise/pydefect is not installed. Please install it first."
+        )
+
+
 def get_structure_with_pot(directory: Path) -> Structure:
     """Reads vasprun.xml and OUTCAR files in a directory.
 
     Args:
         directory: Directory containing vasprun.xml and OUTCAR files.
 
     Returns:
         Structure with "potential" site property.
     """
+    _check_import_pydefect()
     d_ = Path(directory)
     f_vasprun = get_zfile(d_, "vasprun.xml")
     f_outcar = get_zfile(d_, "OUTCAR")
     vasprun = Vasprun(f_vasprun)
     outcar = Outcar(f_outcar)
 
     calc = CalcResults(
@@ -80,14 +85,15 @@
     Args:
         charge: Charge of the defect.
         defect_structure: Defect structure.
         bulk_structure: Bulk structure.
         dielectric_tensor: Dielectric tensor.
         **kwargs: Keyword arguments to pass to `make_efnv_correction`.
     """
+    _check_import_pydefect()
     # ensure that the structures have the "potential" site property
     bulk_potentials = [site.properties["potential"] for site in defect_structure]
     defect_potentials = [site.properties["potential"] for site in bulk_structure]
 
     defect_calc_results = CalcResults(
         structure=defect_structure,
         energy=math.inf,
```

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/thermo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Classes and methods related to thermodynamics and energy."""
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, field
-from itertools import groupby
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional
 
 import numpy as np
 from matplotlib import cm
 from matplotlib import pyplot as plt
 from matplotlib.lines import Line2D
 from monty.json import MSONable
 from numpy.typing import ArrayLike, NDArray
 from pymatgen.analysis.chempot_diagram import ChemicalPotentialDiagram
 from pymatgen.analysis.phase_diagram import PhaseDiagram
-from pymatgen.core import Composition, Structure
+from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
+from pymatgen.core import Composition, Element, Structure
 from pymatgen.electronic_structure.dos import Dos, FermiDos
 from pymatgen.entries.computed_entries import ComputedEntry, ComputedStructureEntry
 from pymatgen.io.vasp import Locpot, Vasprun
 from scipy.constants import value as _cd
 from scipy.optimize import bisect
 from scipy.spatial import ConvexHull
 
 from pymatgen.analysis.defects.core import Defect
 from pymatgen.analysis.defects.corrections.freysoldt import get_freysoldt_correction
 from pymatgen.analysis.defects.finder import DefectSiteFinder
-from pymatgen.analysis.defects.utils import CorrectionResult, get_zfile
+from pymatgen.analysis.defects.utils import CorrectionResult, get_zfile, group_docs
 
 __author__ = "Jimmy-Xuan Shen, Danny Broberg, Shyam Dwaraknath"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy-Xuan Shen"
 __email__ = "jmmshn@gmail.com"
 
 _logger = logging.getLogger(__name__)
@@ -223,15 +223,15 @@
     def __post_init__(self):
         """Post-initialization.
 
         - Reconstruct the phase diagram with the bulk entry
         - Make sure that the bulk entry is stable
         - create the chemical potential diagram using only the formation energies
         """
-        g = group_defects(self.defect_entries)
+        g = group_defect_entries(self.defect_entries)
         if next(g, True) and next(g, False):
             raise ValueError(
                 "Defects are not of same type! "
                 "Use MultiFormationEnergyDiagram for multiple defect types"
             )
         # if all of the `DefectEntry` objects have the same `bulk_entry` then `self.bulk_entry` is not needed
         if any(d.bulk_entry is None for d in self.defect_entries):
@@ -554,27 +554,73 @@
         from pandas import DataFrame
 
         defect_entries = self.defect_entries
         l_ = map(lambda x: x.get_summary_dict(), defect_entries)
         df = DataFrame(l_)
         return df
 
+    def get_chempots(self, rich_element: Element | str, en_tol: float = 0.01):
+        """Get the chemical potential for a desired growth condition.
+
+        Choose an element to be rich in, require the chemical potential of that element
+        to be near zero (en_tol, 0), then sort the remaining elements by:
+            1. Are they in the bulk structure:
+                elements in the bulk structure are prioritized.
+            2. how similar they in electron affinity to the rich element:
+                dis-similar elements are prioritized.
+
+        .. note::
+            Priority 2 is pretty arbitrary, but it is a good starting point.
+
+
+        Based on that priority list, take the minimum chemical potential extrema.
+
+        Args:
+            rich_element: The element that are rich in the growth condition.
+            en_tol: Energy tolerance for the chemical potential of the rich element.
+
+        Returns:
+            A dictionary of the chemical potentials for the growth condition.
+        """
+        rich_element = Element(rich_element)
+        rich_conditions = list(
+            filter(lambda cp: abs(cp[rich_element]) < en_tol, self.chempot_limits)
+        )
+        if len(rich_conditions) == 0:
+            raise ValueError(
+                f"Cannot find a chemical potential condition with {rich_element} near zero."
+            )
+        defect = self.defect_entries[0].defect
+        in_bulk = defect.structure.composition.elements
+        # make sure they are of type Element
+        in_bulk = list(map(lambda x: Element(x.symbol), in_bulk))
+        not_in_bulk = list(set(self.chempot_limits[0].keys()) - set(in_bulk))
+        in_bulk = list(filter(lambda x: x != rich_element, in_bulk))
+
+        def el_sorter(element):
+            return -abs(element.electron_affinity - rich_element.electron_affinity)
+
+        el_list = sorted(in_bulk, key=el_sorter) + sorted(not_in_bulk, key=el_sorter)
+
+        def chempot_sorter(chempot_dict):
+            return (chempot_dict[el] for el in el_list)
+
+        return min(rich_conditions, key=chempot_sorter)
+
 
 @dataclass
 class MultiFormationEnergyDiagram(MSONable):
     """Container for multiple formation energy diagrams."""
 
     formation_energy_diagrams: List[FormationEnergyDiagram]
 
     def __post_init__(self):
         """Set some attributes after initialization."""
         self.band_gap = self.formation_energy_diagrams[0].band_gap
         self.vbm = self.formation_energy_diagrams[0].vbm
-        self.chempot_limits = self.formation_energy_diagrams[0].chempot_limits
-        self.chempot_diagram = self.formation_energy_diagrams[0].chempot_diagram
 
     @classmethod
     def with_atomic_entries(
         cls,
         bulk_entry: ComputedEntry,
         defect_entries: list[DefectEntry],
         atomic_entries: list[ComputedEntry],
@@ -584,15 +630,15 @@
     ) -> MultiFormationEnergyDiagram:
         """Initialize using atomic entries.
 
         Initializes by grouping defect types, and creating a list of single
         FormationEnergyDiagram using the with_atomic_entries method (see above)
         """
         single_form_en_diagrams = []
-        for _, defect_group in group_defects(defect_entries=defect_entries):
+        for _, defect_group in group_defect_entries(defect_entries=defect_entries):
             _fd = FormationEnergyDiagram.with_atomic_entries(
                 bulk_entry=bulk_entry,
                 defect_entries=defect_group,
                 atomic_entries=atomic_entries,
                 phase_diagram=phase_diagram,
                 vbm=vbm,
                 **kwargs,
@@ -640,22 +686,72 @@
                 fermi_level=ef + fdos_vbm, temperature=temperature
             )
             return qd_tot
 
         return bisect(_get_total_q, -1.0, fdos_cbm - fdos_vbm + 1.0)
 
 
-def group_defects(defect_entries: list[DefectEntry]):
-    """Group defects by their representation.
+def group_defect_entries(
+    defect_entries: list[DefectEntry], sm: StructureMatcher = None
+):
+    """Group defect entries by their representation.
+
+    First by name then by structure.
+
+    Args:
+        defect_entries: list of defect entries
+        sm: StructureMatcher to use for grouping
+
+    Returns:
+        Generator of (name, list of defect entries) tuples
+    """
+    if sm is None:
+        sm = StructureMatcher(comparator=ElementComparator())
+
+    def _get_structure(entry):
+        return entry.defect.defect_structure
+
+    def _get_name(entry):
+        return entry.defect.name
+
+    ent_groups = group_docs(
+        defect_entries, sm=sm, get_structure=_get_structure, get_hash=_get_name
+    )
+    for g_name, g_entries in ent_groups:
+        yield g_name, g_entries
+
+
+def group_formation_energy_diagrams(
+    feds: list[FormationEnergyDiagram], sm: StructureMatcher = None
+):
+    """Group formation energy diagrams by their representation.
+
+    First by name then by structure.
+
+    Args:
+        feds: list of formation energy diagrams
+        sm: StructureMatcher to use for grouping
 
-    TODO: Fix this with `defect_structure` grouping with `StructureMatcher`.
+    Returns:
+        Generator of (name, list of formation energy diagrams) tuples
     """
-    sents = sorted(defect_entries, key=lambda x: x.defect.__repr__())
-    for k, group in groupby(sents, key=lambda x: x.defect.__repr__()):
-        yield k, list(group)
+    if sm is None:
+        sm = StructureMatcher(comparator=ElementComparator())
+
+    def _get_structure(fed):
+        return fed.defect.defect_structure
+
+    def _get_name(fed):
+        return fed.defect.name
+
+    fed_groups = group_docs(
+        feds, sm=sm, get_structure=_get_structure, get_hash=_get_name
+    )
+    for g_name, g_entries in fed_groups:
+        yield g_name, g_entries
 
 
 def ensure_stable_bulk(
     pd: PhaseDiagram,
     entry: ComputedEntry,
 ) -> PhaseDiagram:
     """Added entry to phase diagram and ensure that it is stable.
@@ -841,15 +937,16 @@
     return 1.0 / (1.0 + np.exp((energy) / (boltzman_eV_K * temperature)))
 
 
 def plot_formation_energy_diagrams(
     formation_energy_diagrams: FormationEnergyDiagram
     | List[FormationEnergyDiagram]
     | MultiFormationEnergyDiagram,
-    chempots: Dict,
+    rich_element: Element | None = None,
+    chempots: Dict | None = None,
     alignment: float = 0.0,
     xlim: list | None = None,
     ylim: list | None = None,
     only_lower_envelope: bool = True,
     show: bool = True,
     save: bool | str = False,
     colors: list | None = None,
@@ -858,20 +955,22 @@
     transition_markersize: int = 16,
     linestyle: str = "-",
     linewidth: int = 4,
     envelope_alpha: float = 0.8,
     line_alpha: float = 0.5,
     band_edge_color="k",
     filterfunction: Callable | None = None,
+    legend_loc: str = "lower center",
     axis=None,
 ):
     """Plot the formation energy diagram.
 
     Args:
         formation_energy_diagrams: Which formation energy lines to plot.
+        rich_element: The abundant element used to set the limit of the chemical potential.
         chempots: Chemical potentials at which to plot the formation energy lines
             Should be bounded by the chempot_limits property
         alignment: shift the energy axis by this amount. For example, giving bandgap/2
             will visually shift the 0 reference from the VBM to the middle of the band gap.
         xlim: Limits (low, high) to use for the x-axis. Default is to use 0eV for the
             VBM up to the band gap, plus a buffer of 0.2eV on each side
         ylim: Limits (low, high) to use for y-axis. Default is to use the minimum and
@@ -907,16 +1006,17 @@
     filterfunction = filterfunction if filterfunction else lambda x: True
     formation_energy_diagrams = list(filter(filterfunction, formation_energy_diagrams))
 
     band_gap = formation_energy_diagrams[0].band_gap
     if not xlim and not band_gap:
         raise ValueError("Must specify xlim or set band_gap attribute")
 
-    if not axis:
+    if axis is None:
         _, axis = plt.subplots()
+    axis.plot([0, 0], [0, 1], color=band_edge_color, linestyle="--", linewidth=1)
     if not xlim and band_gap:
         xmin, xmax = np.subtract(-0.2, alignment), np.subtract(
             band_gap + 0.2, alignment
         )
     else:
         xmin, xmax = xlim
     ymin, ymax = 0.0, 1.0
@@ -929,56 +1029,51 @@
     colors = (
         colors
         if colors
         else cm.Dark2(np.linspace(0, 1, len(formation_energy_diagrams)))
         if len(formation_energy_diagrams) <= 8
         else cm.gist_rainbow(np.linspace(0, 1, len(formation_energy_diagrams)))
     )
-
-    for fid, single_fed in enumerate(formation_energy_diagrams):
-        lines = single_fed._get_lines(chempots=chempots)
+    named_feds = []
+    for name_, feds_ in group_formation_energy_diagrams(formation_energy_diagrams):
+        for fed_ in feds_:
+            named_feds.append((name_, fed_))
+
+    for fid, (fed_name, single_fed) in enumerate(named_feds):
+        chempots_ = (
+            chempots
+            if chempots
+            else single_fed.get_chempots(rich_element=Element(rich_element))
+        )
+        lines = single_fed._get_lines(chempots=chempots_)
         lowerlines = get_lower_envelope(lines)
-        trans = get_transitions(
-            lowerlines, np.add(xmin, alignment), np.add(xmax, alignment)
+        trans = np.array(
+            get_transitions(
+                lowerlines, np.add(xmin, alignment), np.add(xmax, alignment)
+            )
+        )
+        axis.plot(
+            np.subtract(trans[:, 0], alignment),
+            trans[:, 1],
+            color=colors[fid],
+            ls=linestyle,
+            lw=linewidth,
+            alpha=envelope_alpha,
+            label=fed_name,
+            marker=transition_marker,
+            markersize=transition_markersize,
         )
-
-        # plot lines
         if not only_lower_envelope:
             for line in lines:
                 x = np.linspace(xmin, xmax)
                 y = line[0] * x + line[1]
                 axis.plot(
                     np.subtract(x, alignment), y, color=colors[fid], alpha=line_alpha
                 )
 
-        # plot connecting envelop lines
-        for i, (_x, _y) in enumerate(trans[:-1]):
-            x = np.linspace(_x, trans[i + 1][0])
-            y = ((trans[i + 1][1] - _y) / (trans[i + 1][0] - _x)) * (x - _x) + _y
-            axis.plot(
-                np.subtract(x, alignment),
-                y,
-                color=colors[fid],
-                ls=linestyle,
-                lw=linewidth,
-                alpha=envelope_alpha,
-            )
-
-        # Plot transitions
-        for _x, _y in trans:
-            ymax = max((ymax, _y))
-            ymin = min((ymin, _y))
-            axis.plot(
-                np.subtract(_x, alignment),
-                _y,
-                marker=transition_marker,
-                color=colors[fid],
-                markersize=transition_markersize,
-            )
-
         # get latex-like legend titles
         dfct = single_fed.defect_entries[0].defect
         flds = dfct.name.split("_")
         latexname = f"${flds[0]}_{{{flds[1]}}}$"
         if legend_prefix:
             latexname = f"{legend_prefix} {latexname}"
         legends_txt.append(latexname)
@@ -1024,20 +1119,21 @@
         )
 
     lg = axis.get_legend()
     if lg:
         handle, leg = lg.legendHandles, [txt._text for txt in lg.texts]
     else:
         handle, leg = [], []
+
     axis.legend(
         handles=artists + handle,
         labels=legends_txt + leg,
         fontsize=lg_fontsize * ax_fontsize,
         ncol=3,
-        loc="lower center",
+        loc=legend_loc,
     )
 
     if save:
         save = save if isinstance(save, str) else "formation_energy_diagram.png"
         plt.savefig(save)
     if show:
         plt.show()
```

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -982,7 +982,64 @@
         electrostatic: The electrostatic correction.
         potential_alignment: The potential alignment correction.
         metadata: A dictionary of metadata for plotting and intermediate analysis.
     """
 
     correction_energy: float
     metadata: dict[Any, Any]
+
+
+def _group_docs_by_structure(docs: list, sm: StructureMatcher, get_structure: Callable):
+    """Group docs by structure.
+
+    Args:
+        docs (list): list of generic documents/objects
+        sm (StructureMatcher): StructureMatcher object
+        get_hash (function): function to get the hash from the document
+
+    Returns:
+        Generator of lists of grouped documents/objects.
+    """
+    labs = generic_groupby(
+        docs,
+        comp=lambda x, y: sm.fit(get_structure(x), get_structure(y), symmetric=True),
+    )
+    for ilab in set(labs):
+        sub_g = [docs[itr] for itr, jlab in enumerate(labs) if jlab == ilab]
+        yield [el for el in sub_g]
+
+
+def group_docs(
+    docs: list,
+    sm: StructureMatcher,
+    get_structure: Callable,
+    get_hash: Callable | None = None,
+):
+    """Group docs by a simple hash followed by structure.
+
+    Assuming that you have a basic representation of the defect, like `name`.
+    Will first group the documents by name, then group them by the structure
+    of their representation.
+
+    Args:
+        docs (list): list of generic documents/objects
+        sm (StructureMatcher): StructureMatcher object
+        get_hash (function): function to get the hash from the document,
+            this should be some kind of simple string representation.
+        get_structure (function): function to get the structure from the document
+
+    Returns:
+        Generator of (name, group)
+    """
+    if get_hash is None:
+        for g in _group_docs_by_structure(docs, sm, get_structure):
+            yield None, g
+    else:
+        s_docs = sorted(docs, key=get_hash)
+        for h, g in itertools.groupby(s_docs, key=get_hash):
+            sgroups = list(_group_docs_by_structure(list(g), sm, get_structure))
+            if len(sgroups) <= 1:
+                for group in sgroups:
+                    yield h, group
+            else:
+                for itr, group in enumerate(sgroups):
+                    yield f"{h}:{itr}", group
```

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.4.5
+Version: 2023.5.4
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.4.5/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/pyproject.toml` & `pymatgen-analysis-defects-2023.5.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Programming Language :: Python :: 3.10",
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Science/Research",
   "Operating System :: OS Independent",
   "Topic :: Other/Nonlisted Topic",
   "Topic :: Scientific/Engineering",
 ]
-dependencies = ["pymatgen>=2022.10.22", "scikit-image>=0.19.3"]
+dependencies = ["pymatgen==2023.1.9", "scikit-image>=0.19.3", "mp-pyrho>=0.3.0", "numpy<=1.23.5"]
 description = "Pymatgen extension for defects analysis"
 dynamic = ["version"]
 keywords = ["high-throughput", "automated", "dft", "defects"]
 license = { text = "modified BSD" }
 name = "pymatgen-analysis-defects"
 readme = "README.rst"
 requires-python = '>=3.8'
@@ -29,21 +29,23 @@
 dev = ["pre-commit>=2.12.1"]
 docs = [
   "jupyter-book>=0.13.1",
 ]
 pydefect = ["pydefect>=0.6.2"]
 
 strict = [
-  "pymatgen==2023.2.22",
+  "pymatgen==2023.1.9",
   "dscribe==1.2.2",
   "scikit-image==0.19.3",
   "pytest==7.2.2",
   "pytest-cov==4.0.0",
   "pre-commit==3.1.0",
   "pydefect==0.7.0",
+  "mp-pyrho==0.3.0",
+  "numpy==1.23.5"
 ]
 
 tests = ["pytest==7.2.2", "pytest-cov==4.0.0"]
 
 [tool.setuptools.dynamic]
 readme = { file = ["README.rst"] }
```

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_core.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from pymatgen.core.periodic_table import Element, Specie
+from pymatgen.io.vasp import Poscar
 
 from pymatgen.analysis.defects.core import (
     Adsorbate,
     DefectComplex,
     Interstitial,
     PeriodicSite,
     Substitution,
@@ -41,14 +42,20 @@
     assert sub.get_multiplicity() == 2
     sc = sub.get_supercell_structure()
     assert sc.formula == "Ga64 N63 O1"
     assert sub.name == "O_N"
     assert sub == sub
     assert sub.element_changes == {Element("N"): -1, Element("O"): 1}
 
+    # test supercell with locking
+    sc_locked = sub.get_supercell_structure(relax_radius=1.0)
+    poscar_locked = Poscar(sc_locked)
+    poscar_string = poscar_locked.get_string()
+    assert len(poscar_string.split("\n")) == 138
+
     # test for user defined charge
     dd = sub.as_dict()
     dd["user_charges"] = [-100, 102]
     sub_ = Substitution.from_dict(dd)
     assert sub_.get_charge_states() == [-100, 102]
 
     dd["user_charges"] = []  # empty list == None => use oxidation state info
```

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_corrections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import pytest
 
 from pymatgen.analysis.defects.corrections.freysoldt import (
     get_freysoldt_correction,
     plot_plnr_avg,
 )
-from pymatgen.analysis.defects.corrections.kumagai import (
-    get_efnv_correction,
-    get_structure_with_pot,
-)
 
 
 def test_freysoldt(data_Mg_Ga):
     """Older basic test for Freysoldt correction."""
     bulk_locpot = data_Mg_Ga["bulk_sc"]["locpot"]
     defect_locpot = data_Mg_Ga[f"q=0"]["locpot"]
 
@@ -72,21 +68,21 @@
         ).correction_energy
         for q in range(-1, 3)
     }
     for q in range(-1, 3):
         assert results[q] == pytest.approx(references[q], abs=1e-3)
 
 
-def test_kumagai(test_dir):
-    sb = get_structure_with_pot(test_dir / "Mg_Ga" / "bulk_sc")
-    sd0 = get_structure_with_pot(test_dir / "Mg_Ga" / "q=0")
-    sd1 = get_structure_with_pot(test_dir / "Mg_Ga" / "q=1")
-
-    res0 = get_efnv_correction(
-        0, sd0, sb, dielectric_tensor=[[1, 0, 0], [0, 1, 0], [0, 0, 1]]
-    )
-    assert res0.correction_energy == pytest.approx(0, abs=1e-4)
-
-    res1 = get_efnv_correction(
-        1, sd1, sb, dielectric_tensor=[[1, 0, 0], [0, 1, 0], [0, 0, 1]]
-    )
-    assert res1.correction_energy > 0
+# def test_kumagai(test_dir):
+#     sb = get_structure_with_pot(test_dir / "Mg_Ga" / "bulk_sc")
+#     sd0 = get_structure_with_pot(test_dir / "Mg_Ga" / "q=0")
+#     sd1 = get_structure_with_pot(test_dir / "Mg_Ga" / "q=1")
+
+#     res0 = get_efnv_correction(
+#         0, sd0, sb, dielectric_tensor=[[1, 0, 0], [0, 1, 0], [0, 0, 1]]
+#     )
+#     assert res0.correction_energy == pytest.approx(0, abs=1e-4)
+
+#     res1 = get_efnv_correction(
+#         1, sd1, sb, dielectric_tensor=[[1, 0, 0], [0, 1, 0], [0, 0, 1]]
+#     )
+#     assert res1.correction_energy > 0
```

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_finder.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_generators.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.4.5/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.5.4/tests/test_thermo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import os
 
 import numpy as np
 import pytest
 from matplotlib import pyplot as plt
 from pymatgen.analysis.phase_diagram import PhaseDiagram
-from pymatgen.core import PeriodicSite
+from pymatgen.core import Element, PeriodicSite
 
 from pymatgen.analysis.defects.core import Interstitial
 from pymatgen.analysis.defects.corrections.freysoldt import plot_plnr_avg
 from pymatgen.analysis.defects.thermo import (
     Composition,
     ComputedEntry,
     DefectEntry,
@@ -168,14 +168,17 @@
         chempots={e: 0 for e in def_ent_list[0].defect.element_changes},
         temperature=300,
     ) == pytest.approx(2 * 1.5875937551666035e-17)
 
     # dataframe conversion
     fed.as_dataframe()
 
+    # test that you can get the Ga-rich chempot
+    fed.get_chempots(Element("Ga"))
+
 
 def test_multi(data_Mg_Ga, defect_entries_Mg_Ga, stable_entries_Mg_Ga_N):
     bulk_vasprun = data_Mg_Ga["bulk_sc"]["vasprun"]
     bulk_dos = bulk_vasprun.complete_dos
     _, vbm = bulk_dos.get_cbm_vbm()
     bulk_entry = bulk_vasprun.get_computed_entry(inc_structure=False)
     defect_entries, plot_data = defect_entries_Mg_Ga
@@ -206,17 +209,16 @@
         bulk_entry=bulk_entry,
         defect_entries=def_ent_list,
         vbm=vbm,
         pd_entries=stable_entries_Mg_Ga_N,
         inc_inf_values=False,
     )
     mfed = MultiFormationEnergyDiagram(formation_energy_diagrams=[fed])
-    ef = mfed.solve_for_fermi_level(
-        chempots=mfed.chempot_limits[0], temperature=300, dos=bulk_dos
-    )
+    cpots = fed.get_chempots(Element("Ga"))
+    ef = mfed.solve_for_fermi_level(chempots=cpots, temperature=300, dos=bulk_dos)
     assert ef > 0
 
     # test the constructor with materials project phase diagram
     atomic_entries = list(
         filter(lambda x: len(x.composition.elements) == 1, stable_entries_Mg_Ga_N)
     )
     pd = PhaseDiagram(stable_entries_Mg_Ga_N)
```

