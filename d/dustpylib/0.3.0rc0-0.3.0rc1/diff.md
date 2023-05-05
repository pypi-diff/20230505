# Comparing `tmp/dustpylib-0.3.0rc0.tar.gz` & `tmp/dustpylib-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustpylib-0.3.0rc0.tar", last modified: Fri May  5 08:33:30 2023, max compression
+gzip compressed data, was "dustpylib-0.3.0rc1.tar", last modified: Fri May  5 09:02:17 2023, max compression
```

## Comparing `dustpylib-0.3.0rc0.tar` & `dustpylib-0.3.0rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.841045 dustpylib-0.3.0rc0/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.3.0rc0/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      241 2023-04-27 17:40:52.000000 dustpylib-0.3.0rc0/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-05 08:33:33.837045 dustpylib-0.3.0rc0/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1927 2023-05-05 08:25:55.000000 dustpylib-0.3.0rc0/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:32.706050 dustpylib-0.3.0rc0/docs/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.3.0rc0/docs/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.3.0rc0/docs/make.bat
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.3.0rc0/docs/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.153048 dustpylib-0.3.0rc0/docs/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2803 2023-04-27 14:49:18.000000 dustpylib-0.3.0rc0/docs/source/A_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      655 2023-04-29 20:42:06.000000 dustpylib-0.3.0rc0/docs/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.3.0rc0/docs/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.3.0rc0/docs/source/grid.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   185592 2023-05-05 08:28:58.000000 dustpylib-0.3.0rc0/docs/source/grid_refinement.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      876 2023-04-29 20:40:27.000000 dustpylib-0.3.0rc0/docs/source/index.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   125484 2023-05-05 08:32:29.000000 dustpylib-0.3.0rc0/docs/source/planetary_gaps.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25402 2023-05-05 08:29:25.000000 dustpylib-0.3.0rc0/docs/source/planetesimal_formation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.3.0rc0/docs/source/planetesimals.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1948590 2023-05-05 08:30:24.000000 dustpylib-0.3.0rc0/docs/source/radmc3d.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.3.0rc0/docs/source/radtrans.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.3.0rc0/docs/source/substructures.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.176050 dustpylib-0.3.0rc0/dustpylib/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      356 2023-05-05 08:33:23.000000 dustpylib-0.3.0rc0/dustpylib/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.357052 dustpylib-0.3.0rc0/dustpylib/grid/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-04-29 19:39:21.000000 dustpylib-0.3.0rc0/dustpylib/grid/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.442046 dustpylib-0.3.0rc0/dustpylib/grid/refinement/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      127 2023-04-29 19:39:03.000000 dustpylib-0.3.0rc0/dustpylib/grid/refinement/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1200 2023-04-29 20:25:00.000000 dustpylib-0.3.0rc0/dustpylib/grid/refinement/refinement.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.476045 dustpylib-0.3.0rc0/dustpylib/planetesimals/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      137 2023-04-29 13:09:13.000000 dustpylib-0.3.0rc0/dustpylib/planetesimals/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.548053 dustpylib-0.3.0rc0/dustpylib/planetesimals/formation/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      361 2023-04-29 16:40:19.000000 dustpylib-0.3.0rc0/dustpylib/planetesimals/formation/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3768 2023-04-30 08:03:28.000000 dustpylib-0.3.0rc0/dustpylib/planetesimals/formation/formation.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.583050 dustpylib-0.3.0rc0/dustpylib/radtrans/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      162 2023-04-28 16:08:04.000000 dustpylib-0.3.0rc0/dustpylib/radtrans/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.655046 dustpylib-0.3.0rc0/dustpylib/radtrans/radmc3d/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      417 2023-04-28 16:07:22.000000 dustpylib-0.3.0rc0/dustpylib/radtrans/radmc3d/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    32677 2023-05-05 08:18:25.000000 dustpylib-0.3.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.693048 dustpylib-0.3.0rc0/dustpylib/substructures/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      157 2023-04-29 17:32:32.000000 dustpylib-0.3.0rc0/dustpylib/substructures/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.794046 dustpylib-0.3.0rc0/dustpylib/substructures/gaps/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      171 2023-04-29 17:33:53.000000 dustpylib-0.3.0rc0/dustpylib/substructures/gaps/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1165 2023-04-29 18:20:06.000000 dustpylib-0.3.0rc0/dustpylib/substructures/gaps/gaps.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 08:33:33.328059 dustpylib-0.3.0rc0/dustpylib.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-05 08:33:31.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1104 2023-05-05 08:33:32.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-05 08:33:31.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-05-05 08:33:31.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       10 2023-05-05 08:33:31.000000 dustpylib-0.3.0rc0/dustpylib.egg-info/top_level.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-05 08:33:33.843047 dustpylib-0.3.0rc0/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2133 2023-04-27 17:33:26.000000 dustpylib-0.3.0rc0/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.553678 dustpylib-0.3.0rc1/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.3.0rc1/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      241 2023-04-27 17:40:52.000000 dustpylib-0.3.0rc1/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-05 09:02:20.548677 dustpylib-0.3.0rc1/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1927 2023-05-05 08:25:55.000000 dustpylib-0.3.0rc1/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:18.492151 dustpylib-0.3.0rc1/docs/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.3.0rc1/docs/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.3.0rc1/docs/make.bat
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.3.0rc1/docs/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:19.416676 dustpylib-0.3.0rc1/docs/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2803 2023-04-27 14:49:18.000000 dustpylib-0.3.0rc1/docs/source/A_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      655 2023-04-29 20:42:06.000000 dustpylib-0.3.0rc1/docs/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.3.0rc1/docs/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.3.0rc1/docs/source/grid.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   185592 2023-05-05 08:36:07.000000 dustpylib-0.3.0rc1/docs/source/grid_refinement.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      876 2023-04-29 20:40:27.000000 dustpylib-0.3.0rc1/docs/source/index.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   125484 2023-05-05 08:39:29.000000 dustpylib-0.3.0rc1/docs/source/planetary_gaps.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25402 2023-05-05 08:37:08.000000 dustpylib-0.3.0rc1/docs/source/planetesimal_formation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.3.0rc1/docs/source/planetesimals.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1946614 2023-05-05 09:01:11.000000 dustpylib-0.3.0rc1/docs/source/radmc3d.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.3.0rc1/docs/source/radtrans.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.3.0rc1/docs/source/substructures.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:19.467678 dustpylib-0.3.0rc1/dustpylib/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      356 2023-05-05 09:02:04.000000 dustpylib-0.3.0rc1/dustpylib/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:19.854689 dustpylib-0.3.0rc1/dustpylib/grid/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-04-29 19:39:21.000000 dustpylib-0.3.0rc1/dustpylib/grid/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:19.977687 dustpylib-0.3.0rc1/dustpylib/grid/refinement/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      127 2023-04-29 19:39:03.000000 dustpylib-0.3.0rc1/dustpylib/grid/refinement/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1200 2023-04-29 20:25:00.000000 dustpylib-0.3.0rc1/dustpylib/grid/refinement/refinement.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.047678 dustpylib-0.3.0rc1/dustpylib/planetesimals/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      137 2023-04-29 13:09:13.000000 dustpylib-0.3.0rc1/dustpylib/planetesimals/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.176683 dustpylib-0.3.0rc1/dustpylib/planetesimals/formation/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      361 2023-04-29 16:40:19.000000 dustpylib-0.3.0rc1/dustpylib/planetesimals/formation/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3768 2023-04-30 08:03:28.000000 dustpylib-0.3.0rc1/dustpylib/planetesimals/formation/formation.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.232680 dustpylib-0.3.0rc1/dustpylib/radtrans/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      162 2023-04-28 16:08:04.000000 dustpylib-0.3.0rc1/dustpylib/radtrans/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.343680 dustpylib-0.3.0rc1/dustpylib/radtrans/radmc3d/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      417 2023-04-28 16:07:22.000000 dustpylib-0.3.0rc1/dustpylib/radtrans/radmc3d/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    27457 2023-05-05 09:00:13.000000 dustpylib-0.3.0rc1/dustpylib/radtrans/radmc3d/radmc3d.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.405674 dustpylib-0.3.0rc1/dustpylib/substructures/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      157 2023-04-29 17:32:32.000000 dustpylib-0.3.0rc1/dustpylib/substructures/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:20.507680 dustpylib-0.3.0rc1/dustpylib/substructures/gaps/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      171 2023-04-29 17:33:53.000000 dustpylib-0.3.0rc1/dustpylib/substructures/gaps/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1165 2023-04-29 18:20:06.000000 dustpylib-0.3.0rc1/dustpylib/substructures/gaps/gaps.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-05 09:02:19.797678 dustpylib-0.3.0rc1/dustpylib.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-05 09:02:17.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1104 2023-05-05 09:02:17.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-05 09:02:17.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-05-05 09:02:17.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       10 2023-05-05 09:02:17.000000 dustpylib-0.3.0rc1/dustpylib.egg-info/top_level.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-05 09:02:20.556684 dustpylib-0.3.0rc1/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2133 2023-04-27 17:33:26.000000 dustpylib-0.3.0rc1/setup.py
```

### Comparing `dustpylib-0.3.0rc0/LICENSE` & `dustpylib-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/PKG-INFO` & `dustpylib-0.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.3.0rc0
+Version: 0.3.0rc1
 Home-page: https://github.com/stammler/dustpylib/
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
```

### Comparing `dustpylib-0.3.0rc0/README.md` & `dustpylib-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/Makefile` & `dustpylib-0.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/make.bat` & `dustpylib-0.3.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/A_contrib_bug_feature.ipynb` & `dustpylib-0.3.0rc1/docs/source/A_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/api.rst` & `dustpylib-0.3.0rc1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/conf.py` & `dustpylib-0.3.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/grid_refinement.ipynb` & `dustpylib-0.3.0rc1/docs/source/grid_refinement.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/index.rst` & `dustpylib-0.3.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/planetary_gaps.ipynb` & `dustpylib-0.3.0rc1/docs/source/planetary_gaps.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/planetesimal_formation.ipynb` & `dustpylib-0.3.0rc1/docs/source/planetesimal_formation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/docs/source/radmc3d.ipynb` & `dustpylib-0.3.0rc1/docs/source/radmc3d.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999922396055059%*

 * *Differences: {"'cells'": "{38: {'outputs': {0: {'text': {delete: [36, 35, 34, 33, 32, 31, 30, 29, 28, 27, 26, "*

 * *            "25, 24, 23, 22, 21, 19, 18, 17, 16, 15, 14, 13, 11]}}, 1: {'text': {insert: [(0, "*

 * *            "'/home/stammler/anaconda3/envs/j/lib/python3.11/site-packages/dsharp_opac/dsharp_opac.py:2778: "*

 * *            "RuntimeWarning: invalid value encountered in scalar divide\\n')], delete: [0]}}}}}"}*

```diff
@@ -466,40 +466,16 @@
                         "Writing radmc3d/dust_density.inp.....done.\n",
                         "Writing radmc3d/dust_temperature.dat.....done.\n",
                         "Writing radmc3d/dustopac.inp.....done.\n",
                         "\n",
                         "Computing opacities...\n",
                         "Using dsharp_opac. Please cite Birnstiel et al. (2018).\n",
                         "Using DSHARP mix. Please cite Birnstiel et al. (2018).\n",
-                        "material: Water Ice: Warren & Brandt (2008), downloading IOP_2008_ASCIItable.dat: ... Done!\n",
                         "Please cite Warren & Brandt (2008) when using these optical constants\n",
-                        "material: original astro. silicates, downloading eps_Sil: ... Done!\n",
-                        "material: Draine 2003 astro. silicates, downloading callindex.out_silD03: ... Done!\n",
-                        "material: Weingartner & Draine 2001 astr. silicates, downloading eps_suvSil: ... Done!\n",
-                        "material: Draine 2003 carbon, parallel, A=0.01 micron, downloading callindex.out_CpaD03_0.01: ... Done!\n",
-                        "material: Draine 2003 carbon, parallel, A=0.1 micron, downloading callindex.out_CpaD03_0.10: ... Done!\n",
-                        "material: Draine 2003 carbon, perpendicular, A=0.01 micron, downloading callindex.out_CpeD03_0.01: ... Done!\n",
-                        "material: Draine 2003 carbon, perpendicular, A=0.1 micron, downloading callindex.out_CpeD03_0.10: ... Done!\n",
                         "Please cite Draine 2003 when using these optical constants\n",
-                        "material: Olivine, downloading olivine.lnk: ... Done!\n",
-                        "material: Orthopyroxene, downloading orthopyr.lnk: ... Done!\n",
-                        "material: Iron, downloading iron.lnk: ... Done!\n",
-                        "material: Troilite, downloading troilite.lnk: ... Done!\n",
-                        "material: Organics, downloading organics.lnk: ... Done!\n",
-                        "material: Water Ice, downloading waterice.lnk: ... Done!\n",
-                        "material: Olivine (normal), downloading olmg70k.lnk: ... Done!\n",
-                        "material: Olivine (low), downloading olivinenewk.lnk: ... Done!\n",
-                        "material: Olivine (high), downloading olmg60k.lnk: ... Done!\n",
-                        "material: Orthopyroxene (normal), downloading pyrmg70k.lnk: ... Done!\n",
-                        "material: Orthopyroxene (low), downloading pyrmg100k.lnk: ... Done!\n",
-                        "material: Orthopyroxene (high), downloading pyrmg60k.lnk: ... Done!\n",
-                        "material: Iron, downloading ironk.lnk: ... Done!\n",
-                        "material: Troilite, downloading troilitek.lnk: ... Done!\n",
-                        "material: Organics, downloading organicsk.lnk: ... Done!\n",
-                        "material: Water Ice, downloading watericek.lnk: ... Done!\n",
                         "Reading opacities from troilitek\n",
                         "Please cite Henning & Stognienko (1996) when using these optical constants\n",
                         "Reading opacities from organicsk\n",
                         "Please cite Henning & Stognienko (1996) when using these optical constants\n",
                         "| material                            | volume fractions | mass fractions |\n",
                         "|-------------------------------------|------------------|----------------|\n",
                         "| Water Ice (Warren & Brandt 2008)    | 0.3642           | 0.2            |\n",
@@ -509,15 +485,15 @@
                         "Mie ... Done!\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/home/stammler/anaconda3/envs/j/lib/python3.11/site-packages/dustpylib/radtrans/radmc3d/radmc3d.py:752: RuntimeWarning: invalid value encountered in scalar divide\n",
+                        "/home/stammler/anaconda3/envs/j/lib/python3.11/site-packages/dsharp_opac/dsharp_opac.py:2778: RuntimeWarning: invalid value encountered in scalar divide\n",
                         "  g[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0] * mu, x=mu) / k_sca[grain, i]\n"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
```

### Comparing `dustpylib-0.3.0rc0/dustpylib/grid/refinement/refinement.py` & `dustpylib-0.3.0rc1/dustpylib/grid/refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/dustpylib/planetesimals/formation/formation.py` & `dustpylib-0.3.0rc1/dustpylib/planetesimals/formation/formation.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py` & `dustpylib-0.3.0rc1/dustpylib/radtrans/radmc3d/radmc3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -576,15 +576,15 @@
             mix, rho_s = do.get_dsharp_mix()
         elif opacity == "ricci2010":
             print("Using Ricci mix. Please cite Ricci et al. (2010).")
             mix, rho_s = do.get_ricci_mix(lmax=self.lam_grid[-1], extrapol=True)
         else:
             raise RuntimeError("Unknown opacity '{}'".format(opacity))
         opac_dict = do.get_opacities(self.ac_grid, self.lam_grid, rho_s, mix, extrapolate_large_grains=True, n_angle=int((Nangle-1)/2+1))
-        zscat, _, k_sca, g = self._chop_forward_scattering(opac_dict)
+        zscat, _, k_sca, g = do.chop_forward_scattering(opac_dict)
         opac_dict["k_sca"] = k_sca
         opac_dict["g"] = g
         opac_dict["zscat"] = zscat
         print()
 
         for ia in range(Nspec):
             filename = "dustkapscatmat_{}.inp".format("{:d}".format(ia).zfill(mag))
@@ -618,144 +618,14 @@
                                 zscat[ia, ilam, iang, 3],
                                 zscat[ia, ilam, iang, 4],
                                 zscat[ia, ilam, iang, 5],
                             )
                         )
             print("done.")
 
-    def _calculate_mueller_matrix(self, lam, m, S1, S2, theta=None, k_sca=None):
-        import warnings
-        """
-        Calculate the Mueller matrix elements Zij given the scattering amplitudes
-        S1 and S2.
-        Arguments:
-        ----------
-        lam : array
-            wavelength array of length nlam
-        m : array
-            particle mass array of length nm
-        S1, S2 : arrays
-            scattering amplitudes of shape (nm, nlam, nangles), where
-            nangles is the length of the angle array for which the amplitudes
-            were calculated.
-        Keywords:
-        ---------
-        If theta and k_sca are given, a check is done, if the integral over the
-        scattering matrix elements is identical to the scattering opacities.
-        theta : array
-            array of angles
-        k_sca : array
-            array of scattering opacities
-        Notes:
-        ------
-        The conversion factor `factor` is calculated as defined in Kees Dullemonds
-        code `makeopac.py`:
-        > Compute conversion factor from the Sxx matrix elements
-        > from the Bohren & Huffman code to the Zxx matrix elements we
-        > use (such that 2*pi*int_{-1}^{+1}Z11(mu)dmu=kappa_scat).
-        > This includes the factor k^2 (wavenumber squared) to get
-        > the actual cross section in units of cm^2 / ster, and there
-        > is the mass of the grain to get the cross section per gram.
-        """
-        factor = (lam[None, :] / (2 * np.pi))**2 / m[:, None]
-        #
-        # Compute the scattering Mueller matrix elements at each angle
-        #
-        S11 = 0.5 * (np.abs(S2)**2 + np.abs(S1)**2)
-        S12 = 0.5 * (np.abs(S2)**2 - np.abs(S1)**2)
-        S33 = np.real(S2[:] * np.conj(S1[:]))
-        S34 = np.imag(S2[:] * np.conj(S1[:]))
-
-        zscat = np.zeros([len(m), len(lam), S1.shape[-1], 6])
-
-        zscat[..., 0] = S11 * factor[:, :, None]
-        zscat[..., 1] = S12 * factor[:, :, None]
-        zscat[..., 2] = S11 * factor[:, :, None]
-        zscat[..., 3] = S33 * factor[:, :, None]
-        zscat[..., 4] = S34 * factor[:, :, None]
-        zscat[..., 5] = S33 * factor[:, :, None]
-
-        #
-        # If possible, do a check if the integral over zscat is consistent
-        # with kscat
-        #
-        kscat_from_z11 = np.zeros_like(k_sca)
-        error_tolerance = 0.01
-        error_max = 0.0
-        if theta is not None and k_sca is not None:
-            n_theta = len(theta)
-            mu = np.cos(theta * np.pi / 180.)
-            dmu = np.diff(mu)
-            for ia in range(len(m)):
-                for ilam in range(len(lam)):
-                    zav = 0.5 * (zscat[ia, ilam, 1:n_theta, 0] + zscat[ia, ilam, 0:n_theta - 1, 0])
-                    dum = -0.5 * zav * dmu
-                    integral = dum.sum() * 4 * np.pi
-                    kscat_from_z11[ia, ilam] = integral
-                    err = abs(integral / k_sca[ia, ilam] - 1.0)
-                    error_max = max(err, error_max)
-
-        if error_max > error_tolerance:
-            warnings.warn('Maximum error of {:.2g}%: above error tolerance'.format(error_max * 100))
-
-        return {'zscat': zscat, 'kscat_from_z11': kscat_from_z11, 'error_max': error_max}
-
-    def _chop_forward_scattering(self, opac_dict, chopforward=5):
-        """Chop the forward scattering.
-        This part chops the very-forward scattering part of the phase function.
-        This very-forward scattering part is basically the same as no scattering,
-        but is treated by the code as a scattering event. By cutting this part out
-        of the phase function, we avoid those non-scattering scattering events.
-        This needs to recalculate the scattering opacity kappa_sca and asymmetry
-        factor g.
-        Parameters
-        ----------
-        opac_dict : dict
-            opacity dictionary as produced by dsharp_opac
-        chopforward : float
-            up to which angle to we truncate the forward scattering
-        """
-
-        k_sca = opac_dict['k_sca']
-        theta = opac_dict['theta']
-        g = opac_dict['g']
-        rho_s = opac_dict['rho_s']
-        lam = opac_dict['lam']
-        a = opac_dict['a']
-        m = 4 * np.pi / 3 * rho_s * a ** 3
-
-        n_a = len(a)
-        n_lam = len(lam)
-
-        if 'zscat' in opac_dict:
-            zscat = opac_dict['zscat']
-        else:
-            S1 = opac_dict['S1']
-            S2 = opac_dict['S2']
-            zscat = self._calculate_mueller_matrix(lam, m, S1, S2)['zscat']
-
-        zscat_nochop = zscat.copy()
-
-        mu = np.cos(theta * np.pi / 180.)
-
-        for grain in range(n_a):
-            for i in range(n_lam):
-                if chopforward > 0:
-                    iang = np.where(theta < chopforward)
-                    if theta[0] == 0.0:
-                        iiang = np.max(iang) + 1
-                    else:
-                        iiang = np.min(iang) - 1
-                    zscat[grain, i, iang, :] = zscat[grain, i, iiang, :]
-
-                    k_sca[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0], x=mu)
-                    g[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0] * mu, x=mu) / k_sca[grain, i]
-
-        return zscat, zscat_nochop, k_sca, g
-
 
 def read_model(datadir=""):
     """
     This functions reads the ``RADMC-3D`` model files and returns a namespace with the data.
     It should only be used for models created by ``dustpylib``. For more complex models
     use ``Radmc3dPy``.
```

### Comparing `dustpylib-0.3.0rc0/dustpylib/substructures/gaps/gaps.py` & `dustpylib-0.3.0rc1/dustpylib/substructures/gaps/gaps.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/dustpylib.egg-info/PKG-INFO` & `dustpylib-0.3.0rc1/dustpylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.3.0rc0
+Version: 0.3.0rc1
 Home-page: https://github.com/stammler/dustpylib/
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
```

### Comparing `dustpylib-0.3.0rc0/dustpylib.egg-info/SOURCES.txt` & `dustpylib-0.3.0rc1/dustpylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dustpylib-0.3.0rc0/setup.py` & `dustpylib-0.3.0rc1/setup.py`

 * *Files identical despite different names*

