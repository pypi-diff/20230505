# Comparing `tmp/rnspure-0.5.0.tar.gz` & `tmp/rnspure-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnspure-0.5.0.tar", last modified: Wed Mar  8 13:45:37 2023, max compression
+gzip compressed data, was "rnspure-0.5.1.tar", last modified: Fri May  5 09:18:34 2023, max compression
```

## Comparing `rnspure-0.5.0.tar` & `rnspure-0.5.1.tar`

### file list

```diff
@@ -1,91 +1,97 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.458288 rnspure-0.5.0/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rnspure-0.5.0/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18910 2023-03-08 13:45:37.458288 rnspure-0.5.0/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    18171 2023-02-23 16:10:19.000000 rnspure-0.5.0/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.438288 rnspure-0.5.0/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10082 2023-03-05 17:21:52.000000 rnspure-0.5.0/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19810 2023-03-05 17:21:52.000000 rnspure-0.5.0/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.441622 rnspure-0.5.0/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.5.0/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.441622 rnspure-0.5.0/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.441622 rnspure-0.5.0/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rnspure-0.5.0/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rnspure-0.5.0/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.448288 rnspure-0.5.0/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.448288 rnspure-0.5.0/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rnspure-0.5.0/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49038 2023-02-18 12:40:20.000000 rnspure-0.5.0/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rnspure-0.5.0/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.5.0/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19934 2023-03-07 15:40:16.000000 rnspure-0.5.0/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rnspure-0.5.0/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12643 2023-03-05 17:21:52.000000 rnspure-0.5.0/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30634 2023-02-18 12:01:00.000000 rnspure-0.5.0/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    22238 2022-11-03 13:15:05.000000 rnspure-0.5.0/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4824 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.5.0/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52133 2023-03-05 17:21:52.000000 rnspure-0.5.0/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    21743 2023-03-02 11:05:06.000000 rnspure-0.5.0/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45889 2022-12-19 00:09:16.000000 rnspure-0.5.0/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65037 2023-03-08 13:34:33.000000 rnspure-0.5.0/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129918 2023-03-05 17:21:52.000000 rnspure-0.5.0/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.454955 rnspure-0.5.0/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rnspure-0.5.0/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-02-03 19:26:09.000000 rnspure-0.5.0/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)   198943 2023-03-04 15:46:18.000000 rnspure-0.5.0/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12816 2022-10-29 11:39:50.000000 rnspure-0.5.0/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rnspure-0.5.0/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.5.0/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rnspure-0.5.0/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-03-04 15:40:47.000000 rnspure-0.5.0/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.454955 rnspure-0.5.0/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.458288 rnspure-0.5.0/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/i2plib/utils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.5.0/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.5.0/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-03-08 13:45:37.458288 rnspure-0.5.0/rnspure.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18910 2023-03-08 13:45:37.000000 rnspure-0.5.0/rnspure.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2085 2023-03-08 13:45:37.000000 rnspure-0.5.0/rnspure.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-03-08 13:45:37.000000 rnspure-0.5.0/rnspure.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-03-08 13:45:37.000000 rnspure-0.5.0/rnspure.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-03-08 13:45:37.000000 rnspure-0.5.0/rnspure.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-03-08 13:45:37.461622 rnspure-0.5.0/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1983 2023-03-07 15:24:16.000000 rnspure-0.5.0/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rnspure-0.5.1/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-05 09:18:34.449933 rnspure-0.5.1/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rnspure-0.5.1/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.446600 rnspure-0.5.1/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10082 2023-03-05 17:21:52.000000 rnspure-0.5.1/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19810 2023-03-05 17:21:52.000000 rnspure-0.5.1/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.446600 rnspure-0.5.1/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.5.1/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.446600 rnspure-0.5.1/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.446600 rnspure-0.5.1/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rnspure-0.5.1/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rnspure-0.5.1/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.446600 rnspure-0.5.1/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rnspure-0.5.1/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rnspure-0.5.1/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rnspure-0.5.1/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.5.1/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20050 2023-05-04 15:53:57.000000 rnspure-0.5.1/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rnspure-0.5.1/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-03 10:21:20.000000 rnspure-0.5.1/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rnspure-0.5.1/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rnspure-0.5.1/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rnspure-0.5.1/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.5.1/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52133 2023-03-05 17:21:52.000000 rnspure-0.5.1/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    21750 2023-05-02 15:27:36.000000 rnspure-0.5.1/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45889 2022-12-19 00:09:16.000000 rnspure-0.5.1/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rnspure-0.5.1/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129918 2023-03-05 17:21:52.000000 rnspure-0.5.1/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rnspure-0.5.1/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-02-03 19:26:09.000000 rnspure-0.5.1/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)   205846 2023-05-03 13:56:01.000000 rnspure-0.5.1/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rnspure-0.5.1/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rnspure-0.5.1/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.5.1/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rnspure-0.5.1/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-05-03 10:25:12.000000 rnspure-0.5.1/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rnspure-0.5.1/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rnspure-0.5.1/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rnspure-0.5.1/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rnspure-0.5.1/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rnspure-0.5.1/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.5.1/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.5.1/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:34.449933 rnspure-0.5.1/rnspure.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-05 09:18:34.000000 rnspure-0.5.1/rnspure.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2231 2023-05-05 09:18:34.000000 rnspure-0.5.1/rnspure.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-05-05 09:18:34.000000 rnspure-0.5.1/rnspure.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-05-05 09:18:34.000000 rnspure-0.5.1/rnspure.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-05-05 09:18:34.000000 rnspure-0.5.1/rnspure.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-05-05 09:18:34.449933 rnspure-0.5.1/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rnspure-0.5.1/setup.py
```

### Comparing `rnspure-0.5.0/LICENSE` & `rnspure-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/PKG-INFO` & `rnspure-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: rnspure
-Version: 0.5.0
+Version: 0.5.1
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Reticulum Network Stack β <img align="right" src="https://static.pepy.tech/personalized-badge/rns?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs"/>
 ==========
 
 <p align="center"><img width="200" src="https://raw.githubusercontent.com/markqvist/Reticulum/master/docs/source/graphics/rns_logo_512.png"></p>
@@ -202,15 +202,14 @@
 ## Dependencies
 The installation of the default `rns` package requires the dependencies listed
 below. Almost all systems and distributions have readily available packages for
 these dependencies, and when the `rns` package is installed with `pip`, they
 will be downloaded and installed as well.
 
 - [PyCA/cryptography](https://github.com/pyca/cryptography)
-- [netifaces](https://github.com/al45tair/netifaces)
 - [pyserial](https://github.com/pyserial/pyserial)
 
 On more unusual systems, and in some rare cases, it might not be possible to
 install or even compile one or more of the above modules. In such situations,
 you can use the `rnspure` package instead, which require no external
 dependencies for installation. Please note that the contents of the `rns` and
 `rnspure` packages are *identical*. The only difference is that the `rnspure`
@@ -240,39 +239,33 @@
 before it is publicly released). Sometimes experimental versions of Reticulum
 might be deployed to nodes on the testnet, which means strange behaviour might
 occur. If none of that scares you, you can join the testnet via either TCP or
 I2P. Just add one of the following interfaces to your Reticulum configuration
 file:
 
 ```
-# TCP/IP interface to the Dublin Hub
+# TCP/IP interface to the RNS Dublin Hub
   [[RNS Testnet Dublin]]
     type = TCPClientInterface
     enabled = yes
     target_host = dublin.connect.reticulum.network
     target_port = 4965
 
-# TCP/IP interface to the Frankfurt Hub
-  [[RNS Testnet Frankfurt]]
+# TCP/IP interface to the BetweenTheBorders Hub (community-provided)
+  [[RNS Testnet BetweenTheBorders]]
     type = TCPClientInterface
     enabled = yes
-    target_host = frankfurt.connect.reticulum.network
-    target_port = 5377
+    target_host = betweentheborders.com
+    target_port = 4242
 
-# Interface to I2P Hub A
-  [[RNS Testnet I2P Hub A]]
+# Interface to Testnet I2P Hub
+  [[RNS Testnet I2P Hub]]
     type = I2PInterface
     enabled = yes
     peers = pmlm3l5rpympihoy2o5ago43kluei2jjjzsalcuiuylbve3mwi2a.b32.i2p
-
-# Interface to I2P Hub B
-  [[RNS Testnet I2P Hub B]]
-    type = I2PInterface
-    enabled = yes
-    peers = iwoqtz22dsr73aemwpw7guocplsjjoamyl7sogj33qtcd6ds4mza.b32.i2p
 ```
 
 The testnet also contains a number of [Nomad Network](https://github.com/markqvist/nomadnet) nodes, and LXMF propagation nodes.
 
 ## Support Reticulum
 You can help support the continued development of open, free and private communications systems by donating via one of the following channels:
 
@@ -353,12 +346,12 @@
 - [PyCA/cryptography](https://github.com/pyca/cryptography), *BSD License*
 - [Pure-25519](https://github.com/warner/python-pure25519) by [Brian Warner](https://github.com/warner), *MIT License*
 - [Pysha2](https://github.com/thomdixon/pysha2) by [Thom Dixon](https://github.com/thomdixon), *MIT License*
 - [Python-AES](https://github.com/orgurar/python-aes) by [Or Gur Arie](https://github.com/orgurar), *MIT License*
 - [Curve25519.py](https://gist.github.com/nickovs/cc3c22d15f239a2640c185035c06f8a3#file-curve25519-py) by [Nicko van Someren](https://gist.github.com/nickovs), *Public Domain*
 - [I2Plib](https://github.com/l-n-s/i2plib) by [Viktor Villainov](https://github.com/l-n-s)
 - [PySerial](https://github.com/pyserial/pyserial) by Chris Liechti, *BSD License*
-- [Netifaces](https://github.com/al45tair/netifaces) by [Alastair Houghton](https://github.com/al45tair), *MIT License*
 - [Configobj](https://github.com/DiffSK/configobj) by Michael Foord, Nicola Larosa, Rob Dennis & Eli Courtwright, *BSD License*
 - [Six](https://github.com/benjaminp/six) by [Benjamin Peterson](https://github.com/benjaminp), *MIT License*
+- [ifaddr](https://github.com/pydron/ifaddr) by [Pydron](https://github.com/pydron), *MIT License*
 - [Umsgpack.py](https://github.com/vsergeev/u-msgpack-python) by [Ivan A. Sergeev](https://github.com/vsergeev)
 - [Python](https://www.python.org)
```

### Comparing `rnspure-0.5.0/README.md` & `rnspure-0.5.1/rnspure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+Metadata-Version: 2.1
+Name: rnspure
+Version: 0.5.1
+Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
+Home-page: https://reticulum.network/
+Author: Mark Qvist
+Author-email: mark@unsigned.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Reticulum Network Stack β <img align="right" src="https://static.pepy.tech/personalized-badge/rns?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs"/>
 ==========
 
 <p align="center"><img width="200" src="https://raw.githubusercontent.com/markqvist/Reticulum/master/docs/source/graphics/rns_logo_512.png"></p>
 
+**Warning!** *This package is the zero-dependency version of Reticulum. You should almost certainly use the [normal package](https://pypi.org/project/rns) instead. Do NOT install this package unless you know exactly why you are doing it!*
+
 Reticulum is the cryptography-based networking stack for building local and wide-area
 networks with readily available hardware. It can operate even with very high latency
 and extremely low bandwidth. Reticulum allows you to build wide-area networks
 with off-the-shelf tools, and offers end-to-end encryption and connectivity,
 initiator anonymity, autoconfiguring cryptographically backed multi-hop
 transport, efficient addressing, unforgeable delivery acknowledgements and
 more.
@@ -186,15 +202,14 @@
 ## Dependencies
 The installation of the default `rns` package requires the dependencies listed
 below. Almost all systems and distributions have readily available packages for
 these dependencies, and when the `rns` package is installed with `pip`, they
 will be downloaded and installed as well.
 
 - [PyCA/cryptography](https://github.com/pyca/cryptography)
-- [netifaces](https://github.com/al45tair/netifaces)
 - [pyserial](https://github.com/pyserial/pyserial)
 
 On more unusual systems, and in some rare cases, it might not be possible to
 install or even compile one or more of the above modules. In such situations,
 you can use the `rnspure` package instead, which require no external
 dependencies for installation. Please note that the contents of the `rns` and
 `rnspure` packages are *identical*. The only difference is that the `rnspure`
@@ -224,39 +239,33 @@
 before it is publicly released). Sometimes experimental versions of Reticulum
 might be deployed to nodes on the testnet, which means strange behaviour might
 occur. If none of that scares you, you can join the testnet via either TCP or
 I2P. Just add one of the following interfaces to your Reticulum configuration
 file:
 
 ```
-# TCP/IP interface to the Dublin Hub
+# TCP/IP interface to the RNS Dublin Hub
   [[RNS Testnet Dublin]]
     type = TCPClientInterface
     enabled = yes
     target_host = dublin.connect.reticulum.network
     target_port = 4965
 
-# TCP/IP interface to the Frankfurt Hub
-  [[RNS Testnet Frankfurt]]
+# TCP/IP interface to the BetweenTheBorders Hub (community-provided)
+  [[RNS Testnet BetweenTheBorders]]
     type = TCPClientInterface
     enabled = yes
-    target_host = frankfurt.connect.reticulum.network
-    target_port = 5377
+    target_host = betweentheborders.com
+    target_port = 4242
 
-# Interface to I2P Hub A
-  [[RNS Testnet I2P Hub A]]
+# Interface to Testnet I2P Hub
+  [[RNS Testnet I2P Hub]]
     type = I2PInterface
     enabled = yes
     peers = pmlm3l5rpympihoy2o5ago43kluei2jjjzsalcuiuylbve3mwi2a.b32.i2p
-
-# Interface to I2P Hub B
-  [[RNS Testnet I2P Hub B]]
-    type = I2PInterface
-    enabled = yes
-    peers = iwoqtz22dsr73aemwpw7guocplsjjoamyl7sogj33qtcd6ds4mza.b32.i2p
 ```
 
 The testnet also contains a number of [Nomad Network](https://github.com/markqvist/nomadnet) nodes, and LXMF propagation nodes.
 
 ## Support Reticulum
 You can help support the continued development of open, free and private communications systems by donating via one of the following channels:
 
@@ -337,12 +346,12 @@
 - [PyCA/cryptography](https://github.com/pyca/cryptography), *BSD License*
 - [Pure-25519](https://github.com/warner/python-pure25519) by [Brian Warner](https://github.com/warner), *MIT License*
 - [Pysha2](https://github.com/thomdixon/pysha2) by [Thom Dixon](https://github.com/thomdixon), *MIT License*
 - [Python-AES](https://github.com/orgurar/python-aes) by [Or Gur Arie](https://github.com/orgurar), *MIT License*
 - [Curve25519.py](https://gist.github.com/nickovs/cc3c22d15f239a2640c185035c06f8a3#file-curve25519-py) by [Nicko van Someren](https://gist.github.com/nickovs), *Public Domain*
 - [I2Plib](https://github.com/l-n-s/i2plib) by [Viktor Villainov](https://github.com/l-n-s)
 - [PySerial](https://github.com/pyserial/pyserial) by Chris Liechti, *BSD License*
-- [Netifaces](https://github.com/al45tair/netifaces) by [Alastair Houghton](https://github.com/al45tair), *MIT License*
 - [Configobj](https://github.com/DiffSK/configobj) by Michael Foord, Nicola Larosa, Rob Dennis & Eli Courtwright, *BSD License*
 - [Six](https://github.com/benjaminp/six) by [Benjamin Peterson](https://github.com/benjaminp), *MIT License*
+- [ifaddr](https://github.com/pydron/ifaddr) by [Pydron](https://github.com/pydron), *MIT License*
 - [Umsgpack.py](https://github.com/vsergeev/u-msgpack-python) by [Ivan A. Sergeev](https://github.com/vsergeev)
 - [Python](https://www.python.org)
```

### Comparing `rnspure-0.5.0/RNS/Buffer.py` & `rnspure-0.5.1/RNS/Buffer.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Channel.py` & `rnspure-0.5.1/RNS/Channel.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/AES.py` & `rnspure-0.5.1/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/Ed25519.py` & `rnspure-0.5.1/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/Fernet.py` & `rnspure-0.5.1/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/HKDF.py` & `rnspure-0.5.1/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/HMAC.py` & `rnspure-0.5.1/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/Hashes.py` & `rnspure-0.5.1/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/PKCS7.py` & `rnspure-0.5.1/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/Provider.py` & `rnspure-0.5.1/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/Proxies.py` & `rnspure-0.5.1/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/SHA256.py` & `rnspure-0.5.1/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/SHA512.py` & `rnspure-0.5.1/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/X25519.py` & `rnspure-0.5.1/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/__init__.py` & `rnspure-0.5.1/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/aes/aes.py` & `rnspure-0.5.1/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/aes/utils.py` & `rnspure-0.5.1/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/pure25519/_ed25519.py` & `rnspure-0.5.1/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/pure25519/basic.py` & `rnspure-0.5.1/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/pure25519/ed25519_oop.py` & `rnspure-0.5.1/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Cryptography/pure25519/eddsa.py` & `rnspure-0.5.1/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Destination.py` & `rnspure-0.5.1/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Identity.py` & `rnspure-0.5.1/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/AX25KISSInterface.py` & `rnspure-0.5.1/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/Android/KISSInterface.py` & `rnspure-0.5.1/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/Android/RNodeInterface.py` & `rnspure-0.5.1/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -999,15 +999,15 @@
                             self.platform = byte
                         elif (command == KISS.CMD_MCU):
                             self.mcu = byte
                         elif (command == KISS.CMD_ERROR):
                             if (byte == KISS.ERROR_INITRADIO):
                                 RNS.log(str(self)+" hardware initialisation error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Radio initialisation failure")
-                            elif (byte == KISS.ERROR_INITRADIO):
+                            elif (byte == KISS.ERROR_TXFAILED):
                                 RNS.log(str(self)+" hardware TX error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Hardware transmit failure")
                             else:
                                 RNS.log(str(self)+" hardware error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Unknown hardware failure")
                         elif (command == KISS.CMD_RESET):
                             if (byte == 0xF8):
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/Android/SerialInterface.py` & `rnspure-0.5.1/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/Android/__init__.py` & `rnspure-0.5.1/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/AutoInterface.py` & `rnspure-0.5.1/RNS/Interfaces/AutoInterface.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,24 +58,26 @@
     def descope_linklocal(self, link_local_addr):
         # Drop scope specifier expressd as %ifname (macOS)
         link_local_addr = link_local_addr.split("%")[0]
         # Drop embedded scope specifier (NetBSD, OpenBSD)
         link_local_addr = re.sub(r"fe80:[0-9a-f]*::","fe80::", link_local_addr)
         return link_local_addr
 
+    def list_interfaces(self):
+        ifs = self.netinfo.interfaces()
+        return ifs
+
+    def list_addresses(self, ifname):
+        ifas = self.netinfo.ifaddresses(ifname)
+        return ifas
+
     def __init__(self, owner, name, group_id=None, discovery_scope=None, discovery_port=None, data_port=None, allowed_interfaces=None, ignored_interfaces=None, configured_bitrate=None):
-        import importlib
-        if importlib.util.find_spec('netifaces') != None:
-            import netifaces
-        else:
-            RNS.log("Using AutoInterface requires the netifaces module.", RNS.LOG_CRITICAL)
-            RNS.log("You can install it with the command: python3 -m pip install netifaces", RNS.LOG_CRITICAL)
-            RNS.panic()
+        from RNS.vendor.ifaddr import niwrapper
+        self.netinfo = niwrapper
 
-        self.netifaces = netifaces
         self.rxb = 0
         self.txb = 0
 
         self.HW_MTU = 1064
 
         self.IN  = True
         self.OUT = False
@@ -144,33 +146,33 @@
         gt += ":"+"{:02x}".format(g[7]+(g[6]<<8))
         gt += ":"+"{:02x}".format(g[9]+(g[8]<<8))
         gt += ":"+"{:02x}".format(g[11]+(g[10]<<8))
         gt += ":"+"{:02x}".format(g[13]+(g[12]<<8))
         self.mcast_discovery_address = "ff1"+self.discovery_scope+":"+gt
 
         suitable_interfaces = 0
-        for ifname in self.netifaces.interfaces():
+        for ifname in self.list_interfaces():
             if RNS.vendor.platformutils.is_darwin() and ifname in AutoInterface.DARWIN_IGNORE_IFS and not ifname in self.allowed_interfaces:
                 RNS.log(str(self)+" skipping Darwin AWDL or tethering interface "+str(ifname), RNS.LOG_EXTREME)
             elif RNS.vendor.platformutils.is_darwin() and ifname == "lo0":
                 RNS.log(str(self)+" skipping Darwin loopback interface "+str(ifname), RNS.LOG_EXTREME)
             elif RNS.vendor.platformutils.is_android() and ifname in AutoInterface.ANDROID_IGNORE_IFS and not ifname in self.allowed_interfaces:
                 RNS.log(str(self)+" skipping Android system interface "+str(ifname), RNS.LOG_EXTREME)
             elif ifname in self.ignored_interfaces:
                 RNS.log(str(self)+" ignoring disallowed interface "+str(ifname), RNS.LOG_EXTREME)
             elif ifname in AutoInterface.ALL_IGNORE_IFS:
                 RNS.log(str(self)+" skipping interface "+str(ifname), RNS.LOG_EXTREME)
             else:
                 if len(self.allowed_interfaces) > 0 and not ifname in self.allowed_interfaces:
                     RNS.log(str(self)+" ignoring interface "+str(ifname)+" since it was not allowed", RNS.LOG_EXTREME)
                 else:
-                    addresses = self.netifaces.ifaddresses(ifname)
-                    if self.netifaces.AF_INET6 in addresses:
+                    addresses = self.list_addresses(ifname)
+                    if self.netinfo.AF_INET6 in addresses:
                         link_local_addr = None
-                        for address in addresses[self.netifaces.AF_INET6]:
+                        for address in addresses[self.netinfo.AF_INET6]:
                             if "addr" in address:
                                 if address["addr"].startswith("fe80:"):
                                     link_local_addr = self.descope_linklocal(address["addr"])
                                     self.link_local_addresses.append(link_local_addr)
                                     self.adopted_interfaces[ifname] = link_local_addr
                                     self.multicast_echoes[ifname] = time.time()
                                     RNS.log(str(self)+" Selecting link-local address "+str(link_local_addr)+" for interface "+str(ifname), RNS.LOG_EXTREME)
@@ -192,15 +194,19 @@
                             discovery_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_IF, if_struct)
 
                             # Join multicast group
                             mcast_group = socket.inet_pton(socket.AF_INET6, mcast_addr) + if_struct
                             discovery_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_JOIN_GROUP, mcast_group)
 
                             # Bind socket
-                            addr_info = socket.getaddrinfo(mcast_addr+"%"+ifname, self.discovery_port, socket.AF_INET6, socket.SOCK_DGRAM)
+                            if self.discovery_scope == AutoInterface.SCOPE_LINK:
+                                addr_info = socket.getaddrinfo(mcast_addr+"%"+ifname, self.discovery_port, socket.AF_INET6, socket.SOCK_DGRAM)
+                            else:
+                                addr_info = socket.getaddrinfo(mcast_addr, self.discovery_port, socket.AF_INET6, socket.SOCK_DGRAM)
+
                             discovery_socket.bind(addr_info[0][4])
 
                             # Set up thread for discovery packets
                             def discovery_loop():
                                 self.discovery_handler(discovery_socket, ifname)
 
                             thread = threading.Thread(target=discovery_loop)
@@ -210,14 +216,19 @@
                             suitable_interfaces += 1
 
         if suitable_interfaces == 0:
             RNS.log(str(self)+" could not autoconfigure. This interface currently provides no connectivity.", RNS.LOG_WARNING)
         else:
             self.receives = True
 
+            if configured_bitrate != None:
+                self.bitrate = configured_bitrate
+            else:
+                self.bitrate = AutoInterface.BITRATE_GUESS
+
             peering_wait = self.announce_interval*1.2
             RNS.log(str(self)+" discovering peers for "+str(round(peering_wait, 2))+" seconds...", RNS.LOG_VERBOSE)
 
             self.owner = owner
             socketserver.UDPServer.address_family = socket.AF_INET6
 
             for ifname in self.adopted_interfaces:
@@ -234,19 +245,14 @@
 
             job_thread = threading.Thread(target=self.peer_jobs)
             job_thread.daemon = True
             job_thread.start()
 
             time.sleep(peering_wait)
 
-            if configured_bitrate != None:
-                self.bitrate = configured_bitrate
-            else:
-                self.bitrate = AutoInterface.BITRATE_GUESS
-
             self.online = True
 
 
     def discovery_handler(self, socket, ifname):
         def announce_loop():
             self.announce_handler(ifname)
             
@@ -279,18 +285,18 @@
             for peer_addr in timed_out_peers:
                 removed_peer = self.peers.pop(peer_addr)
                 RNS.log(str(self)+" removed peer "+str(peer_addr)+" on "+str(removed_peer[0]), RNS.LOG_DEBUG)
 
             for ifname in self.adopted_interfaces:
                 # Check that the link-local address has not changed
                 try:
-                    addresses = self.netifaces.ifaddresses(ifname)
-                    if self.netifaces.AF_INET6 in addresses:
+                    addresses = self.list_addresses(ifname)
+                    if self.netinfo.AF_INET6 in addresses:
                         link_local_addr = None
-                        for address in addresses[self.netifaces.AF_INET6]:
+                        for address in addresses[self.netinfo.AF_INET6]:
                             if "addr" in address:
                                 if address["addr"].startswith("fe80:"):
                                     link_local_addr = self.descope_linklocal(address["addr"])
                                     if link_local_addr != self.adopted_interfaces[ifname]:
                                         old_link_local_address = self.adopted_interfaces[ifname]
                                         RNS.log("Replacing link-local address "+str(old_link_local_address)+" for "+str(ifname)+" with "+str(link_local_addr), RNS.LOG_DEBUG)
                                         self.adopted_interfaces[ifname] = link_local_addr
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/I2PInterface.py` & `rnspure-0.5.1/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/Interface.py` & `rnspure-0.5.1/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/KISSInterface.py` & `rnspure-0.5.1/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/LocalInterface.py` & `rnspure-0.5.1/RNS/Interfaces/LocalInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,21 @@
     @staticmethod
     def escape(data):
         data = data.replace(bytes([HDLC.ESC]), bytes([HDLC.ESC, HDLC.ESC^HDLC.ESC_MASK]))
         data = data.replace(bytes([HDLC.FLAG]), bytes([HDLC.ESC, HDLC.FLAG^HDLC.ESC_MASK]))
         return data
 
 class ThreadingTCPServer(socketserver.ThreadingMixIn, socketserver.TCPServer):
-    pass
+    def server_bind(self):
+        if RNS.vendor.platformutils.is_windows():
+            self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_EXCLUSIVEADDRUSE, 1)
+        else:
+            self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.socket.bind(self.server_address)
+        self.server_address = self.socket.getsockname()
 
 class LocalClientInterface(Interface):
     RECONNECT_WAIT = 3
 
     def __init__(self, owner, name, target_port = None, connected_socket=None):
         self.rxb = 0
         self.txb = 0
@@ -295,15 +301,14 @@
                 return createHandler
 
             self.owner = owner
             self.is_local_shared_instance = True
 
             address = (self.bind_ip, self.bind_port)
 
-            ThreadingTCPServer.allow_reuse_address = True
             self.server = ThreadingTCPServer(address, handlerFactory(self.incoming_connection))
 
             thread = threading.Thread(target=self.server.serve_forever)
             thread.daemon = True
             thread.start()
 
             self.announce_rate_target  = None
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/PipeInterface.py` & `rnspure-0.5.1/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/RNodeInterface.py` & `rnspure-0.5.1/RNS/Interfaces/RNodeInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
                             self.platform = byte
                         elif (command == KISS.CMD_MCU):
                             self.mcu = byte
                         elif (command == KISS.CMD_ERROR):
                             if (byte == KISS.ERROR_INITRADIO):
                                 RNS.log(str(self)+" hardware initialisation error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Radio initialisation failure")
-                            elif (byte == KISS.ERROR_INITRADIO):
+                            elif (byte == KISS.ERROR_TXFAILED):
                                 RNS.log(str(self)+" hardware TX error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Hardware transmit failure")
                             else:
                                 RNS.log(str(self)+" hardware error (code "+RNS.hexrep(byte)+")", RNS.LOG_ERROR)
                                 raise IOError("Unknown hardware failure")
                         elif (command == KISS.CMD_RESET):
                             if (byte == 0xF8):
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/SerialInterface.py` & `rnspure-0.5.1/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Interfaces/TCPInterface.py` & `rnspure-0.5.1/RNS/Interfaces/TCPInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,33 +404,23 @@
 
 
 class TCPServerInterface(Interface):
     BITRATE_GUESS      = 10*1000*1000
 
     @staticmethod
     def get_address_for_if(name):
-        import importlib
-        if importlib.util.find_spec('netifaces') != None:
-            import netifaces
-            return netifaces.ifaddresses(name)[netifaces.AF_INET][0]['addr']
-        else:
-            RNS.log("Getting interface addresses from device names requires the netifaces module.", RNS.LOG_CRITICAL)
-            RNS.log("You can install it with the command: python3 -m pip install netifaces", RNS.LOG_CRITICAL)
-            RNS.panic()
+        import RNS.vendor.ifaddr.niwrapper as netinfo
+        ifaddr = netinfo.ifaddresses(name)
+        return ifaddr[netinfo.AF_INET][0]["addr"]
 
     @staticmethod
     def get_broadcast_for_if(name):
-        import importlib
-        if importlib.util.find_spec('netifaces') != None:
-            import netifaces
-            return netifaces.ifaddresses(name)[netifaces.AF_INET][0]['broadcast']
-        else:
-            RNS.log("Getting interface addresses from device names requires the netifaces module.", RNS.LOG_CRITICAL)
-            RNS.log("You can install it with the command: python3 -m pip install netifaces", RNS.LOG_CRITICAL)
-            RNS.panic()
+        import RNS.vendor.ifaddr.niwrapper as netinfo
+        ifaddr = netinfo.ifaddresses(name)
+        return ifaddr[netinfo.AF_INET][0]["broadcast"]
 
     def __init__(self, owner, name, device=None, bindip=None, bindport=None, i2p_tunneled=False):
         self.rxb = 0
         self.txb = 0
 
         self.HW_MTU = 1064
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/UDPInterface.py` & `rnspure-0.5.1/RNS/Interfaces/UDPInterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,33 +30,23 @@
 
 
 class UDPInterface(Interface):
     BITRATE_GUESS = 10*1000*1000
 
     @staticmethod
     def get_address_for_if(name):
-        import importlib
-        if importlib.util.find_spec('netifaces') != None:
-            import netifaces
-            return netifaces.ifaddresses(name)[netifaces.AF_INET][0]['addr']
-        else:
-            RNS.log("Getting interface addresses from device names requires the netifaces module.", RNS.LOG_CRITICAL)
-            RNS.log("You can install it with the command: python3 -m pip install netifaces", RNS.LOG_CRITICAL)
-            RNS.panic()
+        import RNS.vendor.ifaddr.niwrapper as netinfo
+        ifaddr = netinfo.ifaddresses(name)
+        return ifaddr[netinfo.AF_INET][0]["addr"]
 
     @staticmethod
     def get_broadcast_for_if(name):
-        import importlib
-        if importlib.util.find_spec('netifaces') != None:
-            import netifaces
-            return netifaces.ifaddresses(name)[netifaces.AF_INET][0]['broadcast']
-        else:
-            RNS.log("Getting interface addresses from device names requires the netifaces module.", RNS.LOG_CRITICAL)
-            RNS.log("You can install it with the command: python3 -m pip install netifaces", RNS.LOG_CRITICAL)
-            RNS.panic()
+        import RNS.vendor.ifaddr.niwrapper as netinfo
+        ifaddr = netinfo.ifaddresses(name)
+        return ifaddr[netinfo.AF_INET][0]["broadcast"]
 
     def __init__(self, owner, name, device=None, bindip=None, bindport=None, forwardip=None, forwardport=None):
         self.rxb = 0
         self.txb = 0
 
         self.HW_MTU = 1064
```

### Comparing `rnspure-0.5.0/RNS/Interfaces/__init__.py` & `rnspure-0.5.1/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Link.py` & `rnspure-0.5.1/RNS/Link.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Packet.py` & `rnspure-0.5.1/RNS/Packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         self.attached_interface = attached_interface
         self.receiving_interface = None
         self.rssi = None
         self.snr = None
 
     def get_packed_flags(self):
         if self.context == Packet.LRPROOF:
-            packed_flags = (self.header_type << 6) | (self.transport_type << 4) | RNS.Destination.LINK | self.packet_type
+            packed_flags = (self.header_type << 6) | (self.transport_type << 4) | (RNS.Destination.LINK << 2) | self.packet_type
         else:
             packed_flags = (self.header_type << 6) | (self.transport_type << 4) | (self.destination.type << 2) | self.packet_type
         return packed_flags
 
     def pack(self):
         self.destination_hash = self.destination.hash
         self.header = b""
```

### Comparing `rnspure-0.5.0/RNS/Resource.py` & `rnspure-0.5.1/RNS/Resource.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Reticulum.py` & `rnspure-0.5.1/RNS/Reticulum.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     @staticmethod
     def sigterm_handler(signal, frame):
         RNS.Transport.detach_interfaces()
         RNS.exit()
 
 
-    def __init__(self,configdir=None, loglevel=None, logdest=None):
+    def __init__(self,configdir=None, loglevel=None, logdest=None, verbosity=None):
         """
         Initialises and starts a Reticulum instance. This must be
         done before any other operations, and Reticulum will not
         pass any traffic before being instantiated.
 
         :param configdir: Full path to a Reticulum configuration directory.
         """
@@ -207,14 +207,15 @@
         self.local_control_port   = 37429
         self.share_instance       = True
         self.rpc_listener         = None
 
         self.ifac_salt = Reticulum.IFAC_SALT
 
         self.requested_loglevel = loglevel
+        self.requested_verbosity = verbosity
         if self.requested_loglevel != None:
             if self.requested_loglevel > RNS.LOG_EXTREME:
                 self.requested_loglevel = RNS.LOG_EXTREME
             if self.requested_loglevel < RNS.LOG_CRITICAL:
                 self.requested_loglevel = RNS.LOG_CRITICAL
 
             RNS.loglevel = self.requested_loglevel
@@ -333,14 +334,16 @@
 
     def __apply_config(self):
         if "logging" in self.config:
             for option in self.config["logging"]:
                 value = self.config["logging"][option]
                 if option == "loglevel" and self.requested_loglevel == None:
                     RNS.loglevel = int(value)
+                    if self.requested_verbosity != None:
+                        RNS.loglevel += self.requested_verbosity
                     if RNS.loglevel < 0:
                         RNS.loglevel = 0
                     if RNS.loglevel > 7:
                         RNS.loglevel = 7
 
         if "reticulum" in self.config:
             for option in self.config["reticulum"]:
```

### Comparing `rnspure-0.5.0/RNS/Transport.py` & `rnspure-0.5.1/RNS/Transport.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/__init__.py` & `rnspure-0.5.1/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rncp.py` & `rnspure-0.5.1/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rnid.py` & `rnspure-0.5.1/RNS/Utilities/rnid.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rnodeconf.py` & `rnspure-0.5.1/RNS/Utilities/rnodeconf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from time import sleep
 import argparse
 import threading
+import sys
 import os
 import os.path
 import struct
 import datetime
 import time
 import math
 import hashlib
+import zipfile
 from urllib.request import urlretrieve
 from importlib import util
 import RNS
 
 RNS.logtimefmt      = "%H:%M:%S"
 RNS.compact_log_fmt = True
 
-program_version = "2.1.1"
+program_version = "2.1.2"
 eth_addr = "0x81F7B979fEa6134bA9FD5c701b3501A2e61E897a"
 btc_addr = "3CPmacGm34qYvR6XWLVEJmi2aNe3PZqUuq"
 xmr_addr = "87HcDx6jRSkMQ9nPRd5K9hGGpZLn2s7vWETjMaVM5KfV4TD36NcYa8J8WSxhTSvBzzFpqDwp2fg5GX2moZ7VAP9QMZCZGET"
 
 rnode = None
 rnode_serial = None
 rnode_port = None
@@ -73,14 +75,15 @@
     CMD_READY       = 0x0F
     CMD_STAT_RX     = 0x21
     CMD_STAT_TX     = 0x22
     CMD_STAT_RSSI   = 0x23
     CMD_STAT_SNR    = 0x24
     CMD_BLINK       = 0x30
     CMD_RANDOM      = 0x40
+    CMD_DISP_INT    = 0x45
     CMD_BT_CTRL     = 0x46
     CMD_BT_PIN      = 0x62
     CMD_BOARD       = 0x47
     CMD_PLATFORM    = 0x48
     CMD_MCU         = 0x49
     CMD_FW_VERSION  = 0x50
     CMD_ROM_READ    = 0x51
@@ -125,14 +128,18 @@
     MODEL_A4       = 0xA4
     MODEL_A9       = 0xA9
     MODEL_A3       = 0xA3
     MODEL_A8       = 0xA8
     MODEL_A2       = 0xA2
     MODEL_A7       = 0xA7
 
+    PRODUCT_T32_10 = 0xB2
+    MODEL_BA       = 0xBA
+    MODEL_BB       = 0xBB
+
     PRODUCT_T32_20 = 0xB0
     MODEL_B3       = 0xB3
     MODEL_B8       = 0xB8
 
     PRODUCT_T32_21 = 0xB1
     MODEL_B4       = 0xB4
     MODEL_B9       = 0xB9
@@ -176,14 +183,15 @@
     BOARD_LORA32_V2_1   = 0x37
 
 mapped_product = ROM.PRODUCT_RNODE
 products = {
     ROM.PRODUCT_RNODE:  "RNode",
     ROM.PRODUCT_HMBRW:  "Hombrew RNode",
     ROM.PRODUCT_TBEAM:  "LilyGO T-Beam",
+    ROM.PRODUCT_T32_10: "LilyGO LoRa32 v1.0",
     ROM.PRODUCT_T32_20: "LilyGO LoRa32 v2.0",
     ROM.PRODUCT_T32_21: "LilyGO LoRa32 v2.1",
     ROM.PRODUCT_H32_V2: "Heltec LoRa32 v2",
 }
 
 platforms = {
     ROM.PLATFORM_AVR: "AVR",
@@ -203,14 +211,16 @@
     0xA7: [820000000, 1020000000, 17, "820 - 1020 MHz", "rnode_firmware_ng21.zip"],
     0xA3: [410000000, 525000000, 17, "410 - 525 MHz", "rnode_firmware_ng20.zip"],
     0xA8: [820000000, 1020000000, 17, "820 - 1020 MHz", "rnode_firmware_ng20.zip"],
     0xB3: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_lora32v20.zip"],
     0xB8: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v20.zip"],
     0xB4: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_lora32v21.zip"],
     0xB9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v21.zip"],
+    0xBA: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_lora32v10.zip"],
+    0xBB: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v10.zip"],
     0xC4: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_heltec32v2.zip"],
     0xC9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_heltec32v2.zip"],
     0xE4: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_tbeam.zip"],
     0xE9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_tbeam.zip"],
     0xFE: [100000000, 1100000000, 17, "(Band capabilities unknown)", None],
     0xFF: [100000000, 1100000000, 14, "(Band capabilities unknown)", None],
 }
@@ -552,14 +562,21 @@
 
     def leave(self):
         kiss_command = bytes([KISS.FEND, KISS.CMD_LEAVE, 0xFF, KISS.FEND])
         written = self.serial.write(kiss_command)
         if written != len(kiss_command):
             raise IOError("An IO error occurred while sending host left command to device")
 
+    def set_display_intensity(self, intensity):
+        data = bytes([intensity & 0xFF])
+        kiss_command = bytes([KISS.FEND])+bytes([KISS.CMD_DISP_INT])+data+bytes([KISS.FEND])
+        written = self.serial.write(kiss_command)
+        if written != len(kiss_command):
+            raise IOError("An IO error occurred while sending bluetooth enable command to device")
+
     def enable_bluetooth(self):
         kiss_command = bytes([KISS.FEND, KISS.CMD_BT_CTRL, 0x01, KISS.FEND])
         written = self.serial.write(kiss_command)
         if written != len(kiss_command):
             raise IOError("An IO error occurred while sending bluetooth enable command to device")
 
     def disable_bluetooth(self):
@@ -1086,14 +1103,16 @@
         parser.add_argument("-N", "--normal", action="store_true", help="Switch device to normal mode")
         parser.add_argument("-T", "--tnc", action="store_true", help="Switch device to TNC mode")
 
         parser.add_argument("-b", "--bluetooth-on", action="store_true", help="Turn device bluetooth on")
         parser.add_argument("-B", "--bluetooth-off", action="store_true", help="Turn device bluetooth off")
         parser.add_argument("-p", "--bluetooth-pair", action="store_true", help="Put device into bluetooth pairing mode")
 
+        parser.add_argument("-D", "--display", action="store", metavar="i", type=int, default=None, help="Set display intensity (0-255)")
+
         parser.add_argument("--freq", action="store", metavar="Hz", type=int, default=None, help="Frequency in Hz for TNC mode")
         parser.add_argument("--bw", action="store", metavar="Hz", type=int, default=None, help="Bandwidth in Hz for TNC mode")
         parser.add_argument("--txp", action="store", metavar="dBm", type=int, default=None, help="TX power in dBm for TNC mode")
         parser.add_argument("--sf", action="store", metavar="factor", type=int, default=None, help="Spreading factor for TNC mode (7 - 12)")
         parser.add_argument("--cr", action="store", metavar="rate", type=int, default=None, help="Coding rate for TNC mode (5 - 8)")
 
         parser.add_argument("--eeprom-backup", action="store_true", help="Backup EEPROM to file")
@@ -1245,15 +1264,24 @@
 
             if rnode.detected:
                 RNS.log("Trying to read EEPROM...")
                 rnode.download_eeprom()
             else:
                 RNS.log("Could not detect a connected RNode")
 
-            if rnode.provisioned and rnode.signature_valid:
+            if rnode.provisioned:
+                if not rnode.signature_valid:
+                    print("\nThe device signature in this RNode is unknown and cannot be verified. It is still")
+                    print("possible to extract the firmware from it, but you should make absolutely sure that")
+                    print("it comes from a trusted source. It is possible that someone could have modified the")
+                    print("firmware. If that is the case, these modifications will propagate to any new RNodes")
+                    print("descendent from this one!")
+                    print("\nHit enter if you are sure you want to continue.")
+                    input()
+
                 if rnode.firmware_hash != None:
                     extracted_hash = rnode.firmware_hash
                     extracted_version = rnode.version
                     rnode.disconnect()
                     v_str = str(extracted_version)+" "+RNS.hexrep(extracted_hash, delimit=False)
                     print("\nFound RNode Firmvare v"+v_str)
 
@@ -1263,19 +1291,19 @@
                     extract_recovery_esptool()
 
                     hash_f = open(EXT_DIR+"/extracted_rnode_firmware.version", "wb")
                     hash_f.write(v_str.encode("utf-8"))
                     hash_f.close()
 
                     extraction_parts = [
-                        ("bootloader", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port /dev/ttyACM1 --baud 921600 --before default_reset --after hard_reset read_flash 0x1000 0x4650 \""+EXT_DIR+"/extracted_rnode_firmware.bootloader\""),
-                        ("partition table", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port /dev/ttyACM1 --baud 921600 --before default_reset --after hard_reset read_flash 0x8000 0xC00 \""+EXT_DIR+"/extracted_rnode_firmware.partitions\""),
-                        ("app boot", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port /dev/ttyACM1 --baud 921600 --before default_reset --after hard_reset read_flash 0xe000 0x2000 \""+EXT_DIR+"/extracted_rnode_firmware.boot_app0\""),
-                        ("application image", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port /dev/ttyACM1 --baud 921600 --before default_reset --after hard_reset read_flash 0x10000 0x200000 \""+EXT_DIR+"/extracted_rnode_firmware.bin\""),
-                        ("console image", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port /dev/ttyACM1 --baud 921600 --before default_reset --after hard_reset read_flash 0x210000 0x1F0000 \""+EXT_DIR+"/extracted_console_image.bin\""),
+                        ("bootloader", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port "+port_path+" --baud 921600 --before default_reset --after hard_reset read_flash 0x1000 0x4650 \""+EXT_DIR+"/extracted_rnode_firmware.bootloader\""),
+                        ("partition table", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port "+port_path+" --baud 921600 --before default_reset --after hard_reset read_flash 0x8000 0xC00 \""+EXT_DIR+"/extracted_rnode_firmware.partitions\""),
+                        ("app boot", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port "+port_path+" --baud 921600 --before default_reset --after hard_reset read_flash 0xe000 0x2000 \""+EXT_DIR+"/extracted_rnode_firmware.boot_app0\""),
+                        ("application image", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port "+port_path+" --baud 921600 --before default_reset --after hard_reset read_flash 0x10000 0x200000 \""+EXT_DIR+"/extracted_rnode_firmware.bin\""),
+                        ("console image", "python \""+CNF_DIR+"/recovery_esptool.py\" --chip esp32 --port "+port_path+" --baud 921600 --before default_reset --after hard_reset read_flash 0x210000 0x1F0000 \""+EXT_DIR+"/extracted_console_image.bin\""),
                     ]
                     import subprocess, shlex
                     for part, command in extraction_parts:
                         print("Extracting "+part+"...")
                         if subprocess.call(shlex.split(command), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) != 0:
                             print("The extraction failed, the following command did not complete successfully:\n"+command)
                             exit(182)
@@ -1396,16 +1424,17 @@
             print("[2] Homebrew RNode")
             print("       .")
             print("      / \\   Select this option if you have put toghether an RNode")
             print("       |    of your own design, or if you are prototyping one.")
             print("")
             print("[3] LilyGO LoRa32 v2.1 (aka T3 v1.6 / T3 v1.6.1)")
             print("[4] LilyGO LoRa32 v2.0")
-            print("[5] LilyGO T-Beam")
-            print("[6] Heltec LoRa32 v2")
+            print("[5] LilyGO LoRa32 v1.0")
+            print("[6] LilyGO T-Beam")
+            print("[7] Heltec LoRa32 v2")
             print("       .")
             print("      / \\   Select one of these options if you want to easily turn")
             print("       |    a supported development board into an RNode.")
             print("")
             print("---------------------------------------------------------------------------")
             print("\nEnter the number that matches your device type:\n? ", end="")
 
@@ -1429,15 +1458,15 @@
                     print("")
                     print("Important! Using RNode firmware on homebrew devices should currently be")
                     print("considered experimental. It is not intended for production or critical use.")
                     print("The currently supplied firmware is provided AS-IS as a courtesey to those")
                     print("who would like to experiment with it. Hit enter to continue.")
                     print("---------------------------------------------------------------------------")
                     input()
-                elif c_dev == 5:
+                elif c_dev == 6:
                     selected_product = ROM.PRODUCT_TBEAM
                     clear()
                     print("")
                     print("---------------------------------------------------------------------------")
                     print("                          T-Beam RNode Installer")
                     print("")
                     print("The RNode firmware can currently be installed on T-Beam devices using the")
@@ -1459,28 +1488,47 @@
                     print("")
                     print("Important! Using RNode firmware on LoRa32 devices should currently be")
                     print("considered experimental. It is not intended for production or critical use.")
                     print("The currently supplied firmware is provided AS-IS as a courtesey to those")
                     print("who would like to experiment with it. Hit enter to continue.")
                     print("---------------------------------------------------------------------------")
                     input()
+                elif c_dev == 5:
+                    selected_product = ROM.PRODUCT_T32_10
+                    clear()
+                    print("")
+                    print("---------------------------------------------------------------------------")
+                    print("                     LilyGO LoRa32 v1.0 RNode Installer")
+                    print("")
+                    print("Important! Using RNode firmware on LoRa32 devices should currently be")
+                    print("considered experimental. It is not intended for production or critical use.")
+                    print("The currently supplied firmware is provided AS-IS as a courtesey to those")
+                    print("who would like to experiment with it.")
+                    print("")
+                    print("Please Note! This device is known to have a faulty battery charging circuit,")
+                    print("which can result in overcharging and damaging batteries. If at all possible,")
+                    print("it is recommended to avoid this device.")
+                    print("")
+                    print("Hit enter if you're sure you wish to continue.")
+                    print("---------------------------------------------------------------------------")
+                    input()
                 elif c_dev == 3:
                     selected_product = ROM.PRODUCT_T32_21
                     clear()
                     print("")
                     print("---------------------------------------------------------------------------")
                     print("                     LilyGO LoRa32 v2.1 RNode Installer")
                     print("")
                     print("Important! Using RNode firmware on LoRa32 devices should currently be")
                     print("considered experimental. It is not intended for production or critical use.")
                     print("The currently supplied firmware is provided AS-IS as a courtesey to those")
                     print("who would like to experiment with it. Hit enter to continue.")
                     print("---------------------------------------------------------------------------")
                     input()
-                elif c_dev == 6:
+                elif c_dev == 7:
                     selected_product = ROM.PRODUCT_H32_V2
                     clear()
                     print("")
                     print("---------------------------------------------------------------------------")
                     print("                     Heltec LoRa32 v2.0 RNode Installer")
                     print("")
                     print("Important! Using RNode firmware on Heltec devices should currently be")
@@ -1604,14 +1652,36 @@
                     elif c_model > 1:
                         selected_model = ROM.MODEL_E9
                         selected_platform = ROM.PLATFORM_ESP32
                 except Exception as e:
                     print("That band does not exist, exiting now.")
                     exit()
 
+            elif selected_product == ROM.PRODUCT_T32_10:
+                selected_mcu = ROM.MCU_ESP32
+                print("\nWhat band is this LoRa32 for?\n")
+                print("[1] 433 MHz")
+                print("[2] 868 MHz")
+                print("[3] 915 MHz")
+                print("[4] 923 MHz")
+                print("\n? ", end="")
+                try:
+                    c_model = int(input())
+                    if c_model < 1 or c_model > 4:
+                        raise ValueError()
+                    elif c_model == 1:
+                        selected_model = ROM.MODEL_BA
+                        selected_platform = ROM.PLATFORM_ESP32
+                    elif c_model > 1:
+                        selected_model = ROM.MODEL_BB
+                        selected_platform = ROM.PLATFORM_ESP32
+                except Exception as e:
+                    print("That band does not exist, exiting now.")
+                    exit()
+
             elif selected_product == ROM.PRODUCT_T32_20:
                 selected_mcu = ROM.MCU_ESP32
                 print("\nWhat band is this LoRa32 for?\n")
                 print("[1] 433 MHz")
                 print("[2] 868 MHz")
                 print("[3] 915 MHz")
                 print("[4] 923 MHz")
@@ -1925,15 +1995,15 @@
                     import stat
                     os.chmod(flasher, stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP)
 
                 if which(flasher) is not None:
                     if fw_filename == "rnode_firmware_tbeam.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -1943,33 +2013,69 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
                                 "--flash_freq", "80m",
                                 "--flash_size", "4MB",
                                 "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.boot_app0",
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_tbeam.partitions",
                             ]
+                    elif fw_filename == "rnode_firmware_lora32v10.zip":
+                        if numeric_version >= 1.59:
+                            return [
+                                sys.executable, flasher,
+                                "--chip", "esp32",
+                                "--port", args.port,
+                                "--baud", "921600",
+                                "--before", "default_reset",
+                                "--after", "hard_reset",
+                                "write_flash", "-z",
+                                "--flash_mode", "dio",
+                                "--flash_freq", "80m",
+                                "--flash_size", "4MB",
+                                "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v10.boot_app0",
+                                "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v10.bootloader",
+                                "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v10.bin",
+                                "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
+                                "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v10.partitions",
+                            ]
+                        else:
+                            return [
+                                sys.executable, flasher,
+                                "--chip", "esp32",
+                                "--port", args.port,
+                                "--baud", "921600",
+                                "--before", "default_reset",
+                                "--after", "hard_reset",
+                                "write_flash", "-z",
+                                "--flash_mode", "dio",
+                                "--flash_freq", "80m",
+                                "--flash_size", "4MB",
+                                "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.boot_app0",
+                                "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bootloader",
+                                "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bin",
+                                "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.partitions",
+                            ]
                     elif fw_filename == "rnode_firmware_lora32v20.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -1979,15 +2085,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -1997,15 +2103,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v20.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_lora32v21.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2015,15 +2121,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2033,15 +2139,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_lora32v21.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_heltec32v2.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2051,15 +2157,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2069,15 +2175,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_featheresp32.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                               sys.executable,  flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2087,15 +2193,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2105,15 +2211,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_featheresp32.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_esp32_generic.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2123,15 +2229,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2141,15 +2247,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_esp32_generic.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_ng20.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2159,15 +2265,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2177,15 +2283,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng20.partitions",
                             ]
                     elif fw_filename == "rnode_firmware_ng21.zip":
                         if numeric_version >= 1.55:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2195,15 +2301,15 @@
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.bin",
                                 "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.partitions",
                             ]
                         else:
                             return [
-                                flasher,
+                                sys.executable, flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", "921600",
                                 "--before", "default_reset",
                                 "--after", "hard_reset",
                                 "write_flash", "-z",
                                 "--flash_mode", "dio",
@@ -2212,15 +2318,15 @@
                                 "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.boot_app0",
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_ng21.partitions",
                             ]
                     elif fw_filename == "extracted_rnode_firmware.zip":
                         return [
-                            flasher,
+                            sys.executable, flasher,
                             "--chip", "esp32",
                             "--port", args.port,
                             "--baud", "921600",
                             "--before", "default_reset",
                             "--after", "hard_reset",
                             "write_flash", "-z",
                             "--flash_mode", "dio",
@@ -2283,20 +2389,21 @@
                 
                 else:
                     fw_src = UPD_DIR+"/"+selected_version+"/"
                     if os.path.isfile(fw_src+fw_filename):
                         try:
                             if fw_filename.endswith(".zip"):
                                 RNS.log("Decompressing firmware...")
-                                unzip_status = call(get_flasher_call("unzip", fw_filename))
-                                if unzip_status == 0:
-                                    RNS.log("Firmware decompressed")
-                                else:
-                                    RNS.log("Could not extract firmware from downloaded zip file")
+                                try:
+                                    with zipfile.ZipFile(fw_src+fw_filename) as zip:
+                                        zip.extractall(fw_src)
+                                except Exception as e:
+                                    RNS.log("Could not decompress firmware from downloaded zip file")
                                     exit()
+                                RNS.log("Firmware decompressed")
 
                             RNS.log("Flashing RNode firmware to device on "+args.port)
                             from subprocess import call
                             rc = get_flasher_call(args.platform, fw_filename)
                             flash_status = call(rc)
                             if flash_status == 0:
                                 RNS.log("Done flashing")
@@ -2410,21 +2517,23 @@
                                 RNS.log("Override with -U option to install anyway")
                                 exit(0)
 
                     if not fw_file_ensured and selected_version != None:
                         ensure_firmware_file(fw_filename)
 
                     if fw_filename.endswith(".zip") and not fw_filename == "extracted_rnode_firmware.zip":
-                        RNS.log("Extracting firmware...")
-                        unzip_status = call(get_flasher_call("unzip", fw_filename))
-                        if unzip_status == 0:
-                            RNS.log("Firmware extracted")
-                        else:
-                            RNS.log("Could not extract firmware from downloaded zip file")
+                        RNS.log("Decompressing firmware...")
+                        fw_src = UPD_DIR+"/"+selected_version+"/"
+                        try:
+                            with zipfile.ZipFile(fw_src+fw_filename) as zip:
+                                zip.extractall(fw_src)
+                        except Exception as e:
+                            RNS.log("Could not decompress firmware from downloaded zip file")
                             exit()
+                        RNS.log("Firmware decompressed")
 
                 except Exception as e:
                     RNS.log("Could not obtain firmware package for your board")
                     RNS.log("The contained exception was: "+str(e))
                     exit()
 
                 if fw_filename == "extracted_rnode_firmware.zip":
@@ -2517,14 +2626,23 @@
                     file.close()
                     RNS.log("EEPROM backup written to: "+path)
                 except Exception as e:
                     RNS.log("EEPROM was successfully downloaded from device,")
                     RNS.log("but file could not be written to disk.")
                 exit()
 
+            if isinstance(args.display, int):
+                di = args.display
+                if di < 0:
+                    di = 0
+                if di > 255:
+                    di = 255
+                RNS.log("Setting display intensity to "+str(di))
+                rnode.set_display_intensity(di)
+
             if args.bluetooth_on:
                 RNS.log("Enabling Bluetooth...")
                 rnode.enable_bluetooth()
                 rnode.leave()
 
             if args.bluetooth_off:
                 RNS.log("Disabling Bluetooth...")
```

### Comparing `rnspure-0.5.0/RNS/Utilities/rnpath.py` & `rnspure-0.5.1/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rnprobe.py` & `rnspure-0.5.1/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rnsd.py` & `rnspure-0.5.1/RNS/Utilities/rnsd.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 import argparse
 import time
 
 from RNS._version import __version__
 
 
 def program_setup(configdir, verbosity = 0, quietness = 0, service = False):
-    targetloglevel = 3+verbosity-quietness
+    targetverbosity = verbosity-quietness
 
     if service:
         targetlogdest  = RNS.LOG_FILE
-        targetloglevel = None
+        targetverbosity = None
     else:
         targetlogdest  = RNS.LOG_STDOUT
 
-    reticulum = RNS.Reticulum(configdir=configdir, loglevel=targetloglevel, logdest=targetlogdest)
+    reticulum = RNS.Reticulum(configdir=configdir, verbosity=targetverbosity, logdest=targetlogdest)
     if reticulum.is_connected_to_shared_instance:
         RNS.log("Started rnsd version {version} connected to another shared local instance, this is probably NOT what you want!".format(version=__version__), RNS.LOG_WARNING)
     else:
         RNS.log("Started rnsd version {version}".format(version=__version__), RNS.LOG_NOTICE)
 
     while True:
         time.sleep(1)
```

### Comparing `rnspure-0.5.0/RNS/Utilities/rnstatus.py` & `rnspure-0.5.1/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/Utilities/rnx.py` & `rnspure-0.5.1/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/__init__.py` & `rnspure-0.5.1/RNS/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/configobj.py` & `rnspure-0.5.1/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/__init__.py` & `rnspure-0.5.1/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/aiosam.py` & `rnspure-0.5.1/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/exceptions.py` & `rnspure-0.5.1/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/sam.py` & `rnspure-0.5.1/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/tunnel.py` & `rnspure-0.5.1/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/i2plib/utils.py` & `rnspure-0.5.1/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/platformutils.py` & `rnspure-0.5.1/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/six.py` & `rnspure-0.5.1/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/RNS/vendor/umsgpack.py` & `rnspure-0.5.1/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.0/rnspure.egg-info/PKG-INFO` & `rnspure-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-Metadata-Version: 2.1
-Name: rnspure
-Version: 0.5.0
-Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
-Home-page: https://reticulum.network/
-Author: Mark Qvist
-Author-email: mark@unsigned.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Reticulum Network Stack β <img align="right" src="https://static.pepy.tech/personalized-badge/rns?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs"/>
 ==========
 
 <p align="center"><img width="200" src="https://raw.githubusercontent.com/markqvist/Reticulum/master/docs/source/graphics/rns_logo_512.png"></p>
 
-**Warning!** *This package is the zero-dependency version of Reticulum. You should almost certainly use the [normal package](https://pypi.org/project/rns) instead. Do NOT install this package unless you know exactly why you are doing it!*
-
 Reticulum is the cryptography-based networking stack for building local and wide-area
 networks with readily available hardware. It can operate even with very high latency
 and extremely low bandwidth. Reticulum allows you to build wide-area networks
 with off-the-shelf tools, and offers end-to-end encryption and connectivity,
 initiator anonymity, autoconfiguring cryptographically backed multi-hop
 transport, efficient addressing, unforgeable delivery acknowledgements and
 more.
@@ -202,15 +186,14 @@
 ## Dependencies
 The installation of the default `rns` package requires the dependencies listed
 below. Almost all systems and distributions have readily available packages for
 these dependencies, and when the `rns` package is installed with `pip`, they
 will be downloaded and installed as well.
 
 - [PyCA/cryptography](https://github.com/pyca/cryptography)
-- [netifaces](https://github.com/al45tair/netifaces)
 - [pyserial](https://github.com/pyserial/pyserial)
 
 On more unusual systems, and in some rare cases, it might not be possible to
 install or even compile one or more of the above modules. In such situations,
 you can use the `rnspure` package instead, which require no external
 dependencies for installation. Please note that the contents of the `rns` and
 `rnspure` packages are *identical*. The only difference is that the `rnspure`
@@ -240,39 +223,33 @@
 before it is publicly released). Sometimes experimental versions of Reticulum
 might be deployed to nodes on the testnet, which means strange behaviour might
 occur. If none of that scares you, you can join the testnet via either TCP or
 I2P. Just add one of the following interfaces to your Reticulum configuration
 file:
 
 ```
-# TCP/IP interface to the Dublin Hub
+# TCP/IP interface to the RNS Dublin Hub
   [[RNS Testnet Dublin]]
     type = TCPClientInterface
     enabled = yes
     target_host = dublin.connect.reticulum.network
     target_port = 4965
 
-# TCP/IP interface to the Frankfurt Hub
-  [[RNS Testnet Frankfurt]]
+# TCP/IP interface to the BetweenTheBorders Hub (community-provided)
+  [[RNS Testnet BetweenTheBorders]]
     type = TCPClientInterface
     enabled = yes
-    target_host = frankfurt.connect.reticulum.network
-    target_port = 5377
+    target_host = betweentheborders.com
+    target_port = 4242
 
-# Interface to I2P Hub A
-  [[RNS Testnet I2P Hub A]]
+# Interface to Testnet I2P Hub
+  [[RNS Testnet I2P Hub]]
     type = I2PInterface
     enabled = yes
     peers = pmlm3l5rpympihoy2o5ago43kluei2jjjzsalcuiuylbve3mwi2a.b32.i2p
-
-# Interface to I2P Hub B
-  [[RNS Testnet I2P Hub B]]
-    type = I2PInterface
-    enabled = yes
-    peers = iwoqtz22dsr73aemwpw7guocplsjjoamyl7sogj33qtcd6ds4mza.b32.i2p
 ```
 
 The testnet also contains a number of [Nomad Network](https://github.com/markqvist/nomadnet) nodes, and LXMF propagation nodes.
 
 ## Support Reticulum
 You can help support the continued development of open, free and private communications systems by donating via one of the following channels:
 
@@ -353,12 +330,12 @@
 - [PyCA/cryptography](https://github.com/pyca/cryptography), *BSD License*
 - [Pure-25519](https://github.com/warner/python-pure25519) by [Brian Warner](https://github.com/warner), *MIT License*
 - [Pysha2](https://github.com/thomdixon/pysha2) by [Thom Dixon](https://github.com/thomdixon), *MIT License*
 - [Python-AES](https://github.com/orgurar/python-aes) by [Or Gur Arie](https://github.com/orgurar), *MIT License*
 - [Curve25519.py](https://gist.github.com/nickovs/cc3c22d15f239a2640c185035c06f8a3#file-curve25519-py) by [Nicko van Someren](https://gist.github.com/nickovs), *Public Domain*
 - [I2Plib](https://github.com/l-n-s/i2plib) by [Viktor Villainov](https://github.com/l-n-s)
 - [PySerial](https://github.com/pyserial/pyserial) by Chris Liechti, *BSD License*
-- [Netifaces](https://github.com/al45tair/netifaces) by [Alastair Houghton](https://github.com/al45tair), *MIT License*
 - [Configobj](https://github.com/DiffSK/configobj) by Michael Foord, Nicola Larosa, Rob Dennis & Eli Courtwright, *BSD License*
 - [Six](https://github.com/benjaminp/six) by [Benjamin Peterson](https://github.com/benjaminp), *MIT License*
+- [ifaddr](https://github.com/pydron/ifaddr) by [Pydron](https://github.com/pydron), *MIT License*
 - [Umsgpack.py](https://github.com/vsergeev/u-msgpack-python) by [Ivan A. Sergeev](https://github.com/vsergeev)
 - [Python](https://www.python.org)
```

### Comparing `rnspure-0.5.0/rnspure.egg-info/SOURCES.txt` & `rnspure-0.5.1/rnspure.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -67,12 +67,17 @@
 RNS/vendor/i2plib/__version__.py
 RNS/vendor/i2plib/aiosam.py
 RNS/vendor/i2plib/exceptions.py
 RNS/vendor/i2plib/log.py
 RNS/vendor/i2plib/sam.py
 RNS/vendor/i2plib/tunnel.py
 RNS/vendor/i2plib/utils.py
+RNS/vendor/ifaddr/__init__.py
+RNS/vendor/ifaddr/_posix.py
+RNS/vendor/ifaddr/_shared.py
+RNS/vendor/ifaddr/_win32.py
+RNS/vendor/ifaddr/niwrapper.py
 rnspure.egg-info/PKG-INFO
 rnspure.egg-info/SOURCES.txt
 rnspure.egg-info/dependency_links.txt
 rnspure.egg-info/entry_points.txt
 rnspure.egg-info/top_level.txt
```

### Comparing `rnspure-0.5.0/setup.py` & `rnspure-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 if pure_python:
     pkg_name = "rnspure"
     requirements = []
     long_description = long_description.replace("</p>", "</p>"+pure_notice)
 else:
     pkg_name = "rns"
-    requirements = ['cryptography>=3.4.7', 'pyserial>=3.5', 'netifaces']
+    requirements = ['cryptography>=3.4.7', 'pyserial>=3.5']
 
 excluded_modules = exclude=["tests.*", "tests"]
 packages = setuptools.find_packages(exclude=excluded_modules)
 
 setuptools.setup(
     name=pkg_name,
     version=__version__,
@@ -49,9 +49,9 @@
             'rnid=RNS.Utilities.rnid:main',
             'rncp=RNS.Utilities.rncp:main',
             'rnx=RNS.Utilities.rnx:main',
             'rnodeconf=RNS.Utilities.rnodeconf:main',
         ]
     },
     install_requires=requirements,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

