# Comparing `tmp/steam-pysigma-2023.5.1.tar.gz` & `tmp/steam-pysigma-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.5.1.tar", last modified: Fri May  5 07:12:52 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.5.2.tar", last modified: Fri May  5 13:50:28 2023, max compression
```

## Comparing `steam-pysigma-2023.5.1.tar` & `steam-pysigma-2023.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.594184 steam-pysigma-2023.5.1/
--rw-rw-rw-   0        0        0     1030 2023-05-05 07:12:52.594184 steam-pysigma-2023.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 07:12:52.595185 steam-pysigma-2023.5.1/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-05 07:11:11.000000 steam-pysigma-2023.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.585049 steam-pysigma-2023.5.1/steam_pysigma/
--rw-rw-rw-   0        0        0     2317 2023-05-04 13:58:50.000000 steam-pysigma-2023.5.1/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.1/steam_pysigma/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.1/steam_pysigma/helpers.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.1/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.592047 steam-pysigma-2023.5.1/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.700742 steam-pysigma-2023.5.2/
+-rw-rw-rw-   0        0        0     1030 2023-05-05 13:50:28.699741 steam-pysigma-2023.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:50:28.701741 steam-pysigma-2023.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-05 13:49:36.000000 steam-pysigma-2023.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.687478 steam-pysigma-2023.5.2/steam_pysigma/
+-rw-rw-rw-   0        0        0     2484 2023-05-05 08:55:14.000000 steam-pysigma-2023.5.2/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.2/steam_pysigma/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.2/steam_pysigma/helpers.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.2/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.697728 steam-pysigma-2023.5.2/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.5.1/PKG-INFO` & `steam-pysigma-2023.5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SIGMA
+Keywords: STEAM,CERN,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.1/README.md` & `steam-pysigma-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.1/setup.py` & `steam-pysigma-2023.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.5.1",
+    version="2023.5.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.5.1/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.5.2/steam_pysigma/MainSIGMA.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class MainSIGMA:
     """
         Class to generate SIGMA models
     """
 
     def __init__(self, input_file_path: str = None, model_folder: str = None, dm=None,
-                 system_settings_path: Path = None, verbose: bool = False):
+                 system_settings: dict = None, verbose: bool = False):
         """
               Main class for working with FiQuS simulations
               :param input_file_path: input file full path
               :param verbose: if True, more info is printed in the console
               """
         self.start_folder = os.getcwd()
         self.wrk_folder = model_folder
@@ -27,18 +27,18 @@
 
         logger = logging.getLogger()
         if verbose:
             logger.setLevel(logging.INFO)
         else:
             logger.setLevel(logging.DEBUG)
 
-        if Path.exists(system_settings_path):
-            with open(system_settings_path, 'r') as stream:
-                self.settings = yaml.safe_load(stream)
-
+        #if Path.exists(system_settings_path):
+           # with open(system_settings_path, 'r') as stream:
+                #self.settings = yaml.safe_load(stream)
+        self.settings = system_settings
         # Load yaml input file
         if not dm:
             self.dm = Util.FilesAndFolders.read_data_from_yaml(input_file_path, dS.DataSIGMA)
         else:
             self.dm = dm
         self.sdm = Util.FilesAndFolders.read_data_from_yaml(f'{input_file_path[:-5]}.set', dS.MultipoleSettings)
         self.roxie_data = Util.FilesAndFolders.read_data_from_yaml(f'{input_file_path[:-5]}.geom', dS.SIGMAGeometry)
@@ -53,9 +53,12 @@
     #     mp = MainFiQuS(sys.argv[1], sys.argv[2])
 
     magnet = 'MQXA_SIGMA'
     yaml_file = f'{magnet}.yaml'
     output_folder = r"C:\Users\jlidholm\Git-projects\steam-pysigma\steam-pysigma"
     print(os.path.join(output_folder))
     system_settings_path = (Path.joinpath(Path(__file__).parent, "../steam_pysigma/settings.SYSTEM.yaml"))
+    if Path.exists(system_settings_path):
+        with open(system_settings_path, 'r') as stream:
+            settings = yaml.safe_load(stream)
     sim_result = MainSIGMA(input_file_path=yaml_file,
-                           system_settings_path=system_settings_path, model_folder=os.path.join(output_folder))
+                           system_settings=settings, model_folder=os.path.join(output_folder))
```

### Comparing `steam-pysigma-2023.5.1/steam_pysigma/helpers.py` & `steam-pysigma-2023.5.2/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.1/steam_pysigma/pysigma.py` & `steam-pysigma-2023.5.2/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.1/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.5.2/steam_pysigma.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SIGMA
+Keywords: STEAM,CERN,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

