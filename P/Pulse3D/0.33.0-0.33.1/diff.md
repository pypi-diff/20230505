# Comparing `tmp/Pulse3D-0.33.0.tar.gz` & `tmp/Pulse3D-0.33.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.0.tar", last modified: Tue May  2 22:17:34 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.1.tar", last modified: Thu May  4 23:48:48 2023, max compression
```

## Comparing `Pulse3D-0.33.0.tar` & `Pulse3D-0.33.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.977733 Pulse3D-0.33.0/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.977733 Pulse3D-0.33.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 22:17:34.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 22:17:34.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:17:17.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 23:48:48.672560 Pulse3D-0.33.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 23:48:48.672560 Pulse3D-0.33.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 23:48:48.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-04 23:48:48.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:48:33.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33981 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.0/LICENSE` & `Pulse3D-0.33.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/PKG-INFO` & `Pulse3D-0.33.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.0
+Version: 0.33.1
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.0/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.1/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/setup.py` & `Pulse3D-0.33.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.0",
+    version="0.33.1",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.0/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.1/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.0
+Version: 0.33.1
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.0/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.1/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.1/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.1/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.1/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/constants.py` & `Pulse3D-0.33.1/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.1/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/exceptions.py` & `Pulse3D-0.33.1/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.1/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/metrics.py` & `Pulse3D-0.33.1/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.1/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.1/src/pulse3D/plate_recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,20 +587,21 @@
         # add stim timepoints
         aggregate_stim_timepoints_us = None
         if attempt_to_output_stim_data:
             aggregate_stim_timepoints_us = aggregate_timepoints(
                 [session_data[0] for wf in self for session_data in wf.stim_sessions]
             )
             aggregate_stim_timepoints_us_for_plotting = np.repeat(aggregate_stim_timepoints_us, 2)
-            data["Stim Time (µs)"] = pd.Series(aggregate_stim_timepoints_us_for_plotting)
 
         # only outputting stim data if an attempt to output stim data was made and the file actually has stim data in it
         is_outputting_stim_data = (
             aggregate_stim_timepoints_us is not None and aggregate_stim_timepoints_us.any()
         )
+        if is_outputting_stim_data:
+            data["Stim Time (µs)"] = pd.Series(aggregate_stim_timepoints_us_for_plotting)
 
         # iterating over self.wells instead of using __iter__ so well_idx is preserved
         for well_idx, wf in enumerate(self.wells):
             if not wf:
                 continue
 
             well_name = wf.get(WELL_NAME_UUID, TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_idx))
```

### Comparing `Pulse3D-0.33.0/src/pulse3D/plotting.py` & `Pulse3D-0.33.1/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/stimulation.py` & `Pulse3D-0.33.1/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/transforms.py` & `Pulse3D-0.33.1/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.0/src/pulse3D/utils.py` & `Pulse3D-0.33.1/src/pulse3D/utils.py`

 * *Files identical despite different names*

