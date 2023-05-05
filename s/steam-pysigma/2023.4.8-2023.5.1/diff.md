# Comparing `tmp/steam-pysigma-2023.4.8.tar.gz` & `tmp/steam-pysigma-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.4.8.tar", last modified: Thu Apr 13 08:17:06 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.5.1.tar", last modified: Fri May  5 07:12:52 2023, max compression
```

## Comparing `steam-pysigma-2023.4.8.tar` & `steam-pysigma-2023.5.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.453145 steam-pysigma-2023.4.8/
--rw-rw-rw-   0        0        0     1030 2023-04-13 08:17:06.445145 steam-pysigma-2023.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 08:17:06.453145 steam-pysigma-2023.4.8/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-04-13 08:14:39.000000 steam-pysigma-2023.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.427146 steam-pysigma-2023.4.8/steam_pysigma/
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.4.8/steam_pysigma/__init__.py
--rw-rw-rw-   0        0        0    10881 2023-04-05 08:23:05.000000 steam-pysigma-2023.4.8/steam_pysigma/helpers.py
--rw-rw-rw-   0        0        0     8356 2023-04-12 09:10:53.000000 steam-pysigma-2023.4.8/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.443145 steam-pysigma-2023.4.8/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.594184 steam-pysigma-2023.5.1/
+-rw-rw-rw-   0        0        0     1030 2023-05-05 07:12:52.594184 steam-pysigma-2023.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:12:52.595185 steam-pysigma-2023.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-05 07:11:11.000000 steam-pysigma-2023.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.585049 steam-pysigma-2023.5.1/steam_pysigma/
+-rw-rw-rw-   0        0        0     2317 2023-05-04 13:58:50.000000 steam-pysigma-2023.5.1/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.1/steam_pysigma/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.1/steam_pysigma/helpers.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.1/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:12:52.592047 steam-pysigma-2023.5.1/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 07:12:48.000000 steam-pysigma-2023.5.1/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.4.8/PKG-INFO` & `steam-pysigma-2023.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.8
+Version: 2023.5.1
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.4.8/README.md` & `steam-pysigma-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.8/setup.py` & `steam-pysigma-2023.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.4.8",
+    version="2023.5.1",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
     install_requires=required,
     python_requires='>=3.8',
-    package_data={'': ['steam-sigma-2023.4.7.jar']},
+    package_data={'': ['steam-sigma-2023.4.12.jar', 'CFUN_mapping.csv']},
     include_package_data=True,
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Programming Language :: Python :: 3.8"
         ],
 )
```

### Comparing `steam-pysigma-2023.4.8/steam_pysigma/helpers.py` & `steam-pysigma-2023.5.1/steam_pysigma/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,14 +84,50 @@
     else:
         print(stdout)
 
 
 def build_global_variables(g, model_data):
     map = g.gateway.jvm.java.util.HashMap()
     constants = g.constants
+    end_sim_time = model_data["Options_SIGMA"]["time_vector_solution"]["time_step"][-1][-1]
+    # Cliq variables:
+    R_crow =  model_data['Circuit']['R_circuit']
+    L_circuit =model_data['Circuit']['L_circuit']
+    C_cliq = model_data['Quench_Protection']['CLIQ']['C']
+    L_cliq = model_data['Quench_Protection']['CLIQ']['L']
+
+    V_cliq_0 = model_data['Quench_Protection']['CLIQ']['U0']
+    I_cliq_0 = model_data['Quench_Protection']['CLIQ']['I0']
+
+
+    sym_factor = model_data['Quench_Protection']['CLIQ']['sym_factor']
+    cliq_time = model_data['Quench_Protection']['CLIQ']['t_trigger']
+    if cliq_time > end_sim_time:
+        with_cliq = 0
+    else:
+        with_cliq = 1
+
+    if V_cliq_0 == None:
+        V_cliq_0 = 0
+    if I_cliq_0 == None:
+        I_cliq_0 = 0
+    if sym_factor == None:
+        sym_factor = 1
+    if L_circuit == None:
+        L_circuit = "1e-6"
+    if L_cliq == None:
+        L_cliq = "1e-6"
+    map.put(constants.LABEL_CLIQ_RCROW, str(R_crow))
+    map.put(constants.LABEL_CLIQ_LCIR, str(L_circuit))
+    map.put(constants.LABEL_CLIQ_CAPASITOR, str(C_cliq))
+    map.put(constants.LABEL_CLIQ_INDUCTANCE, str(L_cliq))
+    map.put(constants.LABEL_CLIQ_VOLTAGE_INITIAL, str(V_cliq_0))
+    map.put(constants.LABEL_CLIQ_CURRENT_INITIAL, str(I_cliq_0))
+    map.put(constants.LABEL_CLIQ_SYMFACTOR, str(sym_factor))
+    map.put(constants.LABEL_CLIQ_SWITCH, str(with_cliq))
 
     FLAG_M_pers = model_data['Options_SIGMA']['physics']['FLAG_M_pers']
     FLAG_M_pers = "0" if FLAG_M_pers is None else FLAG_M_pers
 
     FLAG_ifcc = model_data['Options_SIGMA']['physics']['FLAG_ifcc']
     FLAG_ifcc = "0" if FLAG_ifcc is None else FLAG_ifcc
 
@@ -145,16 +181,15 @@
                        model_data['Quench_Protection']['Quench_Heaters']['l_copper'])])]
     trigger_time = model_data['Quench_Protection']['Quench_Heaters']['t_trigger']
     ins_thick_to_coil = model_data['Options_SIGMA']['quench_initialization']['th_coils']
     lengths_qh = model_data['Quench_Protection']['Quench_Heaters']['l']
 
     for i in range(num_qh):
         if model_data["Options_SIGMA"]["time_vector_solution"]["time_step"][-1][-1] < trigger_time[i]:
-            trigger_time[i] = model_data["Options_SIGMA"]["time_vector_solution"]["time_step"][-1][-1]
-            + model_data["Options_SIGMA"]["time_vector_solution"]["time_step"][-1][-2]
+            trigger_time[i] = end_sim_time + model_data["Options_SIGMA"]["time_vector_solution"]["time_step"][-1][-2]
         map.put(constants.LABEL_INSULATION_THICKNESS_QH_TO_COIL + str(i + 1), str(ins_list[i]))
         map.put(constants.LABEL_WIDTH_QH + str(i + 1), str(w_list[i]))
         map.put(constants.LABEL_INSULATION_THICKNESS_QH_TO_BATH + str(i + 1), str(qh_to_bath_list[i]))
         map.put(constants.LABEL_INSULATION_THICKNESS_QH_STRIP + str(i + 1), str(qh_steel_strip[i]))
         map.put(constants.LABEL_EXPONENTIAL_TIME_CONSTANT_DECAY + str(i + 1), str(tau[i]))
         map.put(constants.LABEL_NUMBER_OF_QH_SUBDIVISIONS + str(i + 1), str(num_qh_div[i]))
         map.put(constants.LABEL_QH + constants.LABEL_L + str(i + 1), str(lengths_qh[i]))
@@ -177,20 +212,30 @@
         elif (study_type == "Transient"):
             study_API.setNewMonolithicStudy(srv, cfg, "Default_study", timeRange)
 
 
 def create_results(srv, cfg, variables1DvsTime, time2DConverted, variables2DConverted, time1DConverted,
                    variables1DvsTimeVector,
                    result_api, input_coordinates_path, path_to_results):
+
     for i in range(len(variables2DConverted)):
-        time_vector_2D = ', '.join(str(x) for x in time2DConverted[i])
-        time_vector_1D = ', '.join(str(x) for x in time1DConverted[i])
+        if len(time2DConverted)>1:
+            time_vector_2D = ', '.join(str(x) for x in time2DConverted[i])
 
+        else:
+            time_vector_2D = time2DConverted[0]
         result_api.create2DResultNode(srv, cfg, variables2DConverted[i], time_vector_2D, f"data {i}",
                                       input_coordinates_path, path_to_results)
+    for j in range(len(time1DConverted)):
+        if len(time2DConverted)>1:
+            time_vector_1D = ', '.join(str(x) for x in time1DConverted[j])
+
+        else:
+            time_vector_1D = time1DConverted[0]
+
     if cfg.getStudyType() == "Transient":
         for j in range(len(variables1DvsTime)):
             result_api.create1DResultNodeAllTimes(srv, cfg, variables1DvsTime[j], f"1DExport_{j}", path_to_results)
 
         for k in range(len(variables1DvsTimeVector)):
             result_api.create1DResultNodeTimeVector(srv, cfg, variables1DvsTimeVector[k], time_vector_1D,
-                                                    f"data {i + 1 + k}", path_to_results)
+                                                    f"data {i + j + 1 + k}", path_to_results)
```

### Comparing `steam-pysigma-2023.4.8/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.5.1/steam_pysigma.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.8
+Version: 2023.5.1
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

