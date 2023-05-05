# Comparing `tmp/ricco-1.0.0.tar.gz` & `tmp/ricco-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricco-1.0.0.tar", last modified: Wed Feb 15 14:04:00 2023, max compression
+gzip compressed data, was "ricco-1.1.0.tar", last modified: Fri May  5 10:31:41 2023, max compression
```

## Comparing `ricco-1.0.0.tar` & `ricco-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.217908 ricco-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-15 14:04:00.217908 ricco-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-15 14:03:50.000000 ricco-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 14:04:00.217908 ricco-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-15 14:03:50.000000 ricco-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.213908 ricco-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.213908 ricco-1.0.0/src/ricco/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24200 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/coord_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/dt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.217908 ricco-1.0.0/src/ricco/etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/etl/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/etl/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/etl/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.217908 ricco-1.0.0/src/ricco/geocode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geocode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geocode/amap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geocode/baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geocode/geocode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geocode/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-02-15 14:03:50.000000 ricco-1.0.0/src/ricco/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:04:00.217908 ricco-1.0.0/src/ricco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-15 14:04:00.000000 ricco-1.0.0/src/ricco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-15 14:04:00.000000 ricco-1.0.0/src/ricco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:04:00.000000 ricco-1.0.0/src/ricco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-15 14:04:00.000000 ricco-1.0.0/src/ricco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-15 14:04:00.000000 ricco-1.0.0/src/ricco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 10:31:41.215655 ricco-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 10:31:28.000000 ricco-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:31:41.215655 ricco-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 10:31:28.000000 ricco-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.211655 ricco-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/geocode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/amap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/area_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/city_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/epsg_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/building_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/coord_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/id_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/top_level.txt
```

### Comparing `ricco-1.0.0/PKG-INFO` & `ricco-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.0.0
-Summary: tools
+Version: 1.1.0
+Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `ricco-1.0.0/setup.py` & `ricco-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   )
 
 with open(os.path.join(pwd, 'README.md'), encoding='utf-8') as f:
   README = f.read()
 
 setup(name='ricco',
       version=VERSION,
-      description='tools',
+      description='A handy ETL&GEOM kit',
       long_description=README,
       long_description_content_type="text/markdown",
       author="Ricco Wang",
       author_email="wyk_0610@163.com",
       packages=find_packages('src'),
       package_dir={'': 'src'},
       platforms='any',
```

### Comparing `ricco-1.0.0/src/ricco/coord_trans.py` & `ricco-1.1.0/src/ricco/util/coord_trans.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 from shapely import wkt
 from shapely.geometry import LineString
 from shapely.geometry import Point
 from shapely.geometry.base import BaseGeometry
 from shapely.geometry.base import BaseMultipartGeometry
 from shapely.ops import transform as sh_transform
 
+"""
+Dependencies:
+
+pyproj==2.3.1
+pandas==0.24.2
+shapely[vectorized]==1.7a1
+geojson==2.5.0
+"""
+
 __all__ = ['wgs2gcj', 'gcj2wgs', 'gcj2wgs_exact', 'distance', 'gcj2bd',
            'bd2gcj', 'wgs2bd', 'bd2wgs']
 
 earthR = 6378245.0
 x_pi = math.pi * 3000.0 / 180.0
 LNG_CHINA_RANGE = (72.004, 137.8347)
 LAT_CHINA_RANGE = (0.8293, 55.8271)
@@ -305,49 +314,68 @@
   Returns:
     转换后的shapely Geometry
   """
   return sh_transform(
       lambda x, y, z=None: coord_transform(x, y, from_srs, to_srs), geo)
 
 
+def lnglat_check(df):
+  """检查列名"""
+  if ('lng' not in df.columns) | ('lng' not in df.columns):
+    raise KeyError('经纬度列名必须为lng和lat')
+
+
 def coord_trans_x2y(df_org, srs_from: (SRS, str), srs_to: (SRS, str)):
   """
   坐标批量转换工具
 
   :param df_org: 输入的dataframe，经纬度为lng和lat
   :param srs_from: 当前坐标系，可选'wgs84', 'bd09', 'gcj02'
   :param srs_to: 要转的坐标系，可选'wgs84', 'bd09', 'gcj02'
   :return:
   """
 
   def fn(row):
     return coord_transform(row['lng'], row['lat'], srs_from, srs_to)
 
+  lnglat_check(df_org)
   df_org['lng'] = df_org['lng'].astype(float)
   df_org['lat'] = df_org['lat'].astype(float)
   df_org[['lng', 'lat']] = df_org.apply(fn, axis=1, result_type='expand')
   print('坐标转换完成：%s → %s' % (srs_from, srs_to))
   return df_org
 
 
+def BD2WGS(df_org):
+  """百度转WGS84"""
+  df_org = coord_trans_x2y(df_org, SRS.bd09, SRS.wgs84)
+  return df_org
+
+
+def GD2WGS(df_org):
+  """高德转WGS84"""
+  df_org = coord_trans_x2y(df_org, SRS.gcj02, SRS.wgs84)
+  return df_org
+
+
 def coord_trans_geom(df_org, srs_from: (SRS, str), srs_to: (SRS, str)):
   """
   坐标批量转换工具geometry
 
   :param df_org: 输入的dataframe，必须要有geometry列
   :param srs_from: 当前坐标系，可选'wgs84', 'bd09', 'gcj02'
   :param srs_to: 要转的坐标系，可选'wgs84', 'bd09', 'gcj02'
   :return:
   """
-  from ricco.geom import wkb_dumps
-  from ricco.geom import wkb_loads
+  from .geom import wkb_dumps
+  from .geom import wkb_loads
   if 'geometry' not in df_org.columns:
     raise KeyError('必须有geometry列')
   df_org['geometry'] = df_org['geometry'].apply(
-      lambda x: wkb_dumps(coord_transform_geometry(
-          wkb_loads(x, hex=True),
-          srs_from,
-          srs_to),
+      lambda x: wkb_dumps(
+          coord_transform_geometry(wkb_loads(x, hex=True),
+                                   srs_from,
+                                   srs_to),
           hex=True,
           srid=4326))
   print(f'坐标转换：{srs_from} --> {srs_to}')
   return df_org
```

### Comparing `ricco-1.0.0/src/ricco/dt.py` & `ricco-1.1.0/src/ricco/util/dt.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,7 +58,38 @@
       return _date
     elif date_type in ('date', 'datetime'):
       return datetime.strptime(_date, '%Y-%m-%d')
     else:
       raise ValueError('date_type参数错误，可选参数为str或date')
   else:
     return _date
+
+
+class DT:
+  # TODO(wangyukang): 补充日期方法
+  @property
+  def today(self):
+    return
+
+  @property
+  def tomorrow(self):
+    return
+
+  @property
+  def yesterday(self):
+    return
+
+  @property
+  def the_day_after_tomorrow(self):
+    return
+
+  @property
+  def the_day_before_yesterday(self):
+    return
+
+  @property
+  def one_year_ago(self):
+    return
+
+  @property
+  def d(self):
+    return
```

### Comparing `ricco-1.0.0/src/ricco/etl/extract.py` & `ricco-1.1.0/src/ricco/etl/extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import csv
+import os
 import warnings
 
 import geopandas as gpd
 import pandas as pd
 
-from ..os import ext
+from ..util.os import ext
 
 
 def max_grid():
   """防止单个单元格文件过大而报错"""
   import sys
   maxint = sys.maxsize
   decrement = True
@@ -17,27 +18,33 @@
     try:
       csv.field_size_limit(maxint)
     except OverflowError:
       maxint = int(maxint / 10)
       decrement = True
 
 
-def rdxls(filename, sheet_name=0, sheet_contains: str = None, errors='raise'):
+def rdxls(
+    filename,
+    sheet_name=0,
+    sheet_contains: str = None,
+    errors='raise',
+    dtype=None,
+) -> pd.DataFrame:
   """
   读取excel文件
 
   :param filename: 文件名
   :param sheet_name: sheet表的名称
   :param sheet_contains: sheet表包含的字符串
   :param errors: 当没有对应sheet时，raise: 抛出错误, coerce: 返回空的dataframe
   :return:
   """
   if sheet_name == 0:
     if sheet_contains is not None:
-      df = pd.read_excel(filename, sheet_name=None)
+      df = pd.read_excel(filename, sheet_name=None, dtype=dtype)
       sheet_list = [i for i in df.keys() if sheet_contains in i]
       if len(sheet_list) != 0:
         sheet_name = sheet_list[0]
         if len(sheet_list) == 1:
           print(f"sheet:  <'{sheet_name}'>")
         elif len(sheet_list) >= 2:
           warnings.warn(
@@ -49,76 +56,100 @@
           return pd.DataFrame()
         elif errors == 'raise':
           raise ValueError(f'没有包含{sheet_contains}的sheet，请检查')
         else:
           raise KeyError("参数'error'错误, 可选参数为coerce和raise")
   else:
     print(f"sheet:  <'{sheet_name}'>")
-  return pd.read_excel(filename, sheet_name=sheet_name)
+  return pd.read_excel(filename, sheet_name=sheet_name, dtype=dtype)
 
 
-def rdf(file_path: str,
-        sheet_name=0,
-        sheet_contains: str = None,
-        encoding='utf-8-sig',
-        info=False) -> pd.DataFrame:
+def rdf(
+    file_path: str,
+    *,
+    sheet_name=0,
+    sheet_contains: str = None,
+    encoding='utf-8-sig',
+    info=False,
+    dtype=None,
+) -> pd.DataFrame:
   """
-  常用文件读取函数，支持.csv/.xlsx/.shp
+  常用文件读取函数，支持.csv/.xlsx/.shp/.parquet/.pickle/.feather'
   """
   max_grid()
-
-  if ext(file_path) == '.csv':
+  ex = ext(file_path)
+  if ex == '.csv':
     try:
-      df = pd.read_csv(file_path, engine='python', encoding=encoding)
+      df = pd.read_csv(file_path,
+                       engine='python',
+                       encoding=encoding,
+                       dtype=dtype)
     except UnicodeDecodeError:
-      df = pd.read_csv(file_path, engine='python')
-  elif ext(file_path) in ('.xls', '.xlsx'):
-    df = rdxls(file_path, sheet_name=sheet_name, sheet_contains=sheet_contains)
-  elif ext(file_path) == '.shp':
+      df = pd.read_csv(file_path, engine='python', dtype=dtype)
+  elif ex in ('.parquet', '.pickle', '.feather'):
+    _t = ex.strip('.')
+    df = getattr(pd, f'read_{_t}')(
+        file_path
+    )
+  elif ex in ('.xls', '.xlsx'):
+    df = rdxls(file_path,
+               sheet_name=sheet_name,
+               sheet_contains=sheet_contains,
+               dtype=dtype)
+  elif ex == '.shp':
     try:
       df = gpd.GeoDataFrame.from_file(file_path)
     except UnicodeEncodeError:
       df = gpd.GeoDataFrame.from_file(file_path, encoding='GBK')
   else:
     raise Exception('未知文件格式')
   if info:
     print(f'shape: {df.shape}')
     print(f'columns: {df.columns}')
   return df
 
 
-def read_line_json(filename, encoding='utf-8'):
+def read_line_json(filename, encoding='utf-8') -> pd.DataFrame:
   """
-  逐行读取json格式的文件，目前用于金刚石数据读取
+  逐行读取json格式的文件
 
   :param filename: 文件名
   :param encoding: 文件编码，默认为utf-8
   :return:
   """
   import json
   records = []
   with open(filename, 'r', encoding=encoding) as file:
     for line in file:
       row = json.loads(line)
       records.append(row)
   return pd.DataFrame(records)
 
 
-def bigdata2df(filename: str, chunksize: int = 10000,
-               code: str = "utf-8") -> pd.DataFrame:
+def bigdata2df(filename: str,
+               chunksize: int = 10000,
+               code: str = 'utf-8') -> pd.DataFrame:
   reader = pd.read_table(filename,
                          encoding=code,
-                         sep=",",
+                         sep=',',
                          skip_blank_lines=True,
                          iterator=True)
   loop = True
   chunks = []
   while loop:
     try:
       chunk = reader.get_chunk(chunksize)
       chunk.dropna(axis=0, inplace=True)
       chunks.append(chunk)
     except StopIteration:
       loop = False
       print('Iteration is stopped.')
   df = pd.concat(chunks, ignore_index=True, axis=1)
   return df
+
+
+def read_parquet_by_dir(dir_path):
+  df = pd.DataFrame()
+  for filename in os.listdir(dir_path):
+    if ext(filename) == '.parquet':
+      df = pd.concat([df, rdf(os.path.join(dir_path, filename))])
+  return df
```

### Comparing `ricco-1.0.0/src/ricco/etl/file.py` & `ricco-1.1.0/src/ricco/etl/file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from tqdm import tqdm
 
+from ..util.os import fn
+from ..util.os import mkdir_2
 from .extract import rdf
-from ..os import mkdir_2
-from ..os import fn
 
 
 def split_csv(filename: str, n: int = 5, encoding: str = 'utf-8'):
   """将文件拆分为多个同名文件，放置在与文件同名文件夹下的不同Part_文件夹中"""
   dir_name = fn(os.path.basename(filename))
   abs_path = os.getcwd()
   df = rdf(filename)
```

### Comparing `ricco-1.0.0/src/ricco/etl/load.py` & `ricco-1.1.0/src/ricco/etl/load.py`

 * *Files identical despite different names*

### Comparing `ricco-1.0.0/src/ricco/geocode/amap.py` & `ricco-1.1.0/src/ricco/geocode/baidu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,124 @@
 import requests
 from fuzzywuzzy import fuzz
 
-from ricco.geocode.util import MapKeys
-from ricco.geocode.util import MapUrls
-from ricco.geocode.util import error_amap
-from ricco.geocode.util import gcj2xx
+from ..util.util import is_empty
+from .util import MapKeys
+from .util import MapUrls
+from .util import error_baidu
+from .util import fix_address
+from .util import gcj2xx
 
-KEY = MapKeys.amap
+KEY = MapKeys.baidu
 
 
 def address_json(city: str, address: str, key=None):
-  """高德地理编码接口"""
+  """百度地理编码接口"""
+  if is_empty(address):
+    return None
   if not key:
     key = KEY
-  url = f'{MapUrls.amap}?address={address}&city={city}&key={key}'
+  url = f'{MapUrls.baidu}?city={city}&address={address}&output=json&ak={key}&ret_coordtype=gcj02ll'
   js = requests.get(url).json()
-  error_amap(js)
-  if js['status'] == '1' and int(js['count']) >= 1:
-    return js['geocodes'][0]
+  error_baidu(js)
+  if js['status'] == 0:
+    return js['result']
   return None
 
 
 def place_json(city: str, keywords: str, key=None):
-  """高德地点检索接口"""
+  """百度地点检索接口"""
+  if is_empty(keywords):
+    return None
   if not key:
     key = KEY
-  url = f'{MapUrls.amap_poi}?keywords={keywords}&city={city}&key={key}'
+  url = f'{MapUrls.baidu_poi}?query={keywords}&region={city}&city_limit=true&output=json&ak={key}&ret_coordtype=gcj02ll'
   js = requests.get(url).json()
-  error_amap(js)
-  if js['status'] == '1' and int(js['count']) >= 1:
-    return js['pois'][0]
+  error_baidu(js)
+  if js['status'] == 0 and len(js['results']) >= 1:
+    return js['results'][0]
   return None
 
 
-def get_amap(*,
-             address,
-             city,
-             source,
-             with_detail=True,
-             disable_cache=False,
-             key=None):
+def get_baidu(*,
+              address,
+              city,
+              source,
+              disable_cache=False,
+              with_detail=True,
+              key=None):
   """脉策geocode服务"""
+  if is_empty(address):
+    return None
   url = f'{MapUrls.mdt}?address={address}&city={city}&disable_cache={disable_cache}&with_detail={with_detail}&source={source}'
   req = requests.get(url)
   if req.status_code == 200:
     return req.json()['result'][0]['extra']
   elif req.status_code in (400, 403):
-    if source == 'amap':
+    if source == 'baidu':
       return address_json(city=city, address=address, key=key)
-    elif source == 'amap_poi':
+    elif source == 'baidu_poi':
       return place_json(city=city, keywords=address, key=key)
     else:
       raise ValueError('source参数错误')
   else:
     return None
 
 
-def get_address_amap(city: str, address: str, srs: str = 'wgs84', key=None):
+def get_address_baidu(city: str, address: str, srs='wgs84', key=None):
+  if is_empty(address):
+    return {
+      'rv': None,
+      'score': 0,
+      'lng': None,
+      'lat': None,
+    }
   city = city.rstrip('市')
-  address = address.replace('|', '')
-  address_dict = get_amap(city=city, address=address, source='amap', key=key)
-  if address_dict:
-    rv = address_dict['formatted_address']
-    lnglat = address_dict['location'].split(',')
+  address = fix_address(address)
+  res = get_baidu(city=city, address=address, source='baidu', key=key)
+  if res:
+    lnglat = [res['location']['lng'], res['location']['lat']]
+    if res['precise'] == 1:
+      score = 100
+    else:
+      score = res.get('comprehension') if res.get('comprehension') else res.get(
+          'confidence')
     latlng = gcj2xx(lnglat, srs=srs)
     lng = latlng[1]
     lat = latlng[0]
   else:
-    rv, lng, lat = None, None, None
+    score, lng, lat = 0, None, None
   return {
-    'rv': rv,
-    'score': None,
+    'rv': None,
+    'score': score,
     'lng': lng,
     'lat': lat,
   }
 
 
-def get_place_amap(city: str, keywords: str, srs='wgs84', key=None):
+def get_place_baidu(city: str, keywords: str, srs='wgs84', key=None):
+  if is_empty(keywords):
+    return {
+      'rv': None,
+      'score': 0,
+      'lng': None,
+      'lat': None,
+    }
   city = city.rstrip('市')
-  res = get_amap(city=city, address=keywords, source='amap_poi', key=key)
+  keywords = fix_address(keywords)
+  res = get_baidu(city=city, address=keywords, source='baidu_poi', key=key)
   if res:
     rv = res['name']
-    lnglat = res['location'].split(',')
+    lnglat = [res['location']['lng'], res['location']['lat']]
     latlng = gcj2xx(lnglat, srs=srs)
     lng = latlng[1]
     lat = latlng[0]
     score = max(fuzz.ratio(rv, keywords.lstrip(city)),
                 fuzz.partial_ratio(rv, keywords.lstrip(city)))
   else:
     rv, lng, lat, score = None, None, None, 0
   return {
     'rv': rv,
     'score': score,
     'lng': lng,
     'lat': lat,
   }
-
-
-if __name__ == '__main__':
-  res = address_json('上海', '大同路922弄97号', key='111')
-  print(res)
```

### Comparing `ricco-1.0.0/src/ricco/geocode/geocode.py` & `ricco-1.1.0/src/ricco/geocode/geocode.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 import warnings
 
 import pandas as pd
 from requests.exceptions import ConnectionError
 from requests.exceptions import ConnectTimeout
 from tqdm import tqdm
 
-from ricco.geocode.amap import get_address_amap
-from ricco.geocode.amap import get_place_amap
-from ricco.geocode.baidu import get_address_baidu
-from ricco.geocode.baidu import get_place_baidu
+from ..util.util import is_empty
+from .amap import get_address_amap
+from .amap import get_place_amap
+from .baidu import get_address_baidu
+from .baidu import get_place_baidu
 
 
-def geocode(*, address, city, source, srs='wgs84', key_baidu=None,
+def geocode(*,
+            address,
+            city,
+            source,
+            srs='wgs84',
+            key_baidu=None,
             key_amap=None):
   """
   Args:
       address: 地址或项目名称关键词
       city: 城市
       source: 接口选择。baidu/amap：百度或高德的地理编码接口，baidu_poi/amap_poi：百度或高德的地点检索接口
       srs: 返回的坐标系，可选wgs84, bd09, gcj02，默认wgs84
@@ -49,14 +55,16 @@
       keywords: POI名称
       sig: 解析结果相似度，默认为80，范围0-100
       address_geocode: 是否使用地理编码补全，默认False
       srs: 返回的坐标系，可选wgs84, bd09, gcj02，默认wgs84
       key_baidu: 百度接口的key，公共key失效后可自行传入
       key_amap: 高德接口的key，公共key失效后可自行传入
   """
+  if is_empty(keywords):
+    return None, None, None, None, None
   res = {
     'lng': None,
     'lat': None,
     'rv': None,
     'score': None,
   }
   source = None
@@ -83,14 +91,16 @@
     warnings.warn(f'接口超时，【{city}】：【{keywords}】,{e}')
     return None, None, None, None, None
 
 
 def geocode_best_address(city, address, srs='wgs84', key_baidu=None,
                          key_amap=None):
   """获取最优的地理编码结果"""
+  if is_empty(address):
+    return None, None, None, None, None
   try:
     br = get_address_baidu(city, address, srs=srs, key=key_baidu)
     if br['score'] >= 90:
       res, source = br, 'baidu_geocode'
     else:
       ar = get_address_amap(city, address, srs=srs, key=key_amap)
       res, source = ar, 'amap_geocode'
```

### Comparing `ricco-1.0.0/src/ricco/geocode/util.py` & `ricco-1.1.0/src/ricco/geocode/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
-from ricco.coord_trans import gcj2bd
-from ricco.coord_trans import gcj2wgs
+from ..util.coord_trans import gcj2bd
+from ..util.coord_trans import gcj2wgs
+from ..util.util import is_empty
 
 
 class MapUrls:
   # 百度地理编码
   baidu = 'http://api.map.baidu.com/geocoding/v3/'
   # 百度地点检索
   baidu_poi = 'http://api.map.baidu.com/place/v2/search'
@@ -14,16 +15,16 @@
   # 高德地点检索
   amap_poi = 'https://restapi.amap.com/v3/place/text'
   # 脉策geocode服务
   mdt = 'https://geocode.idatatlas.com/geocode'
 
 
 class MapKeys:
-  amap = '2cc433cc0b5e0a737d50800bc2d6eb42'
-  baidu = 'M40WZd3qdNYtRSdyRu3IMAtzpH14kgs4'
+  amap = '7c14855824549a84c543e48990239f3d'
+  baidu = '9Fy1lMHbwpr07WVBFPLw9vpntGUSOUMN'
 
 
 def gcj2xx(lnglat, srs):
   if srs == 'wgs84':
     return gcj2wgs(float(lnglat[1]), float(lnglat[0]))
   elif srs == 'bd09':
     return gcj2bd(float(lnglat[1]), float(lnglat[0]))
@@ -44,7 +45,13 @@
 
 def error_amap(js):
   if js['status'] != '1':
     warnings.warn(
         '接口错误，状态码【%s】，错误原因请查阅：'
         'https://lbs.amap.com/api/webservice/guide/tools/info' % js['infocode']
     )
+
+
+def fix_address(string):
+  if is_empty(string):
+    return ''
+  return str(string)
```

### Comparing `ricco-1.0.0/src/ricco/geom.py` & `ricco-1.1.0/src/ricco/util/geom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,109 @@
+import json
 import logging
 import warnings
 
+import geojson
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from shapely import wkb
 from shapely import wkt
+from shapely.errors import GeometryTypeError
 from shapely.errors import ShapelyDeprecationWarning
 from shapely.errors import WKBReadingError
+from shapely.geometry import LinearRing
+from shapely.geometry import LineString
+from shapely.geometry import MultiLineString
+from shapely.geometry import MultiPoint
+from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
+from shapely.geometry import shape
 from shapely.geos import WKTReadingError
+from simplejson.errors import JSONDecodeError
 
-from ricco.util import ensure_list
-from ricco.util import first_notnull_value
+from ..util.util import ensure_list
+from ..util.util import first_notnull_value
 
 warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
 
-
-def get_epsg(city):
-  """
-  查找citycode，用于投影
-  """
-  from ricco.config import EPSG_CODE
-  if city in EPSG_CODE.keys():
-    return EPSG_CODE[city]
+GeomTypeSet = (
+  Point, MultiPoint,
+  Polygon, MultiPolygon,
+  LineString, MultiLineString,
+  LinearRing
+)
+
+
+class GeomFormat:
+  wkb = 'wkb'
+  wkt = 'wkt'
+  shapely = 'shapely'
+  geojson = 'geojson'
+  unknown = 'unknown'
+
+
+def crs_sh2000():
+  """测绘院（上海2000）crs信息"""
+  from ..resource.crs import CRS_SH2000
+  return CRS_SH2000
+
+
+def get_epsg_by_lng(lng):
+  """通过经度获取epsg代码"""
+  lng_epsg_mapping = {
+    # 中央经线和epsg代码的对应关系
+    75: 4534, 78: 4535, 81: 4536, 84: 4537, 87: 4538,
+    90: 4539, 93: 4540, 96: 4541, 99: 4542,
+    102: 4543, 105: 4544, 108: 4545, 111: 4546,
+    114: 4547, 117: 4548, 120: 4549, 123: 4550,
+    126: 4551, 129: 4552, 132: 4553, 135: 4554,
+  }
+  lng = np.median(lng)
+  key = min(lng_epsg_mapping.keys(), key=lambda x: abs(x - lng))
+  return lng_epsg_mapping.get(key)
+
+
+def get_lng_by_city(city: str):
+  from ..resource.epsg_code import CITY_POINT
+  if city in CITY_POINT.keys():
+    return CITY_POINT[city]['lng']
   else:
-    city = city + '市'
-    if city in EPSG_CODE.keys():
-      return EPSG_CODE[city]
+    city += '市'
+    if city in CITY_POINT.keys():
+      return CITY_POINT[city]['lng']
     else:
-      warnings.warn(
-          "获取城市epsg失败，当前默认为32651。请在config.py中补充该城市")
-      return 32651
+      warnings.warn(f'请补充{city}的epsg信息，默认返回经度120')
+      return 120
 
 
-def projection(gdf, proj_epsg: int = None, city: str = None):
-  if not proj_epsg:
-    if not city:
-      raise ValueError(
-          '获取投影信息失败，请补充参数:proj_epsg投影的坐标系统的epsg编号或city中国城市名称')
+def get_epsg(city: str):
+  """根据城市查询epsg代码，用于投影"""
+  return get_epsg_by_lng(get_lng_by_city(city))
+
+
+def projection(
+    gdf: gpd.GeoDataFrame,
+    epsg: int = None,
+    city: str = None):
+  """投影变换"""
+  if not epsg:
+    if city:
+      epsg = get_epsg(city)
     else:
-      proj_epsg = get_epsg(city)
-  return gdf.to_crs(epsg=proj_epsg)
+      lngs = gdf['geometry'].centroid.x.tolist()
+      epsg = get_epsg_by_lng(lngs)
+  return gdf.to_crs(epsg=epsg)
+
+
+def projection_lnglat(lnglat, crs_from, crs_to):
+  from pyproj import Transformer
+  transformer = Transformer.from_crs(crs_from, crs_to)
+  return transformer.transform(xx=lnglat[1], yy=lnglat[0])
 
 
 def wkb_loads(x, hex=True):
   warnings.filterwarnings('ignore',
                           'Geometry column does not contain geometry.',
                           UserWarning)
 
@@ -55,15 +112,15 @@
 
   try:
     return wkb.loads(x, hex=hex)
   except (AttributeError, WKBReadingError):
     return None
 
 
-def wkb_dumps(x, hex=True, srid=4326):
+def wkb_dumps(x, hex=True, srid=4326) -> (str, None):
   if pd.isna(x):
     return None
 
   try:
     return wkb.dumps(x, hex=hex, srid=srid)
   except AttributeError:
     return None
@@ -74,23 +131,130 @@
     return None
   try:
     return wkt.loads(x)
   except (AttributeError, WKTReadingError):
     return None
 
 
-def wkt_dumps(x):
+def wkt_dumps(x) -> (str, None):
   if pd.isna(x):
     return None
   try:
     return wkt.dumps(x)
   except AttributeError:
     return None
 
 
+def geojson_loads(x):
+  """geojson文本形式转为shapely格式"""
+  if pd.isna(x):
+    return None
+  try:
+    geom = shape(geojson.loads(x))
+    if geom.is_empty:
+      return None
+    return geom
+  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError):
+    return None
+
+
+def geojson_dumps(x) -> (str, None):
+  """shapely转为geojson文本格式"""
+  if pd.isna(x):
+    return None
+  try:
+    geom = geojson.Feature(geometry=x)
+    return json.dumps(geom.geometry)
+  except TypeError:
+    return None
+
+
+def is_shapely(x, na=False) -> bool:
+  """判断是否为shapely格式"""
+  if pd.isna(x):
+    return na
+  if type(x) in GeomTypeSet:
+    return True
+  else:
+    return False
+
+
+def is_wkb(x, na=False) -> bool:
+  """判断是否为wkb格式"""
+  if pd.isna(x):
+    return na
+  try:
+    wkb.loads(x, hex=True)
+    return True
+  except WKBReadingError:
+    return False
+
+
+def is_wkt(x, na=False) -> bool:
+  """判断是否为wkt格式"""
+  if pd.isna(x):
+    return na
+  try:
+    wkt.loads(x)
+    return True
+  except WKTReadingError:
+    return False
+
+
+def is_geojson(x, na=False) -> bool:
+  """判断是否为geojson格式"""
+  if pd.isna(x):
+    return na
+  try:
+    if shape(geojson.loads(x)).is_empty:
+      return False
+    return True
+  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError):
+    return False
+
+
+def infer_geom_format(x):
+  """推断geometry格式"""
+  if is_shapely(x):
+    return GeomFormat.shapely
+  if is_wkb(x):
+    return GeomFormat.wkb
+  if is_wkt(x):
+    return GeomFormat.wkt
+  if is_geojson(x):
+    return GeomFormat.geojson
+  return GeomFormat.unknown
+
+
+def ensure_multi_geom(geom):
+  """将LineString和Polygon转为multi格式"""
+  if geom.geom_type == 'LineString':
+    return MultiLineString([geom])
+  if geom.geom_type == 'Polygon':
+    return MultiPolygon([geom])
+  return geom
+
+
+def multiline2multipolygon(multiline_shapely):
+  """multiline转为multipolygon，直接首尾相连"""
+  coords = []
+  for line in multiline_shapely:
+    lngs = line.xy[0]
+    lats = line.xy[1]
+    for i in range(len(lngs)):
+      lng, lat = lngs[i], lats[i]
+      point = Point((lng, lat))
+      if len(coords) >= 1:
+        if point != coords[-1]:
+          coords.append(point)
+      else:
+        coords.append(point)
+  return MultiPolygon([Polygon(coords)])
+
+
 def geom_wkt2shapely(df, geometry='geometry',
                      epsg_code: int = 4326) -> gpd.GeoDataFrame:
   """wkt转gpd"""
   df[geometry] = df[geometry].apply(wkt_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
@@ -264,62 +428,14 @@
                      predicate='intersects').drop('index_right', axis=1)
 
   # 将geometry转为wkb格式
   df_res['geometry'] = df_res['geometry'].apply(wkb_dumps)
   return df_res
 
 
-def is_shapely(x, na=False):
-  from shapely.geometry import Point
-  from shapely.geometry import MultiPoint
-  from shapely.geometry import Polygon
-  from shapely.geometry import MultiPolygon
-  from shapely.geometry import LineString
-  from shapely.geometry import MultiLineString
-  from shapely.geometry import LinearRing
-
-  geom_type_set = (
-    Point, MultiPoint,
-    Polygon, MultiPolygon,
-    LineString, MultiLineString,
-    LinearRing
-  )
-  if pd.isna(x):
-    return na
-  if type(x) in geom_type_set:
-    return True
-  else:
-    return False
-
-
-def is_geojson(x, na=False):
-  # TODO(wangyukang): 未来考虑支持geojson格式
-  pass
-
-
-def infer_geom_format(x):
-  if is_shapely(x):
-    return 'shapely'
-  if isinstance(x, str):
-    # 尝试是否能成功转为wkb格式
-    try:
-      wkb.loads(x, hex=True)
-      return 'wkb'
-    except WKBReadingError:
-      pass
-    # 尝试是否能成功转为wkt格式
-    try:
-      wkt.loads(x)
-      return 'wkt'
-    except WKTReadingError:
-      pass
-  # TODO(wangyukang): 未来考虑支持geojson格式
-  return 'unknown'
-
-
 def ensure_gdf(df, geometry='geometry'):
   geom = first_notnull_value(df[geometry])
   geom_format = infer_geom_format(geom)
   if geom_format == 'wkb':
     return geom_wkb2shapely(df, geometry=geometry)
   elif geom_format == 'wkt':
     return geom_wkt2shapely(df, geometry=geometry)
@@ -333,15 +449,15 @@
     point_df: pd.DataFrame,
     polygon_df: pd.DataFrame,
     col_list: list = None,
     predicate='intersects',
     drop_geometry=False,
     geometry_format='wkb'):
   """
-  使用面数据给点数据打标签
+  使用面数据通过空间关联（sjoin）给点数据打标签
 
   Args:
       point_df: 点数据
       polygon_df: 面数据
       col_list: 面数据中要关联到结果中的列，若为空则全部关联
       predicate: 关联方法，默认'intersects'
       drop_geometry: 结果是否删除geometry，默认删除
@@ -396,42 +512,47 @@
       pass
     else:
       raise ValueError('不支持的geometry格式')
 
   return pd.DataFrame(point_df)
 
 
-def dis_point2point(lnglat_ori: (tuple, str),
-                    lnglat_dis: (tuple, str),
-                    city: str,
-                    crs_from: int = 4326,
-                    crs_to: (str, int) = 'auto'):
-  """
-  计算两个点（经度，纬度）之间的距离，单位：米
-
-  example:
+def ensure_lnglat(lnglat) -> tuple:
+  if isinstance(lnglat, (list, tuple)):
+    if all([isinstance(i, (float, int)) for i in lnglat]):
+      return lnglat
+    else:
+      raise TypeError('数据类型错误，经度和纬度都应该为数值型')
+  if is_shapely(lnglat):
+    geom = lnglat
+  elif is_wkt(lnglat):
+    geom = wkt_loads(lnglat)
+  elif is_wkb(lnglat):
+    geom = wkb_loads(lnglat)
+  elif is_geojson(lnglat):
+    geom = geojson_loads(lnglat)
+  else:
+    raise ValueError('未知的地理类型')
+  return (geom.x, geom.y)
 
-  >>> dis_point2point((121.579051,31.3402), (121.581099,31.342405), '上海市')
-  >>> 312.6011508211181
 
-  :param lnglat_ori: 经纬度或wkb
-  :param lnglat_dis: 经纬度或wkb
-  :param city: 城市
-  :param crs_from: 原始epsg，默认为4326
-  :param crs_to: 投影epsg，默认为'auto',按城市自动获取
-  :return:
+def distance(
+    p1: (tuple, str),
+    p2: (tuple, str),
+    city: str = None,
+    epsg_from: int = 4326,
+    epsg_to: (str, int) = None):
   """
-  # TODO(wangyukang): 目前会有性能问题，需优化
-  from pyproj import Transformer
-  from shapely.geometry import Point
-  if crs_to == 'auto':
-    crs_to = get_epsg(city)
-  if isinstance(lnglat_ori, str):
-    geom = wkb_loads(lnglat_ori)
-    lnglat_ori = (geom.x, geom.y)
-  if isinstance(lnglat_dis, str):
-    geom = wkb_loads(lnglat_dis)
-    lnglat_dis = (geom.x, geom.y)
-  transformer = Transformer.from_crs(crs_from, crs_to)
-  xy1 = transformer.transform(xx=lnglat_ori[1], yy=lnglat_ori[0])
-  xy2 = transformer.transform(xx=lnglat_dis[1], yy=lnglat_dis[0])
-  return Point(xy1).distance(Point(xy2))
+  计算两个点（经度，纬度）之间的距离，单位：米
+  Args:
+    p1: 点位1，经纬度或geometry
+    p2: 点位2，经纬度或geometry
+    city: 所在城市，用于投影
+    epsg_from: epsg代码
+    epsg_to: 投影epsg代码
+  """
+  p1, p2 = ensure_lnglat(p1), ensure_lnglat(p2)
+  if not epsg_to:
+    epsg_to = get_epsg(city) if city else get_epsg_by_lng([p1[0], p2[0]])
+  p1 = projection_lnglat(p1, epsg_from, epsg_to)
+  p2 = projection_lnglat(p2, epsg_from, epsg_to)
+  return Point(p1).distance(Point(p2))
```

### Comparing `ricco-1.0.0/src/ricco.egg-info/PKG-INFO` & `ricco-1.1.0/src/ricco.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.0.0
-Summary: tools
+Version: 1.1.0
+Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

