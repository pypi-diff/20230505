# Comparing `tmp/pyGrained-1.0.1.tar.gz` & `tmp/pyGrained-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGrained-1.0.1.tar", last modified: Fri May  5 14:49:28 2023, max compression
+gzip compressed data, was "pyGrained-1.0.2.tar", last modified: Fri May  5 15:37:19 2023, max compression
```

## Comparing `pyGrained-1.0.1.tar` & `pyGrained-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.962318 pyGrained-1.0.1/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-03 17:19:11.000000 pyGrained-1.0.1/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       71 2023-05-03 14:59:01.000000 pyGrained-1.0.1/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 14:49:28.962318 pyGrained-1.0.1/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2051 2023-01-03 18:53:54.000000 pyGrained-1.0.1/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.958318 pyGrained-1.0.1/pyGrained/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    27509 2023-05-05 13:55:29.000000 pyGrained-1.0.1/pyGrained/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.962318 pyGrained-1.0.1/pyGrained/data/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     3579 2023-03-24 16:55:13.000000 pyGrained-1.0.1/pyGrained/data/BetancourtThirumalaiEnergyParm.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)    54297 2023-03-24 17:03:10.000000 pyGrained-1.0.1/pyGrained/data/KaranicolasBrooksDiheParm.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)     4303 2023-03-24 17:05:26.000000 pyGrained-1.0.1/pyGrained/data/MiyazawaJerniga1999EnergyParm.json
--rw-------   0 pablo     (1000) pablo     (1000)     3573 2023-03-24 17:06:13.000000 pyGrained-1.0.1/pyGrained/data/MiyazawaJernigaEnergyParm.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      231 2023-03-17 18:40:11.000000 pyGrained-1.0.1/pyGrained/data/aminoacidCharges.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      306 2023-03-17 18:40:18.000000 pyGrained-1.0.1/pyGrained/data/aminoacidMasses.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      218 2023-03-17 18:40:26.000000 pyGrained-1.0.1/pyGrained/data/aminoacidRadii.json
--rw-------   0 pablo     (1000) pablo     (1000)      277 2023-03-24 16:52:18.000000 pyGrained-1.0.1/pyGrained/data/aminoacidRndCoilSASA.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)      280 2023-03-24 16:51:17.000000 pyGrained-1.0.1/pyGrained/data/aminoacids.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)       75 2023-03-24 16:52:57.000000 pyGrained-1.0.1/pyGrained/data/atomMasses.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)       46 2023-03-24 16:48:30.000000 pyGrained-1.0.1/pyGrained/data/atomRadiiSobolev.json
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.962318 pyGrained-1.0.1/pyGrained/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    19150 2023-05-05 13:44:28.000000 pyGrained-1.0.1/pyGrained/models/AlphaCarbon.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    20140 2023-05-05 13:44:28.000000 pyGrained-1.0.1/pyGrained/models/SBCG.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-05 09:33:49.000000 pyGrained-1.0.1/pyGrained/models/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.962318 pyGrained-1.0.1/pyGrained/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      187 2023-03-18 18:27:20.000000 pyGrained-1.0.1/pyGrained/utils/SASA.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-18 16:17:48.000000 pyGrained-1.0.1/pyGrained/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3625 2023-03-23 17:54:04.000000 pyGrained-1.0.1/pyGrained/utils/atomList.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4645 2023-03-24 16:47:01.000000 pyGrained-1.0.1/pyGrained/utils/bonds.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3778 2023-04-25 10:35:41.000000 pyGrained-1.0.1/pyGrained/utils/coarseGrained.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.962318 pyGrained-1.0.1/pyGrained/utils/computeK/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-17 18:13:15.000000 pyGrained-1.0.1/pyGrained/utils/computeK/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2022-12-23 23:49:41.000000 pyGrained-1.0.1/pyGrained/utils/computeK/computeK.cpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      905 2023-03-24 18:28:04.000000 pyGrained-1.0.1/pyGrained/utils/geometric.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11144 2023-05-05 12:56:26.000000 pyGrained-1.0.1/pyGrained/utils/nativeContacts.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-03-24 10:35:09.000000 pyGrained-1.0.1/pyGrained/utils/output.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      387 2023-03-18 17:23:11.000000 pyGrained-1.0.1/pyGrained/utils/sequence.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1284 2023-05-05 14:42:46.000000 pyGrained-1.0.1/pyGrained/utils/trajectory.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 14:49:28.958318 pyGrained-1.0.1/pyGrained.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 14:49:28.000000 pyGrained-1.0.1/pyGrained.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1126 2023-05-05 14:49:28.000000 pyGrained-1.0.1/pyGrained.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-05 14:49:28.000000 pyGrained-1.0.1/pyGrained.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       25 2023-05-05 14:49:28.000000 pyGrained-1.0.1/pyGrained.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       10 2023-05-05 14:49:28.000000 pyGrained-1.0.1/pyGrained.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-05 14:47:43.000000 pyGrained-1.0.1/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 14:49:28.962318 pyGrained-1.0.1/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-05-03 15:03:41.000000 pyGrained-1.0.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-03 17:19:11.000000 pyGrained-1.0.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       71 2023-05-03 14:59:01.000000 pyGrained-1.0.2/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 15:37:19.919853 pyGrained-1.0.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2051 2023-01-03 18:53:54.000000 pyGrained-1.0.2/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    27509 2023-05-05 13:55:29.000000 pyGrained-1.0.2/pyGrained/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/data/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     3579 2023-03-24 16:55:13.000000 pyGrained-1.0.2/pyGrained/data/BetancourtThirumalaiEnergyParm.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)    54297 2023-03-24 17:03:10.000000 pyGrained-1.0.2/pyGrained/data/KaranicolasBrooksDiheParm.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     4303 2023-03-24 17:05:26.000000 pyGrained-1.0.2/pyGrained/data/MiyazawaJerniga1999EnergyParm.json
+-rw-------   0 pablo     (1000) pablo     (1000)     3573 2023-03-24 17:06:13.000000 pyGrained-1.0.2/pyGrained/data/MiyazawaJernigaEnergyParm.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      231 2023-03-17 18:40:11.000000 pyGrained-1.0.2/pyGrained/data/aminoacidCharges.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      306 2023-03-17 18:40:18.000000 pyGrained-1.0.2/pyGrained/data/aminoacidMasses.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      218 2023-03-17 18:40:26.000000 pyGrained-1.0.2/pyGrained/data/aminoacidRadii.json
+-rw-------   0 pablo     (1000) pablo     (1000)      277 2023-03-24 16:52:18.000000 pyGrained-1.0.2/pyGrained/data/aminoacidRndCoilSASA.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      280 2023-03-24 16:51:17.000000 pyGrained-1.0.2/pyGrained/data/aminoacids.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       75 2023-03-24 16:52:57.000000 pyGrained-1.0.2/pyGrained/data/atomMasses.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       46 2023-03-24 16:48:30.000000 pyGrained-1.0.2/pyGrained/data/atomRadiiSobolev.json
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    19150 2023-05-05 13:44:28.000000 pyGrained-1.0.2/pyGrained/models/AlphaCarbon.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    20193 2023-05-05 15:26:26.000000 pyGrained-1.0.2/pyGrained/models/SBCG.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-05 09:33:49.000000 pyGrained-1.0.2/pyGrained/models/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/pyGrained/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      187 2023-03-18 18:27:20.000000 pyGrained-1.0.2/pyGrained/utils/SASA.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-18 16:17:48.000000 pyGrained-1.0.2/pyGrained/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3625 2023-03-23 17:54:04.000000 pyGrained-1.0.2/pyGrained/utils/atomList.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4645 2023-03-24 16:47:01.000000 pyGrained-1.0.2/pyGrained/utils/bonds.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3778 2023-04-25 10:35:41.000000 pyGrained-1.0.2/pyGrained/utils/coarseGrained.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/pyGrained/utils/computeK/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-17 18:13:15.000000 pyGrained-1.0.2/pyGrained/utils/computeK/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2022-12-23 23:49:41.000000 pyGrained-1.0.2/pyGrained/utils/computeK/computeK.cpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      905 2023-03-24 18:28:04.000000 pyGrained-1.0.2/pyGrained/utils/geometric.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11144 2023-05-05 12:56:26.000000 pyGrained-1.0.2/pyGrained/utils/nativeContacts.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-03-24 10:35:09.000000 pyGrained-1.0.2/pyGrained/utils/output.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      387 2023-03-18 17:23:11.000000 pyGrained-1.0.2/pyGrained/utils/sequence.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1284 2023-05-05 14:42:46.000000 pyGrained-1.0.2/pyGrained/utils/trajectory.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1126 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       25 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       10 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-05 15:36:24.000000 pyGrained-1.0.2/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 15:37:19.919853 pyGrained-1.0.2/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-05-03 15:03:41.000000 pyGrained-1.0.2/setup.py
```

### Comparing `pyGrained-1.0.1/LICENSE` & `pyGrained-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/PKG-INFO` & `pyGrained-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGrained
-Version: 1.0.1
+Version: 1.0.2
 Summary: Coarse grained library for Python
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyGrained-1.0.1/README.md` & `pyGrained-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/__init__.py` & `pyGrained-1.0.2/pyGrained/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/data/BetancourtThirumalaiEnergyParm.json` & `pyGrained-1.0.2/pyGrained/data/BetancourtThirumalaiEnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/data/KaranicolasBrooksDiheParm.json` & `pyGrained-1.0.2/pyGrained/data/KaranicolasBrooksDiheParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/data/MiyazawaJerniga1999EnergyParm.json` & `pyGrained-1.0.2/pyGrained/data/MiyazawaJerniga1999EnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/data/MiyazawaJernigaEnergyParm.json` & `pyGrained-1.0.2/pyGrained/data/MiyazawaJernigaEnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/models/AlphaCarbon.py` & `pyGrained-1.0.2/pyGrained/models/AlphaCarbon.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/models/SBCG.py` & `pyGrained-1.0.2/pyGrained/models/SBCG.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,16 @@
 
             differentChain = (ch1Index != ch2Index or mdl1Index != mdl2Index)
 
             if (ch1Index in chainsCg) and (ch2Index in chainsCg):
                 if abs(res1Index-res2Index) > n or differentChain:
                     bead1Index = atom2bead[atomsCA[nc[0]].get_serial_number()]
                     bead2Index = atom2bead[atomsCA[nc[1]].get_serial_number()]
-                    ncBeadsTmp.append((bead1Index,bead2Index))
+                    if bead1Index != bead2Index:
+                        ncBeadsTmp.append((bead1Index,bead2Index))
             else:
                 self.logger.debug(f"While generating native contacts, the chain {ch1Index} or the chain {ch2Index} has been found in the all atom model but not in CG")
 
 
         ncBeads = {nc:0 for nc in set(ncBeadsTmp)}
 
         for nc in ncBeadsTmp:
```

### Comparing `pyGrained-1.0.1/pyGrained/utils/atomList.py` & `pyGrained-1.0.2/pyGrained/utils/atomList.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/bonds.py` & `pyGrained-1.0.2/pyGrained/utils/bonds.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/coarseGrained.py` & `pyGrained-1.0.2/pyGrained/utils/coarseGrained.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/computeK/computeK.cpp` & `pyGrained-1.0.2/pyGrained/utils/computeK/computeK.cpp`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/geometric.py` & `pyGrained-1.0.2/pyGrained/utils/geometric.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/nativeContacts.py` & `pyGrained-1.0.2/pyGrained/utils/nativeContacts.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/output.py` & `pyGrained-1.0.2/pyGrained/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained/utils/trajectory.py` & `pyGrained-1.0.2/pyGrained/utils/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyGrained.egg-info/PKG-INFO` & `pyGrained-1.0.2/pyGrained.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGrained
-Version: 1.0.1
+Version: 1.0.2
 Summary: Coarse grained library for Python
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyGrained-1.0.1/pyGrained.egg-info/SOURCES.txt` & `pyGrained-1.0.2/pyGrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.1/pyproject.toml` & `pyGrained-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pyGrained"
-version="1.0.1"
+version="1.0.2"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "Coarse grained library for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `pyGrained-1.0.1/setup.py` & `pyGrained-1.0.2/setup.py`

 * *Files identical despite different names*

