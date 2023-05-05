# Comparing `tmp/geomulticorr-0.0.6.tar.gz` & `tmp/geomulticorr-0.0.7.tar.gz`

## Comparing `geomulticorr-0.0.6.tar` & `geomulticorr-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_geomorph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_pzone.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_xzone.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20886 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_pair.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/tests/test_xzone.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.0.7/PKG-INFO
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/geomorph.py` & `geomulticorr-0.0.7/src/geomulticorr/geomorph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
-#try:
-import geomulticorr.spine as gmc_spine
-#except ModuleNotFoundError:
-#    import src.geomulticorr.spine as gmc_spine
+try:
+    import geomulticorr.spine as gmc_spine
+except ModuleNotFoundError:
+    import src.geomulticorr.spine as gmc_spine
 
 class Geomorph:
         
     def __init__(self, session, ge_id):
         
         # Check existence and unique
         assert ge_id in session._geomorphs.ge_frogi_id.values, 'key not found in Geomorphs layer'
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/pair.py` & `geomulticorr-0.0.7/src/geomulticorr/pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from telenvi import raster_tools as rt
 
-#try:
-import geomulticorr.thumb as gmc_thumb
-#except ModuleNotFoundError:
-#    import src.geomulticorr.thumb as gmc_thumb
+try:
+    import geomulticorr.thumb as gmc_thumb
+except ModuleNotFoundError:
+    import src.geomulticorr.thumb as gmc_thumb
 
-ROOT_OUTPUTS  = Path(__file__).parent.with_name('temp')
-ROOT_TEMPLATE = Path(__file__).parent.with_name('template')
+ROOT_OUTPUTS  = Path(__file__).with_name('temp')
 
 class Pair:
 
     def __init__(self, session=None, target_path=None, left=None, right=None):
 
         """
         soit session et target_path sont definis
@@ -185,15 +184,15 @@
 
     def corr(self, corr_algorithm=2, corr_kernel_size=7, corr_xthreshold=10):
         
         # Check clip
         self.clip()
 
         # Check existing correlation
-        if self.pa_status == 'complete':
+        if self.get_status() == 'complete':
             return True
 
         # Create a directory in a place where ASP can write their outputs : the temp directory, inside GeoMultiCorr app
         temp = Path(ROOT_OUTPUTS, self.pa_key)
         if not temp.exists():
             temp.mkdir()
 
@@ -209,44 +208,45 @@
             --corr-memory-limit-mb 8000 \
             --save-left-right-disparity-difference\
             --ip-per-tile 200 \
             --min-num-ip 5"
 
         # Launch
         os.system(corr_command)
+        return True
 
     def save_corrdata(self, verbose=False):
         """
         Move the ASP outputs from GeoMultiCorr temporal storage location
         """
 
         # Hide ugly warnings about symlinks
         verbose_mode = {False:' > /dev/null 2>&1', True:''}
 
-        # get the GeoMultiCorr storage location
+        # get the GeoMultiCorr temp storage location
         departure = Path(ROOT_OUTPUTS, self.pa_key)
-        if not departure.exists():
-            return None
 
         # get the displacements folder path in the current session
         destination = self.pa_asp_path
 
         # send the command to bring back the temporal data in the current session
         os.system(f"mv {departure} {destination} {verbose_mode[verbose]}")
         if self.pa_asp_path.exists():
             os.system(f"rm -rf {departure}")
             return True
-    
+
+        return False
+
     def compute_magnitude(self):
 
         assert self.pa_dispf_path.exists(), 'this pair is not yet correlate'
 
         # Check if the file is ever existing
         if self.pa_magn_path.exists():
-            return True
+            return self.get_magn_geoim()
 
         # Open the stack with horizontal and vertical displacements
         xDisp, yDisp = rt.pre_process(str(self.pa_dispf_path), nBands=[1,2], geoim=True).splitBands()
 
         # We switch values using negative values because ASP gives displacements 
         # in pixel coordinates using as reference upper-left corner
         yDisp *= -1.0
@@ -257,14 +257,16 @@
         # Magnitude raster creation
         magn = ((xDisp ** 2 + yDisp ** 2) ** 0.5)
 
         # Magnitude in meters
         magn_in_meters = magn * pxSizeX
         magn_in_meters.save(str(self.pa_magn_path))
 
+        return magn_in_meters
+
     def vectorize(self, output_pixel_size=None, method='average', write=True):
         """
         create a points vector layer, mappable as a vector field in Qgis
 
         output_pixel_size : space between each point. By default, it is the pixel size of the pair disparity map
         method  : algorithm to use to resample the data (is a output_pixel_size value is given)
         """
@@ -306,29 +308,29 @@
 
         # Compute displacement geographic direction (vector orientation)
         array_complex_dx_dy = np.apply_along_axis(lambda args: [complex(*args)], 0, [dx_in_meters.array,dy_in_meters_switched.array]).reshape(nCols, nRows)
         array_direction = np.angle(array_complex_dx_dy, deg=True)
         direction = d_in_meters.copy()
         direction.array = array_direction
 
-        # Make a big GeoIm with all this lovely data
+        # Make a big GeoIm with all this lovely dataset
         to_vectorize = rt.stack([
             dx_in_pixels,
             dy_in_pixels,
             dx_in_meters,
             dy_in_meters,
             d_in_meters,
             dx_in_meters_per_year,
             dy_in_meters_per_year,
             d_in_meters_per_year,
             direction
         ])
-
-        vectors = rt.vectorize(to_vectorize).set_crs(epsg=2154)
         
+        vectors = rt.vectorize(to_vectorize).set_crs(epsg=2154)
+    
         # Write vector layer in geopackage
         if write == True:
             current_vector_layer_name = f"{output_pixel_size}_{self.pa_key}"
             vectors.to_file(self.pa_vect_path, layer=current_vector_layer_name)
 
             # Copy .qml file
             template_style = 'styles/vector-field_style_1.qml'
@@ -337,24 +339,24 @@
             os.system(cp_command)
 
         return vectors
 
     def pa_full(self, corr_algorithm=2, corr_kernel_size=7, corr_xthreshold=10, vector_res=20, method='average'):
 
         # Clip
-        # self.clip()
+        self.clip()
 
         # Corr
-        # self.corr(corr_algorithm, corr_kernel_size, corr_xthreshold)
+        self.corr(corr_algorithm, corr_kernel_size, corr_xthreshold)
 
         # Save
-        # self.save_corrdata()
+        self.save_corrdata()
 
         # Magn
-        # self.compute_magnitude()
+        self.compute_magnitude()
 
         # Vectors
         self.vectorize(output_pixel_size=vector_res, method=method)
 
         return True
 
     def get_interesting_geoim(self, mode):
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/pzone.py` & `geomulticorr-0.0.7/src/geomulticorr/pzone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import geopandas as gpd
 
-#try:
-import geomulticorr.thumb as gmc_thumb
-#except ModuleNotFoundError:
-#    import src.geomulticorr.thumb as gmc_thumb
+try:
+    import geomulticorr.thumb as gmc_thumb
+except ModuleNotFoundError:
+    import src.geomulticorr.thumb as gmc_thumb
 
 class Pzone:
 
     def __init__(self, target_pz_name, session):
         
         # Vérification de la validité du nom de pzone par rapport au projet
         assert target_pz_name in session.pz_names, f'{target_pz_name} not existing in the Pzones layer'
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/session.py` & `geomulticorr-0.0.7/src/geomulticorr/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 import pandas as pd
 
 from osgeo import gdal
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
 ## User
-#try:
-import geomulticorr.geomorph as gmc_geomorph
-import geomulticorr.pzone    as gmc_pzone
-import geomulticorr.pair     as gmc_pair
-import geomulticorr.spine    as gmc_spine
-import geomulticorr.thumb    as gmc_thumb
-import geomulticorr.xzone    as gmc_xzone
-
-## Developer
-#except ModuleNotFoundError:
-#    import src.geomulticorr.geomorph as gmc_geomorph
-#    import src.geomulticorr.pzone    as gmc_pzone
-#    import src.geomulticorr.pair     as gmc_pair
-#    import src.geomulticorr.spine    as gmc_spine
-#    import src.geomulticorr.thumb    as gmc_thumb
-#    import src.geomulticorr.xzone    as gmc_xzone
+try:
+    import geomulticorr.geomorph as gmc_geomorph
+    import geomulticorr.pzone    as gmc_pzone
+    import geomulticorr.pair     as gmc_pair
+    import geomulticorr.spine    as gmc_spine
+    import geomulticorr.thumb    as gmc_thumb
+    import geomulticorr.xzone    as gmc_xzone
+
+# Developer
+except ModuleNotFoundError:
+    import src.geomulticorr.geomorph as gmc_geomorph
+    import src.geomulticorr.pzone    as gmc_pzone
+    import src.geomulticorr.pair     as gmc_pair
+    import src.geomulticorr.spine    as gmc_spine
+    import src.geomulticorr.thumb    as gmc_thumb
+    import src.geomulticorr.xzone    as gmc_xzone
 
 file_location = Path(__file__)
 if file_location.parent.parent.name == 'site-packages':
     print('''-------------
 geomulticorr : online version
 -------------''')
 else:
@@ -200,15 +200,21 @@
         pairs = [gmc_pair.Pair(self, p.pa_path) for p in board.iloc]
         return pairs
 
     def get_spine(self, sp_id):
         """Send a spine.Spine object"""
         return gmc_spine.Spine(self, sp_id)
 
-    def get_protomap(self, rawpath, extensions=['tif', 'jp2']):
+    def get_protomap(self):
+        try:
+            return gpd.read_file(self.p_geodb, layer='Protomap')
+        except ValueError:
+            print('You have to create a protomap first with my_session.create_protomap()')
+
+    def create_new_protomap(self, rawpath, extensions=['tif', 'jp2'], save_in_geodatabase=True):
         """make a vector layer with the extents of all the rasters stored under the rawpath
            and write metadata in hte layer attribute table"""
 
         # check the validity of the rawpath
         rawpath = Path(rawpath)
         assert rawpath.exists(), f"{rawpath} is not an existing path"
 
@@ -271,14 +277,16 @@
             ft["filepath"] = str(ta)
 
             # Add the feature to the future layer (just a list for now)
             features.append(ft)
 
         # Transform the list of GeoSeries features into a GeoDataFrame, and set his CRS
         layer = gpd.GeoDataFrame(features).set_crs(2154)
+        if save_in_geodatabase == True:
+            layer.to_file(self.p_geodb, layer='Protomap')
         return layer
 
     ########### SETTERS ###########
 
     def update_vector_data(self):
         """
         Update the instance session attributes from geodatabase layers
@@ -294,15 +302,15 @@
 
         # Copy the geodatabase before the transaction
         assert self.copy_geodb()
 
         # Get 2 version of the Thumbs layer
         opt_root = Path(self.p_raster_data)
         old = self._thumbs
-        new = gpd.GeoDataFrame([gmc_thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
+        new = gpd.GeoDataFrame([gmc_thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: gmc_thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
 
         # Comparison
         common = new.merge(old, on=['th_path'])
         stables = old[old.th_path.isin(common.th_path)]
         addeds = new[~new.th_path.isin(common.th_path)]
 
         # Push it into the geodatabase
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/spine.py` & `geomulticorr-0.0.7/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/src/geomulticorr/thumb.py` & `geomulticorr-0.0.7/src/geomulticorr/thumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pathlib import Path
 
 import pandas as pd
 
 from osgeo import gdal
 from telenvi import raster_tools as rt
 
-#try:
-import geomulticorr.pair as gmc_pair
-#except ModuleNotFoundError:
-#    import src.geomulticorr.pair as gmc_pair
+try:
+    import geomulticorr.pair as gmc_pair
+except ModuleNotFoundError:
+    import src.geomulticorr.pair as gmc_pair
 
 THUMBNAME_PATTERN = re.compile('^([a-z]|[A-Z]|-)+_[0-9]{4}(-[0-9]{2}){2}_.*.(tif|TIF)$')
 
 class Thumb:
 
     def __init__(self, target_path):
         target_path = Path(target_path)
@@ -37,15 +37,15 @@
             'th_sensor':self.th_sensor,
             'th_date':self.th_date ,
             'th_year':self.th_year,
             'th_valid':self.th_valid,
             'geometry':self.geometry})
 
     def __add__(self, right):
-        return gmc_pair.GMC_Pair(left=self, right=right)
+        return gmc_pair.Pair(left=self, right=right)
 
     def __repr__(self):
         return f"""---------
 type   : GMC_Thumb
 pzone  : {self.th_pz_name}
 date   : {self.th_date}
 sensor : {self.th_sensor}
```

### Comparing `geomulticorr-0.0.6/src/geomulticorr/xzone.py` & `geomulticorr-0.0.7/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.0.7/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.0.7/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.0.7/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/tests/test_session.py` & `geomulticorr-0.0.7/tests/test_pzone.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 import unittest
 import geopandas as gpd
 
 import src.geomulticorr.session
-import src.geomulticorr.spine
 
-class TestSession(unittest.TestCase):
+test_create_protomap = False
+
+class TestPzone(unittest.TestCase):
 
     def setUp(self):
         self.path_to_test_session = '/media/duvanelt/TD002/sandbox_gmc/vanoise'
         self.test_session = src.geomulticorr.session.Session(self.path_to_test_session)
-        self.test_pzone_name = 'iseran'
-        self.test_spine_id = 'ISFR730486'
+        self.test_pzone = self.test_session.get_pzones('ribon')[0]
 
-    def test_is_session(self):
-        self.assertIsInstance(self.test_session, src.geomulticorr.session.Session)
+    def test_is_pzone(self):
+        self.assertIsInstance(self.test_pzone, src.geomulticorr.pzone.Pzone)
 
     def test_get_thumbs(self):
-        self.assertIsInstance(self.test_session.get_thumbs(), list)
-        self.assertIsInstance(self.test_session.get_thumbs(self.test_pzone_name), list)
+        self.assertIsInstance(self.test_pzone.get_thumbs(), list)
+        self.assertIsInstance(self.test_pzone.get_thumbs(2018), list)
 
     def test_get_pairs(self):
-        self.assertIsInstance(self.test_session.get_pairs(), list)
-        self.assertIsInstance(self.test_session.get_pairs(self.test_pzone_name), list)
-
-    def test_get_pzones(self):
-        self.assertIsInstance(self.test_session.get_pzones(), list)
-        self.assertIsInstance(self.test_session.get_pzones(self.test_pzone_name), list)
-
-    def test_get_geomorphs(self):
-        self.assertIsInstance(self.test_session.get_geomorphs(), list)
-        self.assertIsInstance(self.test_session.get_geomorphs(self.test_pzone_name), list)
-
-    def test_get_spine(self):
-        self.assertIsInstance(self.test_session.get_spine(self.test_spine_id), src.geomulticorr.spine.Spine)
-
-    def test_get_protomap(self):
-        self.assertIsInstance(self.test_session.get_protomap(), gpd.GeoDataFrame)
-
-if __name__ == '__main__':
-    unittest.main()
+        self.assertIsInstance(self.test_pzone.get_pairs(), list)
+    
+    def test_get_valid_thumbs(self):
+        self.assertIsInstance(self.test_pzone.get_valid_thumbs(), list)
+    
+    def test_get_valid_pairs(self):
+        self.assertIsInstance(self.test_pzone.get_valid_pairs(), list)
+    
+    # def test_pz_full(self):
+    #     self.assertIsInstance(self.test_pzone.pz_full(), dict)
```

### Comparing `geomulticorr-0.0.6/LICENSE.md` & `geomulticorr-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.6/pyproject.toml` & `geomulticorr-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.0.6/PKG-INFO` & `geomulticorr-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

