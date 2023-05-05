# Comparing `tmp/geomulticorr-0.0.5.tar.gz` & `tmp/geomulticorr-0.0.6.tar.gz`

## Comparing `geomulticorr-0.0.5.tar` & `geomulticorr-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20214 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/src/geomulticorr/xzone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_geomorph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_pzone.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/tests/test_xzone.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/LICENSE.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 geomulticorr-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_geomorph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_pzone.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/tests/test_xzone.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.0.6/PKG-INFO
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/geomorph.py` & `geomulticorr-0.0.6/src/geomulticorr/geomorph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
-import geomulticorr.spine
+#try:
+import geomulticorr.spine as gmc_spine
+#except ModuleNotFoundError:
+#    import src.geomulticorr.spine as gmc_spine
 
 class Geomorph:
         
     def __init__(self, session, ge_id):
         
         # Check existence and unique
         assert ge_id in session._geomorphs.ge_frogi_id.values, 'key not found in Geomorphs layer'
@@ -73,15 +76,15 @@
             row['V'] = row.D/abs(row.L-row.R)        
             disps.append(row)
         return pd.DataFrame(disps)
     
     def get_spines(self):
         all_spines = self.session._spines
         ge_spines  = all_spines[all_spines.sp_ge_id == self.ge_id]
-        return [geomulticorr.spine.Spine(self.session, spine.sp_id) for spine in ge_spines.iloc]
+        return [gmc_spine.Spine(self.session, spine.sp_id) for spine in ge_spines.iloc]
 
     def show_mean_velocities(self, savepath=None, bounds=None):
         fig, ax = plt.subplots(figsize=(10,6.5))
         disps = self.get_disp_overview()
         for pair in disps.iloc:
             ya = pair.L
             yb = pair.R
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/pair.py` & `geomulticorr-0.0.6/src/geomulticorr/pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from telenvi import raster_tools as rt
 
-import geomulticorr.thumb
+#try:
+import geomulticorr.thumb as gmc_thumb
+#except ModuleNotFoundError:
+#    import src.geomulticorr.thumb as gmc_thumb
 
 ROOT_OUTPUTS  = Path(__file__).parent.with_name('temp')
 ROOT_TEMPLATE = Path(__file__).parent.with_name('template')
 
 class Pair:
 
     def __init__(self, session=None, target_path=None, left=None, right=None):
@@ -37,16 +40,16 @@
 
             # Reconstruct their path
             thumbs_pzone_path = Path(session.p_raster_data, pz_name, 'opticals')
             left_path = Path (thumbs_pzone_path, left_key)
             right_path = Path(thumbs_pzone_path, right_key)
 
             # Make Thumbs from them
-            left  = geomulticorr.thumb.Thumb(left_path)
-            right = geomulticorr.thumb.Thumb(right_path)
+            left  = gmc_thumb.Thumb(left_path)
+            right = gmc_thumb.Thumb(right_path)
 
         # Construction from two thumbs
         assert left.th_pz_name == right.th_pz_name, 'left and right have not the same pzone'
         assert left.th_path != right.th_path, 'left thumb is right thumb'
 
         # Metadata
         self.pa_pz_name = left.th_pz_name
@@ -374,10 +377,10 @@
         """
         geoline = [gpd.GeoSeries, path, gpd.GeoDataFrame, shapely.geometry.LineString, (A, B)]
         mode = [m, x, y, vm, vx, vy]
         """
         return self.get_interesting_geoim(mode).inspectGeoLine(geoLine)
 
     def get_slices(self, geoLine, ribLength, ribStep, ribOrientation='v', mode='m'):
-        return self.get_interesting_geoim(mode).inspectRibsAlongSpine(geoLine, ribLength, ribStep, ribOrientation)
+        return self.get_interesting_geoim(mode).inspectRibsAlongthumb(geoLine, ribLength, ribStep, ribOrientation)
 
 # %%
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/pzone.py` & `geomulticorr-0.0.6/src/geomulticorr/pzone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from pathlib import Path
 
 import geopandas as gpd
 
+#try:
+import geomulticorr.thumb as gmc_thumb
+#except ModuleNotFoundError:
+#    import src.geomulticorr.thumb as gmc_thumb
+
 class Pzone:
 
-    def __init__(self, target_pz_name, project):
+    def __init__(self, target_pz_name, session):
         
         # Vérification de la validité du nom de pzone par rapport au projet
-        assert target_pz_name in project.pz_names, f'{target_pz_name} not existing in the Pzones layer'
-        assert Path(project.p_root, 'raster_data', target_pz_name).exists(), f'no raster data folder for {target_pz_name}'
+        assert target_pz_name in session.pz_names, f'{target_pz_name} not existing in the Pzones layer'
+        assert Path(session.p_root, session.p_raster_data, target_pz_name).exists(), f'no raster data folder for {target_pz_name}'
 
         # Ecriture attributs
-        self.proj = project
+        self.proj = session
         self.pz_name = target_pz_name
 
     def get_thumbs_overview(self, criterias=''):
         criterias = [criterias] + [self.pz_name]
         return self.proj.get_thumbs_overview(criterias)
 
     def get_thumbs(self, criterias=''):
@@ -44,15 +49,15 @@
 
     def get_valid_thumbs(self):
         """
         Renvoie les vignettes selectionnées par l'user dans qgis, en modifiant la valeur attributaire "th_valid" dans la table Thumbs
         """
         ths = self.proj.get_thumbs_overview(self.pz_name)
         ths_valid = ths[ths.th_valid=='1']
-        gmc_ths_valid = [GMC_Thumb(th.th_path) for th in ths_valid.iloc]
+        gmc_ths_valid = [gmc_thumb.Thumb(th.th_path) for th in ths_valid.iloc]
         return gmc_ths_valid
 
     def get_valid_pairs(self):
         ps = []
         for left in self.get_valid_thumbs():
             for right in self.get_valid_thumbs():
                 try:
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/session.py` & `geomulticorr-0.0.6/src/geomulticorr/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,31 @@
 import tqdm
 import pandas as pd
 
 from osgeo import gdal
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
-import geomulticorr.geomorph
-import geomulticorr.pzone
-import geomulticorr.pair
-import geomulticorr.spine
-import geomulticorr.thumb
-import geomulticorr.xzone
+## User
+#try:
+import geomulticorr.geomorph as gmc_geomorph
+import geomulticorr.pzone    as gmc_pzone
+import geomulticorr.pair     as gmc_pair
+import geomulticorr.spine    as gmc_spine
+import geomulticorr.thumb    as gmc_thumb
+import geomulticorr.xzone    as gmc_xzone
+
+## Developer
+#except ModuleNotFoundError:
+#    import src.geomulticorr.geomorph as gmc_geomorph
+#    import src.geomulticorr.pzone    as gmc_pzone
+#    import src.geomulticorr.pair     as gmc_pair
+#    import src.geomulticorr.spine    as gmc_spine
+#    import src.geomulticorr.thumb    as gmc_thumb
+#    import src.geomulticorr.xzone    as gmc_xzone
 
 file_location = Path(__file__)
 if file_location.parent.parent.name == 'site-packages':
     print('''-------------
 geomulticorr : online version
 -------------''')
 else:
@@ -136,66 +147,66 @@
 
     def get_thumbs_overview(self, criterias=''):
         """Send a dataframe with informations about each thumb raster file meeting the criterias.
            If there's no criterias, send informations about all the thumbs of the project """
         return self._search_engine('Thumbs', criterias)
 
     def get_thumbs(self, criterias=''):
-        """Send a list of geomulticorr.thumb.Thumb objects meeting the criterias"""
+        """Send a list of thumb.Thumb objects meeting the criterias"""
         selected_thumbs = self.get_thumbs_overview(criterias)
-        return [geomulticorr.thumb.Thumb(x.th_path) for x in selected_thumbs.iloc]
+        return [gmc_thumb.Thumb(x.th_path) for x in selected_thumbs.iloc]
 
     def get_pairs_overview(self, criterias=''):
         """Send a dataframe with each possible Pair according to the Thumbs"""
         return self._search_engine('Pairs', criterias)
     
     def get_pairs(self, criterias=''):
-        """Send a list of geomulticorr.pair.Pairs objects meeting the criterias"""
+        """Send a list of pair.Pairs objects meeting the criterias"""
         selected_pairs = self.get_pairs_overview(criterias)
-        return [geomulticorr.pair.Pair(self, target_path = x.pa_path) for x in selected_pairs.iloc]
+        return [gmc_pair.Pair(self, target_path = x.pa_path) for x in selected_pairs.iloc]
 
     def get_pzones_overview(self, pz_name=''):
         """Send a dataframe with each pzone"""
         return self._search_engine('Pzones', pz_name)
 
     def get_pzones(self, pz_name=''):
-        """Send a list of geomulticorr.pzone.Pzones objects"""
+        """Send a list of pzone.Pzones objects"""
         selected_pzones = self.get_pzones_overview(pz_name)
-        return [geomulticorr.pzone.Pzone(x.pz_name, self) for x in selected_pzones.iloc]
+        return [gmc_pzone.Pzone(x.pz_name, self) for x in selected_pzones.iloc]
 
     def get_geomorphs_overview(self, criterias=''):
         """Send a dataframe with each geomorph"""
         return self._search_engine('Geomorphs', criterias)
 
     def get_geomorphs(self, criterias=''):
-        """Send a list of geomulticorr.geomorph.Geomorphs objects"""
+        """Send a list of geomorph.Geomorphs objects"""
         selected_geomorphs = self.get_geomorphs_overview(criterias)
-        return [geomulticorr.geomorph.Geomorph(self, x.ge_frogi_id) for x in selected_geomorphs.iloc]
+        return [gmc_geomorph.Geomorph(self, x.ge_frogi_id) for x in selected_geomorphs.iloc]
 
     def get_xzone(self, xz_id):
-        """Send a geomulticorr.xzones.Xzones object"""
-        return geomulticorr.xzones.Xzones(self, xz_id)
+        """Send a xzones.Xzones object"""
+        return gmc_xzone.Xzones(self, xz_id)
 
     def get_pairs_overview_on_period(self, ymin, ymax, criterias=''):
         """Retourne un tableau des paires completement incluses dans la période [yMin;yMax]"""
         pairs = self.get_pairs_overview(criterias)
         pairs['chrono_min'] = pairs.apply(lambda row: min(int(row.pa_left_date.split('-')[0]), int(row.pa_right_date.split('-')[0])), axis=1)
         pairs['chrono_max'] = pairs.apply(lambda row: max(int(row.pa_left_date.split('-')[0]), int(row.pa_right_date.split('-')[0])), axis=1)
         pairs = pairs[(pairs.chrono_min>=ymin)&(pairs.chrono_max<=ymax)]
         return pairs
 
     def get_pairs_on_period(self, ymin, ymax, criterias=''):
         """Retourne les paires completement incluses dans la période [yMin;yMax]"""
         board = self.get_pairs_overview_on_period(ymin, ymax, criterias)
-        pairs = [geomulticorr.pair.Pair(self, p.pa_path) for p in board.iloc]
+        pairs = [gmc_pair.Pair(self, p.pa_path) for p in board.iloc]
         return pairs
 
     def get_spine(self, sp_id):
-        """Send a geomulticorr.spine.Spine object"""
-        return geomulticorr.spine.Spine(self, sp_id)
+        """Send a spine.Spine object"""
+        return gmc_spine.Spine(self, sp_id)
 
     def get_protomap(self, rawpath, extensions=['tif', 'jp2']):
         """make a vector layer with the extents of all the rasters stored under the rawpath
            and write metadata in hte layer attribute table"""
 
         # check the validity of the rawpath
         rawpath = Path(rawpath)
@@ -283,15 +294,15 @@
 
         # Copy the geodatabase before the transaction
         assert self.copy_geodb()
 
         # Get 2 version of the Thumbs layer
         opt_root = Path(self.p_raster_data)
         old = self._thumbs
-        new = gpd.GeoDataFrame([geomulticorr.thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: geomulticorr.thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
+        new = gpd.GeoDataFrame([gmc_thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
 
         # Comparison
         common = new.merge(old, on=['th_path'])
         stables = old[old.th_path.isin(common.th_path)]
         addeds = new[~new.th_path.isin(common.th_path)]
 
         # Push it into the geodatabase
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/spine.py` & `geomulticorr-0.0.6/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.5/src/geomulticorr/thumb.py` & `geomulticorr-0.0.6/src/geomulticorr/thumb.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from pathlib import Path
 
 import pandas as pd
 
 from osgeo import gdal
 from telenvi import raster_tools as rt
 
-import geomulticorr.pair
+#try:
+import geomulticorr.pair as gmc_pair
+#except ModuleNotFoundError:
+#    import src.geomulticorr.pair as gmc_pair
 
 THUMBNAME_PATTERN = re.compile('^([a-z]|[A-Z]|-)+_[0-9]{4}(-[0-9]{2}){2}_.*.(tif|TIF)$')
 
 class Thumb:
 
     def __init__(self, target_path):
         target_path = Path(target_path)
@@ -34,15 +37,15 @@
             'th_sensor':self.th_sensor,
             'th_date':self.th_date ,
             'th_year':self.th_year,
             'th_valid':self.th_valid,
             'geometry':self.geometry})
 
     def __add__(self, right):
-        return geomulticorr.pair.GMC_Pair(left=self, right=right)
+        return gmc_pair.GMC_Pair(left=self, right=right)
 
     def __repr__(self):
         return f"""---------
 type   : GMC_Thumb
 pzone  : {self.th_pz_name}
 date   : {self.th_date}
 sensor : {self.th_sensor}
```

### Comparing `geomulticorr-0.0.5/src/geomulticorr/xzone.py` & `geomulticorr-0.0.6/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.5/LICENSE.md` & `geomulticorr-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.5/pyproject.toml` & `geomulticorr-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.0.5/PKG-INFO` & `geomulticorr-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # GeoMultiCorr
 A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 
+# Requirements
+Unix OS
+
+Ames Stereo Pipeline
+
+telenvi
+
+geocube
+
+tqdm
+
+...
+(to complete)
+
 ## GitHub repo
-https://github.com/rgdyn-toolbox/GeoMultiCorr
+https://github.com/rgdyn-toolbox/GeoMultiCorr
```

