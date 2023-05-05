# Comparing `tmp/antspymm-0.9.1.tar.gz` & `tmp/antspymm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.9.1.tar", last modified: Tue May  2 15:03:01 2023, max compression
+gzip compressed data, was "antspymm-0.9.2.tar", last modified: Fri May  5 18:32:37 2023, max compression
```

## Comparing `antspymm-0.9.1.tar` & `antspymm-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.606745 antspymm-0.9.1/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.1/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.1/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-02 15:03:01.606494 antspymm-0.9.1/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.1/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.588075 antspymm-0.9.1/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.1/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   284731 2023-05-02 11:53:10.000000 antspymm-0.9.1/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.590417 antspymm-0.9.1/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      763 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.601325 antspymm-0.9.1/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.1/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.1/docs/bids_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.1/docs/example_run_from_directory.py
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.1/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.1/docs/nrg_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.1/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.1/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.1/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-02 15:03:01.606801 antspymm-0.9.1/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-02 11:55:31.000000 antspymm-0.9.1/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.605975 antspymm-0.9.1/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.1/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.1/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.1/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.1/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.1/tests/test_dti_reg.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.1/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.1/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.1/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.1/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.1/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.1/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.1/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:37.005564 antspymm-0.9.2/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.2/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.2/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-05 18:32:37.005158 antspymm-0.9.2/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.2/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.986983 antspymm-0.9.2/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.2/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   284852 2023-05-05 18:23:38.000000 antspymm-0.9.2/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.989465 antspymm-0.9.2/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.997387 antspymm-0.9.2/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.2/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.2/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.2/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.2/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.2/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.2/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.2/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.2/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-05 18:32:37.005651 antspymm-0.9.2/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-05 18:19:33.000000 antspymm-0.9.2/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:37.004406 antspymm-0.9.2/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.2/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.2/tests/mm_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.2/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.2/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.2/tests/test_dti_reg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.2/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.2/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.2/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.2/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.2/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.2/tests/test_ukbb_rsfmri.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.2/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.2/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.1/LICENSE` & `antspymm-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/PKG-INFO` & `antspymm-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.1
+Version: 0.9.2
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.1/README.md` & `antspymm-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/antspymm/__init__.py` & `antspymm-0.9.2/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/antspymm/mm.py` & `antspymm-0.9.2/antspymm/mm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1842,32 +1842,36 @@
             lowerindices.append(x)
 
     return {
     'lowermeans':lowerindices,
     'highermeans':higherindices }
 
 
-def get_average_rsf( x ):
+def get_average_rsf( x, min_t=10, max_t=35 ):
     """
     automatically generates the average bold image with quick registration
 
     returns:
         avg_bold
     """
     output_directory = tempfile.mkdtemp()
     ofn = output_directory + "/w"
     bavg = ants.slice_image( x, axis=3, idx=0 ) * 0.0
     oavg = ants.slice_image( x, axis=3, idx=0 )
-    for myidx in range(x.shape[3]):
+    if x.shape[3] < min_t:
+        min_t=0
+    if x.shape[3] < max_t:
+        max_t=x.shape[3]
+    for myidx in range(min_t,max_t):
         b0 = ants.slice_image( x, axis=3, idx=myidx)
         bavg = bavg + ants.registration(oavg,b0,'Rigid',outprefix=ofn)['warpedmovout']
     bavg = ants.iMath( bavg, 'Normalize' )
     oavg = ants.image_clone( bavg )
     bavg = oavg * 0.0
-    for myidx in range(x.shape[3]):
+    for myidx in range(min_t,max_t):
         b0 = ants.slice_image( x, axis=3, idx=myidx)
         bavg = bavg + ants.registration(oavg,b0,'Rigid',outprefix=ofn)['warpedmovout']
     import shutil
     shutil.rmtree(output_directory, ignore_errors=True )
     return ants.n4_bias_field_correction(bavg)
 
 
@@ -3821,15 +3825,15 @@
       'NM_q0pt95' : np.quantile( nm_avg_cropped.numpy(), 0.95 ),
       'NM_substantianigra_z_coordinate' : sn_z,
       'NM_evr' : nm_evr,
       'NM_count': len( list_nm_images )
        }
 
 def resting_state_fmri_networks( fmri, fmri_template, t1, t1segmentation,
-    f=[0.03,0.08], FD_threshold=0.5, spa = 1.5, spt = 0.5, nc = 6, type_of_transform='SyN',
+    f=[0.03,0.08], FD_threshold=0.5, spa = 1.5, spt = 0.5, nc = 6, type_of_transform='Rigid',
     verbose=False ):
 
   """
   Compute resting state network correlation maps based on the J Power labels.
   This will output a map for each of the major network systems.
 
   Arguments
@@ -3874,15 +3878,15 @@
   corrmo = timeseries_reg(
     fmri, fmri_template,
     type_of_transform=type_of_transform,
     total_sigma=0.0,
     fdOffset=2.0,
     trim = 8,
     output_directory=None,
-    verbose=False,
+    verbose=verbose,
     syn_metric='cc',
     syn_sampling=2,
     reg_iterations=[40,20,5] )
   if verbose:
       print("End rsfmri motion correction")
       # ants.image_write( corrmo['motion_corrected'], '/tmp/temp.nii.gz' )
```

### Comparing `antspymm-0.9.1/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.2/antspymm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.1
+Version: 0.9.2
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.1/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.2/antspymm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 tests/test_dti_recon.py
 tests/test_dti_reg.py
 tests/test_dwi_run.py
 tests/test_flair_run.py
 tests/test_joint_dti_recon.py
 tests/test_mm_csv.py
 tests/test_rsfmri_run.py
+tests/test_ukbb_rsfmri.py
 tests/testsr.py
 tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.1/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.2/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/bids_cohort_example.py` & `antspymm-0.9.2/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/example_run_from_directory.py` & `antspymm-0.9.2/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/nrg_cohort_example.py` & `antspymm-0.9.2/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/outlierness.py` & `antspymm-0.9.2/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/ukbb_to_nrg_processing.py` & `antspymm-0.9.2/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/docs/ukbb_to_nrg_processing2.py` & `antspymm-0.9.2/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/setup.py` & `antspymm-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.9.1',
+      version='0.9.2',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.9.1/tests/mm.py` & `antspymm-0.9.2/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/mm_nrg.py` & `antspymm-0.9.2/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/test_dti_reg.py` & `antspymm-0.9.2/tests/test_dti_reg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/test_dwi_run.py` & `antspymm-0.9.2/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/test_joint_dti_recon.py` & `antspymm-0.9.2/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/test_mm_csv.py` & `antspymm-0.9.2/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/test_rsfmri_run.py` & `antspymm-0.9.2/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/testsr.py` & `antspymm-0.9.2/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.1/tests/visualize_tractogram.py` & `antspymm-0.9.2/tests/visualize_tractogram.py`

 * *Files identical despite different names*

