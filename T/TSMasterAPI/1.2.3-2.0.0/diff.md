# Comparing `tmp/TSMasterAPI-1.2.3.tar.gz` & `tmp/TSMasterAPI-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-1.2.3.tar", last modified: Wed Apr 12 10:00:57 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.0.0.tar", last modified: Fri May  5 02:53:10 2023, max compression
```

## Comparing `TSMasterAPI-1.2.3.tar` & `TSMasterAPI-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.062585 TSMasterAPI-1.2.3/
--rw-rw-rw-   0        0        0     1024 2023-04-12 10:00:57.055643 TSMasterAPI-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.046611 TSMasterAPI-1.2.3/TSMasterAPI/
--rw-rw-rw-   0        0        0   151843 2023-04-12 09:54:48.000000 TSMasterAPI-1.2.3/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.3/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.054138 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-12 10:00:57.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.3/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:00:57.063087 TSMasterAPI-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-04-12 10:00:55.000000 TSMasterAPI-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.530181 TSMasterAPI-2.0.0/
+-rw-rw-rw-   0        0        0     1024 2023-05-05 02:53:10.529116 TSMasterAPI-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.511001 TSMasterAPI-2.0.0/TSMasterAPI/
+-rw-rw-rw-   0        0        0    32218 2023-04-24 02:03:02.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70568 2023-04-23 08:15:26.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1257 2023-04-21 03:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4382 2023-04-23 08:23:36.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    23724 2023-04-23 02:39:01.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.0/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.528036 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 02:53:10.531184 TSMasterAPI-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-05-05 02:53:02.000000 TSMasterAPI-2.0.0/setup.py
```

### Comparing `TSMasterAPI-1.2.3/PKG-INFO` & `TSMasterAPI-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.3
+Version: 2.0.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.2.3/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.0.0/TSMasterAPI/TSMasterAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-06 16:36:32
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 17:52:14
+LastEditTime: 2023-04-23 09:16:58
 github:https://github.com/sy950915/TSMasterAPI.git
 ''' 
 from ctypes import *
 from enum import Enum
 import copy
 import os
 from sys import getsizeof
@@ -1871,17 +1871,14 @@
     return dll.tscom_can_rbs_activate_message_by_name(AIdxChn,AEnable, ANetworkName, NodeName, MessageName)
 
 
 def tscom_can_rbs_activate_all_networks(AEnable: bool, AIncludingChildren: bool):
     return dll.tscom_can_rbs_activate_all_networks(AEnable, AIncludingChildren)
 
 
-def tscom_can_rbs_enable(AEnable: bool):
-    return dll.tscom_can_rbs_enable(AEnable)
-
 
 def tscom_can_rbs_get_signal_value_by_address(ASymboladdress: str, Avalue: c_double):
     return dll.tscom_can_rbs_get_signal_value_by_address(ASymboladdress, byref(Avalue))
 
 
 def tscom_can_rbs_get_signal_value_by_element(AIdchn: c_int32, ANetwork: str, ANodeName: str, AMessageName: str,
                                               ASignalName: str, Avalue: c_double):
@@ -1971,15 +1968,15 @@
     r = dll.tslog_add_online_replay_config(AFileName.encode("utf8"), byref(AIndex))
     return r
 
 
 # 设置在线回放配置
 def tslog_set_online_replay_config(AIndex: c_int32, AName: str, AFileName: str, AAutoStart: c_bool,
                                    AIsRepetitiveMode: c_bool, AStartTimingMode: c_int32, AStartDelayTimeMs: c_int32,
-                                   ASendTx: c_bool, ASendRx: c_bool, AMappings: c_char * 32):
+                                   ASendTx: c_bool, ASendRx: c_bool, AMappings: c_char_p):
     r = dll.tslog_set_online_replay_config(AIndex, AName, AFileName, AAutoStart, AIsRepetitiveMode, AStartTimingMode,
                                            AStartDelayTimeMs, ASendTx, ASendRx, AMappings)
     return r
 
 
 # 获取在线回放文件数量
 def tslog_get_online_replay_count(ACount: c_int32):
@@ -2136,15 +2133,15 @@
     tslog_blf_read_end(blfID)
     tslog_blf_write_end(writeHandle)
     """
     r = dll.tslog_blf_write_can(AHeadle, byref(ACAN))
     return r
 
 
-def tslog_blf_write_canfd(AHeadle: c_int32, ACANFD: TLIBCANFD):
+def tslog_blf_write_can_fd(AHeadle: c_int32, ACANFD: TLIBCANFD):
     """
     blfID = c_int32(0)
     count = c_ulong(0)
     tslog_blf_read_start(b'D:/1.blf', blfID, count)
     realCount = c_ulong(0)
     messageType = TSupportedObjType.sotUnknown
     CANtemp = TLIBCAN()
@@ -2154,15 +2151,15 @@
         tslog_blf_read_object(blfID, realCount, messageType, CANtemp, LINtemp, CANFDtemp)
         if messageType.value == TSupportedObjType.sotCANFD.value:
             CANtemp.FIdxChn = 2
             tslog_blf_write_canfd(writeHandle, CANFDtemp)
     tslog_blf_read_end(blfID)
     tslog_blf_write_end(writeHandle)
     """
-    r = dll.tslog_blf_write_canfd(AHeadle, byref(ACANFD))
+    r = dll.tslog_blf_write_can_fd(AHeadle, byref(ACANFD))
     return r
 
 
 def tslog_blf_write_lin(AHeadle: c_int32, ALIN: TLIBLIN):
     """
     blfID = c_int32(0)
     count = c_ulong(0)
@@ -2647,25 +2644,25 @@
 def tstp_lin_master_request(AChnIdx: CHANNEL_INDEX, ANAD: c_int8, AData: bytearray, ADataNum: c_int,
                             ATimeoutMs: c_int32):
     AReqdata = POINTER(c_ubyte * len(AData))((c_ubyte * len(AData))(*AData))
     r = dll.tstp_lin_master_request(AChnIdx, ANAD, byref(AReqdata), c_int32(ADataNum), c_int32(ATimeoutMs))
     return r
 
 
-def tstp_lin_master_request_intervalms(AChnIdx: CHANNEL_INDEX, AData: c_int8):
+def tstp_lin_master_request_intervalms(AChnIdx: CHANNEL_INDEX, AData: c_uint16):
     r = dll.tstp_lin_master_request_intervalms(AChnIdx, AData)
     return r
 
 
 def tstp_lin_reset(AChnIdx: CHANNEL_INDEX):
     r = dll.tstp_lin_reset(AChnIdx)
     return r
 
 
-def tstp_lin_slave_response_intervalms(AChnIdx: CHANNEL_INDEX, AData: c_int8):
+def tstp_lin_slave_response_intervalms(AChnIdx: CHANNEL_INDEX, AData: c_uint16):
     r = dll.tstp_lin_slave_response_intervalms(AChnIdx, AData)
     return r
 
 
 def tsdiag_lin_read_data_by_identifier(AChnIdx: CHANNEL_INDEX, ANAD: c_int8, AId: c_ushort, AResNAD: c_byte,
                                        AResData: bytearray, AResDataNum: c_int32, ATimeoutMS: c_int32):
     Resdata = POINTER(c_ubyte * len(AResData))((c_ubyte * len(AResData))(*AResData))
```

### Comparing `TSMasterAPI-1.2.3/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.0.0/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.3
+Version: 2.0.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.2.3/license.txt` & `TSMasterAPI-2.0.0/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-1.2.3/setup.py` & `TSMasterAPI-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='1.2.3',  # 版本号
+      version='2.0.0',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

