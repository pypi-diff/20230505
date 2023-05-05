# Comparing `tmp/simplepyble-0.6.2.dev1.tar.gz` & `tmp/simplepyble-0.6.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepyble-0.6.2.dev1.tar", last modified: Sat Mar 18 22:49:58 2023, max compression
+gzip compressed data, was "simplepyble-0.6.2.dev2.tar", last modified: Fri May  5 18:02:08 2023, max compression
```

## Comparing `simplepyble-0.6.2.dev1.tar` & `simplepyble-0.6.2.dev2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.797365 simplepyble-0.6.2.dev1/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/cmake/epilogue.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.797365 simplepyble-0.6.2.dev1/cmake/find/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/cmake/find/FindDBus1.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/cmake/find/Findfmt.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/cmake/parse_version.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/cmake/prelude.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.797365 simplepyble-0.6.2.dev1/simpleble/
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.797365 simplepyble-0.6.2.dev1/simpleble/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/cmake/simpleble.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.785365 simplepyble-0.6.2.dev1/simpleble/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.801365 simplepyble-0.6.2.dev1/simpleble/include/simpleble/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Adapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/AdapterSafe.h
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Characteristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Descriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Peripheral.h
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/PeripheralSafe.h
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Service.h
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/SimpleBLE.h
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Types.h
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.805365 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/adapter.h
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/peripheral.h
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/simpleble.h
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/types.h
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.805365 simplepyble-0.6.2.dev1/simpleble/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/CommonUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/Exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/Logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/LoggingInternal.h
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/Utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.789365 simplepyble-0.6.2.dev1/simpleble/src/backends/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.809365 simplepyble-0.6.2.dev1/simpleble/src/backends/common/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/AdapterBaseTypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/CharacteristicBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/CharacteristicBase.h
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/DescriptorBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/DescriptorBase.h
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/ServiceBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/common/ServiceBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.809365 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/AdapterBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/AdapterBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/Bluez.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/Bluez.h
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/PeripheralBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/linux/PeripheralBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBase.mm
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBaseMacOS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBaseMacOS.mm
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBase.mm
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBaseMacOS.h
--rw-r--r--   0 runner    (1001) docker     (123)    25420 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBaseMacOS.mm
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/macos/Utils.mm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/backends/plain/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/plain/AdapterBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/plain/AdapterBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/plain/PeripheralBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/plain/PeripheralBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/AdapterBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/AdapterBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    18753 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/PeripheralBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/PeripheralBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/backends/windows/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/AdapterBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/AdapterBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/CharacteristicBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/CharacteristicBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/DescriptorBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/DescriptorBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/PeripheralBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/PeripheralBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/ServiceBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/builders/ServiceBuilder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/external/kvn_safe_callback.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/external/logfwd.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.789365 simplepyble-0.6.2.dev1/simpleble/src/frontends/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.813365 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Adapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Characteristic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Descriptor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Peripheral.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Service.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simpleble/src/frontends/safe/
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/safe/AdapterSafe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src/frontends/safe/PeripheralSafe.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simpleble/src_c/
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src_c/adapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src_c/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src_c/peripheral.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src_c/simpleble.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpleble/src_c/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simplebluez/
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simplebluez/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/cmake/simplebluez.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.789365 simplepyble-0.6.2.dev1/simplebluez/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Adapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Agent.h
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Bluez.h
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Characteristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Descriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Device.h
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/ProxyOrg.h
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/ProxyOrgBluez.h
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Service.h
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.817365 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Adapter1.h
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Agent1.h
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/AgentManager1.h
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Battery1.h
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Device1.h
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/GattCharacteristic1.h
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/GattDescriptor1.h
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/GattService1.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simplebluez/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Adapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Agent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Bluez.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Characteristic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Descriptor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Device.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/ProxyOrg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/ProxyOrgBluez.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/Service.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Adapter1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Agent1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/AgentManager1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Battery1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Device1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattCharacteristic1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattDescriptor1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattService1.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/cmake/simpledbus.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.793365 simplepyble-0.6.2.dev1/simpledbus/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.793365 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/advanced/Interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/advanced/Proxy.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Connection.h
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Holder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Message.h
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Path.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/external/kvn_safe_callback.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/external/logfwd.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/interfaces/ObjectManager.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.793365 simplepyble-0.6.2.dev1/simpledbus/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/src/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/advanced/Interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/advanced/Proxy.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/src/base/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Connection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Holder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Logging.h
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Message.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/base/Path.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simpledbus/src/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simpledbus/src/interfaces/ObjectManager.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.821365 simplepyble-0.6.2.dev1/simplepyble/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/simplepyble/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:49:58.825365 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-18 22:49:58.000000 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-03-18 22:49:58.000000 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 22:49:58.000000 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-18 22:49:58.000000 simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_adapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_characteristic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_descriptor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_peripheral.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_service.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-18 22:49:39.000000 simplepyble-0.6.2.dev1/simplepyble/src/wrap_types.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/cmake/epilogue.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/cmake/find/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/cmake/find/FindDBus1.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/cmake/find/Findfmt.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/cmake/parse_version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/cmake/prelude.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/simpleble/
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/simpleble/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/cmake/simpleble.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpleble/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/simpleble/include/simpleble/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Adapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/AdapterSafe.h
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Characteristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Descriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Peripheral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/PeripheralSafe.h
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Service.h
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/SimpleBLE.h
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/adapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/peripheral.h
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/simpleble.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.126860 simplepyble-0.6.2.dev2/simpleble/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/CommonUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/Exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/Logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/LoggingInternal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/Utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpleble/src/backends/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.130860 simplepyble-0.6.2.dev2/simpleble/src/backends/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/AdapterBaseTypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/CharacteristicBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/CharacteristicBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/DescriptorBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/DescriptorBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/ServiceBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/common/ServiceBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.130860 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/AdapterBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/AdapterBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/Bluez.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/Bluez.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/PeripheralBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/linux/PeripheralBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.130860 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBase.mm
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBaseMacOS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBaseMacOS.mm
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBase.mm
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBaseMacOS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25327 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBaseMacOS.mm
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/macos/Utils.mm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.130860 simplepyble-0.6.2.dev2/simpleble/src/backends/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/plain/AdapterBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/plain/AdapterBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/plain/PeripheralBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/plain/PeripheralBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.130860 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/AdapterBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/AdapterBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18753 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/PeripheralBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/PeripheralBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/backends/windows/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simpleble/src/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/AdapterBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/AdapterBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/CharacteristicBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/CharacteristicBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/DescriptorBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/DescriptorBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/PeripheralBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/PeripheralBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/ServiceBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/builders/ServiceBuilder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simpleble/src/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/external/kvn_safe_callback.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/external/logfwd.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpleble/src/frontends/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Adapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Characteristic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Descriptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Peripheral.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Service.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simpleble/src/frontends/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/safe/AdapterSafe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src/frontends/safe/PeripheralSafe.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simpleble/src_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src_c/adapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src_c/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src_c/peripheral.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src_c/simpleble.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpleble/src_c/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simplebluez/
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simplebluez/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/cmake/simplebluez.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simplebluez/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Adapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Agent.h
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Bluez.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Characteristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Descriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Device.h
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/ProxyOrg.h
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/ProxyOrgBluez.h
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Service.h
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.134860 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Adapter1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Agent1.h
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/AgentManager1.h
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Battery1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Device1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/GattCharacteristic1.h
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/GattDescriptor1.h
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/GattService1.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simplebluez/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Adapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Agent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Bluez.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Characteristic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Descriptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Device.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/ProxyOrg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/ProxyOrgBluez.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/Service.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Adapter1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Agent1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/AgentManager1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Battery1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Device1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattCharacteristic1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattDescriptor1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattService1.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/cmake/simpledbus.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpledbus/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/advanced/Interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/advanced/Proxy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Connection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Holder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Message.h
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Path.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/external/kvn_safe_callback.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/external/logfwd.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/interfaces/ObjectManager.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.122860 simplepyble-0.6.2.dev2/simpledbus/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.138860 simplepyble-0.6.2.dev2/simpledbus/src/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/advanced/Interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/advanced/Proxy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simpledbus/src/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Connection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Holder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Message.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/base/Path.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simpledbus/src/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simpledbus/src/interfaces/ObjectManager.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simplepyble/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simplepyble/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:02:08.142860 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-05 18:02:08.000000 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-05 18:02:08.000000 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:02:08.000000 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 18:02:08.000000 simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_adapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_characteristic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_descriptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_peripheral.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_service.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-05 18:01:50.000000 simplepyble-0.6.2.dev2/simplepyble/src/wrap_types.cpp
```

### Comparing `simplepyble-0.6.2.dev1/LICENSE.md` & `simplepyble-0.6.2.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/PKG-INFO` & `simplepyble-0.6.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepyble
-Version: 0.6.2.dev1
+Version: 0.6.2.dev2
 Summary: The ultimate fully-fledged cross-platform BLE library, designed for simplicity and ease of use.
 Home-page: https://github.com/OpenBluetoothToolbox/SimpleBLE
 Author: Kevin Dewald
 Author-email: kevin@dewald.me
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `simplepyble-0.6.2.dev1/cmake/epilogue.cmake` & `simplepyble-0.6.2.dev2/cmake/epilogue.cmake`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/cmake/find/FindDBus1.cmake` & `simplepyble-0.6.2.dev2/cmake/find/FindDBus1.cmake`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/cmake/find/Findfmt.cmake` & `simplepyble-0.6.2.dev2/cmake/find/Findfmt.cmake`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/cmake/parse_version.cmake` & `simplepyble-0.6.2.dev2/cmake/parse_version.cmake`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/setup.py` & `simplepyble-0.6.2.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 sys.argv = [sys.argv[0]] + unknown
 
 root = pathlib.Path(__file__).parent.resolve()
 
 # Generate the version string
 # TODO: Make the dev portion smarter by looking at tags.
 version_str = (root / "VERSION").read_text(encoding="utf-8").strip()
-version_str += ".dev1"  # ! Ensure it matches the intended release version!
+version_str += ".dev2"  # ! Ensure it matches the intended release version!
 
 # Get the long description from the README file
 long_description = (root / "simplepyble" / "README.rst").read_text(encoding="utf-8")
 
 cmake_options = []
 cmake_options.append(f"-Dpybind11_DIR={pybind11.get_cmake_dir()}")
 if sys.platform == "win32":
```

### Comparing `simplepyble-0.6.2.dev1/simpleble/CMakeLists.txt` & `simplepyble-0.6.2.dev2/simpleble/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Adapter.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Adapter.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/AdapterSafe.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/AdapterSafe.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Characteristic.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Characteristic.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Exceptions.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Exceptions.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Logging.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Logging.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Peripheral.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Peripheral.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/PeripheralSafe.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/PeripheralSafe.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Service.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Service.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble/Types.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble/Types.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/adapter.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/adapter.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/logging.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/logging.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/peripheral.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/peripheral.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/types.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/types.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/include/simpleble_c/utils.h` & `simplepyble-0.6.2.dev2/simpleble/include/simpleble_c/utils.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/CommonUtils.h` & `simplepyble-0.6.2.dev2/simpleble/src/CommonUtils.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/Exceptions.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/Exceptions.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/Logging.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/Logging.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/LoggingInternal.h` & `simplepyble-0.6.2.dev2/simpleble/src/LoggingInternal.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/common/CharacteristicBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/common/CharacteristicBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/common/CharacteristicBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/common/CharacteristicBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/common/ServiceBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/common/ServiceBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/common/ServiceBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/common/ServiceBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/linux/AdapterBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/linux/AdapterBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/linux/AdapterBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/linux/AdapterBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/linux/Bluez.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/linux/Bluez.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/linux/PeripheralBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/linux/PeripheralBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/linux/PeripheralBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/linux/PeripheralBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBase.mm` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBase.mm`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 bool AdapterBase::scan_is_active() {
     AdapterBaseMacOS* internal = (__bridge AdapterBaseMacOS*)opaque_internal_;
     return [internal scanIsActive];
 }
 
 std::vector<Peripheral> AdapterBase::scan_get_results() {
     std::vector<Peripheral> peripherals;
-    for (auto& [opaque_peripheral, base_peripheral] : this->peripherals_) {
+    for (auto& [opaque_peripheral, base_peripheral] : this->seen_peripherals_) {
         PeripheralBuilder peripheral_builder(base_peripheral);
         peripherals.push_back(peripheral_builder);
     }
     return peripherals;
 }
 
 void AdapterBase::set_callback_on_scan_start(std::function<void()> on_scan_start) {
```

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/AdapterBaseMacOS.mm` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/AdapterBaseMacOS.mm`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return CBCentralManager.authorization == CBManagerAuthorizationAllowedAlways && _centralManager.state == CBManagerStatePoweredOn;
 }
 
 - (instancetype)init:(SimpleBLE::AdapterBase*)adapter {
     self = [super init];
     if (self) {
         _adapter = adapter;
-        _uuid = [[NSUUID UUID] UUIDString];
+        _uuid = @"39a76676-2788-46c9-afa0-f0c0c31e6fd9";
 
         // Use a high-priority queue to ensure that events are processed immediately.
         dispatch_queue_attr_t qos = dispatch_queue_attr_make_with_qos_class(DISPATCH_QUEUE_SERIAL, QOS_CLASS_USER_INITIATED, -1);
         _centralManagerQueue = dispatch_queue_create("AdapterBaseMacOS.centralManagerQueue", qos);
         _centralManager = [[CBCentralManager alloc] initWithDelegate:self queue:_centralManagerQueue options:nil];
 
         // Wait for the central manager state to be updated for up to 5 seconds.
```

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBase.mm` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBase.mm`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBaseMacOS.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBaseMacOS.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/macos/PeripheralBaseMacOS.mm` & `simplepyble-0.6.2.dev2/simpleble/src/backends/macos/PeripheralBaseMacOS.mm`

 * *Files 0% similar despite different names*

```diff
@@ -84,18 +84,17 @@
 
         if (self.peripheral.state != CBPeripheralStateConnected) {
             throw SimpleBLE::Exception::OperationFailed("Peripheral Connection");
         }
 
         [self.peripheral discoverServices:nil];
 
-        // Wait for services to be discovered for up to 1 second.
+        // Wait for services to be discovered
         // NOTE: This is a bit of a hack but avoids the need of having a dedicated flag.
-        endDate = [NSDate dateWithTimeInterval:1.0 sinceDate:NSDate.now];
-        while (self.peripheral.services == nil && [NSDate.now compare:endDate] == NSOrderedAscending) {
+        while (self.peripheral.services == nil && self.peripheral.state == CBPeripheralStateConnected) {
             [NSThread sleepForTimeInterval:0.01];
         }
 
         if (self.peripheral.services == nil) {
             // If services could not be discovered, raise an exception.
             NSLog(@"Services could not be discovered.");
             throw SimpleBLE::Exception::OperationFailed("Service Discovery");
```

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/plain/AdapterBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/plain/AdapterBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/plain/AdapterBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/plain/AdapterBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/plain/PeripheralBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/plain/PeripheralBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/plain/PeripheralBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/plain/PeripheralBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/AdapterBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/AdapterBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/AdapterBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/AdapterBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/PeripheralBase.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/PeripheralBase.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/PeripheralBase.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/PeripheralBase.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/Utils.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/Utils.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/backends/windows/Utils.h` & `simplepyble-0.6.2.dev2/simpleble/src/backends/windows/Utils.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/AdapterBuilder.h` & `simplepyble-0.6.2.dev2/simpleble/src/builders/AdapterBuilder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/CharacteristicBuilder.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/builders/CharacteristicBuilder.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/CharacteristicBuilder.h` & `simplepyble-0.6.2.dev2/simpleble/src/builders/CharacteristicBuilder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/DescriptorBuilder.h` & `simplepyble-0.6.2.dev2/simpleble/src/builders/DescriptorBuilder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/PeripheralBuilder.h` & `simplepyble-0.6.2.dev2/simpleble/src/builders/PeripheralBuilder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/ServiceBuilder.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/builders/ServiceBuilder.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/builders/ServiceBuilder.h` & `simplepyble-0.6.2.dev2/simpleble/src/builders/ServiceBuilder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/external/kvn_safe_callback.hpp` & `simplepyble-0.6.2.dev2/simpleble/src/external/kvn_safe_callback.hpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/external/logfwd.hpp` & `simplepyble-0.6.2.dev2/simpleble/src/external/logfwd.hpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Adapter.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Adapter.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Characteristic.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Characteristic.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/frontends/base/Peripheral.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/frontends/base/Peripheral.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/frontends/safe/AdapterSafe.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/frontends/safe/AdapterSafe.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src/frontends/safe/PeripheralSafe.cpp` & `simplepyble-0.6.2.dev2/simpleble/src/frontends/safe/PeripheralSafe.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src_c/adapter.cpp` & `simplepyble-0.6.2.dev2/simpleble/src_c/adapter.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src_c/logging.cpp` & `simplepyble-0.6.2.dev2/simpleble/src_c/logging.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpleble/src_c/peripheral.cpp` & `simplepyble-0.6.2.dev2/simpleble/src_c/peripheral.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/CMakeLists.txt` & `simplepyble-0.6.2.dev2/simplebluez/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Adapter.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Adapter.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Agent.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Agent.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Bluez.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Bluez.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Characteristic.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Characteristic.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Descriptor.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Descriptor.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Device.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Device.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Exceptions.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Exceptions.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/ProxyOrg.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/ProxyOrg.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/ProxyOrgBluez.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/ProxyOrgBluez.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/Service.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/Service.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Adapter1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Adapter1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Agent1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Agent1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Battery1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Battery1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/Device1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/Device1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/GattCharacteristic1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/GattCharacteristic1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/include/simplebluez/interfaces/GattDescriptor1.h` & `simplepyble-0.6.2.dev2/simplebluez/include/simplebluez/interfaces/GattDescriptor1.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Adapter.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Adapter.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Agent.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Agent.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Bluez.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Bluez.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Characteristic.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Characteristic.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Descriptor.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Descriptor.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Device.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Device.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Exceptions.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Exceptions.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Logging.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Logging.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Logging.h` & `simplepyble-0.6.2.dev2/simplebluez/src/Logging.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/ProxyOrg.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/ProxyOrg.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/ProxyOrgBluez.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/ProxyOrgBluez.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/Service.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/Service.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Adapter1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Adapter1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Agent1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Agent1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/AgentManager1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/AgentManager1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Battery1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Battery1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/Device1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/Device1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattCharacteristic1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattCharacteristic1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattDescriptor1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattDescriptor1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplebluez/src/interfaces/GattService1.cpp` & `simplepyble-0.6.2.dev2/simplebluez/src/interfaces/GattService1.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/CMakeLists.txt` & `simplepyble-0.6.2.dev2/simpledbus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/advanced/Interface.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/advanced/Interface.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/advanced/Proxy.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/advanced/Proxy.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Connection.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Connection.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Exceptions.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Exceptions.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Holder.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Holder.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Message.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Message.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/base/Path.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/base/Path.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/external/kvn_safe_callback.hpp` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/external/kvn_safe_callback.hpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/external/logfwd.hpp` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/external/logfwd.hpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/include/simpledbus/interfaces/ObjectManager.h` & `simplepyble-0.6.2.dev2/simpledbus/include/simpledbus/interfaces/ObjectManager.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/advanced/Interface.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/advanced/Interface.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/advanced/Proxy.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/advanced/Proxy.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Connection.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Connection.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Exceptions.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Exceptions.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Holder.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Holder.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Logging.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Logging.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Logging.h` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Logging.h`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Message.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Message.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/base/Path.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/base/Path.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simpledbus/src/interfaces/ObjectManager.cpp` & `simplepyble-0.6.2.dev2/simpledbus/src/interfaces/ObjectManager.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/CMakeLists.txt` & `simplepyble-0.6.2.dev2/simplepyble/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/README.rst` & `simplepyble-0.6.2.dev2/simplepyble/README.rst`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/main.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/main.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/PKG-INFO` & `simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepyble
-Version: 0.6.2.dev1
+Version: 0.6.2.dev2
 Summary: The ultimate fully-fledged cross-platform BLE library, designed for simplicity and ease of use.
 Home-page: https://github.com/OpenBluetoothToolbox/SimpleBLE
 Author: Kevin Dewald
 Author-email: kevin@dewald.me
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/simplepyble.egg-info/SOURCES.txt` & `simplepyble-0.6.2.dev2/simplepyble/src/simplepyble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/wrap_adapter.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/wrap_adapter.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/wrap_descriptor.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/wrap_descriptor.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/wrap_peripheral.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/wrap_peripheral.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -145,20 +145,22 @@
             },
             kDocsPeripheralReadCharacteristic)
         .def(
             "write_request",
             [](SimpleBLE::Peripheral& p, std::string service, std::string characteristic, py::bytes payload) {
                 p.write_request(service, characteristic, payload);
             },
+            py::call_guard<py::gil_scoped_release>(),
             kDocsPeripheralWriteRequest)
         .def(
             "write_command",
             [](SimpleBLE::Peripheral& p, std::string service, std::string characteristic, py::bytes payload) {
                 p.write_command(service, characteristic, payload);
             },
+            py::call_guard<py::gil_scoped_release>(),
             kDocsPeripheralWriteCommand)
         .def(
             "notify",
             [](SimpleBLE::Peripheral& p, std::string service, std::string characteristic,
                std::function<void(py::bytes payload)> cb) {
                 p.notify(service, characteristic, [cb](SimpleBLE::ByteArray payload) { cb(py::bytes(payload)); });
             },
```

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/wrap_service.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/wrap_service.cpp`

 * *Files identical despite different names*

### Comparing `simplepyble-0.6.2.dev1/simplepyble/src/wrap_types.cpp` & `simplepyble-0.6.2.dev2/simplepyble/src/wrap_types.cpp`

 * *Files identical despite different names*

