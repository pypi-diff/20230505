# Comparing `tmp/wahoomc-4.0.0a9.tar.gz` & `tmp/wahoomc-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wahoomc-4.0.0a9.tar", last modified: Sun Apr  2 17:46:28 2023, max compression
+gzip compressed data, was "wahoomc-4.0.1.tar", last modified: Fri May  5 19:49:52 2023, max compression
```

## Comparing `wahoomc-4.0.0a9.tar` & `wahoomc-4.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.349439 wahoomc-4.0.0a9/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4296 2023-04-02 17:46:28.349529 wahoomc-4.0.0a9/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3755 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/README.md
--rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/pyproject.toml
--rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-04-02 17:46:28.349898 wahoomc-4.0.0a9/setup.cfg
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.342668 wahoomc-4.0.0a9/tests/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.0a9/tests/test_cli.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/tests/test_constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5493 2023-04-02 09:13:20.000000 wahoomc-4.0.0a9/tests/test_constants_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-04-01 20:49:53.000000 wahoomc-4.0.0a9/tests/test_downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/tests/test_generated_files.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     8067 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/tests/test_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7069 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/tests/test_osm_maps.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/tests/test_setup.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.344904 wahoomc-4.0.0a9/wahoomc/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/wahoomc/constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-04-01 12:11:17.000000 wahoomc-4.0.0a9/wahoomc/constants_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    12624 2023-04-02 08:07:59.000000 wahoomc-4.0.0a9/wahoomc/downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6299 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/file_directory_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    20267 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4567 2023-04-02 09:13:20.000000 wahoomc-4.0.0a9/wahoomc/geofabrik_json.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346004 wahoomc-4.0.0a9/wahoomc/init/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/init/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/init/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    17318 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/input.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3178 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/main.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    35409 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/osm_maps_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346634 wahoomc-4.0.0a9/wahoomc/resources/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/sea.osm
--rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/shape2osm.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.346992 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6369 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.347221 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_initial/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779     2282 2023-03-27 20:10:10.000000 wahoomc-4.0.0a9/wahoomc/resources/tags-to-keep.json
--rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.0a9/wahoomc/resources/tunnel-transform.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779     8209 2023-04-02 17:43:43.000000 wahoomc-4.0.0a9/wahoomc/setup_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.349149 wahoomc-4.0.0a9/wahoomc/tooling_win/
--rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7za.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7za.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/7zxa.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/lzma.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-04-02 17:46:28.345729 wahoomc-4.0.0a9/wahoomc.egg-info/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4296 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/SOURCES.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/dependency_links.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-04-02 17:46:28.000000 wahoomc-4.0.0a9/wahoomc.egg-info/top_level.txt
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.915034 wahoomc-4.0.1/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4401 2023-05-05 19:49:52.915125 wahoomc-4.0.1/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-05-05 19:23:35.000000 wahoomc-4.0.1/README.md
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.1/pyproject.toml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      827 2023-05-05 19:49:52.915504 wahoomc-4.0.1/setup.cfg
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.902398 wahoomc-4.0.1/tests/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.1/tests/test_cli.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5494 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_constants_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_generated_files.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9487 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7214 2023-05-05 19:23:35.000000 wahoomc-4.0.1/tests/test_osm_maps.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.1/tests/test_setup.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.905256 wahoomc-4.0.1/wahoomc/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.1/wahoomc/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1590 2023-05-05 19:49:29.000000 wahoomc-4.0.1/wahoomc/constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/constants_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    12209 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5720 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/file_directory_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    21372 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4635 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/geofabrik_json.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.906272 wahoomc-4.0.1/wahoomc/init/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.1/wahoomc/init/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.1/wahoomc/init/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    17504 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/input.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3646 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/main.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    40022 2023-05-05 19:47:49.000000 wahoomc-4.0.1/wahoomc/osm_maps_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.907470 wahoomc-4.0.1/wahoomc/resources/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/resources/sea.osm
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/resources/shape2osm.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.907944 wahoomc-4.0.1/wahoomc/resources/tag_wahoo_adjusted/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9575 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.908456 wahoomc-4.0.1/wahoomc/resources/tag_wahoo_initial/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     2304 2023-05-05 19:21:07.000000 wahoomc-4.0.1/wahoomc/resources/tags-to-keep.json
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.1/wahoomc/resources/tunnel-transform.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10562 2023-05-05 19:23:35.000000 wahoomc-4.0.1/wahoomc/setup_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.914357 wahoomc-4.0.1/wahoomc/tooling_win/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/tooling_win/7za.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/tooling_win/7za.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.1/wahoomc/tooling_win/7zxa.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.1/wahoomc/tooling_win/lzma.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.1/wahoomc/tooling_win/osmconvert.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.1/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-05 19:49:52.906013 wahoomc-4.0.1/wahoomc.egg-info/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4401 2023-05-05 19:49:52.000000 wahoomc-4.0.1/wahoomc.egg-info/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-05-05 19:49:52.000000 wahoomc-4.0.1/wahoomc.egg-info/SOURCES.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-05-05 19:49:52.000000 wahoomc-4.0.1/wahoomc.egg-info/dependency_links.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-05-05 19:49:52.000000 wahoomc-4.0.1/wahoomc.egg-info/top_level.txt
```

### Comparing `wahoomc-4.0.0a9/PKG-INFO` & `wahoomc-4.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.0a9
+Version: 4.0.1
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,16 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
+* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
+
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a9 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.1 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
@@ -22,30 +22,31 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
-tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
-[:computer: Preview your generated maps with cruiser ](docs/
-USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
-control what and in which zoom-level certain elements are rendered](docs/
-TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
-Contribution / Questions You are welcome to provide input via Pull Requests,
-Issues or in any other way! If you have trouble using wahooMapsCreator, look
-into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
-FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
-treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
-TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
-CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
-(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
-(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
-github.com/mweirauch) for bringing in new ideas, testing and using the tool
-[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
-(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
-/github.com/macdet) for bringing in new thoughts, testing and making this a
-little more public [@vti](https://github.com/vti) for creating a GUI
-application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
+Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
+of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
+USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
+with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
+theme on your Wahoo to control what and in which zoom-level certain elements
+are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
+on-your-device-) ## Contribution / Questions You are welcome to provide input
+via Pull Requests, Issues or in any other way! If you have trouble using
+wahooMapsCreator, look into the FAQ, write an issue or join the telegram
+channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
+(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
+https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
+[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
+Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
+the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
+[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
+and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
+done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
+[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
+making this a little more public [@vti](https://github.com/vti) for creating a
+GUI application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a9/README.md` & `wahoomc-4.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
+* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
+
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -14,30 +14,31 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
-tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
-[:computer: Preview your generated maps with cruiser ](docs/
-USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
-control what and in which zoom-level certain elements are rendered](docs/
-TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
-Contribution / Questions You are welcome to provide input via Pull Requests,
-Issues or in any other way! If you have trouble using wahooMapsCreator, look
-into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
-FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
-treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
-TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
-CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
-(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
-(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
-github.com/mweirauch) for bringing in new ideas, testing and using the tool
-[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
-(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
-/github.com/macdet) for bringing in new thoughts, testing and making this a
-little more public [@vti](https://github.com/vti) for creating a GUI
-application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
+Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
+of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
+USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
+with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
+theme on your Wahoo to control what and in which zoom-level certain elements
+are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
+on-your-device-) ## Contribution / Questions You are welcome to provide input
+via Pull Requests, Issues or in any other way! If you have trouble using
+wahooMapsCreator, look into the FAQ, write an issue or join the telegram
+channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
+(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
+https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
+[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
+Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
+the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
+[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
+and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
+done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
+[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
+making this a little more public [@vti](https://github.com/vti) for creating a
+GUI application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a9/setup.cfg` & `wahoomc-4.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wahoomc
-version = 4.0.0a9
+version = 4.0.1
 author = Benjamin Kreuscher
 author_email = benni.kreuscher@gmail.com
 description = Create maps for your Wahoo bike computer based on latest OSM maps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/treee111/wahooMapsCreator
 project_urls =
```

### Comparing `wahoomc-4.0.0a9/tests/test_cli.py` & `wahoomc-4.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/tests/test_constants.py` & `wahoomc-4.0.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/tests/test_constants_geofabrik.py` & `wahoomc-4.0.1/tests/test_constants_geofabrik.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 tests for the constants geofabrik & geofabrik file
 """
 import os
 import unittest
 
-import geojson # pylint: disable=import-error
+import geojson  # pylint: disable=import-error
 
 # import custom python packages
 from wahoomc.downloader import Downloader
 from wahoomc import constants
 from wahoomc.geofabrik_json import GeofabrikJson
 from wahoomc.geofabrik_json import CountyIsNoGeofabrikCountry
```

### Comparing `wahoomc-4.0.0a9/tests/test_downloader.py` & `wahoomc-4.0.1/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/tests/test_generated_files.py` & `wahoomc-4.0.1/tests/test_generated_files.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/tests/test_geofabrik.py` & `wahoomc-4.0.1/tests/test_geofabrik.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 import os
 # import sys
 import unittest
 from shapely.geometry import shape  # pylint: disable=import-error
 
 # import custom python packages
-from wahoomc.geofabrik import CountryGeofabrik, XYGeofabrik
-from wahoomc.geofabrik import calc_bounding_box_tiles, get_xy_coordinates_from_input
+from wahoomc.geofabrik import CountryGeofabrik, XYCombinationHasNoCountries, XYGeofabrik
+from wahoomc.geofabrik import calc_bounding_box_tiles
 from wahoomc.downloader import Downloader
 from wahoomc import constants
-from wahoomc.geofabrik_json import GeofabrikJson
+from wahoomc.geofabrik_json import CountyIsNoGeofabrikCountry, GeofabrikJson
 
 
 def calc_tiles_via_geofabrik_json(input_argument):
     """
     calculate tiles using downloaded geofabrik file
     the "new" way of doing
     """
@@ -156,33 +156,69 @@
         self.assertEqual(wanted_region_exp, wanted_region_string)
 
     def test_splitting_of_single_xy_coordinate(self):
         """
         use static json files in the repo to calculate relevant tiles
         """
 
-        xy_tuple = get_xy_coordinates_from_input("133/88")
+        xy_tuple = XYGeofabrik.split_input_to_list("133/88")
         self.assertEqual(xy_tuple, [{"x": 133, "y": 88}])
 
-        xy_tuple = get_xy_coordinates_from_input("11/92")
+        xy_tuple = XYGeofabrik.split_input_to_list("11/92")
         self.assertEqual(xy_tuple, [{"x": 11, "y": 92}])
 
-        xy_tuple = get_xy_coordinates_from_input("138/100")
+        xy_tuple = XYGeofabrik.split_input_to_list("138/100")
         self.assertEqual(xy_tuple, [{"x": 138, "y": 100}])
 
     def test_splitting_of_multiple_xy_coordinate(self):
         """
         use static json files in the repo to calculate relevant tiles
         """
 
-        xy_tuple = get_xy_coordinates_from_input("133/88,138/100")
+        xy_tuple = XYGeofabrik.split_input_to_list("133/88,138/100")
         expected_result = [{"x": 133, "y": 88}, {"x": 138, "y": 100}]
 
         self.assertEqual(xy_tuple, expected_result)
 
+    def test_if_countrygeofabrik_raises_exception(self):
+        """
+        initialize CountryGeofabrik class and let the class check if the country is OK
+        in other words: if the exception raised by translate_id_no_to_geofabrik
+        is transported all up
+        """
+        CountryGeofabrik('germany')
+        CountryGeofabrik('malta')
+        CountryGeofabrik('malta,germany')
+
+        with self.assertRaises(CountyIsNoGeofabrikCountry):
+            CountryGeofabrik('germanyd')
+        with self.assertRaises(CountyIsNoGeofabrikCountry):
+            CountryGeofabrik('xy')
+        with self.assertRaises(CountyIsNoGeofabrikCountry):
+            CountryGeofabrik('maltad,germany')
+        with self.assertRaises(CountyIsNoGeofabrikCountry):
+            CountryGeofabrik('malta,tekke')
+
+    def test_if_xy_geofabrik_raises_exception(self):
+        """
+        initialize XYGeofabrik class + check if xy coordinate has countries
+        """
+        o_geofabrik = XYGeofabrik('133/87')
+        o_geofabrik.get_tiles_of_wanted_map()
+
+        o_geofabrik = XYGeofabrik('100/138')
+        o_geofabrik.get_tiles_of_wanted_map()
+
+        o_geofabrik = XYGeofabrik('138/100')
+        o_geofabrik.get_tiles_of_wanted_map()
+
+        with self.assertRaises(XYCombinationHasNoCountries):
+            o_geofabrik = XYGeofabrik('200/1')
+            o_geofabrik.get_tiles_of_wanted_map()
+
     # def test_get_tile_via_xy_coordinate_error(self):
     #     """
     #     use static json files in the repo to calculate a not-existing tile.
 
     #     does not error out due to new Geofabrik Json processing. Nevertheless, the tile is not existing
     #     only +/- 180 -/+90: https://epsg.io/4326
     #     """
```

### Comparing `wahoomc-4.0.0a9/tests/test_osm_maps.py` & `wahoomc-4.0.1/tests/test_osm_maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 tests for the osm maps file
 """
 import os
 # import sys
 import unittest
 
 # import custom python packages
-from wahoomc.osm_maps_functions import OsmData
+from wahoomc.osm_maps_functions import CountryOsmData, XYOsmData
 from wahoomc.osm_maps_functions import OsmMaps
 # from wahoomc.osm_maps_functions import TileNotFoundError
 from wahoomc.input import InputData
 from wahoomc import file_directory_functions as fd_fct
 from wahoomc import constants
 
 
@@ -116,22 +116,24 @@
 
     def process_and_check_border_countries(self, inp_val, calc_border_c, exp_result, inp_mode):
         """
         helper method to process a country or json file and check the calculated border countries
         """
 
         o_input_data = InputData()
+        o_input_data.process_border_countries = calc_border_c
+
         if inp_mode == 'country':
             o_input_data.country = inp_val
+            o_osm_data = CountryOsmData(o_input_data)
         elif inp_mode == 'xy_coordinate':
             o_input_data.xy_coordinates = inp_val
-        o_input_data.process_border_countries = calc_border_c
+            o_osm_data = XYOsmData(o_input_data)
 
-        o_osm_data = OsmData()
-        o_osm_data.process_input_of_the_tool(o_input_data)
+        o_osm_data.process_input_of_the_tool()
 
         result = o_osm_data.border_countries
 
         # delete the path to the file, here, only the correct border countries are checked
         for res in result:
             result[res] = {}
 
@@ -148,16 +150,16 @@
         Test "malta" as input to the wahooMapsCreator
         check, if the given input-parameter is saved to the OsmMaps instance
         """
 
         o_input_data = InputData()
         o_input_data.country = 'malta'
 
-        o_osm_data = OsmData()
-        o_osm_data.process_input_of_the_tool(o_input_data)
+        o_osm_data = CountryOsmData(o_input_data)
+        o_osm_data.process_input_of_the_tool()
 
         result = o_osm_data.country_name
         self.assertEqual(result, 'malta')
 
     def test_encoding_open_sea_osm(self):
         """
         use static json files in the repo to calculate relevant tile
@@ -182,28 +184,30 @@
         """
 
         o_input_data = InputData()
         o_input_data.country = 'malta'
         # prevent from downloading land_polygons each time
         o_input_data.max_days_old = 1000
 
-        o_osm_data = OsmData()
-        o_downloader = o_osm_data.process_input_of_the_tool(o_input_data)
+        o_osm_data = CountryOsmData(o_input_data)
+        o_osm_data.process_input_of_the_tool()
+
+        o_downloader = o_osm_data.get_downloader()
 
         # download files marked for download to fill up map_file per country to write to config
         o_downloader.download_files_if_needed()
 
         o_osm_maps = OsmMaps(o_osm_data)
 
         o_osm_maps.write_country_config_file(o_input_data.country)
 
         self.assertTrue(
             o_osm_maps.tags_are_identical_to_last_run(o_input_data.country))
 
-        country_config = fd_fct.read_json_file(os.path.join(
+        country_config = fd_fct.read_json_file_country_config(os.path.join(
             constants.USER_OUTPUT_DIR, o_input_data.country, ".config.json"))
 
         self.assertEqual(constants.VERSION, country_config["version_last_run"])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wahoomc-4.0.0a9/tests/test_setup.py` & `wahoomc-4.0.1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/constants.py` & `wahoomc-4.0.1/wahoomc/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Python Package - wahooMapsCreator directory
 WAHOO_MC_DIR = os.path.dirname(__file__)
 RESOURCES_DIR = os.path.join(WAHOO_MC_DIR, 'resources')
 TOOLING_WIN_DIR = os.path.join(WAHOO_MC_DIR, 'tooling_win')
 # location of repo / python installation - not used
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-VERSION = '4.0.0a0'
+VERSION = '4.0.1'
 
 
 block_download = ['dach', 'alps', 'britain-and-ireland', 'south-africa-and-lesotho',
                   'us-midwest', 'us-northeast', 'us-pacific', 'us-south', 'us-west']
 
 # Special_regions like (former) colonies where the map of the wanted region is not present in the map of the parent country.
 # example Guadeloupe, it's Geofabrik parent country is France but Guadeloupe is not located within the region covered by the map of France.
```

### Comparing `wahoomc-4.0.0a9/wahoomc/constants_functions.py` & `wahoomc-4.0.1/wahoomc/constants_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/downloader.py` & `wahoomc-4.0.1/wahoomc/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -293,39 +293,33 @@
         log.info('-' * 80)
         log.info('# check countries .osm.pbf files')
 
         # Check for expired maps and delete them
         log.info('+ Checking for old maps and remove them')
 
         for country in self.border_countries:
-            # get translated country (geofabrik) of country
-            # do not download the same file for different countries
-            # --> e.g. China, Hong Kong and Macao, see Issue #11
-            transl_c = self.o_geofabrik_json.translate_id_no_to_geofabrik(
-                country)
-
             # check for already existing .osm.pbf file
             map_file_path = glob.glob(
-                f'{USER_MAPS_DIR}/{transl_c}-latest.osm.pbf')
+                f'{USER_MAPS_DIR}/{country}-latest.osm.pbf')
             if len(map_file_path) != 1:
                 map_file_path = glob.glob(
-                    f'{USER_MAPS_DIR}/**/{transl_c}-latest.osm.pbf')
+                    f'{USER_MAPS_DIR}/**/{country}-latest.osm.pbf')
 
             # delete .osm.pbf file if out of date
             if len(map_file_path) == 1 and os.path.isfile(map_file_path[0]):
                 if self.should_file_be_downloaded(map_file_path[0]):
                     log.info(
-                        '+ mapfile for %s: deleted. Input: %s.', transl_c, country)
+                        '+ mapfile for %s: deleted.', country)
                     os.remove(map_file_path[0])
                     self.need_to_dl.append('osm_pbf')
                 else:
                     self.border_countries[country] = {
                         'map_file': map_file_path[0]}
                     log.info(
-                        '+ mapfile for %s: up-to-date. Input: %s.', transl_c, country)
+                        '+ mapfile for %s: up-to-date.', country)
 
             # mark country .osm.pbf file for download if there exists no file or it is no file
             map_file_path = self.border_countries[country].get('map_file')
             if map_file_path is None or (not os.path.isfile(map_file_path) or self.force_download):
                 self.border_countries[country]['download'] = True
                 self.need_to_dl.append('osm_pbf')
 
@@ -333,16 +327,15 @@
         """
         download countries' OSM files
         """
         for country, item in self.border_countries.items():
             try:
                 if item['download'] is True:
                     # build path to downloaded file with translated geofabrik country
-                    map_file_path = build_osm_pbf_filepath(
-                        self.o_geofabrik_json.translate_id_no_to_geofabrik(country))
+                    map_file_path = build_osm_pbf_filepath(country)
                     # fetch the geofabrik download url to countries' OSM file
                     url = self.o_geofabrik_json.get_geofabrik_url(country)
                     download_file(map_file_path, url)
                     self.border_countries[country] = {
                         'map_file': map_file_path}
             except KeyError:
                 pass
```

### Comparing `wahoomc-4.0.0a9/wahoomc/file_directory_functions.py` & `wahoomc-4.0.1/wahoomc/file_directory_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,45 +56,47 @@
         os.makedirs(outdir, exist_ok=True)
 
     for country in border_countries:
         outdir = os.path.join(parent_dir, country)
         os.makedirs(outdir, exist_ok=True)
 
 
-def read_json_file(json_file_path):
+def read_json_file_country_config(json_file_path):
     """
-    read the tiles from the given json file
+    read the country config (of last run) from the given json file
     """
 
     log.debug('-' * 80)
-    log.debug('# Read json file')
+    log.debug('# Read country config json file')
 
-    with open(json_file_path, encoding="utf-8") as json_file:
-        tiles_from_json = json.load(json_file)
-        json_file.close()
-    if tiles_from_json == '':
+    country_config = read_json_file_generic(json_file_path)
+    if country_config == '':
         log.error('! Json file could not be opened.')
         sys.exit()
 
     log.debug(
-        '+ Use json file %s with %s tiles', json_file.name, len(tiles_from_json))
-    log.debug('+ Read json file: OK')
+        '+ Use country config file %s', json_file_path)
+    log.debug('+ Read country config json file: OK')
 
-    return tiles_from_json
+    return country_config
 
 
 def read_json_file_generic(json_file_path):
     """
     reads content of given .json file
     """
-    with open(json_file_path, encoding="utf-8") as json_file:
-        json_content = json.load(json_file)
-        json_file.close()
+    try:
+        with open(json_file_path, encoding="utf-8") as json_file:
+            json_content = json.load(json_file)
+            json_file.close()
 
-    return json_content
+        return json_content
+
+    except FileNotFoundError:
+        return {}
 
 
 def write_json_file_generic(json_file_path, json_content):
     """
     writes content to .json file
     """
     # Serializing json
@@ -102,48 +104,23 @@
 
     # Writing to file
     with open(json_file_path, "w", encoding="utf-8") as json_file:
         json_file.write(json_content)
         json_file.close()
 
 
-def get_folders_in_folder(folder):
-    """
-    return foldernames of given folder without path as list
-    """
-    onlyfolders = [f for f in os.listdir(
-        folder) if not isfile(join(folder, f))]
-
-    return onlyfolders
-
-
 def get_files_in_folder(folder):
     """
     return filenames of given folder without path as list
     """
     onlyfiles = [f for f in os.listdir(folder) if isfile(join(folder, f))]
 
     return onlyfiles
 
 
-def get_filenames_of_jsons_in_folder(folder):
-    """
-    return json-file filenames of given folder without path as list
-    """
-    json_files = []
-
-    for file in get_files_in_folder(folder):
-        if file.endswith('.json'):
-            # filename = file.split('.')[0]
-            filename = os.path.splitext(file)[0]
-            json_files.extend([filename])
-
-    return json_files
-
-
 def delete_o5m_pbf_files_in_folder(folder):
     """
     delete .o5m and .pbf files of given folder
     """
     onlyfiles = [f for f in os.listdir(folder) if isfile(join(folder, f))]
 
     for file in onlyfiles:
```

### Comparing `wahoomc-4.0.0a9/wahoomc/geofabrik.py` & `wahoomc-4.0.1/wahoomc/geofabrik.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 import sys
 import math
 import logging
 from shapely.geometry import Polygon, shape
 
 # import custom python packages
 from wahoomc.constants import special_regions, block_download
-from wahoomc.geofabrik_json import GeofabrikJson
+from wahoomc.geofabrik_json import CountyIsNoGeofabrikCountry, GeofabrikJson
 
 log = logging.getLogger('main-logger')
 
 
+class XYCombinationHasNoCountries(Exception):
+    """Raised when no tile is found for x/y combination"""
+
+    def __init__(self, xy_coordinate):
+        message = f"Given XY coordinate '{xy_coordinate}' consists of no countries. Please check if your input is valid."
+        super().__init__(message)
+
+
 class InformalGeofabrikInterface:
     """Informal class for Geofabrik processing"""
     wanted_maps = []
     tiles = []
     border_countries = {}
     output = {}
 
@@ -34,45 +42,57 @@
         """
         calculates tiles of all input wanted-maps
         :returns: list of tiles
         """
 
         tiles_of_input = []
 
-        for country in self.wanted_maps:
-            tiles_of_input.extend(self.get_tiles_of_wanted_map_single(country))
+        for wanted_map in self.wanted_maps:
+            try:
+                tiles_of_input.extend(
+                    self.get_tiles_of_wanted_map_single(wanted_map))
+            except XYCombinationHasNoCountries as exception:
+                # this exception is actually only raised in class XYGeofabrik
+                raise exception
 
         return tiles_of_input
 
     def find_needed_countries(self, bbox_tiles, wanted_map, wanted_region_polygon) -> dict:
         """find needed countries for requested country or X/Y combination"""
         pass
 
     def compose_bouding_box(self, bounds) -> dict:
         """calculate bounding box based on geometry or X/Y combination"""
         pass
 
+    def log_tile(self, counter, all):
+        """
+        unified status logging for this class
+        """
+        log.info(
+            '(+ tile %s of %s) Find needed countries ', counter, all)
+
+    def split_input_to_list(input_value) -> list:
+        """split the input to single values in a list"""
+        pass
+
 
 class CountryGeofabrik(InformalGeofabrikInterface):
     """Geofabrik processing for countries"""
 
     def __init__(self, input_countries):
         """
         :param input: string with countries: 'malta' or 'malta, switzerland'
         :returns: object for country geofabrik processing
         """
         self.o_geofabrik_json = GeofabrikJson()
         self.wanted_maps = []
 
         # input parameters
-        input_countries = get_countries_from_input(input_countries)
-
-        for country in input_countries:
-            self.wanted_maps.append(self.o_geofabrik_json.translate_id_no_to_geofabrik(
-                country))
+        self.wanted_maps = self.split_input_to_list(input_countries)
 
     def get_tiles_of_wanted_map_single(self, wanted_map):
         """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map_single()"""
         # Check if wanted_map is in the json file and if so get the polygon (shape)
         wanted_map_geom = self.o_geofabrik_json.get_geofabrik_geometry(
             wanted_map)
 
@@ -98,16 +118,15 @@
         geofabrik_regions = self.o_geofabrik_json.geofabrik_regions
 
         # itterate through tiles and find Geofabrik regions that are in the tiles
         counter = 1
         for tile in bbox_tiles:
             # Do progress indicator every 50 tiles
             if counter % 50 == 0:
-                log.info(
-                    'Processing tile %s of %s', counter, len(bbox_tiles)+1)
+                self.log_tile(counter, len(bbox_tiles)+1)
             counter += 1
 
             parent_added = 0
             force_added = 0
 
             # example contents of tile: {'index': 0, 'x': 130, 'y': 84, 'tile_left': 2.8125,
             # 'tile_top': 52.48278022207821, 'tile_right': 4.21875, 'tile_bottom': 51.6180165487737}
@@ -247,27 +266,47 @@
         if bot_y < 0:
             bot_y = 0
         if bot_y > 255:
             bot_y = 255
 
         return {'top_x': top_x, 'top_y': top_y, 'bot_x': bot_x, 'bot_y': bot_y}
 
+    @staticmethod
+    def split_input_to_list(input_value) -> list:
+        """
+        extract/split x/y combinations by given X/Y coordinates.
+        input should be "188/88" or for multiple values "188/88,100/10,109/99".
+        returns a list of x/y combinations as integers
+        """
+        countries = []
+        o_geofabrik_json = GeofabrikJson()
+
+        try:
+            # split by "," first for multiple x/y combinations, then by "/" for x and y value
+            for country in input_value.split(","):
+                countries.append(o_geofabrik_json.translate_id_no_to_geofabrik(
+                    country))
+        except CountyIsNoGeofabrikCountry as exception:
+            raise exception
+
+        return countries
+
 
 class XYGeofabrik(InformalGeofabrikInterface):
     """Geofabrik processing for X/Y coordinates"""
 
     def __init__(self, input_xy_coordinates):
         """
         :param input: string with xy-coordinates: 133/88 or 133/88,134/88
         :returns: object for xy geofabrik processing
         """
         self.o_geofabrik_json = GeofabrikJson()
 
         # use Geofabrik-URL to get the relevant tiles
-        self.wanted_maps = get_xy_coordinates_from_input(input_xy_coordinates)
+        self.wanted_maps = self.split_input_to_list(input_xy_coordinates)
 
     def get_tiles_of_wanted_map_single(self, wanted_map):
         """Overrides InformalGeofabrikInterface.get_tiles_of_wanted_map_single()"""
         # calc bounding box - the whole area to be created
         bbox = self.compose_bouding_box(wanted_map)
 
         # Build bounding box list of tiles - several X/Y combinations making up the area
@@ -276,14 +315,18 @@
         # convert X/Y combination to shape (multipolygon)
         wanted_region = self.compose_shape(bbox_tiles)
 
         # get all infos of these bounding box tiles
         tiles_of_input = self.find_needed_countries(
             bbox_tiles, wanted_map, wanted_region)
 
+        if len(tiles_of_input[0]['countries']) == 0:
+            raise XYCombinationHasNoCountries(
+                f'{wanted_map["x"]}/{wanted_map["y"]}')
+
         return tiles_of_input
 
     def find_needed_countries(self, bbox_tiles, wanted_map, wanted_region_polygon) -> dict:
         """Overrides InformalGeofabrikInterface.find_needed_countries()"""
         output = []
 
         geofabrik_regions = self.o_geofabrik_json.geofabrik_regions
@@ -291,16 +334,15 @@
         log.info('Searching for needed maps, this can take a while.')
 
         # itterate through tiles and find Geofabrik regions that are in the tiles
         counter = 1
         for tile in bbox_tiles:
             # Do progress indicator every 50 tiles
             if counter % 50 == 0:
-                log.info(
-                    'Processing tile %s of %s', counter, len(bbox_tiles)+1)
+                self.log_tile(counter, len(bbox_tiles)+1)
             counter += 1
 
             parent_added = 0
             force_added = 0
 
             # example contents of tile: {'index': 0, 'x': 130, 'y': 84, 'tile_left': 2.8125,
             # 'tile_top': 52.48278022207821, 'tile_right': 4.21875, 'tile_bottom': 51.6180165487737}
@@ -361,14 +403,33 @@
     def compose_shape(self, bbox_tiles):
         coords = [(bbox_tiles[0]["tile_top"], bbox_tiles[0]["tile_left"]), (bbox_tiles[0]["tile_top"], bbox_tiles[0]["tile_right"]),
                   (bbox_tiles[0]["tile_bottom"], bbox_tiles[0]["tile_right"]), (bbox_tiles[0]["tile_bottom"], bbox_tiles[0]["tile_left"])]
         coords_polygon = Polygon(coords)
         wanted_region = shape(coords_polygon)
         return wanted_region
 
+    @staticmethod
+    def split_input_to_list(input_value) -> list:
+        """
+        extract/split x/y combinations by given X/Y coordinates.
+        input should be "188/88" or for multiple values "188/88,100/10,109/99".
+        returns a list of x/y combinations as integers
+        """
+        xy_combinations = []
+
+        # split by "," first for multiple x/y combinations, then by "/" for x and y value
+        for xy_coordinate in input_value.split(","):
+            splitted = xy_coordinate.split("/")
+
+            if len(splitted) == 2:
+                xy_combinations.append(
+                    {"x": int(splitted[0]), "y": int(splitted[1])})
+
+        return xy_combinations
+
 
 def calc_bounding_box_tiles(bbox):
     bbox_tiles = []
     for x_value in range(bbox['top_x'], bbox['bot_x'] + 1):
         for y_value in range(bbox['top_y'], bbox['bot_y'] + 1):
             (tile_top, tile_left) = num2deg(x_value, y_value)
             (tile_bottom, tile_right) = num2deg(x_value+1, y_value+1)
@@ -411,43 +472,7 @@
     Convert tile numbers to lon./lat.
     """
     n = 2.0 ** zoom
     lon_deg = xtile / n * 360.0 - 180.0
     lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * ytile / n)))
     lat_deg = math.degrees(lat_rad)
     return (lat_deg, lon_deg)
-
-
-def get_countries_from_input(input_countries):
-    """
-    extract/split x/y combinations by given X/Y coordinates.
-    input should be "188/88" or for multiple values "188/88,100/10,109/99".
-    returns a list of x/y combinations as integers
-    """
-
-    countries = []
-
-    # split by "," first for multiple x/y combinations, then by "/" for x and y value
-    for country in input_countries.split(","):
-        countries.append(country)
-
-    return countries
-
-
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
```

### Comparing `wahoomc-4.0.0a9/wahoomc/geofabrik_json.py` & `wahoomc-4.0.1/wahoomc/geofabrik_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 # import custom python packages
 from wahoomc.constants import GEOFABRIK_PATH
 
 
 class CountyIsNoGeofabrikCountry(Exception):
     """Raised when actual country is not a geofabrik country"""
 
+    def __init__(self, country):
+        message = f"Entered country '{country}' is not a geofabrik country. \
+                \nPlease check this URL for possible countries: https://download.geofabrik.de/index.html"
+        super().__init__(message)
+
 
 class GeofabrikJson:
     """
     This is a Geofabrik .json processing class for constants in the Geofabrik .json file
     """
     raw_json = None
     geofabrik_overview = {}
@@ -66,48 +71,44 @@
                     'pbf_url': pbf_url}
                 geofabrik_regions.append(id_no)
 
         return raw_json, geofabrik_overview, geofabrik_region_overview, geofabrik_regions
 
     def get_geofabrik_parent_country(self, id_no):
         """
-        Get the parent map/region of a region from the already loaded json data
+        Get the parent map/region of a country from the already loaded json data
         """
-        id_no_translated = self.translate_id_no_to_geofabrik(id_no)
-
         try:
-            entry = self.geofabrik_overview[id_no_translated]
+            entry = self.geofabrik_overview[id_no]
             if 'parent' in entry:
-                return (entry['parent'], id_no_translated)
+                return (entry['parent'], id_no)
 
-            return ('', id_no_translated)
-        except KeyError:
-            return None, None
+            return ('', id_no)
+        except KeyError as exception:
+            raise CountyIsNoGeofabrikCountry(id_no) from exception
 
     def get_geofabrik_url(self, id_no):
         """
-        Get the map download url from a region with the already loaded json data
+        Get the map download url from a country/region with the already loaded json data
         """
-        id_no_translated = self.translate_id_no_to_geofabrik(id_no)
         try:
-            entry = self.geofabrik_overview[id_no_translated]
+            entry = self.geofabrik_overview[id_no]
             if 'pbf_url' in entry:
                 return entry['pbf_url']
         except KeyError:
             pass
 
         return None
 
     def get_geofabrik_geometry(self, id_no):
         """
-        Get the geometry from a region with the already loaded json data
+        Get the geometry from a country/region with the already loaded json data
         """
-        id_no_translated = self.translate_id_no_to_geofabrik(id_no)
         try:
-            entry = self.geofabrik_overview[id_no_translated]
+            entry = self.geofabrik_overview[id_no]
             if 'geometry' in entry:
                 return entry['geometry']
         except KeyError:
             pass
 
         return None
 
@@ -131,8 +132,8 @@
         if country.replace('_', '-') in self.geofabrik_overview:
             return country.replace('_', '-')
 
         if 'us/'+country.replace('_', '-') in self.geofabrik_overview:
             return 'us/'+country.replace('_', '-')
 
         # if none of them got triggert --> exception
-        raise CountyIsNoGeofabrikCountry
+        raise CountyIsNoGeofabrikCountry(country)
```

### Comparing `wahoomc-4.0.0a9/wahoomc/input.py` & `wahoomc-4.0.1/wahoomc/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # for gui
 import tkinter as tk
 from tkinter import ttk
 
 # import custom python packages
 from wahoomc.geofabrik_json import GeofabrikJson
 from wahoomc.geofabrik_json import CountyIsNoGeofabrikCountry
-from wahoomc.geofabrik import get_countries_from_input
+from wahoomc.geofabrik import CountryGeofabrik
 
 
 def process_call_of_the_tool():
     """
     process CLI arguments
     """
     # input argument creation and processing
@@ -55,14 +55,17 @@
         title='Options', description='Options for map generation')
     # Maximum age of source maps or land shape files before they are redownloaded
     options_args.add_argument('-md', '--maxdays', type=int, default=InputData().max_days_old,
                               help="maximum age of source maps and other files")
     # Do not calculate border countries of input country
     options_args.add_argument('-nbc', '--bordercountries', action='store_false',
                               help="do not process border countries of tiles involving more than one country")
+    # calculate contour lines
+    options_args.add_argument('-con', '--contour', action='store_true',
+                              help="process contour lines (elevation data)")
     # Force download of source maps and the land shape file
     # If False use Max_Days_Old to check for expired maps
     # If True force redownloading of maps and landshape
     options_args.add_argument('-fd', '--forcedownload', action='store_true',
                               help="force download of files")
     # Force (re)processing of source maps and the land shape file
     # If False only process files if not existing
@@ -96,14 +99,16 @@
     # cli processing
     o_input_data = InputData()
     o_input_data.country = args.country
     o_input_data.xy_coordinates = args.xy_coordinates
     o_input_data.max_days_old = args.maxdays
 
     o_input_data.process_border_countries = args.bordercountries
+    o_input_data.contour = args.contour
+
     o_input_data.force_download = args.forcedownload
     o_input_data.force_processing = args.forceprocessing
 
     o_input_data.tag_wahoo_xml = args.tag_wahoo_xml
     o_input_data.save_cruiser = args.cruiser
     o_input_data.zip_folder = args.zip
 
@@ -175,14 +180,15 @@
         self.country = ""
         self.xy_coordinates = ""
         self.max_days_old = 14
 
         self.force_download = False
         self.force_processing = False
         self.process_border_countries = True
+        self.contour = False
         self.save_cruiser = False
 
         self.tag_wahoo_xml = "tag-wahoo-poi.xml"
 
         self.zip_folder = False
         self.verbose = False
 
@@ -201,22 +207,18 @@
             else:
                 sys.exit()
         elif self.country and self.xy_coordinates:
             sys.exit(
                 "Country and X/Y coordinates are given. Only one of both is allowed!")
         elif self.country:
             # countries =
-            for country in get_countries_from_input(self.country):
-                try:
-                    country = GeofabrikJson().translate_id_no_to_geofabrik(
-                        country)
-                except CountyIsNoGeofabrikCountry:
-                    sys.exit(
-                        f"Entered country '{country}' is not a geofabrik country. Please check this URL for possible countries \
-                            https://download.geofabrik.de/index.html!")
+            try:
+                CountryGeofabrik.split_input_to_list(self.country)
+            except CountyIsNoGeofabrikCountry as exception:
+                sys.exit(exception)
 
             # if we made it until here, sys.exit() was not called and therefore all countries OK ;-)
             return True
         else:
             return True
 
 
@@ -294,14 +296,15 @@
 
         self.o_input_data.country = tab1.first.cb_country.get()
         self.o_input_data.max_days_old = int(tab1.first.input_maxdays.get())
 
         self.o_input_data.force_download = tab1.third.checkb_download.get()
         self.o_input_data.force_processing = tab1.third.checkb_processing_val.get()
         self.o_input_data.process_border_countries = tab1.third.checkb_border_countries_val.get()
+        self.o_input_data.contour = tab1.third.checkb_contour_val.get()
 
         self.o_input_data.save_cruiser = tab2.first.checkb_save_cruiser_val.get()
         self.o_input_data.zip_folder = tab2.first.checkb_zip_folder_val.get()
         self.o_input_data.verbose = tab2.first.checkb_verbose_val.get()
 
         # get text without \n in the end
         self.o_input_data.tag_wahoo_xml = tab2.second.input_tag_wahoo_xml.get()
@@ -390,18 +393,21 @@
         self.chk_force_download = tk.Checkbutton(self, text="Force download",
                                                  var=self.checkb_download)
         self.chk_force_download.bind(
             "<Button-1>", self.controller.switch_reload)
 
         self.checkb_border_countries_val = create_checkbox(self, oInputData.process_border_countries,
                                                            "Process border countries", 0)
+        self.checkb_contour_val = create_checkbox(self, oInputData.verbose,
+                                                  "process contour lines (elevation data)", 1)
+
         self.chk_force_download.grid(
-            column=0, row=1, sticky=tk.W, padx=15, pady=5)
+            column=0, row=2, sticky=tk.W, padx=15, pady=5)
         self.checkb_processing_val = create_checkbox(self, oInputData.force_processing,
-                                                     "Force processing", 2)
+                                                     "Force processing", 3)
 
 
 class Buttons(tk.Frame):
     """
     Buttons for GUI
     """
```

### Comparing `wahoomc-4.0.0a9/wahoomc/main.py` & `wahoomc-4.0.1/wahoomc/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import logging
 
 # import custom python packages
 from wahoomc.input import process_call_of_the_tool, cli_init
 from wahoomc.setup_functions import initialize_work_directories, \
     check_installation_of_required_programs, write_config_file, \
     adjustments_due_to_breaking_changes, copy_jsons_from_repo_to_user, \
-    check_installed_version_against_latest_pypi
+    check_installed_version_against_latest_pypi, check_installation_of_programs_credentials_for_contour_lines
 from wahoomc.downloader import download_tooling
 
 from wahoomc.osm_maps_functions import OsmMaps
-from wahoomc.osm_maps_functions import OsmData
+from wahoomc.osm_maps_functions import CountryOsmData, XYOsmData
 
 # logging used in the terminal output:
 # # means top-level command
 # ! means error
 # + means additional comment in a working-unit
 
 
@@ -51,17 +51,25 @@
     if run_level == 'init':
         copy_jsons_from_repo_to_user('tag_wahoo_adjusted')
         copy_jsons_from_repo_to_user('.', 'tags-to-keep.json')
     else:
         # Is there something to do?
         o_input_data.is_required_input_given_or_exit(issue_message=True)
 
-        o_osm_data = OsmData()
+        if o_input_data.contour:
+            check_installation_of_programs_credentials_for_contour_lines()
+
+        if o_input_data.country:
+            o_osm_data = CountryOsmData(o_input_data)
+        elif o_input_data.xy_coordinates:
+            o_osm_data = XYOsmData(o_input_data)
+
         # Check for not existing or expired files. Mark for download, if dl is needed
-        o_downloader = o_osm_data.process_input_of_the_tool(o_input_data)
+        o_osm_data.process_input_of_the_tool()
+        o_downloader = o_osm_data.get_downloader()
 
         # Download files marked for download
         o_downloader.download_files_if_needed()
 
         o_osm_maps = OsmMaps(o_osm_data)
 
         # Filter tags from country osm.pbf files'
@@ -69,14 +77,18 @@
 
         # Generate land
         o_osm_maps.generate_land()
 
         # Generate sea
         o_osm_maps.generate_sea()
 
+        # Generate elevation
+        if o_input_data.contour:
+            o_osm_maps.generate_elevation()
+
         # Split filtered country files to tiles
         o_osm_maps.split_filtered_country_files_to_tiles()
 
         # Merge splitted tiles with land an sea
         o_osm_maps.merge_splitted_tiles_with_land_and_sea(
             o_input_data.process_border_countries)
```

### Comparing `wahoomc-4.0.0a9/wahoomc/osm_maps_functions.py` & `wahoomc-4.0.1/wahoomc/osm_maps_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,209 +11,280 @@
 import subprocess
 import sys
 import platform
 import shutil
 import logging
 
 # import custom python packages
-from wahoomc.file_directory_functions import read_json_file, create_empty_directories, write_json_file_generic
+from wahoomc.file_directory_functions import read_json_file_country_config, create_empty_directories, write_json_file_generic
 from wahoomc.constants_functions import translate_tags_to_keep, \
     get_tooling_win_path, get_tag_wahoo_xml_path, TagWahooXmlNotFoundError
 
+from wahoomc.setup_functions import read_earthexplorer_credentials
+
 from wahoomc.constants import USER_WAHOO_MC
 from wahoomc.constants import USER_OUTPUT_DIR
 from wahoomc.constants import RESOURCES_DIR
 from wahoomc.constants import LAND_POLYGONS_PATH
 from wahoomc.constants import VERSION
 from wahoomc.constants import OSMOSIS_WIN_FILE_PATH
+from wahoomc.constants import USER_DL_DIR
 
 from wahoomc.downloader import Downloader
-from wahoomc.geofabrik import CountryGeofabrik, XYGeofabrik
+from wahoomc.geofabrik import CountryGeofabrik, XYCombinationHasNoCountries, XYGeofabrik
 
 log = logging.getLogger('main-logger')
 
 
-class TileNotFoundError(Exception):
-    """Raised when no tile is found for x/y combination"""
-
-
 def run_subprocess_and_log_output(cmd, error_message, cwd=""):
     """
     run given cmd-subprocess and issue error message if wished
     """
     if not cwd:
-        with subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) as process:
-            for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
-                try:
-                    log.debug('subprocess:%r', line.decode("utf-8").strip())
-                except UnicodeDecodeError:
-                    log.debug('subprocess:%r', line.decode("latin-1").strip())
+        process = subprocess.Popen(
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     else:
-        with subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd) as process:
-            for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
-                try:
-                    log.debug('subprocess:%r', line.decode("utf-8").strip())
-                except UnicodeDecodeError:
-                    log.debug('subprocess:%r', line.decode("latin-1").strip())
+        process = subprocess.Popen(  # pylint: disable=consider-using-with
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd)
 
     if error_message and process.wait() != 0:  # 0 means success
+        for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
+            # print(line.rstrip())
+            try:
+                log.error('subprocess:%r', line.decode("utf-8").strip())
+            except UnicodeDecodeError:
+                log.error('subprocess:%r', line.decode("latin-1").strip())
+
         log.error(error_message)
         sys.exit()
 
+    else:
+        for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
+            # print(line.rstrip())
+            try:
+                log.debug('subprocess:%r', line.decode("utf-8").strip())
+            except UnicodeDecodeError:
+                log.debug('subprocess:%r', line.decode("latin-1").strip())
+
 
 def get_timestamp_last_changed(file_path):
     """
     returns the timestamp of the last-changed datetime of the given file
     """
     chg_time = os.path.getmtime(file_path)
 
     return datetime.fromtimestamp(chg_time).isoformat()
 
 
-class OsmData():  # pylint: disable=too-few-public-methods
+class InformalOsmDataInterface:
     """
     object with all internal parameters to process maps
     """
 
-    def __init__(self):
+    def __init__(self, o_input_data):
         """
-        xxx
+        steps in constructor:
+        1. take over input paramters (force_processing is changed in the function further down)
+        2. check + download geofabrik file (always)
         """
         self.force_processing = False
         self.tiles = []
         self.border_countries = {}
         self.country_name = ''
 
-    def process_input_of_the_tool(self, o_input_data):
-        """
-        Process input: get relevant tiles and if border countries should be calculated
-        The three primary inputs are giving by a separate value each and have separate processing:
-        1. country name
-        2. x/y combinations
-
-        # Check for not existing or expired files. Mark for download, if dl is needed
-        # - land polygons file
-        # - .osm.pbf files
-
-        steps in this function:
-        1. take over input paramters (force_processing is changed in the function further down)
-        2. check + download geofabrik file if geofabrik-processing
-        3. calculate relevant tiles for map creation
-        4. calculate border countries for map creation
-        5. evaluate the country-name for folder cration during processing
-        6. calculate if force_processing should be set to true
-        """
-
-        o_downloader = Downloader(
+        self.o_downloader = Downloader(
             o_input_data.max_days_old, o_input_data.force_download, self.border_countries)
         # takeover what is given by user first for force_processing
         self.force_processing = o_input_data.force_processing
+        self.process_border_countries = o_input_data.process_border_countries
 
         log.info('-' * 80)
 
         # geofabrik file
-        if o_downloader.should_geofabrik_file_be_downloaded():
+        if self.o_downloader.should_geofabrik_file_be_downloaded():
             self.force_processing = True
-            o_downloader.download_geofabrik_file()
+            self.o_downloader.download_geofabrik_file()
 
-        # calc tiles
-        if o_input_data.country:
-            o_geofabrik = self.calc_tiles_country(o_input_data)
-        elif o_input_data.xy_coordinates:
-            self.calc_tiles_xy(o_input_data)
+    def process_input_of_the_tool(self):
+        """
+        Process input: get relevant tiles and if border countries should be calculated
+        The three primary inputs are giving by a separate value each and have separate processing:
+        1. country name
+        2. x/y combinations
+        """
 
-        # calc border countries
-        log.info('-' * 80)
-        if o_input_data.country:
-            self.calc_border_countries_country(o_input_data, o_geofabrik)
-        elif o_input_data.xy_coordinates:
-            self.calc_border_countries()
-        # log border countries when and when not calculated to output the processed country(s)
-        self.log_border_countries()
+    def calc_tiles(self):
+        """
+        calculate relevant tiles for input country or xy coordinate
+        """
 
-        # calc country name
-        if o_input_data.country:
-            # country name is the input argument
-            self.country_name = o_input_data.country
-        elif o_input_data.xy_coordinates:
-            self.calc_country_name_xy()
+    def calc_border_countries(self):
+        """
+        calculate the border countries for the given tiles. i.e.
+        - if CLI/GUI input by user
+        - if processing x/y coordinates
+        """
+        log.info('# Determine involved/border countries')
 
+        # Build list of countries needed
+        for tile in self.tiles:
+            for country in tile['countries']:
+                if country not in self.border_countries:
+                    self.border_countries[country] = {}
+
+    def log_border_countries(self):
+        """
+        write calculated border countries/involved countries to log
+        """
+        for country in self.border_countries:
+            log.info('+ Involved country: %s', country)
+
+        # input can be only one country, if there are more than one,
+        # border countries must be selected
+        if len(self.border_countries) > 1:
+            log.info('+ Border countries will be processed')
+
+    def get_downloader(self):
+        """
+        steps in this function:
+        1. Check for not existing or expired files. Mark for download, if dl is needed
+        - land polygons file
+        - .osm.pbf files
+        2. Calculate if force_processing should be set to true
+        """
         # calc force processing
         # Check for not existing or expired files. Mark for download, if dl is needed
-        o_downloader.check_land_polygons_file()
-        o_downloader.check_osm_pbf_file()
+        self.o_downloader.check_land_polygons_file()
+        self.o_downloader.check_osm_pbf_file()
 
         # If one of the files needs to be downloaded, reprocess all files
-        if o_downloader.need_to_dl:
+        if self.o_downloader.need_to_dl:
             self.force_processing = True
 
-        return o_downloader
+        return self.o_downloader
+
+
+class CountryOsmData(InformalOsmDataInterface):
+    """
+    object with all internal parameters to process maps for countries
+    """
+
+    def __init__(self, o_input_data):
+        super().__init__(o_input_data)
+        self.input_country = o_input_data.country
+
+        self.o_geofabrik = CountryGeofabrik(self.input_country)
 
-    def calc_tiles_country(self, o_input_data):
+    def process_input_of_the_tool(self):
         """
-        option 1: input a country as parameter, e.g. germany
+        steps in this function:
+        1. calculate relevant tiles for map creation
+        2. calculate border countries for map creation
+        3. evaluate the country-name for folder cration during processing
         """
-        log.info('# Input country: %s.', o_input_data.country)
 
-        # use Geofabrik-URL to calculate the relevant tiles
-        o_geofabrik = CountryGeofabrik(o_input_data.country)
-        self.tiles = o_geofabrik.get_tiles_of_wanted_map()
+        # calc tiles
+        self.calc_tiles()
+
+        # calc border countries
+        log.info('-' * 80)
+        self.calc_border_countries()
+        # log border countries when and when not calculated to output the processed country(s)
+        self.log_border_countries()
 
-        return o_geofabrik
+        # calc country name
+        self.calc_country_name()
 
-    def calc_tiles_xy(self, o_input_data):
+    def calc_tiles(self):
         """
-        option 2: input a x/y combinations as parameter, e.g. 134/88  or 133/88,130/100
+        option 1: input a country as parameter, e.g. germany
         """
-        log.info(
-            '# Input X/Y coordinates: %s.', o_input_data.xy_coordinates)
+        log.info('# Input country: %s.', self.input_country)
 
-        o_geofabrik = XYGeofabrik(o_input_data.xy_coordinates)
-        # find the tiles for  x/y combinations in the geofabrik json files
-        self.tiles = o_geofabrik.get_tiles_of_wanted_map()
+        # use Geofabrik-URL to calculate the relevant tiles
+        self.tiles = self.o_geofabrik.get_tiles_of_wanted_map()
 
-    def calc_border_countries_country(self, o_input_data, o_geofabrik):
+    def calc_border_countries(self):
         """
         calculate the border countries for the given tiles when input is a country
         - if CLI/GUI input by user
         """
-        if o_input_data.process_border_countries:
-            self.calc_border_countries()
+        if self.process_border_countries:
+            super().calc_border_countries()
         # set the to-be-processed country as border country
         else:
-            for country in o_geofabrik.wanted_maps:
+            for country in self.o_geofabrik.wanted_maps:
                 self.border_countries[country] = {}
 
-    def calc_border_countries(self):
+    def calc_country_name(self):
         """
-        calculate the border countries for the given tiles. i.e.
-        - if CLI/GUI input by user
-        - if processing x/y coordinates
+        country name is the country
+        >1 countries are separated by underscore
         """
-        log.info('# Determine involved/border countries')
+        for country in self.o_geofabrik.wanted_maps:
+            if not self.country_name:
+                self.country_name = country
+            else:
+                self.country_name = f'{self.country_name}_{country}'
 
-        # Build list of countries needed
-        for tile in self.tiles:
-            for country in tile['countries']:
-                if country not in self.border_countries:
-                    self.border_countries[country] = {}
 
-    def log_border_countries(self):
+class XYOsmData(InformalOsmDataInterface):
+    """
+    object with all internal parameters to process maps for XY coordinates
+    """
+
+    def __init__(self, o_input_data):
+        super().__init__(o_input_data)
+        self.input_xy_coordinates = o_input_data.xy_coordinates
+
+    def process_input_of_the_tool(self):
         """
-        write calculated border countries/involved countries to log
+        Process input: get relevant tiles and if border countries should be calculated
+        The three primary inputs are giving by a separate value each and have separate processing:
+        1. country name
+        2. x/y combinations
+
+        # Check for not existing or expired files. Mark for download, if dl is needed
+        # - land polygons file
+        # - .osm.pbf files
+
+        steps in this function:
+        1. calculate relevant tiles for map creation
+        2. calculate border countries for map creation
+        3. evaluate the country-name for folder cration during processing
         """
-        for country in self.border_countries:
-            log.info('+ Involved country: %s', country)
 
-        # input can be only one country, if there are more than one,
-        # border countries must be selected
-        if len(self.border_countries) > 1:
-            log.info('+ Border countries will be processed')
+        # calc tiles
+        self.calc_tiles()
+
+        # calc border countries
+        log.info('-' * 80)
+        self.calc_border_countries()
+        # log border countries when and when not calculated to output the processed country(s)
+        self.log_border_countries()
 
-    def calc_country_name_xy(self):
+        # calc country name
+        self.calc_country_name()
+
+    def calc_tiles(self):
+        """
+        option 2: input a x/y combinations as parameter, e.g. 134/88  or 133/88,130/100
+        """
+        log.info(
+            '# Input X/Y coordinates: %s.', self.input_xy_coordinates)
+
+        o_geofabrik = XYGeofabrik(self.input_xy_coordinates)
+        # find the tiles for  x/y combinations in the geofabrik json files
+        try:
+            self.tiles = o_geofabrik.get_tiles_of_wanted_map()
+        except XYCombinationHasNoCountries as exception:
+            # this exception is actually only raised in class XYGeofabrik
+            sys.exit(exception)
+
+    def calc_country_name(self):
         """
         country name is the X/Y combinations separated by minus
         >1 x/y combinations are separated by underscore
         """
         for tile in self.tiles:
             if not self.country_name:
                 self.country_name = f'{tile["x"]}-{tile["y"]}'
@@ -367,16 +438,15 @@
             land_file = os.path.join(USER_OUTPUT_DIR,
                                      f'{tile["x"]}', f'{tile["y"]}', 'land.shp')
             out_file_land1 = os.path.join(USER_OUTPUT_DIR,
                                           f'{tile["x"]}', f'{tile["y"]}', 'land')
 
             # create land.dbf, land.prj, land.shp, land.shx
             if not os.path.isfile(land_file) or self.o_osm_data.force_processing is True:
-                log.info(
-                    '+ Coordinates: %s,%s. (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
+                self.log_tile(tile["x"], tile["y"], tile_count)
                 cmd = ['ogr2ogr', '-overwrite', '-skipfailures']
                 # Try to prevent getting outside of the +/-180 and +/- 90 degrees borders. Normally the +/- 0.1 are there to prevent white lines at border borders.
                 if tile["x"] == 255 or tile["y"] == 255 or tile["x"] == 0 or tile["y"] == 0:
                     cmd.extend(['-spat', f'{tile["left"]:.6f}',
                                 f'{tile["bottom"]:.6f}',
                                 f'{tile["right"]:.6f}',
                                 f'{tile["top"]:.6f}'])
@@ -418,16 +488,15 @@
         log.info('# Generate sea for each coordinate')
 
         tile_count = 1
         for tile in self.o_osm_data.tiles:
             out_file_sea = os.path.join(USER_OUTPUT_DIR,
                                         f'{tile["x"]}', f'{tile["y"]}', 'sea.osm')
             if not os.path.isfile(out_file_sea) or self.o_osm_data.force_processing is True:
-                log.info(
-                    '+ Coordinates: %s,%s. (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
+                self.log_tile(tile["x"], tile["y"], tile_count)
                 with open(os.path.join(RESOURCES_DIR, 'sea.osm'), encoding="utf-8") as sea_file:
                     sea_data = sea_file.read()
 
                     # Try to prevent getting outside of the +/-180 and +/- 90 degrees borders. Normally the +/- 0.1 are there to prevent white lines at tile borders
                     if tile["x"] == 255 or tile["y"] == 255 or tile["x"] == 0 or tile["y"] == 0:
                         sea_data = sea_data.replace(
                             '$LEFT', f'{tile["left"]:.6f}')
@@ -449,29 +518,69 @@
 
                     with open(out_file_sea, mode='w', encoding="utf-8") as output_file:
                         output_file.write(sea_data)
             tile_count += 1
 
         log.info('+ Generate sea for each coordinate: OK')
 
+    def generate_elevation(self):
+        """
+        Generate contour lines for all tiles
+        """
+        username, password = read_earthexplorer_credentials()
+
+        log.info('-' * 80)
+        log.info('# Generate contour lines for each coordinate')
+
+        hgt_path = os.path.join(USER_DL_DIR, 'hgt')
+
+        tile_count = 1
+        for tile in self.o_osm_data.tiles:
+            out_file_elevation = os.path.join(
+                USER_OUTPUT_DIR, f'{tile["x"]}', f'{tile["y"]}', 'elevation')
+            # as the elevation file has a suffix, they need to be searched with glob.glob
+            # example elevation filename: elevation_lon14.06_15.47lat35.46_36.60_view1,view3.osm
+            out_file_elevation_existing = glob.glob(os.path.join(
+                USER_OUTPUT_DIR, str(tile["x"]), str(tile["y"]), 'elevation*.osm'))
+            # check for already existing elevation .osm file (the ones matched via glob)
+            if not (len(out_file_elevation_existing) == 1 and os.path.isfile(out_file_elevation_existing[0])) \
+                    or self.o_osm_data.force_processing is True:
+                log.info(
+                    '+ Coordinates: %s,%s. (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
+                cmd = ['phyghtmap']
+                cmd.append('-a ' + f'{tile["left"]}' + ':' + f'{tile["bottom"]}' +
+                           ':' + f'{tile["right"]}' + ':' + f'{tile["top"]}')
+                cmd.extend(['-o', f'{out_file_elevation}', '-s 10', '-c 100,50', '--source=srtm1,view1,view3,srtm3',
+                            '--jobs=8', '--viewfinder-mask=1', '--start-node-id=20000000000',
+                            '--max-nodes-per-tile=0', '--start-way-id=2000000000', '--write-timestamp',
+                            '--no-zero-contour', '--hgtdir=' + hgt_path])
+                cmd.append('--earthexplorer-user=' + username)
+                cmd.append('--earthexplorer-password=' + password)
+
+                run_subprocess_and_log_output(
+                    cmd, f'! Error in phyghtmap with tile: {tile["x"]},{tile["y"]}. Win_macOS/elevation')
+
+            tile_count += 1
+
+        log.info('+ Generate contour lines for each coordinate: OK')
+
     def split_filtered_country_files_to_tiles(self):
         """
         Split filtered country files to tiles
         """
 
         log.info('-' * 80)
         log.info('# Split filtered country files to tiles')
         tile_count = 1
         for tile in self.o_osm_data.tiles:
 
             for country, val in self.o_osm_data.border_countries.items():
                 if country not in tile['countries']:
                     continue
-                log.info(
-                    '+ Coordinates: %s,%s / %s (%s of %s)', tile["x"], tile["y"], country, tile_count, len(self.o_osm_data.tiles))
+                self.log_tile(tile["x"], tile["y"], tile_count, country)
                 out_file = os.path.join(USER_OUTPUT_DIR,
                                         f'{tile["x"]}', f'{tile["y"]}', f'split-{country}.osm.pbf')
                 out_file_names = os.path.join(USER_OUTPUT_DIR,
                                               f'{tile["x"]}', f'{tile["y"]}', f'split-{country}-names.osm.pbf')
 
                 # split filtered country files to tiles every time because the result is different per constants (user input)
                 # Windows
@@ -526,30 +635,32 @@
 
             tile_count += 1
 
         log.info('+ Split filtered country files to tiles: OK')
 
     def merge_splitted_tiles_with_land_and_sea(self, process_border_countries):
         """
-        Merge splitted tiles with land an sea
+        Merge splitted tiles with land elevation and sea
         """
 
         log.info('-' * 80)
-        log.info('# Merge splitted tiles with land an sea')
+        log.info('# Merge splitted tiles with land, elevation and sea')
         tile_count = 1
         for tile in self.o_osm_data.tiles:  # pylint: disable=too-many-nested-blocks
-            log.info(
-                '+ Coordinates: %s,%s (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
+            self.log_tile(tile["x"], tile["y"], tile_count)
 
             out_tile_dir = os.path.join(USER_OUTPUT_DIR,
                                         f'{tile["x"]}', f'{tile["y"]}')
             out_file_merged = os.path.join(out_tile_dir, 'merged.osm.pbf')
 
             land_files = glob.glob(os.path.join(out_tile_dir, 'land*.osm'))
 
+            elevation_files = glob.glob(
+                os.path.join(out_tile_dir, 'elevation*.osm'))
+
             # merge splitted tiles with land and sea every time because the result is different per constants (user input)
             # sort land* osm files
             self.sort_osm_files(tile)
 
             # Windows
             if platform.system() == "Windows":
                 cmd = [OSMOSIS_WIN_FILE_PATH]
@@ -577,25 +688,29 @@
 
                     loop += 1
 
             for land in land_files:
                 cmd.extend(
                     ['--rx', 'file='+land, '--s', '--m'])
 
+            for elevation in elevation_files:
+                cmd.extend(
+                    ['--rx', 'file='+elevation, '--s', '--m'])
+
             cmd.extend(
                 ['--rx', 'file='+os.path.join(out_tile_dir, 'sea.osm'), '--s', '--m'])
             cmd.extend(['--tag-transform', 'file=' + os.path.join(RESOURCES_DIR,
                                                                   'tunnel-transform.xml'), '--wb', out_file_merged, 'omitmetadata=true'])
 
             run_subprocess_and_log_output(
                 cmd, f'! Error in Osmosis with tile: {tile["x"]},{tile["y"]}')
 
             tile_count += 1
 
-        log.info('+ Merge splitted tiles with land an sea: OK')
+        log.info('+ Merge splitted tiles with land, elevation and sea: OK')
 
     def sort_osm_files(self, tile):
         """
         sort land*.osm files to be in this order: nodes, then ways, then relations.
         this is mandatory for osmium-merge since:
         https://github.com/osmcode/osmium-tool/releases/tag/v1.13.2
         """
@@ -633,16 +748,15 @@
         # Number of threads to use in the mapwriter plug-in
         threads = multiprocessing.cpu_count() - 1
         if int(threads) < 1:
             threads = 1
 
         tile_count = 1
         for tile in self.o_osm_data.tiles:
-            log.info(
-                '+ Coordinates: %s,%s (%s of %s)', tile["x"], tile["y"], tile_count, len(self.o_osm_data.tiles))
+            self.log_tile(tile["x"], tile["y"], tile_count)
 
             out_file_map = os.path.join(USER_OUTPUT_DIR,
                                         f'{tile["x"]}', f'{tile["y"]}.map')
 
             # apply tag-wahoo xml every time because the result is different per .xml file (user input)
             merged_file = os.path.join(USER_OUTPUT_DIR,
                                        f'{tile["x"]}', f'{tile["y"]}', 'merged.osm.pbf')
@@ -799,15 +913,15 @@
     def tags_are_identical_to_last_run(self, country):
         """
         compare tags of this run with used tags from last run stored in _tiles/{country} directory
         """
         tags_are_identical = True
 
         try:
-            country_config = read_json_file(os.path.join(
+            country_config = read_json_file_country_config(os.path.join(
                 USER_OUTPUT_DIR, country, ".config.json"))
             if not country_config["tags_last_run"] == translate_tags_to_keep(sys_platform=platform.system()) \
                     or not country_config["name_tags_last_run"] == translate_tags_to_keep(name_tags=True, sys_platform=platform.system()):
                 tags_are_identical = False
         except (FileNotFoundError, KeyError):
             tags_are_identical = False
 
@@ -816,15 +930,26 @@
     def last_changed_is_identical_to_last_run(self, country):
         """
         compare tags of this run with used tags from last run stored in _tiles/{country} directory
         """
         last_changed_is_identical = True
 
         try:
-            country_config = read_json_file(os.path.join(
+            country_config = read_json_file_country_config(os.path.join(
                 USER_OUTPUT_DIR, country, ".config.json"))
             if not country_config["changed_ts_map_last_run"] == get_timestamp_last_changed(self.o_osm_data.border_countries[country]['map_file']):
                 last_changed_is_identical = False
         except (FileNotFoundError, KeyError):
             last_changed_is_identical = False
 
         return last_changed_is_identical
+
+    def log_tile(self, tile_x, tile_y, tile_count, additional_info=''):
+        """
+        unified status logging for this class
+        """
+        if additional_info:
+            log.info('+ (tile %s of %s) Coordinates: %s,%s / %s', tile_count, len(self.o_osm_data.tiles), tile_x,
+                     tile_y, additional_info)
+        else:
+            log.info('+ (tile %s of %s) Coordinates: %s,%s',
+                     tile_count, len(self.o_osm_data.tiles), tile_x, tile_y)
```

### Comparing `wahoomc-4.0.0a9/wahoomc/resources/sea.osm` & `wahoomc-4.0.1/wahoomc/resources/sea.osm`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/resources/shape2osm.py` & `wahoomc-4.0.1/wahoomc/resources/shape2osm.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml` & `wahoomc-4.0.1/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml`

 * *Files 22% similar despite different names*

#### Comparing `wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml` & `wahoomc-4.0.1/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml`

```diff
@@ -1,113 +1,128 @@
 <?xml version="1.0" encoding="utf-8"?>
 <tag-mapping xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://mapsforge.org/tag-mapping" default-zoom-appear="16" profile-name="default-profile" xsi:schemaLocation="http://mapsforge.org/tag-mapping https://raw.githubusercontent.com/mapsforge/mapsforge/master/resources/tag-mapping.xsd">
   <!-- ************* POIS *************** -->
+  <!-- HIGHWAY TAGS -->
   <pois>
-    <osm-tag key="amenity" value="fuel" zoom-appear="14"/>
-    <osm-tag key="amenity" value="cafe" zoom-appear="14"/>
-    <osm-tag key="amenity" value="drinking_water" zoom-appear="14"/>
-    <osm-tag key="shop" value="bakery" zoom-appear="14"/>
-    <osm-tag key="shop" value="bicycle" zoom-appear="14"/>
-    <osm-tag key="railway" value="station" zoom-appear="13"/>
-    <osm-tag key="railway" value="stop" zoom-appear="13"/>
+    <osm-tag key="highway" value="mini_roundabout" zoom-appear="17"/>
+    <osm-tag key="highway" value="traffic_signals" zoom-appear="17"/>
+    <osm-tag key="highway" value="turning_circle" zoom-appear="15"/>
   </pois>
-  <ways>
-    <osm-tag key="amenity" label-position="true" value="fuel" zoom-appear="14"/>
-    <osm-tag key="amenity" label-position="true" value="cafe" zoom-appear="14"/>
-    <osm-tag key="amenity" label-position="true" value="drinking_water" zoom-appear="14"/>
-    <osm-tag key="shop" label-position="true" value="bakery" zoom-appear="14"/>
-    <osm-tag key="shop" label-position="true" value="bicycle" zoom-appear="14"/>
-    <osm-tag key="railway" label-position="true" value="station" zoom-appear="13"/>
-    <osm-tag key="railway" label-position="true" value="stop" zoom-appear="13"/>
-  </ways>
   <!-- PLACES TAGS -->
   <pois>
     <osm-tag key="place" value="city" zoom-appear="6"/>
-    <osm-tag key="place" value="hamlet" zoom-appear="10"/>
-    <osm-tag key="place" value="island" zoom-appear="10"/>
-    <osm-tag key="place" value="locality" zoom-appear="10"/>
-    <osm-tag key="place" value="suburb" zoom-appear="10"/>
-    <osm-tag key="place" value="town" zoom-appear="8"/>
-    <osm-tag key="place" value="village" zoom-appear="11"/>
+    <osm-tag key="place" value="country" zoom-appear="3"/>
+    <osm-tag key="place" value="hamlet" zoom-appear="13"/>
+    <osm-tag key="place" value="suburb" zoom-appear="12"/>
+    <osm-tag key="place" value="town" zoom-appear="9"/>
+    <osm-tag key="place" value="village" zoom-appear="12"/>
   </pois>
   <!-- ************* WAYS *************** -->
   <!-- HIGHWAY TAGS -->
   <ways>
-    <osm-tag key="highway" value="bridleway" zoom-appear="10"/>
-    <osm-tag key="highway" value="construction" zoom-appear="10"/>
-    <osm-tag key="highway" value="cycleway" zoom-appear="10"/>
-    <osm-tag key="highway" value="footway" zoom-appear="10"/>
-    <osm-tag key="highway" value="living_street" zoom-appear="10"/>
+    <osm-tag key="highway" value="bridleway" zoom-appear="13"/>
+    <osm-tag key="highway" value="construction" zoom-appear="13"/>
+    <osm-tag key="highway" value="cycleway" zoom-appear="13"/>
+    <osm-tag key="highway" value="footway" zoom-appear="13"/>
+    <osm-tag key="highway" value="living_street" zoom-appear="13"/>
     <osm-tag key="highway" value="motorway" zoom-appear="6"/>
-    <osm-tag key="highway" value="motorway_link" zoom-appear="10"/>
-    <osm-tag key="highway" value="path" zoom-appear="10"/>
-    <osm-tag key="highway" value="pedestrian" zoom-appear="10"/>
+    <osm-tag key="highway" value="motorway_link" zoom-appear="6"/>
+    <osm-tag key="highway" value="path" zoom-appear="14"/>
+    <osm-tag key="highway" value="pedestrian" zoom-appear="14"/>
     <osm-tag key="highway" value="primary" zoom-appear="8"/>
-    <osm-tag key="highway" value="primary_link" zoom-appear="10"/>
-    <osm-tag key="highway" value="residential" zoom-appear="10"/>
-    <osm-tag key="highway" value="road" zoom-appear="10"/>
-    <osm-tag key="highway" value="secondary" zoom-appear="10"/>
-    <osm-tag key="highway" value="secondary_link" zoom-appear="10"/>
-    <osm-tag key="highway" value="service" zoom-appear="10"/>
-    <osm-tag key="highway" value="steps" zoom-appear="10"/>
-    <osm-tag key="highway" value="tertiary" zoom-appear="10"/>
-    <osm-tag key="highway" value="tertiary_link" zoom-appear="10"/>
-    <osm-tag key="highway" value="track" zoom-appear="10"/>
-    <osm-tag key="highway" value="trunk" zoom-appear="8"/>
-    <osm-tag key="highway" value="trunk_link" zoom-appear="10"/>
-    <osm-tag key="highway" value="unclassified" zoom-appear="10"/>
-  </ways>
-  <!-- NATURAL / WATERWAY TAGS -->
-  <ways>
-    <osm-tag key="natural" value="nosea" zoom-appear="3"/>
-    <osm-tag key="natural" value="sea" zoom-appear="3"/>
-    <osm-tag key="natural" value="beach" zoom-appear="10"/>
-    <osm-tag key="natural" value="scrub" zoom-appear="8"/>
-    <osm-tag key="natural" value="water" zoom-appear="8"/>
-    <osm-tag key="natural" value="wetland" zoom-appear="8"/>
-    <osm-tag key="natural" value="wood" zoom-appear="9"/>
-    <osm-tag key="landuse" value="forest" zoom-appear="8"/>
-    <osm-tag key="waterway" value="stream" zoom-appear="8"/>
-    <osm-tag key="waterway" value="river" zoom-appear="8"/>
-    <osm-tag key="waterway" value="riverbank" zoom-appear="8"/>
+    <osm-tag key="highway" value="primary_link" zoom-appear="8"/>
+    <osm-tag key="highway" value="raceway" zoom-appear="12"/>
+    <osm-tag key="highway" value="residential" zoom-appear="12"/>
+    <osm-tag key="highway" value="road" zoom-appear="12"/>
+    <osm-tag key="highway" value="secondary" zoom-appear="12"/>
+    <osm-tag key="highway" value="secondary_link" zoom-appear="12"/>
+    <osm-tag key="highway" value="service" zoom-appear="14"/>
+    <osm-tag key="highway" value="steps" zoom-appear="16"/>
+    <osm-tag key="highway" value="tertiary" zoom-appear="12"/>
+    <osm-tag key="highway" value="tertiary_link" zoom-appear="12"/>
+    <osm-tag key="highway" value="track" zoom-appear="13"/>
+    <osm-tag key="highway" value="trunk" zoom-appear="6"/>
+    <osm-tag key="highway" value="trunk_link" zoom-appear="6"/>
+    <osm-tag key="highway" value="unclassified" zoom-appear="13"/>
   </ways>
-  <!-- LEISURE/SPORT TAGS -->
   <ways>
-    <osm-tag key="leisure" value="nature_reserve" zoom-appear="8"/>
-    <osm-tag key="leisure" value="park" zoom-appear="8"/>
+    <osm-tag key="natural" value="nosea" zoom-appear="0"/>
+    <osm-tag key="natural" value="sea" zoom-appear="0"/>
+    <osm-tag key="natural" value="water" zoom-appear="8"/>
   </ways>
-  <!-- BUILDINGS -->
   <ways>
-    <osm-tag key="landuse" value="building" equivalent-values="commercial,industrial,residential,retail" zoom-appear="10"/>
+    <osm-tag key="oneway" value="yes" equivalent-values="1,true" renderable="false"/>
   </ways>
-  <!-- PUBLIC TRANSPORT -->
   <ways>
+    <osm-tag key="railway" value="disused" zoom-appear="15"/>
+    <osm-tag key="railway" value="funicular" zoom-appear="12"/>
+    <osm-tag key="railway" value="miniature" zoom-appear="14"/>
+    <osm-tag key="railway" value="light_rail" zoom-appear="12"/>
+    <osm-tag key="railway" value="monorail" zoom-appear="14"/>
+    <osm-tag key="railway" value="narrow_gauge" zoom-appear="14"/>
+    <osm-tag key="railway" value="platform" zoom-appear="14"/>
+    <osm-tag key="railway" value="preserved" zoom-appear="14"/>
     <osm-tag key="railway" value="rail" zoom-appear="10"/>
-    <osm-tag key="railway" value="tram" zoom-appear="12"/>
-  </ways>
-  <!-- OTHER TAGS -->
-  <ways>
-    <osm-tag key="area" value="yes" zoom-appear="3"/>
+    <osm-tag key="railway" value="subway" zoom-appear="15"/>
+    <osm-tag key="railway" value="tram" zoom-appear="15"/>
   </ways>
-  <!-- NOT TO RENDER -->
   <ways>
-    <osm-tag key="id" renderable="false" value="%f"/>
-    <osm-tag key="ref" renderable="false" value="%s"/>
-    <osm-tag key="name" renderable="false" value="%s"/>
-    <osm-tag key="access" value="destination" renderable="false"/>
-    <osm-tag key="access" value="private" renderable="false"/>
-    <osm-tag key="bridge" value="yes" renderable="false"/>
     <osm-tag key="tracktype" value="grade1" renderable="false"/>
     <osm-tag key="tracktype" value="grade2" renderable="false"/>
     <osm-tag key="tracktype" value="grade3" renderable="false"/>
     <osm-tag key="tracktype" value="grade4" renderable="false"/>
     <osm-tag key="tracktype" value="grade5" renderable="false"/>
-    <osm-tag key="surface" value="bic_paved" equivalent-values="paved,asphalt,concrete" renderable="false"/>
-    <osm-tag key="surface" value="bic_unpaved" equivalent-values="raw,gravel,rock,pebblestone,ground,dirt,earth,mud" renderable="false"/>
+  </ways>
+  <ways>
     <osm-tag key="tunnel" value="yes" renderable="false"/>
     <osm-tag key="tunnel" value="no" renderable="false"/>
-    <osm-tag key="bicycle" value="bic_yes" equivalent-values="yes,public,allowed" renderable="false"/>
-    <osm-tag key="bicycle" value="bic_designated" equivalent-values="designated,official" renderable="false"/>
-    <osm-tag key="foot" value="ft_yes" equivalent-values="yes,public,allowed" renderable="false"/>
-    <osm-tag key="foot" value="ft_designated" equivalent-values="designated,official" renderable="false"/>
+  </ways>
+  <ways>
+    <osm-tag key="waterway" value="canal" zoom-appear="10"/>
+    <osm-tag key="waterway" value="dam" zoom-appear="10"/>
+    <osm-tag key="waterway" value="drain" zoom-appear="13"/>
+    <osm-tag key="waterway" value="river" zoom-appear="8"/>
+    <osm-tag key="waterway" value="riverbank" zoom-appear="8"/>
+    <osm-tag key="waterway" value="stream" zoom-appear="13"/>
+  </ways>
+  <ways>
+    <osm-tag key="access" value="destination" renderable="false"/>
+    <osm-tag key="access" value="private" renderable="false"/>
+  </ways>
+  <ways>
+    <osm-tag key="aerialway" value="rope_tow" zoom-appear="13"/>
+  </ways>
+  <ways>
+    <osm-tag key="aeroway" value="runway" zoom-appear="10"/>
+    <osm-tag key="aeroway" value="taxiway" zoom-appear="10"/>
+    <osm-tag key="aeroway" value="helipad" zoom-appear="17"/>
+  </ways>
+  <ways>
+    <osm-tag force-polygon-line="true" key="boundary" value="administrative" zoom-appear="0"/>
+  </ways>
+  <ways>
+    <osm-tag key="bridge" value="yes" renderable="false"/>
+  </ways>
+  <ways>
+    <osm-tag force-polygon-line="true" key="admin_level" value="1" zoom-appear="4">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+    <osm-tag force-polygon-line="true" key="admin_level" value="2" zoom-appear="4">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+    <osm-tag force-polygon-line="true" key="admin_level" value="3" zoom-appear="4">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+    <osm-tag force-polygon-line="true" key="admin_level" value="4" zoom-appear="6">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+    <osm-tag force-polygon-line="true" key="admin_level" value="5" zoom-appear="6">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+    <osm-tag force-polygon-line="true" key="admin_level" value="6" zoom-appear="6">
+      <zoom-override key="boundary" value="administrative"/>
+    </osm-tag>
+  </ways>
+  <ways>
+    <osm-tag key="barrier" value="city_wall" zoom-appear="14"/>
   </ways>
 </tag-mapping>
```

### Comparing `wahoomc-4.0.0a9/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml` & `wahoomc-4.0.1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/resources/tags-to-keep.json` & `wahoomc-4.0.1/wahoomc/resources/tags-to-keep.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985294117647059%*

 * *Differences: {"'TAGS_TO_KEEP_UNIVERSAL'": "{'waterway': {insert: [(4, 'stream')]}}"}*

```diff
@@ -95,12 +95,13 @@
         "surface": "",
         "tracktype": "",
         "tunnel": "",
         "waterway": [
             "canal",
             "drain",
             "river",
-            "riverbank"
+            "riverbank",
+            "stream"
         ],
         "wood": "deciduous"
     }
 }
```

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/7za.dll` & `wahoomc-4.0.1/wahoomc/tooling_win/7za.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/7za.exe` & `wahoomc-4.0.1/wahoomc/tooling_win/7za.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/7zxa.dll` & `wahoomc-4.0.1/wahoomc/tooling_win/7zxa.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/lzma.exe` & `wahoomc-4.0.1/wahoomc/tooling_win/lzma.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert.exe` & `wahoomc-4.0.1/wahoomc/tooling_win/osmconvert.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc/tooling_win/osmconvert64-0.8.8p.exe` & `wahoomc-4.0.1/wahoomc/tooling_win/osmconvert64-0.8.8p.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.0a9/wahoomc.egg-info/PKG-INFO` & `wahoomc-4.0.1/wahoomc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.0a9
+Version: 4.0.1
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,16 @@
 ```
 
 3. [:floppy_disk: Copy the map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-files-to-wahoo-device-)
 
 ## To further adjust...
 * [:cookie: Get POIs displayed on your Wahoo](docs/USAGE.md#pois---points-of-interest)
 
+* [:mount_fuji: Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-of-interest)
+
 * [:wrench: Control OSM tags to be included in your maps ](docs/USAGE.md#user-specific-configuration)
 
 * [:computer: Preview your generated maps with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser)
 
 
 * [:mag: Use a custom theme on your Wahoo to control what and in which zoom-level certain elements are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.0a9 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.1 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
@@ -22,30 +22,31 @@
 QUICKSTART_ANACONDA.md#download-and-install-required-programs) 2. [:computer:
 Run wahooMapsCreator - detailled usage description](docs/USAGE.md#usage-of-
 wahoomapscreator) > In short: activate Anaconda environment, run
 wahooMapsCreator via CLI or via GUI. ``` conda activate gdal-user python -
 m wahoomc cli -co malta python -m wahoomc gui ``` 3. [:floppy_disk: Copy the
 map-files to your device after generation](docs/COPY_TO_WAHOO.md#copy-maps-
 files-to-wahoo-device-) ## To further adjust... * [:cookie: Get POIs displayed
-on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:wrench: Control OSM
-tags to be included in your maps ](docs/USAGE.md#user-specific-configuration) *
-[:computer: Preview your generated maps with cruiser ](docs/
-USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom theme on your Wahoo to
-control what and in which zoom-level certain elements are rendered](docs/
-TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-on-your-device-) ##
-Contribution / Questions You are welcome to provide input via Pull Requests,
-Issues or in any other way! If you have trouble using wahooMapsCreator, look
-into the FAQ, write an issue or join the telegram channel - [FAQ](docs/
-FAQ.md#frequently-asked-questions) - [:pencil2: issue](https://github.com/
-treee111/wahooMapsCreator/issues) - telegram channel: https://t.me/joinchat/
-TaMhjouxlsAzNWZk More details can be found here: [CONTRIBUTING](docs/
-CONTRIBUTING.md#contributing-to-wahoomapscreator-) ## Thanks to [@Intyre]
-(https://github.com/Intyre)/Hank for the initial version of the script [@Ebe66]
-(https://github.com/Ebe66)/ebo for the Windows- port [@mweirauch](https://
-github.com/mweirauch) for bringing in new ideas, testing and using the tool
-[@zenziwerken](https://github.com/zenziwerken) for the work done for [POIs]
-(https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)! [@macdet](https:/
-/github.com/macdet) for bringing in new thoughts, testing and making this a
-little more public [@vti](https://github.com/vti) for creating a GUI
-application to copy maps to wahoo and configure the device [POIs](https://
+on your Wahoo](docs/USAGE.md#pois---points-of-interest) * [:mount_fuji:
+Integrate contour lines into the generated maps](docs/USAGE.md#pois---points-
+of-interest) * [:wrench: Control OSM tags to be included in your maps ](docs/
+USAGE.md#user-specific-configuration) * [:computer: Preview your generated maps
+with cruiser ](docs/USAGE_CRUISER.md#usage-of-cruiser) * [:mag: Use a custom
+theme on your Wahoo to control what and in which zoom-level certain elements
+are rendered](docs/TAGS_ON_MAP_AND_DEVICE.md#osm-tags-during-map-creation-and-
+on-your-device-) ## Contribution / Questions You are welcome to provide input
+via Pull Requests, Issues or in any other way! If you have trouble using
+wahooMapsCreator, look into the FAQ, write an issue or join the telegram
+channel - [FAQ](docs/FAQ.md#frequently-asked-questions) - [:pencil2: issue]
+(https://github.com/treee111/wahooMapsCreator/issues) - telegram channel:
+https://t.me/joinchat/TaMhjouxlsAzNWZk More details can be found here:
+[CONTRIBUTING](docs/CONTRIBUTING.md#contributing-to-wahoomapscreator-) ##
+Thanks to [@Intyre](https://github.com/Intyre)/Hank for the initial version of
+the script [@Ebe66](https://github.com/Ebe66)/ebo for the Windows- port
+[@mweirauch](https://github.com/mweirauch) for bringing in new ideas, testing
+and using the tool [@zenziwerken](https://github.com/zenziwerken) for the work
+done for [POIs](https://github.com/zenziwerken/Bolt2-Mapsforge-Rendertheme)!
+[@macdet](https://github.com/macdet) for bringing in new thoughts, testing and
+making this a little more public [@vti](https://github.com/vti) for creating a
+GUI application to copy maps to wahoo and configure the device [POIs](https://
 github.com/vti/elemntary) as well as an [docker image](https://github.com/vti/
 wahooMapsCreator-docker) for wahooMapsCreator!
```

### Comparing `wahoomc-4.0.0a9/wahoomc.egg-info/SOURCES.txt` & `wahoomc-4.0.1/wahoomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

