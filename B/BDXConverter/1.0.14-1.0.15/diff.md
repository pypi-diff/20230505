# Comparing `tmp/BDXConverter-1.0.14.tar.gz` & `tmp/BDXConverter-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.14.tar", last modified: Wed May  3 07:50:47 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.15.tar", last modified: Fri May  5 14:08:47 2023, max compression
```

## Comparing `BDXConverter-1.0.14.tar` & `BDXConverter-1.0.15.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.858207 BDXConverter-1.0.14/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.626987 BDXConverter-1.0.15/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/setup.py
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.15/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.15/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.15/BDXConverter/General/GeneralClass.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 
     def __init__(self) -> None:
         self.operationNumber: int
         self.operationName: str
 
     def Marshal(self, writer: BytesIO) -> None:
         """
-        Marshal GeneralClass into the writer
+        Marshal Self@GeneralClass into the writer(io object)
         """
         ...
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         """
-        Unmarshal the buffer(io object) into GeneralClass
+        Unmarshal the buffer(io object) into Self@GeneralClass
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
-        Convert jsonDict:dict into GeneralClass
+        Load datas from jsonDict:dict
         """
-        ...
+        if 'operationNumber' in self.__dict__:
+            jsonDict['operationNumber'] = self.operationNumber
+            jsonDict['operationName'] = self.operationName
+        for i in self.__dict__:
+            if i in jsonDict:
+                self.__dict__[i] = jsonDict[i]
 
     def Dumps(self) -> dict:
         """
-        Convert GeneralClass into basic dictionary
+        Convert Self@GeneralClass into the basic dictionary
         """
         return self.__dict__
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from io import BytesIO
-from struct import pack, unpack
+from struct import unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt16XValue(GeneralClass):
+class AddInt8ZValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt16XValue'
-        self.operationNumber: int = 20
+        self.operationName: str = 'AddInt8ZValue'
+        self.operationNumber: int = 30
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>h', self.value))
+        writer.write(self.value.to_bytes(
+            length=1, byteorder='big', signed=True))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+        self.value = unpack('>b', getByte(buffer, 1))[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt8YValue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from io import BytesIO
-from struct import pack, unpack
+from struct import unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt16YValue(GeneralClass):
+class AddInt8YValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt16YValue'
-        self.operationNumber: int = 22
+        self.operationName: str = 'AddInt8YValue'
+        self.operationNumber: int = 29
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>h', self.value))
+        writer.write(self.value.to_bytes(
+            length=1, byteorder='big', signed=True))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+        self.value = unpack('>b', getByte(buffer, 1))[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,7 @@
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>h', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,10 +11,7 @@
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>H', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32YValue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt32XValue(GeneralClass):
+class AddInt32YValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt32XValue'
-        self.operationNumber: int = 21
+        self.operationName: str = 'AddInt32YValue'
+        self.operationNumber: int = 23
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>i', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt32YValue(GeneralClass):
+class AddInt32ZValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt32YValue'
-        self.operationNumber: int = 23
+        self.operationName: str = 'AddInt32ZValue'
+        self.operationNumber: int = 25
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>i', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32XValue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt32ZValue(GeneralClass):
+class AddInt32XValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt32ZValue'
-        self.operationNumber: int = 25
+        self.operationName: str = 'AddInt32XValue'
+        self.operationNumber: int = 21
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>i', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,10 +11,7 @@
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>I', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.value = unpack('>I', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16XValue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from io import BytesIO
-from struct import unpack
+from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt8XValue(GeneralClass):
+class AddInt16XValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt8XValue'
-        self.operationNumber: int = 28
+        self.operationName: str = 'AddInt16XValue'
+        self.operationNumber: int = 20
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.value.to_bytes(
-            length=1, byteorder='big', signed=True))
+        writer.write(pack('>h', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>b', getByte(buffer, 1))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+        self.value = unpack('>h', getByte(buffer, 2))[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16YValue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from io import BytesIO
-from struct import unpack
+from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt8YValue(GeneralClass):
+class AddInt16YValue(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt8YValue'
-        self.operationNumber: int = 29
+        self.operationName: str = 'AddInt16YValue'
+        self.operationNumber: int = 22
         self.value: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.value.to_bytes(
-            length=1, byteorder='big', signed=True))
+        writer.write(pack('>h', self.value))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>b', getByte(buffer, 1))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+        self.value = unpack('>h', getByte(buffer, 2))[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.15/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from io import BytesIO
-from struct import unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class AddInt8ZValue(GeneralClass):
+class UseRuntimeIDPool(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'AddInt8ZValue'
-        self.operationNumber: int = 30
-        self.value: int = 0
+        self.operationName: str = 'UseRuntimeIDPool'
+        self.operationNumber: int = 31
+        self.poolId: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.value.to_bytes(
-            length=1, byteorder='big', signed=True))
+        writer.write(self.poolId.to_bytes(
+            length=1, byteorder='big', signed=False))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>b', getByte(buffer, 1))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+        self.poolId = getByte(buffer, 1)[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.15/BDXConverter/Operation/CreateConstantString.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,10 +10,7 @@
         self.constantString: str = ''
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(self.constantString.encode(encoding='utf-8') + b'\x00')
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.constantString = getString(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.constantString = jsonDict['constantString'] if 'constantString' in jsonDict else ''
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class PlaceBlock(GeneralClass):
+class PlaceBlockWithBlockStates(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlock'
-        self.operationNumber: int = 7
+        self.operationName: str = 'PlaceBlockWithBlockStates'
+        self.operationNumber: int = 5
         self.blockConstantStringID: int = 0
-        self.blockData: int = 0
+        self.blockStatesConstantStringID: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>H', self.blockConstantStringID) +
-                     pack('>H', self.blockData))
+                     pack('>H', self.blockStatesConstantStringID))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockData = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
+        self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,11 +14,7 @@
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>H', self.blockConstantStringID) +
                      self.blockStatesString.encode(encoding='utf-8') + b'\x00')
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         self.blockStatesString = getString(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockStatesString = jsonDict['blockStatesString'] if 'blockStatesString' in jsonDict else ''
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
         self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
         self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
-        # self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
         newChestData = ChestData()
         if 'data' in jsonDict:
             newChestData.Loads(jsonDict['data'])
         self.slotCount = self.data.slotCount
         self.data = newChestData
 
     def Dumps(self) -> dict:
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getString import getByte, getString
 
 
-class PlaceBlockWithCommandBlockData(GeneralClass):
+class PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithCommandBlockData'
-        self.operationNumber: int = 27
-        self.blockConstantStringID: int = 0
-        self.blockData: int = 0
+        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID'
+        self.operationNumber: int = 35
+        self.runtimeId: int = 0
         self.mode: int = 0
         self.command: str = ''
         self.customName: str = ''
         self.lastOutput: str = ''
         self.tickdelay: int = 0
         self.executeOnFirstTick: bool = True
         self.trackOutput: bool = True
         self.conditional: bool = False
         self.needsRedstone: bool = False
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H', self.blockData) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
+        writer.write(pack('>I', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
                      self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockData = unpack('>H', getByte(buffer, 2))[0]
+        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
         self.mode = unpack('>I', getByte(buffer, 4))[0]
         self.command = getString(buffer)
         self.customName = getString(buffer)
         self.lastOutput = getString(buffer)
         self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
         self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
         self.trackOutput = bool(getByte(buffer, 1)[0])
         self.conditional = bool(getByte(buffer, 1)[0])
         self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,10 +11,7 @@
         self.runtimeId: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>I', self.runtimeId))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getString import getByte, getString
 
 
-class PlaceCommandBlockWithCommandBlockData(GeneralClass):
+class PlaceRuntimeBlockWithCommandBlockData(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'PlaceCommandBlockWithCommandBlockData'
-        self.operationNumber: int = 36
-        self.data: int = 0
+        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockData'
+        self.operationNumber: int = 34
+        self.runtimeId: int = 0
         self.mode: int = 0
         self.command: str = ''
         self.customName: str = ''
         self.lastOutput: str = ''
         self.tickdelay: int = 0
         self.executeOnFirstTick: bool = True
         self.trackOutput: bool = True
         self.conditional: bool = False
         self.needsRedstone: bool = False
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.data) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) + self.executeOnFirstTick.to_bytes(
-            length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
+        writer.write(pack('>H', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
+                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.data = unpack('>H', getByte(buffer, 2))[0]
+        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
         self.mode = unpack('>I', getByte(buffer, 4))[0]
         self.command = getString(buffer)
         self.customName = getString(buffer)
         self.lastOutput = getString(buffer)
         self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
         self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
         self.trackOutput = bool(getByte(buffer, 1)[0])
         self.conditional = bool(getByte(buffer, 1)[0])
         self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.data = jsonDict['data'] if 'data' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,7 @@
         self.runtimeId: int = 0
 
     def Marshal(self, writer: BytesIO) -> None:
         writer.write(pack('>H', self.runtimeId))
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from io import BytesIO
 from struct import pack, unpack
 from .structOfChest import ChestData
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class PlaceRuntimeBlockWithChestData(GeneralClass):
+class PlaceRuntimeBlockWithChestDataAndUint32RuntimeID(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'PlaceRuntimeBlockWithChestData'
-        self.operationNumber: int = 37
+        self.operationName: str = 'PlaceRuntimeBlockWithChestDataAndUint32RuntimeID'
+        self.operationNumber: int = 38
         self.runtimeId: int = 0
         self.slotCount: int = 0
         self.data: ChestData = ChestData()
 
     def Marshal(self, writer: BytesIO) -> None:
         self.data.slotCount = self.slotCount
-        writer.write(pack('>H', self.runtimeId) +
+        writer.write(pack('>I', self.runtimeId) +
                      self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
         self.data.Marshal(writer)
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
+        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
         self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
         newChestData = ChestData()
         if 'data' in jsonDict:
             newChestData.Loads(jsonDict['data'])
+        self.slotCount = self.data.slotCount
         self.data = newChestData
 
     def Dumps(self) -> dict:
         result: dict = {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
             'runtimeId': self.runtimeId,
-            'slotCount': self.slotCount,
+            'slotCount': len(self.data.chestData),
             'data': self.data.Dumps()
         }
         return result
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from io import BytesIO
 from struct import pack, unpack
 from .structOfChest import ChestData
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-class PlaceRuntimeBlockWithChestDataAndUint32RuntimeID(GeneralClass):
+class PlaceRuntimeBlockWithChestData(GeneralClass):
     def __init__(self) -> None:
-        self.operationName: str = 'PlaceRuntimeBlockWithChestDataAndUint32RuntimeID'
-        self.operationNumber: int = 38
+        self.operationName: str = 'PlaceRuntimeBlockWithChestData'
+        self.operationNumber: int = 37
         self.runtimeId: int = 0
         self.slotCount: int = 0
         self.data: ChestData = ChestData()
 
     def Marshal(self, writer: BytesIO) -> None:
         self.data.slotCount = self.slotCount
-        writer.write(pack('>I', self.runtimeId) +
+        writer.write(pack('>H', self.runtimeId) +
                      self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
         self.data.Marshal(writer)
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
+        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
         self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
         newChestData = ChestData()
         if 'data' in jsonDict:
             newChestData.Loads(jsonDict['data'])
+        self.slotCount = self.data.slotCount
         self.data = newChestData
 
     def Dumps(self) -> dict:
         result: dict = {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
             'runtimeId': self.runtimeId,
-            'slotCount': self.slotCount,
+            'slotCount': len(self.data.chestData),
             'data': self.data.Dumps()
         }
         return result
```

### Comparing `BDXConverter-1.0.14/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.15/BDXConverter/Operation/structOfChest.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,20 +21,14 @@
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.itemName = getString(buffer)
         self.count = getByte(buffer, 1)[0]
         self.data = unpack('>H', getByte(buffer, 2))[0]
         self.slotID = getByte(buffer, 1)[0]
 
-    def Loads(self, jsonDict: dict) -> None:
-        self.itemName = jsonDict['itemName'] if 'itemName' in jsonDict else ''
-        self.count = jsonDict['count'] if 'count' in jsonDict else 0
-        self.data = jsonDict['data'] if 'data' in jsonDict else 0
-        self.slotID = jsonDict['slotID'] if 'slotID' in jsonDict else 0
-
 
 class ChestData(GeneralClass):
     """
     Note: `ChestData` is not a operation
     """
 
     def __init__(self) -> None:
```

### Comparing `BDXConverter-1.0.14/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.15/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.0.15/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.15/BDXConverter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.14
+Version: 1.0.15
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,42 +93,47 @@
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
-    Any Operation eration of the BDX file will inherit this class
+    Any operation of the BDX file will inherit this class
     """
 
     def __init__(self) -> None:
         self.operationNumber: int
         self.operationName: str
 
     def Marshal(self, writer: BytesIO) -> None:
         """
-        Marshal GeneralClass into the writer
+        Marshal Self@GeneralClass into the writer(io object)
         """
         ...
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         """
-        Unmarshal the buffer(io object) into GeneralClass
+        Unmarshal the buffer(io object) into Self@GeneralClass
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
-        Convert jsonDict:dict into GeneralClass
+        Load datas from jsonDict:dict
         """
-        ...
+        if 'operationNumber' in self.__dict__:
+            jsonDict['operationNumber'] = self.operationNumber
+            jsonDict['operationName'] = self.operationName
+        for i in self.__dict__:
+            if i in jsonDict:
+                self.__dict__[i] = jsonDict[i]
 
     def Dumps(self) -> dict:
         """
-        Convert GeneralClass into basic dictionary
+        Convert Self@GeneralClass into the basic dictionary
         """
         return self.__dict__
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。
```

### Comparing `BDXConverter-1.0.14/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.15/BDXConverter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 BDXConverter.egg-info/dependency_links.txt
 BDXConverter.egg-info/requires.txt
 BDXConverter.egg-info/top_level.txt
 BDXConverter/Converter/ConvertErrorDefine.py
 BDXConverter/Converter/Converter.py
 BDXConverter/Converter/__init__.py
 BDXConverter/General/GeneralClass.py
+BDXConverter/General/Operation.py
 BDXConverter/General/Pool.py
 BDXConverter/General/__init__.py
 BDXConverter/Operation/AddInt16XValue.py
 BDXConverter/Operation/AddInt16YValue.py
 BDXConverter/Operation/AddInt16ZValue.py
 BDXConverter/Operation/AddInt16ZValue0.py
 BDXConverter/Operation/AddInt32XValue.py
```

### Comparing `BDXConverter-1.0.14/LICENSE` & `BDXConverter-1.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.14/PKG-INFO` & `BDXConverter-1.0.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.14
+Version: 1.0.15
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,42 +93,47 @@
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
-    Any Operation eration of the BDX file will inherit this class
+    Any operation of the BDX file will inherit this class
     """
 
     def __init__(self) -> None:
         self.operationNumber: int
         self.operationName: str
 
     def Marshal(self, writer: BytesIO) -> None:
         """
-        Marshal GeneralClass into the writer
+        Marshal Self@GeneralClass into the writer(io object)
         """
         ...
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         """
-        Unmarshal the buffer(io object) into GeneralClass
+        Unmarshal the buffer(io object) into Self@GeneralClass
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
-        Convert jsonDict:dict into GeneralClass
+        Load datas from jsonDict:dict
         """
-        ...
+        if 'operationNumber' in self.__dict__:
+            jsonDict['operationNumber'] = self.operationNumber
+            jsonDict['operationName'] = self.operationName
+        for i in self.__dict__:
+            if i in jsonDict:
+                self.__dict__[i] = jsonDict[i]
 
     def Dumps(self) -> dict:
         """
-        Convert GeneralClass into basic dictionary
+        Convert Self@GeneralClass into the basic dictionary
         """
         return self.__dict__
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。
```

### Comparing `BDXConverter-1.0.14/README.md` & `BDXConverter-1.0.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -79,42 +79,47 @@
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
-    Any Operation eration of the BDX file will inherit this class
+    Any operation of the BDX file will inherit this class
     """
 
     def __init__(self) -> None:
         self.operationNumber: int
         self.operationName: str
 
     def Marshal(self, writer: BytesIO) -> None:
         """
-        Marshal GeneralClass into the writer
+        Marshal Self@GeneralClass into the writer(io object)
         """
         ...
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         """
-        Unmarshal the buffer(io object) into GeneralClass
+        Unmarshal the buffer(io object) into Self@GeneralClass
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
-        Convert jsonDict:dict into GeneralClass
+        Load datas from jsonDict:dict
         """
-        ...
+        if 'operationNumber' in self.__dict__:
+            jsonDict['operationNumber'] = self.operationNumber
+            jsonDict['operationName'] = self.operationName
+        for i in self.__dict__:
+            if i in jsonDict:
+                self.__dict__[i] = jsonDict[i]
 
     def Dumps(self) -> dict:
         """
-        Convert GeneralClass into basic dictionary
+        Convert Self@GeneralClass into the basic dictionary
         """
         return self.__dict__
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。
```

### Comparing `BDXConverter-1.0.14/setup.py` & `BDXConverter-1.0.15/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt', 'r+', encoding='utf-8') as file:
     dependences = file.read().strip().split('\n')
 
 with open('README.md', 'r+', encoding='utf-8') as file:
     long_description = file.read()
 
 with open('version', 'r+', encoding='utf-8') as file:
-    version = file.read()
+    version = file.read().strip()
 
 setuptools.setup(
     name='BDXConverter',
     version=version,
     author='Minecraft Muti-Media Organization',
     author_email='TriM-Organization@hotmail.com',
     description='A code library to marshal, unmarshal, visual and reverse visualization of BDX files',
```

