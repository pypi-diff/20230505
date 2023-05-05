# Comparing `tmp/atmoswing-vigicrues-1.0.1.tar.gz` & `tmp/atmoswing-vigicrues-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.0.1.tar", last modified: Tue Apr 18 16:26:33 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.0.2.tar", last modified: Fri May  5 12:52:33 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.0.1.tar` & `atmoswing-vigicrues-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.586480 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 16:26:33.000000 atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:26:33.590480 atmoswing-vigicrues-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 16:26:14.000000 atmoswing-vigicrues-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.427347 atmoswing-vigicrues-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 12:52:33.427347 atmoswing-vigicrues-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-05 12:52:33.427347 atmoswing-vigicrues-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.407347 atmoswing-vigicrues-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.415347 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.419347 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.419347 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.423347 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.419347 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 12:52:33.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-05 12:52:33.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:52:33.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 12:52:33.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 12:52:33.000000 atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:52:33.427347 atmoswing-vigicrues-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-05 12:52:07.000000 atmoswing-vigicrues-1.0.2/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.0.1/LICENSE` & `atmoswing-vigicrues-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/pyproject.toml` & `atmoswing-vigicrues-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,13 +87,13 @@
         if not hasattr(self.cli_options, 'config_file') or \
                 self.cli_options.config_file is None:
             raise asv.OptionError(
                 "Le chemin du fichier de configuration n'a pas été fourni.")
 
     def _load_config(self):
         asv.check_file_exists(self.cli_options.config_file)
-        with open(self.cli_options.config_file) as f:
+        with open(self.cli_options.config_file, mode='rb') as f:
             self.config = yaml.load(f, Loader=yaml.FullLoader)
 
     def _override_options(self):
         if hasattr(self.cli_options, 'batch_file'):
             self.config['atmoswing']['with']['batch_file'] = self.cli_options.batch_file
```

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.0.2/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_controller.py` & `atmoswing-vigicrues-1.0.2/tests/test_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,7 +92,18 @@
     options = types.SimpleNamespace(
         config_file=DIR_PATH + '/files/config_atmoswing_now_full.yaml',
         batch_file=DIR_PATH + '/files/batch_file.xml'
     )
     controller = asv.Controller(options)
     if RUN_ATMOSWING:
         controller.run()
+
+
+def test_special_characters_in_config_file():
+    options = types.SimpleNamespace(
+        config_file=DIR_PATH + '/files/config_with_special_characters.yaml',
+        batch_file=DIR_PATH + '/files/batch_file.xml'
+    )
+    controller = asv.Controller(options)
+    decoded_password = controller.options.config['pre_actions'][0]['with']['password']
+    assert decoded_password == '@#°§&£¢$*[]{}()+'
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.0.2/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_exceptions.py` & `atmoswing-vigicrues-1.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.0.2/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_export_prv.py` & `atmoswing-vigicrues-1.0.2/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_options.py` & `atmoswing-vigicrues-1.0.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.1/tests/test_utils.py` & `atmoswing-vigicrues-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

