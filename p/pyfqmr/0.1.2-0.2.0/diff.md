# Comparing `tmp/pyfqmr-0.1.2-cp39-cp39-win_amd64.whl.zip` & `tmp/pyfqmr-0.2.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 97929 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   183296 b- defN 22-May-24 12:26 pyfqmr/Simplify.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    31993 b- defN 22-May-24 12:15 pyfqmr/Simplify.h
--rw-rw-rw-  2.0 fat     8138 b- defN 22-May-24 12:15 pyfqmr/Simplify.pyx
--rw-rw-rw-  2.0 fat       23 b- defN 22-May-24 12:15 pyfqmr/__init__.py
--rw-rw-rw-  2.0 fat     1086 b- defN 22-May-24 12:26 pyfqmr-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3810 b- defN 22-May-24 12:26 pyfqmr-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-May-24 12:26 pyfqmr-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 22-May-24 12:26 pyfqmr-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      698 b- defN 22-May-24 12:26 pyfqmr-0.1.2.dist-info/RECORD
-9 files, 229151 bytes uncompressed, 96739 bytes compressed:  57.8%
+Zip file size: 99718 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   187904 b- defN 23-May-05 01:04 pyfqmr/Simplify.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    31993 b- defN 23-May-05 00:54 pyfqmr/Simplify.h
+-rw-rw-rw-  2.0 fat     8138 b- defN 23-May-05 00:54 pyfqmr/Simplify.pyx
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-05 00:54 pyfqmr/__init__.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-May-05 01:04 pyfqmr-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3939 b- defN 23-May-05 01:04 pyfqmr-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-05 01:04 pyfqmr-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-05 01:04 pyfqmr-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      698 b- defN 23-May-05 01:04 pyfqmr-0.2.0.dist-info/RECORD
+9 files, 233888 bytes uncompressed, 98528 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pyfqmr/Simplify.pyx
 Comment: 
 
 Filename: pyfqmr/__init__.py
 Comment: 
 
-Filename: pyfqmr-0.1.2.dist-info/LICENSE
+Filename: pyfqmr-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyfqmr-0.1.2.dist-info/METADATA
+Filename: pyfqmr-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pyfqmr-0.1.2.dist-info/WHEEL
+Filename: pyfqmr-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyfqmr-0.1.2.dist-info/top_level.txt
+Filename: pyfqmr-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfqmr-0.1.2.dist-info/RECORD
+Filename: pyfqmr-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyfqmr-0.1.2.dist-info/LICENSE` & `pyfqmr-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfqmr-0.1.2.dist-info/METADATA` & `pyfqmr-0.2.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,108 @@
-Metadata-Version: 2.1
-Name: pyfqmr
-Version: 0.1.2
-Summary: cython wrapper around C++ library for fast triangular mesh reduction
-Home-page: https://github.com/Kramer84/pyfqmr-Fast-quadric-Mesh-Reduction
-Author: kramer84
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-License-File: LICENSE
-
-pyfqmr : Python Fast Quadric Mesh Reduction
-===========================================
-
-Cython wrapper around `sp4acerat's quadrics mesh reduction
-algorithm <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification>`__.
-
-Requirements:
-~~~~~~~~~~~~~
-
--  *Numpy*
--  *Cython* (only for compilation, but not needed if installed from PyPI)
-
-Installation :
-~~~~~~~~~~~~~~
-pyfqmr can be installed via  `pip <https://pypi.org/project/pyfqmr/0.1.1/>`_ :
-
-
-.. code:: bash
-
-    pip install pyfqmr
-
-
-Compilation :
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Run:
-
-.. code:: bash
-
-    python setup.py install
-
-Usage:
-~~~~~~
-
-.. code:: python
-
-    >>> #We assume you have a numpy based mesh processing software
-    >>> #Where you can get the vertices and faces of the mesh as numpy arrays.
-    >>> #For example Trimesh or meshio
-    >>> import pyfqmr
-    >>> import trimesh as tr
-    >>> bunny = tr.load_mesh('example/Stanford_Bunny_sample.stl')
-    >>> #Simplify object
-    >>> mesh_simplifier = pyfqmr.Simplify()
-    >>> mesh_simplifier.setMesh(bunny.vertices, bunny.faces)
-    >>> mesh_simplifier.simplify_mesh(target_count = 1000, aggressiveness=7, preserve_border=True, verbose=10)
-    iteration 0 - triangles 112402 threshold 2.187e-06
-    iteration 5 - triangles 62674 threshold 0.00209715
-    iteration 10 - triangles 21518 threshold 0.0627485
-    iteration 15 - triangles 9086 threshold 0.61222
-    iteration 20 - triangles 4692 threshold 3.40483
-    iteration 25 - triangles 2796 threshold 13.4929
-    iteration 30 - triangles 1812 threshold 42.6184
-    iteration 35 - triangles 1262 threshold 114.416
-    simplified mesh in 0.2518 seconds 
-    >>> vertices, faces, normals = mesh_simplifier.getMesh()
-
-Controlling the reduction algorithm
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Parameters of the '''simplify\_mesh''' method that can be tuned.
-
--  **target\_count**
-    Target number of triangles.
--  **update\_rate**
-    Number of iterations between each update.
--  **max\_iterations**
-    Maximal number of iterations
--  **aggressiveness**
-    Parameter controlling the growth rate of the threshold at each iteration when lossless is False.
--  **preserve\_border**
-    Flag for preserving the vertices situated on open borders. Applies the method descriped in `this issue <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification/issues/14>`__.
--  **alpha**
-    Parameter for controlling the threshold growth. Exact implication described below.
--  **K**
-    Parameter for controlling the thresold growth. Exact implication described below.
--  **lossless**
-    Flag for using the lossless simplification method. Sets the update rate to 1 .
--  **threshold\_lossless**
-    Maximal error after which a vertex is not deleted, only when the lossless flag is set to True.
--  **verbose**
-    Controls verbosity
-
-Implications of the parameters of the threshold growth rate
-'''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-This is only true when not in lossless mode. - **threshold = alpha \* (iteration + K)\*\*agressiveness**
-
-More information is to be found on Sp4cerat's repo : `Fast-Quadric-Mesh-Simplification <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification>`__
-
-Huge thanks to Sp4cerat for making his code available!
+Metadata-Version: 2.1
+Name: pyfqmr
+Version: 0.2.0
+Summary: cython wrapper around C++ library for fast triangular mesh reduction
+Home-page: https://github.com/Kramer84/pyfqmr-Fast-quadric-Mesh-Reduction
+Author: kramer84
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+License-File: LICENSE
+
+pyfqmr : Python Fast Quadric Mesh Reduction
+===========================================
+
+Cython wrapper around `sp4acerat's quadrics mesh reduction
+algorithm <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification>`__.
+
+Requirements:
+~~~~~~~~~~~~~
+
+-  *Numpy*
+-  *Cython* (only for compilation, but not needed if installed from PyPI)
+
+Installation :
+~~~~~~~~~~~~~~
+pyfqmr can be installed via  `pip <https://pypi.org/project/pyfqmr/0.1.1/>`_ :
+
+
+.. code:: bash
+
+    pip install pyfqmr
+
+
+Compilation :
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Run:
+
+.. code:: bash
+
+    python setup.py install
+
+Usage:
+~~~~~~
+
+.. code:: python
+
+    >>> #We assume you have a numpy based mesh processing software
+    >>> #Where you can get the vertices and faces of the mesh as numpy arrays.
+    >>> #For example Trimesh or meshio
+    >>> import pyfqmr
+    >>> import trimesh as tr
+    >>> bunny = tr.load_mesh('example/Stanford_Bunny_sample.stl')
+    >>> #Simplify object
+    >>> mesh_simplifier = pyfqmr.Simplify()
+    >>> mesh_simplifier.setMesh(bunny.vertices, bunny.faces)
+    >>> mesh_simplifier.simplify_mesh(target_count = 1000, aggressiveness=7, preserve_border=True, verbose=10)
+    iteration 0 - triangles 112402 threshold 2.187e-06
+    iteration 5 - triangles 62674 threshold 0.00209715
+    iteration 10 - triangles 21518 threshold 0.0627485
+    iteration 15 - triangles 9086 threshold 0.61222
+    iteration 20 - triangles 4692 threshold 3.40483
+    iteration 25 - triangles 2796 threshold 13.4929
+    iteration 30 - triangles 1812 threshold 42.6184
+    iteration 35 - triangles 1262 threshold 114.416
+    simplified mesh in 0.2518 seconds 
+    >>> vertices, faces, normals = mesh_simplifier.getMesh()
+
+Controlling the reduction algorithm
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Parameters of the '''simplify\_mesh''' method that can be tuned.
+
+-  **target\_count**
+    Target number of triangles.
+-  **update\_rate**
+    Number of iterations between each update.
+-  **max\_iterations**
+    Maximal number of iterations
+-  **aggressiveness**
+    Parameter controlling the growth rate of the threshold at each iteration when lossless is False.
+-  **preserve\_border**
+    Flag for preserving the vertices situated on open borders. Applies the method described in `this issue <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification/issues/14>`__.
+-  **alpha**
+    Parameter for controlling the threshold growth. Exact implication described below.
+-  **K**
+    Parameter for controlling the threshold growth. Exact implication described below.
+-  **lossless**
+    Flag for using the lossless simplification method. Sets the update rate to 1 .
+-  **threshold\_lossless**
+    Maximal error after which a vertex is not deleted, only when the lossless flag is set to True.
+-  **verbose**
+    Controls verbosity
+
+Implications of the parameters of the threshold growth rate (when not in lossless mode) :
+'''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
+$$threshold = alpha \* (iteration + K)^{agressiveness}$$
+
+\
+
+More information is to be found on Sp4cerat's repository : `Fast-Quadric-Mesh-Simplification <https://github.com/sp4cerat/Fast-Quadric-Mesh-Simplification>`__
+
+Huge thanks to Sp4cerat for making his code available!
```

## Comparing `pyfqmr-0.1.2.dist-info/RECORD` & `pyfqmr-0.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyfqmr/Simplify.cp39-win_amd64.pyd,sha256=rG8IhA0QZsGBQVtegWNn08afA4su0aY0buOnBkYhHBA,183296
+pyfqmr/Simplify.cp39-win_amd64.pyd,sha256=YAkChMy6tZustgDcD_3MULaDAFak55H0WE4GtaR2t74,187904
 pyfqmr/Simplify.h,sha256=jWxUu2LdINx2NY9OKANPYqfCferJHu3-h1J9ryGuD2o,31993
 pyfqmr/Simplify.pyx,sha256=etOGZNAyNvaSgkJXqANPp8SYuVb6jgZQa_N7InmDRu4,8138
 pyfqmr/__init__.py,sha256=m5XhES3bG6gA-udX4w7rXcAuxsNapkPwhJxNIOSN-Mo,23
-pyfqmr-0.1.2.dist-info/LICENSE,sha256=faEX425hyMnZ5zIqUNCLD5_yPxIsFU-4qzWxGqV1A5Y,1086
-pyfqmr-0.1.2.dist-info/METADATA,sha256=8LwqKjLYlL32xHn3i-Ud1uUMW-dAptXtQgLsIi321vo,3810
-pyfqmr-0.1.2.dist-info/WHEEL,sha256=fVcVlLzi8CGi_Ul8vjMdn8gER25dn5GBg9E6k9z41-Y,100
-pyfqmr-0.1.2.dist-info/top_level.txt,sha256=3uGhpvmIA3O4AbEmef4YmNLpU7aC6h6gePtTcBjuw_c,7
-pyfqmr-0.1.2.dist-info/RECORD,,
+pyfqmr-0.2.0.dist-info/LICENSE,sha256=faEX425hyMnZ5zIqUNCLD5_yPxIsFU-4qzWxGqV1A5Y,1086
+pyfqmr-0.2.0.dist-info/METADATA,sha256=AS7qmY_OUcZIU38MpNb0OJ9aOg979NzYsHpiI7G4LSA,3939
+pyfqmr-0.2.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+pyfqmr-0.2.0.dist-info/top_level.txt,sha256=3uGhpvmIA3O4AbEmef4YmNLpU7aC6h6gePtTcBjuw_c,7
+pyfqmr-0.2.0.dist-info/RECORD,,
```

