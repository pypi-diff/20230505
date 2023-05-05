# Comparing `tmp/FacetClumps-0.1.tar.gz` & `tmp/FacetClumps-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FacetClumps-0.1.tar", last modified: Thu Sep  8 03:30:53 2022, max compression
+gzip compressed data, was "dist\FacetClumps-0.2.tar", last modified: Thu Sep  8 05:09:58 2022, max compression
```

## Comparing `FacetClumps-0.1.tar` & `FacetClumps-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-08 03:30:53.756591 FacetClumps-0.1/
-drwxrwxrwx   0        0        0        0 2022-09-08 03:30:53.734650 FacetClumps-0.1/FacetClumps/
--rw-rw-rw-   0        0        0    10245 2022-09-06 10:58:15.000000 FacetClumps-0.1/FacetClumps/Detect_Files.py
--rw-rw-rw-   0        0        0    21807 2022-09-06 10:30:21.000000 FacetClumps-0.1/FacetClumps/FacetClumps_2D.py
--rw-rw-rw-   0        0        0    30554 2022-09-06 10:13:59.000000 FacetClumps-0.1/FacetClumps/FacetClumps_3D.py
--rw-rw-rw-   0        0        0       84 2022-09-06 11:07:50.000000 FacetClumps-0.1/FacetClumps/Test_File.py
--rw-rw-rw-   0        0        0      102 2022-09-06 11:00:44.000000 FacetClumps-0.1/FacetClumps/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-08 03:30:53.751604 FacetClumps-0.1/FacetClumps.egg-info/
--rw-rw-rw-   0        0        0      195 2022-09-08 03:30:53.000000 FacetClumps-0.1/FacetClumps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2022-09-08 03:30:53.000000 FacetClumps-0.1/FacetClumps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-08 03:30:53.000000 FacetClumps-0.1/FacetClumps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-09-08 03:30:53.000000 FacetClumps-0.1/FacetClumps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      195 2022-09-08 03:30:53.753602 FacetClumps-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       77 2022-09-06 11:18:55.000000 FacetClumps-0.1/README.md
--rw-rw-rw-   0        0        0       42 2022-09-08 03:30:53.756591 FacetClumps-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1316 2022-09-08 03:30:46.000000 FacetClumps-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-08 05:09:58.377574 FacetClumps-0.2/
+drwxrwxrwx   0        0        0        0 2022-09-08 05:09:58.366619 FacetClumps-0.2/FacetClumps/
+-rw-rw-rw-   0        0        0    10272 2022-09-08 04:58:11.000000 FacetClumps-0.2/FacetClumps/Detect_Files.py
+-rw-rw-rw-   0        0        0    21807 2022-09-06 10:30:21.000000 FacetClumps-0.2/FacetClumps/FacetClumps_2D.py
+-rw-rw-rw-   0        0        0    30554 2022-09-06 10:13:59.000000 FacetClumps-0.2/FacetClumps/FacetClumps_3D.py
+-rw-rw-rw-   0        0        0       84 2022-09-06 11:07:50.000000 FacetClumps-0.2/FacetClumps/Test_File.py
+-rw-rw-rw-   0        0        0      102 2022-09-06 11:00:44.000000 FacetClumps-0.2/FacetClumps/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-08 05:09:58.375577 FacetClumps-0.2/FacetClumps.egg-info/
+-rw-rw-rw-   0        0        0      195 2022-09-08 05:09:58.000000 FacetClumps-0.2/FacetClumps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2022-09-08 05:09:58.000000 FacetClumps-0.2/FacetClumps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-08 05:09:58.000000 FacetClumps-0.2/FacetClumps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2022-09-08 05:09:58.000000 FacetClumps-0.2/FacetClumps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      195 2022-09-08 05:09:58.376577 FacetClumps-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2022-09-06 11:18:55.000000 FacetClumps-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-08 05:09:58.378569 FacetClumps-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2022-09-08 04:41:00.000000 FacetClumps-0.2/setup.py
```

### Comparing `FacetClumps-0.1/FacetClumps/Detect_Files.py` & `FacetClumps-0.2/FacetClumps/Detect_Files.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         d_outcat = np.hstack([[index_id, Peak1, Peak2, Peak3, Cen1, Cen2, Cen3, Size1, Size2, Size3, Peak, Sum, Volume]]).T
         df_outcat = pd.DataFrame(d_outcat, columns= \
             ['ID', 'Peak1', 'Peak2', 'Peak3', 'Cen1', 'Cen2', 'Cen3', 'Size1', 'Size2', 'Size3', 'Peak', 'Sum', 'Volume'])
     return df_outcat
 
 
 def Detect(file_name, parameters, mask_name, outcat_name, outcat_wcs_name):
+    global did_table
     start_1 = time.time()
     start_2 = time.ctime()
     RMS = parameters[0]
     Threshold = parameters[1]
     KBins = parameters[2]
     Vmm = parameters[3]
 
@@ -204,16 +205,16 @@
     np.savez(outcat_name[:-4] + '_Facet_npz', did_Facet=did_table)
     regions_data = did_table['regions_data']
     fits.writeto(mask_name, regions_data, overwrite=True)
     df_outcat = Table_Interface(did_table,ndim)
     df_outcat.to_csv(outcat_name, sep='\t', index=False)
 
     data_wcs = get_wcs(file_name)
-    outcat_wcs = change_pix2word(data_wcs, df_outcat, ndim)
-    save_outcat(outcat_name=outcat_wcs_name, outcat=outcat_wcs)
+    outcat_wcs = change_pix2word(data_wcs, df_outcat)
+    save_outcat(outcat_name=outcat_wcs_name, outcat=outcat_wcs, ndim=ndim)
 
     end_1 = time.time()
     end_2 = time.ctime()
     delta_time = end_1 - start_1
     time_record = []
     time_record = np.hstack([[start_2, end_2, delta_time]])
     time_record = pd.DataFrame(time_record, index=['Start', 'End', 'DTime'])
```

### Comparing `FacetClumps-0.1/FacetClumps/FacetClumps_2D.py` & `FacetClumps-0.2/FacetClumps/FacetClumps_2D.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.1/FacetClumps/FacetClumps_3D.py` & `FacetClumps-0.2/FacetClumps/FacetClumps_3D.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.1/setup.py` & `FacetClumps-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FacetClumps',  # 包名
-    version='0.1',  # 版本
+    version='0.2',  # 版本
     description="FacetClumps: A molecular cloud clump detection algorithm based on Facet model",  # 包简介
     # long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     # include_package_data=True,  # 是否允许上传资源文件
     author='Jiang Yu',  # 作者
     author_email="yujiang@pmo.ac.cn",  # 作者邮件
     # maintainer='',  # 维护者
     # maintainer_email="yujiang@pmo.ac.cn",  # 维护者邮件
```

