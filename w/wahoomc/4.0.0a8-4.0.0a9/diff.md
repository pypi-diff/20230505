# Comparing `tmp/wahoomc-4.0.0a8.tar.gz` & `tmp/wahoomc-4.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wahoomc-4.0.0a8.tar", last modified: Sun Apr  2 17:42:50 2023, max compression
+gzip compressed data, was "wahoomc-4.0.0a9.tar", last modified: Sun Apr  2 17:46:28 2023, max compression
```

## Comparing `wahoomc-4.0.0a8.tar` & `wahoomc-4.0.0a9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.184610 wahoomc-4.0.0a8/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-04-02 17:42:50.184701 wahoomc-4.0.0a8/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/README.md
--rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/pyproject.toml
--rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-04-02 17:42:50.185070 wahoomc-4.0.0a8/setup.cfg
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.171728 wahoomc-4.0.0a8/tests/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.0a8/tests/test_cli.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-04-01 12:11:17.000000 wahoomc-4.0.0a8/tests/test_constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5493 2023-04-02 09:13:20.000000 wahoomc-4.0.0a8/tests/test_constants_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-04-01 20:49:53.000000 wahoomc-4.0.0a8/tests/test_downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-04-01 12:11:17.000000 wahoomc-4.0.0a8/tests/test_generated_files.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6749 2023-04-02 09:13:20.000000 wahoomc-4.0.0a8/tests/test_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7726 2023-04-02 17:41:23.000000 wahoomc-4.0.0a8/tests/test_osm_maps.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.0a8/tests/test_setup.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.174756 wahoomc-4.0.0a8/wahoomc/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.0a8/wahoomc/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-04-01 12:11:17.000000 wahoomc-4.0.0a8/wahoomc/constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-04-01 12:11:17.000000 wahoomc-4.0.0a8/wahoomc/constants_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    12624 2023-04-02 08:07:59.000000 wahoomc-4.0.0a8/wahoomc/downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6373 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/file_directory_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    18349 2023-04-02 09:13:20.000000 wahoomc-4.0.0a8/wahoomc/geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4567 2023-04-02 09:13:20.000000 wahoomc-4.0.0a8/wahoomc/geofabrik_json.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.175656 wahoomc-4.0.0a8/wahoomc/init/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.0a8/wahoomc/init/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.0a8/wahoomc/init/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    17116 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/input.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3418 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/main.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    38747 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/osm_maps_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.176844 wahoomc-4.0.0a8/wahoomc/resources/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/resources/sea.osm
--rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/resources/shape2osm.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.177224 wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_adjusted/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     9515 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.178018 wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_initial/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779     2282 2023-03-27 20:10:10.000000 wahoomc-4.0.0a8/wahoomc/resources/tags-to-keep.json
--rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.0a8/wahoomc/resources/tunnel-transform.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10445 2023-04-02 17:41:33.000000 wahoomc-4.0.0a8/wahoomc/setup_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.183856 wahoomc-4.0.0a8/wahoomc/tooling_win/
--rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/7za.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/7za.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/7zxa.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/lzma.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/osmconvert.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.0a8/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:42:50.175391 wahoomc-4.0.0a8/wahoomc.egg-info/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-04-02 17:42:50.000000 wahoomc-4.0.0a8/wahoomc.egg-info/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-04-02 17:42:50.000000 wahoomc-4.0.0a8/wahoomc.egg-info/SOURCES.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-04-02 17:42:50.000000 wahoomc-4.0.0a8/wahoomc.egg-info/dependency_links.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-04-02 17:42:50.000000 wahoomc-4.0.0a8/wahoomc.egg-info/top_level.txt
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.349439 wahoomc-4.0.0a9/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4296 2023-04-02 17:46:28.349529 wahoomc-4.0.0a9/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3755 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/README.md
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/pyproject.toml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-04-02 17:46:28.349898 wahoomc-4.0.0a9/setup.cfg
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.342668 wahoomc-4.0.0a9/tests/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.0a9/tests/test_cli.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/tests/test_constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5493 2023-04-02 09:13:20.000000 wahoomc-4.0.0a9/tests/test_constants_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-04-01 20:49:53.000000 wahoomc-4.0.0a9/tests/test_downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/tests/test_generated_files.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     8067 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/tests/test_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7069 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/tests/test_osm_maps.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/tests/test_setup.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.344904 wahoomc-4.0.0a9/wahoomc/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/wahoomc/constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/wahoomc/constants_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    12624 2023-04-02 08:07:59.000000 wahoomc-4.0.0a9/wahoomc/downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6299 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/file_directory_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    20267 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4567 2023-04-02 09:13:20.000000 wahoomc-4.0.0a9/wahoomc/geofabrik_json.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346004 wahoomc-4.0.0a9/wahoomc/init/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/init/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/init/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    17318 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/input.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3178 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/main.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    35409 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/osm_maps_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346634 wahoomc-4.0.0a9/wahoomc/resources/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/sea.osm
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/shape2osm.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346992 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6369 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.347221 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_initial/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     2282 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/resources/tags-to-keep.json
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.0a9/wahoomc/resources/tunnel-transform.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     8209 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/setup_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.349149 wahoomc-4.0.0a9/wahoomc/tooling_win/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7za.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7za.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7zxa.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/lzma.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.345729 wahoomc-4.0.0a9/wahoomc.egg-info/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4296 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/SOURCES.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/dependency_links.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/top_level.txt
```

### Comparing `wahoomc-4.0.0a8/PKG-INFO` & `wahoomc-4.0.0a9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.0a8
+Version: 4.0.0a9
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,14 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
-* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
-
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a8 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a9 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
@@ -22,31 +22,30 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
-Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
-of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
-USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
-with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
-theme on your Wahoo to control what and in which zoom-level certain elements
-are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
-on-your-device-) ## Contribution / Questions You are welcome to provide input
-via Pull Requests, Issues or in any other way! If you have trouble using
-wahooMapsCreator, look into the FAQ, write an issue or join the telegram
-channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
-(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
-https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
-[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
-Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
-the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
-[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
-and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
-done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
-[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
-making this a little more public [@vti](https://github.com/vti) for creating a
-GUI application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
+tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
+[:computer: Preview your generated maps with cruiser ](docs/
+USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
+control what and in which zoom-level certain elements are rendered](docs/
+TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
+Contribution / Questions You are welcome to provide input via Pull Requests,
+Issues or in any other way! If you have trouble using wahooMapsCreator, look
+into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
+FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
+treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
+TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
+CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
+(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
+(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
+github.com/mweirauch) for bringing in new ideas, testing and using the tool
+[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
+(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
+/github.com/macdet) for bringing in new thoughts, testing and making this a
+little more public [@vti](https://github.com/vti) for creating a GUI
+application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a8/README.md` & `wahoomc-4.0.0a9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,14 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
-* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
-
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -14,31 +14,30 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
-Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
-of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
-USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
-with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
-theme on your Wahoo to control what and in which zoom-level certain elements
-are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
-on-your-device-) ## Contribution / Questions You are welcome to provide input
-via Pull Requests, Issues or in any other way! If you have trouble using
-wahooMapsCreator, look into the FAQ, write an issue or join the telegram
-channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
-(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
-https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
-[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
-Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
-the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
-[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
-and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
-done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
-[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
-making this a little more public [@vti](https://github.com/vti) for creating a
-GUI application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
+tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
+[:computer: Preview your generated maps with cruiser ](docs/
+USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
+control what and in which zoom-level certain elements are rendered](docs/
+TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
+Contribution / Questions You are welcome to provide input via Pull Requests,
+Issues or in any other way! If you have trouble using wahooMapsCreator, look
+into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
+FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
+treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
+TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
+CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
+(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
+(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
+github.com/mweirauch) for bringing in new ideas, testing and using the tool
+[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
+(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
+/github.com/macdet) for bringing in new thoughts, testing and making this a
+little more public [@vti](https://github.com/vti) for creating a GUI
+application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a8/setup.cfg` & `wahoomc-4.0.0a9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wahoomc
-version = 4.0.0a8
+version = 4.0.0a9
 author = Benjamin Kreuscher
 author_email = benni.kreuscher@gmail.com
 description = Create maps for your Wahoo bike computer based on latest OSM maps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/treee111/wahooMapsCreator
 project_urls =
```

### Comparing `wahoomc-4.0.0a8/tests/test_cli.py` & `wahoomc-4.0.0a9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/tests/test_constants.py` & `wahoomc-4.0.0a9/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/tests/test_constants_geofabrik.py` & `wahoomc-4.0.0a9/tests/test_constants_geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/tests/test_downloader.py` & `wahoomc-4.0.0a9/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/tests/test_generated_files.py` & `wahoomc-4.0.0a9/tests/test_generated_files.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/tests/test_osm_maps.py` & `wahoomc-4.0.0a9/tests/test_osm_maps.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 # import sys
 import unittest
 
 # import custom python packages
 from wahoomc.osm_maps_functions import OsmData
 from wahoomc.osm_maps_functions import OsmMaps
-from wahoomc.osm_maps_functions import get_xy_coordinates_from_input
 # from wahoomc.osm_maps_functions import TileNotFoundError
 from wahoomc.input import InputData
 from wahoomc import file_directory_functions as fd_fct
 from wahoomc import constants
 
 
 class TestOsmMapsCalculation(unittest.TestCase):
@@ -36,14 +35,21 @@
         # germany
         expected_result = {'czech-republic': {}, 'germany': {}, 'austria': {}, 'liechtenstein': {},
                            'switzerland': {}, 'italy': {}, 'netherlands': {}, 'belgium': {},
                            'luxembourg': {}, 'france': {}, 'poland': {}, 'denmark': {}, 'sweden': {}}
         self.process_and_check_border_countries(
             'germany', True, expected_result, 'country')
 
+        # germany,malta
+        expected_result = {'czech-republic': {}, 'germany': {}, 'austria': {}, 'liechtenstein': {},
+                           'switzerland': {}, 'italy': {}, 'netherlands': {}, 'belgium': {},
+                           'luxembourg': {}, 'france': {}, 'poland': {}, 'denmark': {}, 'sweden': {}, 'malta': {}}
+        self.process_and_check_border_countries(
+            'germany,malta', True, expected_result, 'country')
+
     def test_calc_border_countries_input_xy_coordinates_1tile(self):
         """
         Test initialized border countries
         - of a file with 1 tile and two countries
         """
 
         # one tile - france and germany
@@ -74,26 +80,34 @@
         self.process_and_check_border_countries(
             'germany', False, {'germany': {}}, 'country')
 
         # china
         self.process_and_check_border_countries(
             'china', False, {'china': {}}, 'country')
 
-    def test_calc_without_border_countries__xy_coordinates_1tile(self):
+        # malta,liechtenstein
+        self.process_and_check_border_countries(
+            'malta,liechtenstein', False, {'malta': {}, 'liechtenstein': {}}, 'country')
+
+        # malta,tunisia
+        self.process_and_check_border_countries(
+            'malta,tunisia', False, {'malta': {}, 'tunisia': {}}, 'country')
+
+    def test_calc_without_border_countries_xy_coordinates_1tile(self):
         """
         Test initialized countries without border countries
         - of one tile
         """
 
         # one tile - france and germany
         expected_result = {'france': {}, 'germany': {}}
         self.process_and_check_border_countries(
             "133/88", False, expected_result, 'xy_coordinate')
 
-    def test_calc_without_border_countries__xy_coordinates_2tiles(self):
+    def test_calc_without_border_countries_xy_coordinates_2tiles(self):
         """
         Test initialized countries without border countries
         - of two tiles
         """
 
         # two tiles - germany
         expected_result = {'germany': {}}
@@ -140,53 +154,14 @@
 
         o_osm_data = OsmData()
         o_osm_data.process_input_of_the_tool(o_input_data)
 
         result = o_osm_data.country_name
         self.assertEqual(result, 'malta')
 
-    def test_splitting_of_single_xy_coordinate(self):
-        """
-        use static json files in the repo to calculate relevant tiles
-        """
-
-        xy_tuple = get_xy_coordinates_from_input("133/88")
-        self.assertEqual(xy_tuple, [{"x": 133, "y": 88}])
-
-        xy_tuple = get_xy_coordinates_from_input("11/92")
-        self.assertEqual(xy_tuple, [{"x": 11, "y": 92}])
-
-        xy_tuple = get_xy_coordinates_from_input("138/100")
-        self.assertEqual(xy_tuple, [{"x": 138, "y": 100}])
-
-    def test_splitting_of_multiple_xy_coordinate(self):
-        """
-        use static json files in the repo to calculate relevant tiles
-        """
-
-        xy_tuple = get_xy_coordinates_from_input("133/88,138/100")
-        expected_result = [{"x": 133, "y": 88}, {"x": 138, "y": 100}]
-
-        self.assertEqual(xy_tuple, expected_result)
-
-    # def test_get_tile_via_xy_coordinate_error(self):
-    #     """
-    #     use static json files in the repo to calculate a not-existing tile.
-
-    #     does not error out due to new Geofabrik Json processing. Nevertheless, the tile is not existing
-    #     only +/- 180 -/+90: https://epsg.io/4326
-    #     """
-
-    #     o_geofabrik = XYGeofabrik([{"x": 200, "y": 1}])
-
-    #     # tiles =
-
-    #     with self.assertRaises(TileNotFoundError):
-    #         o_geofabrik.get_tiles_of_wanted_map()
-
     def test_encoding_open_sea_osm(self):
         """
         use static json files in the repo to calculate relevant tile
         """
 
         with open(os.path.join(constants.RESOURCES_DIR, 'sea.osm')) as sea_file:  # pylint: disable=unspecified-encoding
             sea_data_no_encoding = sea_file.read()
```

### Comparing `wahoomc-4.0.0a8/tests/test_setup.py` & `wahoomc-4.0.0a9/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/constants.py` & `wahoomc-4.0.0a9/wahoomc/constants.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/constants_functions.py` & `wahoomc-4.0.0a9/wahoomc/constants_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/downloader.py` & `wahoomc-4.0.0a9/wahoomc/downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/file_directory_functions.py` & `wahoomc-4.0.0a9/wahoomc/file_directory_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,19 @@
     return tiles_from_json
 
 
 def read_json_file_generic(json_file_path):
     """
     reads content of given .json file
     """
-    try:
-        with open(json_file_path, encoding="utf-8") as json_file:
-            json_content = json.load(json_file)
-            json_file.close()
+    with open(json_file_path, encoding="utf-8") as json_file:
+        json_content = json.load(json_file)
+        json_file.close()
 
-        return json_content
-
-    except FileNotFoundError:
-        return {}
+    return json_content
 
 
 def write_json_file_generic(json_file_path, json_content):
     """
     writes content to .json file
     """
     # Serializing json
```

### Comparing `wahoomc-4.0.0a8/wahoomc/geofabrik.py` & `wahoomc-4.0.0a9/wahoomc/geofabrik.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,74 +4,94 @@
 #!/usr/bin/python
 # pylint: skip-file
 
 # import official python packages
 import sys
 import math
 import logging
-import geojson
 from shapely.geometry import Polygon, shape
 
 # import custom python packages
-from wahoomc.constants import GEOFABRIK_PATH
 from wahoomc.constants import special_regions, block_download
 from wahoomc.geofabrik_json import GeofabrikJson
 
 log = logging.getLogger('main-logger')
 
 
 class InformalGeofabrikInterface:
-    wanted_map = ''
+    """Informal class for Geofabrik processing"""
+    wanted_maps = []
     tiles = []
     border_countries = {}
     output = {}
 
     o_geofabrik_json = None
 
-    def get_tiles_of_wanted_map(self) -> str:
-        """Get the relevant tiles for the wanted country or X/Y coordinate"""
+    def get_tiles_of_wanted_map_single(self, wanted_map) -> str:
+        """Get the relevant tiles for ONE wanted country or X/Y coordinate"""
         pass
 
+    def get_tiles_of_wanted_map(self) -> list:
+        """
+        calculates tiles of all input wanted-maps
+        :returns: list of tiles
+        """
+
+        tiles_of_input = []
+
+        for country in self.wanted_maps:
+            tiles_of_input.extend(self.get_tiles_of_wanted_map_single(country))
+
+        return tiles_of_input
+
     def find_needed_countries(self, bbox_tiles, wanted_map, wanted_region_polygon) -> dict:
         """find needed countries for requested country or X/Y combination"""
         pass
 
-    def compose_bouding_box(self, input) -> dict:
+    def compose_bouding_box(self, bounds) -> dict:
         """calculate bounding box based on geometry or X/Y combination"""
         pass
 
 
 class CountryGeofabrik(InformalGeofabrikInterface):
     """Geofabrik processing for countries"""
 
-    def __init__(self, input):
+    def __init__(self, input_countries):
+        """
+        :param input: string with countries: 'malta' or 'malta, switzerland'
+        :returns: object for country geofabrik processing
+        """
         self.o_geofabrik_json = GeofabrikJson()
+        self.wanted_maps = []
 
-        # get geofabrik country
-        self.wanted_map = self.o_geofabrik_json.translate_id_no_to_geofabrik(
-            input)
+        # input parameters
+        input_countries = get_countries_from_input(input_countries)
 
-    def get_tiles_of_wanted_map(self):
-        """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map()"""
+        for country in input_countries:
+            self.wanted_maps.append(self.o_geofabrik_json.translate_id_no_to_geofabrik(
+                country))
+
+    def get_tiles_of_wanted_map_single(self, wanted_map):
+        """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map_single()"""
         # Check if wanted_map is in the json file and if so get the polygon (shape)
         wanted_map_geom = self.o_geofabrik_json.get_geofabrik_geometry(
-            self.wanted_map)
+            wanted_map)
 
         # convert to shape (multipolygon)
         wanted_region = shape(wanted_map_geom)
 
         # calc bounding box - the whole area to be created
         bbox = self.compose_bouding_box(wanted_region.bounds)
 
         # Build bounding box list of tiles - several X/Y combinations making up the area
         bbox_tiles = calc_bounding_box_tiles(bbox)
 
         # get all infos of these bounding box tiles
         tiles_of_input = self.find_needed_countries(
-            bbox_tiles, self.wanted_map, wanted_region)
+            bbox_tiles, wanted_map, wanted_region)
 
         return tiles_of_input
 
     def find_needed_countries(self, bbox_tiles, wanted_map, wanted_region_polygon) -> list:
         """Overrides InformalGeofabrikInterface.find_needed_countries()"""
         output = []
 
@@ -231,37 +251,38 @@
 
         return {'top_x': top_x, 'top_y': top_y, 'bot_x': bot_x, 'bot_y': bot_y}
 
 
 class XYGeofabrik(InformalGeofabrikInterface):
     """Geofabrik processing for X/Y coordinates"""
 
-    def __init__(self, input):
+    def __init__(self, input_xy_coordinates):
+        """
+        :param input: string with xy-coordinates: 133/88 or 133/88,134/88
+        :returns: object for xy geofabrik processing
+        """
         self.o_geofabrik_json = GeofabrikJson()
 
-        # already splitted pairs of xy-coordinates
-        self.wanted_map = input
+        # use Geofabrik-URL to get the relevant tiles
+        self.wanted_maps = get_xy_coordinates_from_input(input_xy_coordinates)
 
-    def get_tiles_of_wanted_map(self) -> str:
-        """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map()"""
-        tiles_of_input = []
-        for xy_combination in self.wanted_map:
-
-            # calc bounding box - the whole area to be created
-            bbox = self.compose_bouding_box(xy_combination)
+    def get_tiles_of_wanted_map_single(self, wanted_map):
+        """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map_single()"""
+        # calc bounding box - the whole area to be created
+        bbox = self.compose_bouding_box(wanted_map)
 
-            # Build bounding box list of tiles - several X/Y combinations making up the area
-            bbox_tiles = calc_bounding_box_tiles(bbox)
+        # Build bounding box list of tiles - several X/Y combinations making up the area
+        bbox_tiles = calc_bounding_box_tiles(bbox)
 
-            # convert X/Y combination to shape (multipolygon)
-            wanted_region = self.compose_shape(bbox_tiles)
+        # convert X/Y combination to shape (multipolygon)
+        wanted_region = self.compose_shape(bbox_tiles)
 
-            # get all infos of these bounding box tiles
-            tiles_of_input.extend(self.find_needed_countries(
-                bbox_tiles, self.wanted_map, wanted_region))
+        # get all infos of these bounding box tiles
+        tiles_of_input = self.find_needed_countries(
+            bbox_tiles, wanted_map, wanted_region)
 
         return tiles_of_input
 
     def find_needed_countries(self, bbox_tiles, wanted_map, wanted_region_polygon) -> dict:
         """Overrides InformalGeofabrikInterface.find_needed_countries()"""
         output = []
 
@@ -336,16 +357,16 @@
 
         return {'top_x': xy_combination["x"], 'bot_x': xy_combination["x"],
                 'top_y': xy_combination["y"], 'bot_y': xy_combination["y"]}
 
     def compose_shape(self, bbox_tiles):
         coords = [(bbox_tiles[0]["tile_top"], bbox_tiles[0]["tile_left"]), (bbox_tiles[0]["tile_top"], bbox_tiles[0]["tile_right"]),
                   (bbox_tiles[0]["tile_bottom"], bbox_tiles[0]["tile_right"]), (bbox_tiles[0]["tile_bottom"], bbox_tiles[0]["tile_left"])]
-        p = Polygon(coords)
-        wanted_region = shape(p)
+        coords_polygon = Polygon(coords)
+        wanted_region = shape(coords_polygon)
         return wanted_region
 
 
 def calc_bounding_box_tiles(bbox):
     bbox_tiles = []
     for x_value in range(bbox['top_x'], bbox['bot_x'] + 1):
         for y_value in range(bbox['top_y'], bbox['bot_y'] + 1):
@@ -390,7 +411,43 @@
     Convert tile numbers to lon./lat.
     """
     n = 2.0 ** zoom
     lon_deg = xtile / n * 360.0 - 180.0
     lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * ytile / n)))
     lat_deg = math.degrees(lat_rad)
     return (lat_deg, lon_deg)
+
+
+def get_countries_from_input(input_countries):
+    """
+    extract/split x/y combinations by given X/Y coordinates.
+    input should be "188/88" or for multiple values "188/88,100/10,109/99".
+    returns a list of x/y combinations as integers
+    """
+
+    countries = []
+
+    # split by "," first for multiple x/y combinations, then by "/" for x and y value
+    for country in input_countries.split(","):
+        countries.append(country)
+
+    return countries
+
+
+def get_xy_coordinates_from_input(input_xy_coordinates):
+    """
+    extract/split x/y combinations by given X/Y coordinates.
+    input should be "188/88" or for multiple values "188/88,100/10,109/99".
+    returns a list of x/y combinations as integers
+    """
+
+    xy_combinations = []
+
+    # split by "," first for multiple x/y combinations, then by "/" for x and y value
+    for xy_coordinate in input_xy_coordinates.split(","):
+        splitted = xy_coordinate.split("/")
+
+        if len(splitted) == 2:
+            xy_combinations.append(
+                {"x": int(splitted[0]), "y": int(splitted[1])})
+
+    return xy_combinations
```

### Comparing `wahoomc-4.0.0a8/wahoomc/geofabrik_json.py` & `wahoomc-4.0.0a9/wahoomc/geofabrik_json.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/input.py` & `wahoomc-4.0.0a9/wahoomc/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # for gui
 import tkinter as tk
 from tkinter import ttk
 
 # import custom python packages
 from wahoomc.geofabrik_json import GeofabrikJson
 from wahoomc.geofabrik_json import CountyIsNoGeofabrikCountry
+from wahoomc.geofabrik import get_countries_from_input
 
 
 def process_call_of_the_tool():
     """
     process CLI arguments
     """
     # input argument creation and processing
@@ -31,40 +32,37 @@
 
     # create the parser for the "gui" command
     parser_gui = subparsers.add_parser(  # pylint: disable=unused-variable
         'gui', help='Start graphical user interface to select options')
 
     # create the parser for the "cli" command
     parser_cli = subparsers.add_parser(
-        'cli', help='Run the tool via command line interface')
+        'cli', help='Run the tool via command line interface', formatter_class=argparse.RawTextHelpFormatter)
 
     # group: primary input parameters to create map for. One needs to be given
     primary_args = parser_cli.add_argument_group(
         title='Primary input', description='Generate maps for...')
     primary_args_excl = primary_args.add_mutually_exclusive_group(
         required=True)
     # country to create maps for
     primary_args_excl.add_argument(
-        "-co", "--country", help="country to generate maps for")
+        "-co", "--country", help="country to generate maps for.\nExample: -co malta, multiple countries separated by comma: -co malta,italy")
     # X/Y coordinates to create maps for
     primary_args_excl.add_argument(
-        "-xy", "--xy_coordinates", help="x/y coordinates to generate maps for. Example: 133/88")
+        "-xy", "--xy_coordinates", help="x/y coordinates to generate maps for.\nExample: -xy 133/88, multiple xy coordinates separated by comma: -xy 133/88,134/89")
 
     # group: options for map generation
     options_args = parser_cli.add_argument_group(
         title='Options', description='Options for map generation')
     # Maximum age of source maps or land shape files before they are redownloaded
     options_args.add_argument('-md', '--maxdays', type=int, default=InputData().max_days_old,
                               help="maximum age of source maps and other files")
     # Do not calculate border countries of input country
     options_args.add_argument('-nbc', '--bordercountries', action='store_false',
                               help="do not process border countries of tiles involving more than one country")
-    # calculate contour lines
-    options_args.add_argument('-con', '--contour', action='store_true',
-                              help="process contour lines (elevation data)")
     # Force download of source maps and the land shape file
     # If False use Max_Days_Old to check for expired maps
     # If True force redownloading of maps and landshape
     options_args.add_argument('-fd', '--forcedownload', action='store_true',
                               help="force download of files")
     # Force (re)processing of source maps and the land shape file
     # If False only process files if not existing
@@ -98,16 +96,14 @@
     # cli processing
     o_input_data = InputData()
     o_input_data.country = args.country
     o_input_data.xy_coordinates = args.xy_coordinates
     o_input_data.max_days_old = args.maxdays
 
     o_input_data.process_border_countries = args.bordercountries
-    o_input_data.contour = args.contour
-
     o_input_data.force_download = args.forcedownload
     o_input_data.force_processing = args.forceprocessing
 
     o_input_data.tag_wahoo_xml = args.tag_wahoo_xml
     o_input_data.save_cruiser = args.cruiser
     o_input_data.zip_folder = args.zip
 
@@ -179,15 +175,14 @@
         self.country = ""
         self.xy_coordinates = ""
         self.max_days_old = 14
 
         self.force_download = False
         self.force_processing = False
         self.process_border_countries = True
-        self.contour = False
         self.save_cruiser = False
 
         self.tag_wahoo_xml = "tag-wahoo-poi.xml"
 
         self.zip_folder = False
         self.verbose = False
 
@@ -205,22 +200,26 @@
                          "Or in the GUI select a country to create maps for.")
             else:
                 sys.exit()
         elif self.country and self.xy_coordinates:
             sys.exit(
                 "Country and X/Y coordinates are given. Only one of both is allowed!")
         elif self.country:
-            try:
-                self.country = GeofabrikJson().translate_id_no_to_geofabrik(
-                    self.country)
-                return True
-            except CountyIsNoGeofabrikCountry:
-                sys.exit(
-                    f"Entered country '{self.country}' is not a geofabrik country. Please check this URL for possible countries \
-                        https://download.geofabrik.de/index.html!")
+            # countries =
+            for country in get_countries_from_input(self.country):
+                try:
+                    country = GeofabrikJson().translate_id_no_to_geofabrik(
+                        country)
+                except CountyIsNoGeofabrikCountry:
+                    sys.exit(
+                        f"Entered country '{country}' is not a geofabrik country. Please check this URL for possible countries \
+                            https://download.geofabrik.de/index.html!")
+
+            # if we made it until here, sys.exit() was not called and therefore all countries OK ;-)
+            return True
         else:
             return True
 
 
 class GuiInput(tk.Tk):
     """
     This is the class to proces user-input via GUI
```

### Comparing `wahoomc-4.0.0a8/wahoomc/main.py` & `wahoomc-4.0.0a9/wahoomc/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 
 # import custom python packages
 from wahoomc.input import process_call_of_the_tool, cli_init
 from wahoomc.setup_functions import initialize_work_directories, \
     check_installation_of_required_programs, write_config_file, \
     adjustments_due_to_breaking_changes, copy_jsons_from_repo_to_user, \
-    check_installed_version_against_latest_pypi, check_installation_of_additional_programs
+    check_installed_version_against_latest_pypi
 from wahoomc.downloader import download_tooling
 
 from wahoomc.osm_maps_functions import OsmMaps
 from wahoomc.osm_maps_functions import OsmData
 
 # logging used in the terminal output:
 # # means top-level command
@@ -51,17 +51,14 @@
     if run_level == 'init':
         copy_jsons_from_repo_to_user('tag_wahoo_adjusted')
         copy_jsons_from_repo_to_user('.', 'tags-to-keep.json')
     else:
         # Is there something to do?
         o_input_data.is_required_input_given_or_exit(issue_message=True)
 
-        if o_input_data.contour:
-            check_installation_of_additional_programs()
-
         o_osm_data = OsmData()
         # Check for not existing or expired files. Mark for download, if dl is needed
         o_downloader = o_osm_data.process_input_of_the_tool(o_input_data)
 
         # Download files marked for download
         o_downloader.download_files_if_needed()
 
@@ -72,18 +69,14 @@
 
         # Generate land
         o_osm_maps.generate_land()
 
         # Generate sea
         o_osm_maps.generate_sea()
 
-        # Generate elevation
-        if o_input_data.contour:
-            o_osm_maps.generate_elevation()
-
         # Split filtered country files to tiles
         o_osm_maps.split_filtered_country_files_to_tiles()
 
         # Merge splitted tiles with land an sea
         o_osm_maps.merge_splitted_tiles_with_land_and_sea(
             o_input_data.process_border_countries)
```

### Comparing `wahoomc-4.0.0a8/wahoomc/osm_maps_functions.py` & `wahoomc-4.0.0a9/wahoomc/osm_maps_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,54 +15,31 @@
 import logging
 
 # import custom python packages
 from wahoomc.file_directory_functions import read_json_file, create_empty_directories, write_json_file_generic
 from wahoomc.constants_functions import translate_tags_to_keep, \
     get_tooling_win_path, get_tag_wahoo_xml_path, TagWahooXmlNotFoundError
 
-from wahoomc.setup_functions import read_earthexplorer_credentials, ask_for_and_write_earthexplorer_credentials
-
 from wahoomc.constants import USER_WAHOO_MC
 from wahoomc.constants import USER_OUTPUT_DIR
 from wahoomc.constants import RESOURCES_DIR
 from wahoomc.constants import LAND_POLYGONS_PATH
 from wahoomc.constants import VERSION
 from wahoomc.constants import OSMOSIS_WIN_FILE_PATH
-from wahoomc.constants import USER_DL_DIR
 
 from wahoomc.downloader import Downloader
 from wahoomc.geofabrik import CountryGeofabrik, XYGeofabrik
 
 log = logging.getLogger('main-logger')
 
 
 class TileNotFoundError(Exception):
     """Raised when no tile is found for x/y combination"""
 
 
-def get_xy_coordinates_from_input(input_xy_coordinates):
-    """
-    extract/split x/y combinations by given X/Y coordinates.
-    input should be "188/88" or for multiple values "188/88,100/10,109/99".
-    returns a list of x/y combinations as integers
-    """
-
-    xy_combinations = []
-
-    # split by "," first for multiple x/y combinations, then by "/" for x and y value
-    for xy_coordinate in input_xy_coordinates.split(","):
-        splitted = xy_coordinate.split("/")
-
-        if len(splitted) == 2:
-            xy_combinations.append(
-                {"x": int(splitted[0]), "y": int(splitted[1])})
-
-    return xy_combinations
-
-
 def run_subprocess_and_log_output(cmd, error_message, cwd=""):
     """
     run given cmd-subprocess and issue error message if wished
     """
     if not cwd:
         with subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) as process:
             for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
@@ -136,22 +113,22 @@
         # geofabrik file
         if o_downloader.should_geofabrik_file_be_downloaded():
             self.force_processing = True
             o_downloader.download_geofabrik_file()
 
         # calc tiles
         if o_input_data.country:
-            self.calc_tiles_country(o_input_data)
+            o_geofabrik = self.calc_tiles_country(o_input_data)
         elif o_input_data.xy_coordinates:
             self.calc_tiles_xy(o_input_data)
 
         # calc border countries
         log.info('-' * 80)
         if o_input_data.country:
-            self.calc_border_countries_country(o_input_data)
+            self.calc_border_countries_country(o_input_data, o_geofabrik)
         elif o_input_data.xy_coordinates:
             self.calc_border_countries()
         # log border countries when and when not calculated to output the processed country(s)
         self.log_border_countries()
 
         # calc country name
         if o_input_data.country:
@@ -177,39 +154,38 @@
         """
         log.info('# Input country: %s.', o_input_data.country)
 
         # use Geofabrik-URL to calculate the relevant tiles
         o_geofabrik = CountryGeofabrik(o_input_data.country)
         self.tiles = o_geofabrik.get_tiles_of_wanted_map()
 
+        return o_geofabrik
+
     def calc_tiles_xy(self, o_input_data):
         """
         option 2: input a x/y combinations as parameter, e.g. 134/88  or 133/88,130/100
         """
         log.info(
             '# Input X/Y coordinates: %s.', o_input_data.xy_coordinates)
 
-        # use Geofabrik-URL to get the relevant tiles
-        xy_coordinates = get_xy_coordinates_from_input(
-            o_input_data.xy_coordinates)
-
-        o_geofabrik = XYGeofabrik(xy_coordinates)
+        o_geofabrik = XYGeofabrik(o_input_data.xy_coordinates)
         # find the tiles for  x/y combinations in the geofabrik json files
         self.tiles = o_geofabrik.get_tiles_of_wanted_map()
 
-    def calc_border_countries_country(self, o_input_data):
+    def calc_border_countries_country(self, o_input_data, o_geofabrik):
         """
         calculate the border countries for the given tiles when input is a country
         - if CLI/GUI input by user
         """
         if o_input_data.process_border_countries:
             self.calc_border_countries()
         # set the to-be-processed country as border country
         else:
-            self.border_countries[o_input_data.country] = {}
+            for country in o_geofabrik.wanted_maps:
+                self.border_countries[country] = {}
 
     def calc_border_countries(self):
         """
         calculate the border countries for the given tiles. i.e.
         - if CLI/GUI input by user
         - if processing x/y coordinates
         """
@@ -473,56 +449,14 @@
 
                     with open(out_file_sea, mode='w', encoding="utf-8") as output_file:
                         output_file.write(sea_data)
             tile_count += 1
 
         log.info('+ Generate sea for each coordinate: OK')
 
-    def generate_elevation(self):
-        """
-        Generate contour lines for all tiles
-        """
-        username, password = read_earthexplorer_credentials()
-
-        if not username or not password:
-            username, password = ask_for_and_write_earthexplorer_credentials()
-
-        log.info('-' * 80)
-        log.info('# Generate contour lines for each coordinate')
-
-        hgt_path = os.path.join(USER_DL_DIR, 'hgt')
-
-        tile_count = 1
-        for tile in self.o_osm_data.tiles:
-            out_file_elevation = os.path.join(
-                USER_OUTPUT_DIR, f'{tile["x"]}', f'{tile["y"]}', 'elevation')
-            # as the elevation file has a suffix, they need to be searched with glob.glob
-            # example elevation filename: elevation_lon14.06_15.47lat35.46_36.60_view1,view3.osm
-            out_file_elevation_existing = glob.glob(os.path.join(
-                USER_OUTPUT_DIR, str(tile["x"]), str(tile["y"]), 'elevation*.osm'))
-            # check for already existing .osm file
-            if not (len(out_file_elevation_existing) == 1 and os.path.isfile(out_file_elevation_existing[0])) \
-                    or self.o_osm_data.force_processing is True:
-                print(
-                    f'# Generate elevation {tile_count} for coordinates: {tile["x"]} {tile["y"]}')
-                cmd = ['phyghtmap']
-                cmd.append('-a ' + f'{tile["left"]}' + ':' + f'{tile["bottom"]}' +
-                            ':' + f'{tile["right"]}' + ':' + f'{tile["top"]}')
-                cmd.extend(['-o', f'{out_file_elevation}', '-s 10', '-c 100,50', '--source=view1,view3,srtm3',
-                            '--jobs=8', '--viewfinder-mask=1', '--start-node-id=20000000000',
-                            '--max-nodes-per-tile=0', '--start-way-id=2000000000', '--write-timestamp',
-                            '--no-zero-contour', '--hgtdir=' + hgt_path])
-                cmd.append('--earthexplorer-user=' + username)
-                cmd.append('--earthexplorer-password=' + password)
-
-                run_subprocess_and_log_output(
-                    cmd, f'! Error in phyghtmap with tile: {tile["x"]},{tile["y"]}. Win/out_file')
-
-        log.info('+ Generate contour lines for each coordinate: OK')
-
     def split_filtered_country_files_to_tiles(self):
         """
         Split filtered country files to tiles
         """
 
         log.info('-' * 80)
         log.info('# Split filtered country files to tiles')
@@ -592,33 +526,30 @@
 
             tile_count += 1
 
         log.info('+ Split filtered country files to tiles: OK')
 
     def merge_splitted_tiles_with_land_and_sea(self, process_border_countries):
         """
-        Merge splitted tiles with land elevation and sea
+        Merge splitted tiles with land an sea
         """
 
         log.info('-' * 80)
-        log.info('# Merge splitted tiles with land, elevation and sea')
+        log.info('# Merge splitted tiles with land an sea')
         tile_count = 1
         for tile in self.o_osm_data.tiles:  # pylint: disable=too-many-nested-blocks
             log.info(
                 '+ Coordinates: %s,%s (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
 
             out_tile_dir = os.path.join(USER_OUTPUT_DIR,
                                         f'{tile["x"]}', f'{tile["y"]}')
             out_file_merged = os.path.join(out_tile_dir, 'merged.osm.pbf')
 
             land_files = glob.glob(os.path.join(out_tile_dir, 'land*.osm'))
 
-            elevation_files = glob.glob(
-                os.path.join(out_tile_dir, 'elevation*.osm'))
-
             # merge splitted tiles with land and sea every time because the result is different per constants (user input)
             # sort land* osm files
             self.sort_osm_files(tile)
 
             # Windows
             if platform.system() == "Windows":
                 cmd = [OSMOSIS_WIN_FILE_PATH]
@@ -646,29 +577,25 @@
 
                     loop += 1
 
             for land in land_files:
                 cmd.extend(
                     ['--rx', 'file='+land, '--s', '--m'])
 
-            for elevation in elevation_files:
-                cmd.extend(
-                    ['--rx', 'file='+elevation, '--s', '--m'])
-
             cmd.extend(
                 ['--rx', 'file='+os.path.join(out_tile_dir, 'sea.osm'), '--s', '--m'])
             cmd.extend(['--tag-transform', 'file=' + os.path.join(RESOURCES_DIR,
                                                                   'tunnel-transform.xml'), '--wb', out_file_merged, 'omitmetadata=true'])
 
             run_subprocess_and_log_output(
                 cmd, f'! Error in Osmosis with tile: {tile["x"]},{tile["y"]}')
 
             tile_count += 1
 
-        log.info('+ Merge splitted tiles with land, elevation and sea: OK')
+        log.info('+ Merge splitted tiles with land an sea: OK')
 
     def sort_osm_files(self, tile):
         """
         sort land*.osm files to be in this order: nodes, then ways, then relations.
         this is mandatory for osmium-merge since:
         https://github.com/osmcode/osmium-tool/releases/tag/v1.13.2
         """
```

### Comparing `wahoomc-4.0.0a8/wahoomc/resources/sea.osm` & `wahoomc-4.0.0a9/wahoomc/resources/sea.osm`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/resources/shape2osm.py` & `wahoomc-4.0.0a9/wahoomc/resources/shape2osm.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml` & `wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml` & `wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/resources/tags-to-keep.json` & `wahoomc-4.0.0a9/wahoomc/resources/tags-to-keep.json`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/7za.dll` & `wahoomc-4.0.0a9/wahoomc/tooling_win/7za.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/7za.exe` & `wahoomc-4.0.0a9/wahoomc/tooling_win/7za.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/7zxa.dll` & `wahoomc-4.0.0a9/wahoomc/tooling_win/7zxa.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/lzma.exe` & `wahoomc-4.0.0a9/wahoomc/tooling_win/lzma.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/osmconvert.exe` & `wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc/tooling_win/osmconvert64-0.8.8p.exe` & `wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert64-0.8.8p.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a8/wahoomc.egg-info/PKG-INFO` & `wahoomc-4.0.0a9/wahoomc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.0a8
+Version: 4.0.0a9
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,14 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
-* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
-
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a8 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a9 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
@@ -22,31 +22,30 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
-Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
-of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
-USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
-with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
-theme on your Wahoo to control what and in which zoom-level certain elements
-are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
-on-your-device-) ## Contribution / Questions You are welcome to provide input
-via Pull Requests, Issues or in any other way! If you have trouble using
-wahooMapsCreator, look into the FAQ, write an issue or join the telegram
-channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
-(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
-https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
-[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
-Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
-the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
-[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
-and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
-done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
-[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
-making this a little more public [@vti](https://github.com/vti) for creating a
-GUI application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
+tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
+[:computer: Preview your generated maps with cruiser ](docs/
+USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
+control what and in which zoom-level certain elements are rendered](docs/
+TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
+Contribution / Questions You are welcome to provide input via Pull Requests,
+Issues or in any other way! If you have trouble using wahooMapsCreator, look
+into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
+FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
+treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
+TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
+CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
+(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
+(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
+github.com/mweirauch) for bringing in new ideas, testing and using the tool
+[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
+(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
+/github.com/macdet) for bringing in new thoughts, testing and making this a
+little more public [@vti](https://github.com/vti) for creating a GUI
+application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a8/wahoomc.egg-info/SOURCES.txt` & `wahoomc-4.0.0a9/wahoomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

