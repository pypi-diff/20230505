# Comparing `tmp/onvif-zeep-async-2.0.0.tar.gz` & `tmp/onvif-zeep-async-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-2.0.0.tar", last modified: Thu May  4 15:11:53 2023, max compression
+gzip compressed data, was "onvif-zeep-async-2.1.0.tar", last modified: Thu May  4 20:49:08 2023, max compression
```

## Comparing `onvif-zeep-async-2.0.0.tar` & `onvif-zeep-async-2.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943804 onvif-zeep-async-2.0.0/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.0.0/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.0.0/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 15:11:53.943872 onvif-zeep-async-2.0.0/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.937467 onvif-zeep-async-2.0.0/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.938153 onvif-zeep-async-2.0.0/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    24532 2023-05-04 15:11:27.000000 onvif-zeep-async-2.0.0/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 15:11:34.000000 onvif-zeep-async-2.0.0/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.942818 onvif-zeep-async-2.0.0/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.0.0/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943583 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-04 15:11:53.944110 onvif-zeep-async-2.0.0/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943705 onvif-zeep-async-2.0.0/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.678523 onvif-zeep-async-2.1.0/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.0/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 20:49:08.678595 onvif-zeep-async-2.1.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.670458 onvif-zeep-async-2.1.0/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.671114 onvif-zeep-async-2.1.0/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    27861 2023-05-04 20:48:40.000000 onvif-zeep-async-2.1.0/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 20:48:45.000000 onvif-zeep-async-2.1.0/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.677520 onvif-zeep-async-2.1.0/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.0/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.678297 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 20:49:08.000000 onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-04 20:49:08.678833 onvif-zeep-async-2.1.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 20:49:08.678404 onvif-zeep-async-2.1.0/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.0/tests/test.py
```

### Comparing `onvif-zeep-async-2.0.0/.gitignore` & `onvif-zeep-async-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/.pre-commit-config.yaml` & `onvif-zeep-async-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/LICENSE` & `onvif-zeep-async-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/Makefile` & `onvif-zeep-async-2.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/PKG-INFO` & `onvif-zeep-async-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.0.0
+Version: 2.1.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.0.0/README.rst` & `onvif-zeep-async-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/examples/events.py` & `onvif-zeep-async-2.1.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/examples/rotate_image.py` & `onvif-zeep-async-2.1.0/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/examples/streaming.py` & `onvif-zeep-async-2.1.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/__init__.py` & `onvif-zeep-async-2.1.0/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/client.py` & `onvif-zeep-async-2.1.0/onvif/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import contextlib
 import datetime as dt
 from functools import lru_cache
 import logging
 import os.path
 import ssl
-from typing import Any, Callable, Dict, Optional, Tuple
+from typing import Any, Awaitable, Callable, Dict, Optional, ParamSpec, Tuple, TypeVar
 
 import httpx
 from httpx import AsyncClient, BasicAuth, DigestAuth, TransportError
 from zeep.cache import SqliteCache
 from zeep.client import AsyncClient as BaseZeepAsyncClient, Settings
 from zeep.exceptions import Fault, XMLSyntaxError
 import zeep.helpers
@@ -31,14 +31,78 @@
 
 _DEFAULT_SETTINGS = Settings()
 _DEFAULT_SETTINGS.strict = False
 _DEFAULT_SETTINGS.xml_huge_tree = True
 
 _WSDL_PATH = os.path.join(os.path.dirname(os.path.dirname(__file__)), "wsdl")
 
+_DEFAULT_TIMEOUT = 30
+_PULLPOINT_TIMEOUT = 90
+_CONNECT_TIMEOUT = 30
+_READ_TIMEOUT = 30
+_WRITE_TIMEOUT = 30
+
+
+KEEPALIVE_EXPIRY = 4
+BACKOFF_TIME = KEEPALIVE_EXPIRY + 0.5
+HTTPX_LIMITS = httpx.Limits(keepalive_expiry=4)
+
+
+DEFAULT_ATTEMPTS = 2
+
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
+def retry_connection_error(
+    attempts: int = DEFAULT_ATTEMPTS,
+) -> Callable[[Callable[P, Awaitable[T]]], Callable[P, Awaitable[T]]]:
+    """Define a wrapper to retry on connection error."""
+
+    def _decorator_retry_connection_error(
+        func: Callable[P, Awaitable[T]]
+    ) -> Callable[P, Awaitable[T]]:
+        """Define a wrapper to retry on connection error.
+
+        The remote server is allowed to disconnect us any time so
+        we need to retry the operation.
+        """
+
+        async def _async_wrap_connection_error_retry(  # type: ignore[return]
+            *args: P.args, **kwargs: P.kwargs
+        ) -> T:
+            for attempt in range(attempts):
+                try:
+                    return await func(*args, **kwargs)
+                except httpx.RequestError as ex:
+                    #
+                    # We should only need to retry on RemoteProtocolError but some cameras
+                    # are flakey and sometimes do not respond to the Renew request so we
+                    # retry on RequestError as well.
+                    #
+                    # For RemoteProtocolError:
+                    # http://datatracker.ietf.org/doc/html/rfc2616#section-8.1.4 allows the server
+                    # to close the connection at any time, we treat this as a normal and try again
+                    # once since we do not want to declare the camera as not supporting PullPoint
+                    # if it just happened to close the connection at the wrong time.
+                    if attempt == attempts - 1:
+                        raise
+                    logger.debug(
+                        "Error: %s while calling %s, backing off: %s, retrying...",
+                        ex,
+                        func,
+                        BACKOFF_TIME,
+                        exc_info=True,
+                    )
+                    await asyncio.sleep(BACKOFF_TIME)
+
+        return _async_wrap_connection_error_retry
+
+    return _decorator_retry_connection_error
+
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
     ssl verify turned off and old SSL versions enabled.
 
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
@@ -182,14 +246,16 @@
         passwd: Optional[str],
         url: str,
         encrypt=True,
         no_cache=False,
         dt_diff=None,
         binding_name="",
         binding_key="",
+        read_timeout: Optional[int] = None,
+        write_timeout: Optional[int] = None,
     ) -> None:
         if not _path_isfile(url):
             raise ONVIFError("%s doesn`t exist!" % url)
 
         self.url = url
         self.xaddr = xaddr
         self.binding_key = binding_key
@@ -197,19 +263,29 @@
         self.user = user
         self.passwd = passwd
         # Indicate wether password digest is needed
         self.encrypt = encrypt
         self.dt_diff = dt_diff
         self.binding_name = binding_name
         # Create soap client
-        client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
+        timeouts = httpx.Timeout(
+            _DEFAULT_TIMEOUT,
+            connect=_CONNECT_TIMEOUT,
+            read=read_timeout or _READ_TIMEOUT,
+            write=write_timeout or _WRITE_TIMEOUT,
+        )
+        client = AsyncClient(
+            verify=_NO_VERIFY_SSL_CONTEXT, timeout=timeouts, limits=HTTPX_LIMITS
+        )
         # The wsdl client should never actually be used, but it is required
         # to avoid creating another ssl context since the underlying code
         # will try to create a new one if it doesn't exist.
-        wsdl_client = httpx.Client(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
+        wsdl_client = httpx.Client(
+            verify=_NO_VERIFY_SSL_CONTEXT, timeout=timeouts, limits=HTTPX_LIMITS
+        )
         self.transport = (
             AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
                 client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
@@ -479,33 +555,35 @@
 
     def create_notification_manager(
         self, config: Optional[Dict[str, Any]] = None
     ) -> NotificationManager:
         """Create a notification manager."""
         return NotificationManager(self, config)
 
-    async def close(self):
+    async def close(self) -> None:
         """Close all transports."""
         await self._snapshot_client.aclose()
         for service in self.services.values():
             await service.close()
 
-    async def get_snapshot_uri(self, profile_token):
+    async def get_snapshot_uri(self, profile_token: str) -> str:
         """Get the snapshot uri for a given profile."""
         uri = self._snapshot_uris.get(profile_token)
         if uri is None:
             media_service = await self.create_media_service()
             req = media_service.create_type("GetSnapshotUri")
             req.ProfileToken = profile_token
             result = await media_service.GetSnapshotUri(req)
             uri = result.Uri
             self._snapshot_uris[profile_token] = uri
         return uri
 
-    async def get_snapshot(self, profile_token, basic_auth=False):
+    async def get_snapshot(
+        self, profile_token: str, basic_auth: bool = False
+    ) -> Optional[bytes]:
         """Get a snapshot image from the camera."""
         uri = await self.get_snapshot_uri(profile_token)
         if uri is None:
             return None
 
         auth = None
         if self.user and self.passwd:
@@ -562,15 +640,19 @@
         xaddr = self.xaddrs.get(namespace)
         if not xaddr:
             raise ONVIFError("Device doesn`t support service: %s" % name)
 
         return xaddr, wsdlpath, binding_name
 
     async def create_onvif_service(
-        self, name: str, port_type: Optional[str] = None
+        self,
+        name: str,
+        port_type: Optional[str] = None,
+        read_timeout: Optional[int] = None,
+        write_timeout: Optional[int] = None,
     ) -> ONVIFService:
         """Create ONVIF service client"""
         name = name.lower()
         # Don't re-create bindings if the xaddr remains the same.
         # The xaddr can change when a new PullPointSubscription is created.
         binding_key = (name, port_type)
 
@@ -599,71 +681,78 @@
             self.passwd,
             wsdl_file,
             self.encrypt,
             no_cache=self.no_cache,
             dt_diff=self.dt_diff,
             binding_name=binding_name,
             binding_key=binding_key,
+            read_timeout=read_timeout,
+            write_timeout=write_timeout,
         )
         await service.setup()
 
         self.services[binding_key] = service
 
         return service
 
-    async def create_devicemgmt_service(self):
+    async def create_devicemgmt_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("devicemgmt")
 
-    async def create_media_service(self):
+    async def create_media_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("media")
 
-    async def create_ptz_service(self):
+    async def create_ptz_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("ptz")
 
-    async def create_imaging_service(self):
+    async def create_imaging_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("imaging")
 
-    async def create_deviceio_service(self):
+    async def create_deviceio_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("deviceio")
 
-    async def create_events_service(self):
+    async def create_events_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("events")
 
-    async def create_analytics_service(self):
+    async def create_analytics_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("analytics")
 
-    async def create_recording_service(self):
+    async def create_recording_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("recording")
 
-    async def create_search_service(self):
+    async def create_search_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("search")
 
-    async def create_replay_service(self):
+    async def create_replay_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("replay")
 
-    async def create_pullpoint_service(self):
+    async def create_pullpoint_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service(
-            "pullpoint", port_type="PullPointSubscription"
+            "pullpoint",
+            port_type="PullPointSubscription",
+            read_timeout=_PULLPOINT_TIMEOUT,
+            write_timeout=_PULLPOINT_TIMEOUT,
         )
 
-    async def create_notification_service(self):
+    async def create_notification_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("notification")
 
-    async def create_subscription_service(self, port_type=None):
+    async def create_subscription_service(
+        self, port_type: Optional[str] = None
+    ) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("subscription", port_type=port_type)
 
-    async def create_receiver_service(self):
+    async def create_receiver_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("receiver")
```

### Comparing `onvif-zeep-async-2.0.0/onvif/definition.py` & `onvif-zeep-async-2.1.0/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/exceptions.py` & `onvif-zeep-async-2.1.0/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-2.1.0/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/addressing` & `onvif-zeep-async-2.1.0/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/display.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/envelope` & `onvif-zeep-async-2.1.0/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/events.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/media.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/search.wsdl` & `onvif-zeep-async-2.1.0/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/types.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/xml.xsd` & `onvif-zeep-async-2.1.0/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif/wsdl/xmlmime` & `onvif-zeep-async-2.1.0/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.0.0
+Version: 2.1.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-2.1.0/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/pylintrc` & `onvif-zeep-async-2.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/setup.py` & `onvif-zeep-async-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.0.0/tests/test.py` & `onvif-zeep-async-2.1.0/tests/test.py`

 * *Files identical despite different names*

