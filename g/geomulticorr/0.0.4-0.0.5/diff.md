# Comparing `tmp/geomulticorr-0.0.4.tar.gz` & `tmp/geomulticorr-0.0.5.tar.gz`

## Comparing `geomulticorr-0.0.4.tar` & `geomulticorr-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20214 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/src/geomulticorr/xzone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_geomorph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_pzone.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/tests/test_xzone.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/LICENSE.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 geomulticorr-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20214 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/xzone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_geomorph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_pzone.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_xzone.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/PKG-INFO
```

### Comparing `geomulticorr-0.0.4/src/geomulticorr/geomorph.py` & `geomulticorr-0.0.5/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/pair.py` & `geomulticorr-0.0.5/src/geomulticorr/pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/pzone.py` & `geomulticorr-0.0.5/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/session.py` & `geomulticorr-0.0.5/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/spine.py` & `geomulticorr-0.0.5/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/thumb.py` & `geomulticorr-0.0.5/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/src/geomulticorr/xzone.py` & `geomulticorr-0.0.5/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/tests/test_session.py` & `geomulticorr-0.0.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/LICENSE.md` & `geomulticorr-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.4/pyproject.toml` & `geomulticorr-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.0.4/PKG-INFO` & `geomulticorr-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

