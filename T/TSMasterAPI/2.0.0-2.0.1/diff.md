# Comparing `tmp/TSMasterAPI-2.0.0.tar.gz` & `tmp/TSMasterAPI-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.0.0.tar", last modified: Fri May  5 02:53:10 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.0.1.tar", last modified: Fri May  5 03:10:44 2023, max compression
```

## Comparing `TSMasterAPI-2.0.0.tar` & `TSMasterAPI-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.530181 TSMasterAPI-2.0.0/
--rw-rw-rw-   0        0        0     1024 2023-05-05 02:53:10.529116 TSMasterAPI-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.511001 TSMasterAPI-2.0.0/TSMasterAPI/
--rw-rw-rw-   0        0        0    32218 2023-04-24 02:03:02.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70568 2023-04-23 08:15:26.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1257 2023-04-21 03:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4382 2023-04-23 08:23:36.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    23724 2023-04-23 02:39:01.000000 TSMasterAPI-2.0.0/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.0/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:53:10.528036 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 02:53:10.000000 TSMasterAPI-2.0.0/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 02:53:10.531184 TSMasterAPI-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-05-05 02:53:02.000000 TSMasterAPI-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/
+-rw-rw-rw-   0        0        0     1024 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.533488 TSMasterAPI-2.0.1/TSMasterAPI/
+-rw-rw-rw-   0        0        0    32271 2023-05-05 03:07:38.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70571 2023-05-05 03:07:30.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   151756 2023-04-23 03:00:28.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    23491 2023-05-05 03:08:22.000000 TSMasterAPI-2.0.1/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.0.1/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:10:44.543583 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 03:10:44.000000 TSMasterAPI-2.0.1/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.0.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 03:10:44.544637 TSMasterAPI-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-05-05 03:10:11.000000 TSMasterAPI-2.0.1/setup.py
```

### Comparing `TSMasterAPI-2.0.0/PKG-INFO` & `TSMasterAPI-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSBUSDriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:19:14
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-24 10:03:01
+LastEditTime: 2023-05-05 11:07:38
+github:https://github.com/sy950915/TSMasterAPI.git
 '''
 import time
-from TSCommon import *
+from .TSCommon import *
 
 
 mapping = {
     "CAN":{"CHNCount":4,"HW_Names":["TC1014","TC1014","TC1014"],"HW_Chns":["0,1","0","3"]},
     "LIN":{"CHNCount":4,"HW_Names":["TC1016","TC1016","TC1016"],"HW_Chns":["0,1","0","1"]},
     "Flexray":{"CHNCount":4,"HW_Names":["TC1034","TC1034","TC1034"],"HW_Chns":["0,1","0","1"]}
 }
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
 LastEditTime: 2023-04-23 13:36:50
 '''
-from TSDirver import *
-from TSStructure import *  
-from TSEnumdefine import *  
+from .TSDirver import *
+from .TSStructure import *  
+from .TSEnumdefine import *  
 
 
 # Common Functions
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSDirver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:21:33
 LastEditors: seven 865762826@qq.com
 LastEditTime: 2023-04-21 11:53:08
-FilePath: \TSMasterAPI\TSMasterApi\TSMasterAPI\TSDirver.py
-Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from ctypes import WinDLL
 import os
 import winreg
 
 
 TSMaster_location = r"Software\TOSUN\TSMaster"
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSEnumdefine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 10:04:48
 LastEditors: seven 865762826@qq.com
 LastEditTime: 2023-04-21 10:17:38
-FilePath: \TSMasterAPI\TSMasterApi\TSMasterAPI\TSdefine.py
-Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from enum import IntEnum, IntFlag
 
 class MSGType(IntEnum):
     CANMSG = 0
     CANFDMSG = 1
     LINMSG = 2
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.0.1/TSMasterAPI/TSStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 10:21:17
 LastEditors: seven 865762826@qq.com
 LastEditTime: 2023-04-23 10:37:49
-FilePath: \TSMasterAPI\TSMasterApi\TSMasterAPI\TSStructure.py
-Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from ctypes import Structure,c_char,c_int32,c_bool,c_uint8,c_int64,c_uint64,c_uint32,c_uint16,c_double,c_char_p,byref,string_at,string_at,CDLL,CFUNCTYPE,POINTER,pointer,c_void_p,c_float,c_int16,c_int8,WINFUNCTYPE
 
 
 u8 = c_uint8
 pu8 = POINTER(c_uint8)
 s8 = c_int8
```

### Comparing `TSMasterAPI-2.0.0/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.0.1/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.0.0/license.txt` & `TSMasterAPI-2.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.0.0/setup.py` & `TSMasterAPI-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 18:00:55
+LastEditTime: 2023-05-05 11:10:11
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.0.0',  # 版本号
+      version='2.0.1',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

