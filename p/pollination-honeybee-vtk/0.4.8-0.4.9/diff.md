# Comparing `tmp/pollination-honeybee-vtk-0.4.8.tar.gz` & `tmp/pollination-honeybee-vtk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-vtk-0.4.8.tar", last modified: Thu Nov 10 19:40:22 2022, max compression
+gzip compressed data, was "dist/pollination-honeybee-vtk-0.4.9.tar", last modified: Tue Nov 22 00:01:14 2022, max compression
```

## Comparing `pollination-honeybee-vtk-0.4.8.tar` & `pollination-honeybee-vtk-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/assets/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/assets/logo/vtk.png
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9074 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/post_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 19:39:23.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 19:40:22.000000 pollination-honeybee-vtk-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/tests/export_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/tests/post_process_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-10 19:38:58.000000 pollination-honeybee-vtk-0.4.8/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/.dependabot/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/.dependabot/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (122)     3203 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/assets/logo/vtk.png
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9074 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2691 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 00:00:19.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 00:01:14.000000 pollination-honeybee-vtk-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/tests/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/tests/post_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2022-11-21 23:59:47.000000 pollination-honeybee-vtk-0.4.9/tests/translate_test.py
```

### Comparing `pollination-honeybee-vtk-0.4.8/.github/workflows/ci.yaml` & `pollination-honeybee-vtk-0.4.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/LICENSE` & `pollination-honeybee-vtk-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/PKG-INFO` & `pollination-honeybee-vtk-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-vtk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Honeybee vtk plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-vtk
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: Devang, ladybug-tools
 Maintainer-email: devang@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-vtk-0.4.8/assets/logo/vtk.png` & `pollination-honeybee-vtk-0.4.9/assets/logo/vtk.png`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/config.py` & `pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/config.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/export.py` & `pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/export.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/post_process.py` & `pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/post_process.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/pollination/honeybee_vtk/translate.py` & `pollination-honeybee-vtk-0.4.9/pollination/honeybee_vtk/translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,14 @@
     """Translate hbjson file to vtkjs/vtp/vtk format."""
 
     hbjson_file = Inputs.file(
         description='HBJSON file.',
         path='input.hbjson'
     )
 
-    name = Inputs.str(
-        description='Name of the zip file.',
-        default='model'
-    )
-
     file_type = Inputs.str(
         description='Choose the type of files to export from: vtkjs, vtp, vtk.',
         default='vtkjs',
         spec={'type': 'string',
               'enum': ['vtkjs', 'vtp', 'vtk']}
     )
 
@@ -60,19 +55,19 @@
     data = Inputs.folder(
         description='Input data folder. This folder must include a config.json file',
         path='input_data', optional=True
     )
 
     @command
     def translate_model(self):
-        return 'honeybee-vtk translate --name {{self.name}} --file-type' \
+        return 'honeybee-vtk translate --name model --file-type' \
             ' {{self.file_type}} --model-display-mode {{self.model_display_mode}}' \
             ' --grid-display-mode {{self.grid_display_mode}}' \
             ' --grid-options {{self.grid_options}}'\
             ' --triangle-angle {{self.triangle_angle}}' \
             ' --triangle-radius {{self.triangle_radius}}'\
             ' --config input_data/config.json input.hbjson --folder target_folder'
 
     output_file = Outputs.file(
         description='Created file.',
-        path='target_folder/{{self.name}}.{{self.file_type}}'
+        path='target_folder/model.{{self.file_type}}'
     )
```

### Comparing `pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/PKG-INFO` & `pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-vtk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Honeybee vtk plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-vtk
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: Devang, ladybug-tools
 Maintainer-email: devang@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-vtk-0.4.8/pollination_honeybee_vtk.egg-info/SOURCES.txt` & `pollination-honeybee-vtk-0.4.9/pollination_honeybee_vtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/setup.py` & `pollination-honeybee-vtk-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-vtk-0.4.8/tests/export_test.py` & `pollination-honeybee-vtk-0.4.9/tests/export_test.py`

 * *Files identical despite different names*

