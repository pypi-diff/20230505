# Comparing `tmp/ovos-tts-server-0.0.2a3.tar.gz` & `tmp/ovos-tts-server-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-server-0.0.2a3.tar", last modified: Fri May  5 03:15:24 2023, max compression
+gzip compressed data, was "ovos-tts-server-0.0.2a4.tar", last modified: Fri May  5 16:11:31 2023, max compression
```

## Comparing `ovos-tts-server-0.0.2a3.tar` & `ovos-tts-server-0.0.2a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/ovos_tts_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:31.344123 ovos-tts-server-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 16:11:31.344123 ovos-tts-server-0.0.2a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:31.344123 ovos-tts-server-0.0.2a4/ovos_tts_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/ovos_tts_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/ovos_tts_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/ovos_tts_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/ovos_tts_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:11:31.344123 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:11:31.000000 ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:11:31.344123 ovos-tts-server-0.0.2a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-05-05 16:11:30.000000 ovos-tts-server-0.0.2a4/setup.py
```

### Comparing `ovos-tts-server-0.0.2a3/LICENSE.md` & `ovos-tts-server-0.0.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.2a3/PKG-INFO` & `ovos-tts-server-0.0.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.2a3/ovos_tts_server/__init__.py` & `ovos-tts-server-0.0.2a4/ovos_tts_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.2a3/ovos_tts_server/__main__.py` & `ovos-tts-server-0.0.2a4/ovos_tts_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/PKG-INFO` & `ovos-tts-server-0.0.2a4/ovos_tts_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.2a3/setup.py` & `ovos-tts-server-0.0.2a4/setup.py`

 * *Files identical despite different names*

