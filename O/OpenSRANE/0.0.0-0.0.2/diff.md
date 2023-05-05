# Comparing `tmp/OpenSRANE-0.0.0.tar.gz` & `tmp/OpenSRANE-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenSRANE-0.0.0.tar", last modified: Wed Dec 14 06:15:31 2022, max compression
+gzip compressed data, was "OpenSRANE-0.0.2.tar", last modified: Fri May  5 18:30:38 2023, max compression
```

## Comparing `OpenSRANE-0.0.0.tar` & `OpenSRANE-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 06:15:31.835960 OpenSRANE-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 06:15:31.835960 OpenSRANE-0.0.0/OpenSRANE/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2022-12-14 06:15:24.000000 OpenSRANE-0.0.0/OpenSRANE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-14 06:15:24.000000 OpenSRANE-0.0.0/OpenSRANE/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 06:15:31.835960 OpenSRANE-0.0.0/OpenSRANE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-14 06:15:31.000000 OpenSRANE-0.0.0/OpenSRANE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 06:15:31.000000 OpenSRANE-0.0.0/OpenSRANE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 06:15:31.000000 OpenSRANE-0.0.0/OpenSRANE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-14 06:15:31.000000 OpenSRANE-0.0.0/OpenSRANE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-14 06:15:31.000000 OpenSRANE-0.0.0/OpenSRANE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-14 06:15:31.835960 OpenSRANE-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 06:15:24.000000 OpenSRANE-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 06:15:31.835960 OpenSRANE-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2022-12-14 06:15:24.000000 OpenSRANE-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.024228 OpenSRANE-0.0.2/OpenSRANE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 18:30:37.000000 OpenSRANE-0.0.2/OpenSRANE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 18:30:37.000000 OpenSRANE-0.0.2/OpenSRANE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:30:37.000000 OpenSRANE-0.0.2/OpenSRANE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 18:30:37.000000 OpenSRANE-0.0.2/OpenSRANE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 18:30:37.000000 OpenSRANE-0.0.2/OpenSRANE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/All/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/All/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/All/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/All/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/Analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/ScenarioAnalyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_DispSprd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_Frag_OutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_NodesGroupsVulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_PhysicalAssign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_PhysicalEffects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_Prob_OutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_Sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/_ZeroLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Analyze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/Connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Connectors/DS_LOC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Connectors/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Connectors/Out_Physic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Connectors/Pb_LOC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/DateAndTime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DateAndTime/DateTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DateAndTime/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DateAndTime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.028228 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/
+-rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/BritterMcQuaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29223 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/GasGaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/LiquidSpread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38372 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/LqdSprdGaussianGasDisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/DispersionSpreadModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.032228 OpenSRANE-0.0.2/opensrane/Fragilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Fragilities/Fragility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Fragilities/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Fragilities/Probit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Fragilities/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Fragilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.032228 OpenSRANE-0.0.2/opensrane/Hazard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Hazard/Earthquake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Hazard/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Hazard/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Hazard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.032228 OpenSRANE-0.0.2/opensrane/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Misc/MiscFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Misc/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Misc/WarningRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Misc/_NewClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.032228 OpenSRANE-0.0.2/opensrane/NodesGroups/
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/NodesGroups/Nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/NodesGroups/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/NodesGroups/RectangNodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/NodesGroups/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/NodesGroups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.032228 OpenSRANE-0.0.2/opensrane/OutFlowModel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/GasUnitHole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/Liquid10min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/NoOutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/SimultaniousGas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/SimultaniousLiquid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/TankHole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/TankHoleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/TankHoleFixStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/TankHoleInitRate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/OutFlowModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/PhysicalEffect/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/Simple_fire_point_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/VCE_TNT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PhysicalEffect/fire_point_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/PlantUnits/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PlantUnits/ONGStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PlantUnits/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PlantUnits/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PlantUnits/_Position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PlantUnits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/Plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Plot/Matplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Plot/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42461 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Plot/Plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/PostProcess/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PostProcess/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PostProcess/ObjsRecorderPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PostProcess/PlotPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20168 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PostProcess/RecorderPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/PostProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/Recorders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Recorders/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Recorders/Objs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Recorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Recorders/recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/Safety/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Safety/Dike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Safety/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Safety/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Safety/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.036228 OpenSRANE-0.0.2/opensrane/Sites/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Sites/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Sites/Site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Sites/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/opensrane/Substance/
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Substance/DataBank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Substance/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Substance/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Substance/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/Substance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/opensrane/WindData/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/WindData/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/WindData/WindRose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/WindData/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/WindData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/opensrane/_New_module/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/_New_module/New_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/_New_module/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/_New_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/opensrane/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:30:38.040228 OpenSRANE-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-05 18:30:25.000000 OpenSRANE-0.0.2/setup.py
```

### Comparing `OpenSRANE-0.0.0/OpenSRANE/__init__.py` & `OpenSRANE-0.0.2/opensrane/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 # /* ****************************************************************** **
 # **    OpeSRANE - Open Software for Risk Assessment of Natech Events   **
 # **                                                                    **
 # **                                                                    **
 # **                                                                    **
-# ** (C) Copyright 2022, Bijan Sayyafzadeh                              **
+# ** (C) Copyright 2023, Mentioned Regents in 'COPYRIGHT' file.         **
 # **                                                                    **
 # ** All Rights Reserved.                                               **
 # **                                                                    **
 # ** Commercial use of this program without express permission of the   **
-# ** owner (Bijan SayyafZadeh and following Developers), is             **
+# ** owner (The Regents), is                                            **
 # ** strictly prohibited.  See file 'COPYRIGHT'  in main directory      **
 # ** for information on usage and redistribution,  and for a            **
 # ** DISCLAIMER OF ALL WARRANTIES.                                      **
 # **                                                                    **
 # ** Developed by:                                                      **
-# **   Bijan SayyafZadeh (B.Sayyaf@yahoo.com)                           **
+# **   Bijan SayyafZadeh (OpenSRANE@Gmail.com)                          **
 # **   MehDi Sharifi                                                    **
-# **   Abdolreza Sarvghad Moghaddam                                     **
+# **   Abdolreza S. Moghadam                                            **
 # **   Eslam Kashi                                                      **
 # **                                                                    **
 # ** ****************************************************************** */
 
+'''
+ Written: Bijan Sayyafzadeh
+ Created: 2022
+ 
+ Revision: -
+ By & Date: -
+'''
 
+
+import os
+
+
+def string():
+    try:
+        with open(os.path.dirname(__file__) + "/VERSION", "r", encoding="utf-8") as fh:
+            version = fh.read().strip()
+            if version:
+                return version
+    except:
+        pass
+    return "unknown (git checkout)"
```

### Comparing `OpenSRANE-0.0.0/OpenSRANE.egg-info/PKG-INFO` & `OpenSRANE-0.0.2/OpenSRANE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenSRANE
-Version: 0.0.0
+Version: 0.0.2
 Summary: Open Software for Risk Assessment of Natech Events
 Home-page: https://github.com/OpenSRANE/OpenSRANE
 Author: Bijan Sayyafzadeh
 Author-email: <OpenSRANE@Gmail.com>
 Keywords: python,NaTech,Modeling,Risk
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `OpenSRANE-0.0.0/PKG-INFO` & `OpenSRANE-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenSRANE
-Version: 0.0.0
+Version: 0.0.2
 Summary: Open Software for Risk Assessment of Natech Events
 Home-page: https://github.com/OpenSRANE/OpenSRANE
 Author: Bijan Sayyafzadeh
 Author-email: <OpenSRANE@Gmail.com>
 Keywords: python,NaTech,Modeling,Risk
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `OpenSRANE-0.0.0/setup.py` & `OpenSRANE-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # /* ****************************************************************** **
 # **    OpeSRANE - Open Software for Risk Assessment of Natech Events   **
 # **                                                                    **
 # **                                                                    **
 # **                                                                    **
-# ** (C) Copyright 2022, Bijan Sayyafzadeh                              **
+# ** (C) Copyright 2023, Mentioned Regents in 'COPYRIGHT' file.         **
 # **                                                                    **
 # ** All Rights Reserved.                                               **
 # **                                                                    **
 # ** Commercial use of this program without express permission of the   **
-# ** owner (Bijan SayyafZadeh and following Developers), is             **
+# ** owner (The Regents), is                                            **
 # ** strictly prohibited.  See file 'COPYRIGHT'  in main directory      **
 # ** for information on usage and redistribution,  and for a            **
 # ** DISCLAIMER OF ALL WARRANTIES.                                      **
 # **                                                                    **
 # ** Developed by:                                                      **
-# **   Bijan SayyafZadeh (B.Sayyaf@yahoo.com)                           **
+# **   Bijan SayyafZadeh (OpenSRANE@Gmail.com)                          **
 # **   MehDi Sharifi                                                    **
-# **   Abdolreza Sarvghad Moghaddam                                     **
+# **   Abdolreza S. Moghadam                                            **
 # **   Eslam Kashi                                                      **
 # **                                                                    **
 # ** ****************************************************************** */
 
 from setuptools import setup, find_packages
 
 import subprocess
@@ -30,16 +30,16 @@
     subprocess.run(["git", "describe", "--tags"], stdout=subprocess.PIPE)
     .stdout.decode("utf-8")
     .strip()
 )
 
 assert "." in OpenSRANE_version
 
-assert os.path.isfile("OpenSRANE/version.py")
-with open("OpenSRANE/VERSION", "w", encoding="utf-8") as fh:
+assert os.path.isfile("opensrane/version.py")
+with open("opensrane/VERSION", "w", encoding="utf-8") as fh:
     fh.write(f"{OpenSRANE_version}\n")
 
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
@@ -53,15 +53,15 @@
     long_description_content_type="text/markdown",
     long_description=long_description ,
     package_data={
         # "":["*.jpg","*.at2","*.pyd"],
 
     },
     packages=find_packages(),
-    install_requires=['numpy','plotly','scipy','kaleido','tqdm'],
+    install_requires=['numpy','plotly','scipy','kaleido','tqdm','pandas'],
     url="https://github.com/OpenSRANE/OpenSRANE",
     keywords=['python', 'NaTech', 'Modeling', 'Risk'],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Operating System :: Microsoft :: Windows'
     ],
```

