# Comparing `tmp/vodesfunc-1.3.5.tar.gz` & `tmp/vodesfunc-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.5.tar", last modified: Thu May  4 22:52:46 2023, max compression
+gzip compressed data, was "vodesfunc-1.3.6.tar", last modified: Thu May  4 22:58:44 2023, max compression
```

## Comparing `vodesfunc-1.3.5.tar` & `vodesfunc-1.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.067706 vodesfunc-1.3.5/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.5/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-05-04 22:52:46.066706 vodesfunc-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 22:52:46.067706 vodesfunc-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.051116 vodesfunc-1.3.5/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.5/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-05-04 22:52:33.000000 vodesfunc-1.3.5/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.5/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.066706 vodesfunc-1.3.5/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.5/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.5/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.5/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.5/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.5/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.5/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.5/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.5/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12864 2023-05-04 21:46:43.000000 vodesfunc-1.3.5/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.5/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.5/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    14121 2023-04-28 23:11:05.000000 vodesfunc-1.3.5/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.5/vodesfunc/types.py
--rw-rw-rw-   0        0        0     7612 2023-05-04 22:46:04.000000 vodesfunc-1.3.5/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.062658 vodesfunc-1.3.5/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 22:58:44.720537 vodesfunc-1.3.6/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-05-04 22:58:44.720537 vodesfunc-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.6/README.md
+-rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 22:58:44.720537 vodesfunc-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:58:44.712356 vodesfunc-1.3.6/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.6/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-05-04 22:58:20.000000 vodesfunc-1.3.6/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.6/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:58:44.719536 vodesfunc-1.3.6/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.6/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.6/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.6/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.6/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.6/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.6/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.6/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.6/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    12864 2023-05-04 21:46:43.000000 vodesfunc-1.3.6/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.6/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.6/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14121 2023-04-28 23:11:05.000000 vodesfunc-1.3.6/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.6/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     7717 2023-05-04 22:57:47.000000 vodesfunc-1.3.6/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:58:44.716357 vodesfunc-1.3.6/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-05-04 22:58:44.000000 vodesfunc-1.3.6/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-05-04 22:58:44.000000 vodesfunc-1.3.6/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 22:58:44.000000 vodesfunc-1.3.6/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-04 22:58:44.000000 vodesfunc-1.3.6/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 22:58:44.000000 vodesfunc-1.3.6/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.5/LICENSE` & `vodesfunc-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/PKG-INFO` & `vodesfunc-1.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.5
+Version: 1.3.6
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.5/setup.py` & `vodesfunc-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/aa.py` & `vodesfunc-1.3.6/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/convert.py` & `vodesfunc-1.3.6/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/download.py` & `vodesfunc-1.3.6/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/fonts.py` & `vodesfunc-1.3.6/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/muxing.py` & `vodesfunc-1.3.6/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/parsing.py` & `vodesfunc-1.3.6/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/auto/webhook.py` & `vodesfunc-1.3.6/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/automation.py` & `vodesfunc-1.3.6/vodesfunc/automation.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/denoise.py` & `vodesfunc-1.3.6/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/descale.py` & `vodesfunc-1.3.6/vodesfunc/descale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/misc.py` & `vodesfunc-1.3.6/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/noise.py` & `vodesfunc-1.3.6/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/scale.py` & `vodesfunc-1.3.6/vodesfunc/scale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/types.py` & `vodesfunc-1.3.6/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.5/vodesfunc/util.py` & `vodesfunc-1.3.6/vodesfunc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,32 +73,33 @@
 
     import shutil as sh
     from pathlib import Path
 
     forceFallBack = sh.which('dgindexnv') is None or not hasattr(core, "dgdecodenv")
 
     # I don't want that to be a hard dependency :trollhd:
-    try:
-        import pymediainfo as pym
-        parsed = pym.MediaInfo.parse(filePath, parse_speed=0.25)
-        trackmeta = parsed.video_tracks[0].to_data()
-        format = trackmeta.get('format')
-        bitdepth = trackmeta.get('bit_depth')
-        if (format is not None and bitdepth is not None):
-            if (str(format).strip().lower() == 'avc' and int(bitdepth) > 8):
-                forceFallBack = True
-                print(f'Falling back to lsmas for Hi10 ({Path(filePath).name})')
-            elif(str(format).strip().lower() == 'ffv1'):
-                forceFallBack = True
-                print(f'Falling back to lsmas for FFV1 ({Path(filePath).name})')
-    except OSError:
-        print('pymediainfo could not find the mediainfo library! (it needs to be in path)')
-    except:
-        print('Parsing mediainfo failed. (Do you have pymediainfo installed?)')
-
+    if not force_lsmas:
+        try:
+            import pymediainfo as pym
+            parsed = pym.MediaInfo.parse(filePath, parse_speed=0.25)
+            trackmeta = parsed.video_tracks[0].to_data()
+            format = trackmeta.get('format')
+            bitdepth = trackmeta.get('bit_depth')
+            if (format is not None and bitdepth is not None):
+                if (str(format).strip().lower() == 'avc' and int(bitdepth) > 8):
+                    forceFallBack = True
+                    print(f'Falling back to lsmas for Hi10 ({Path(filePath).name})')
+                elif(str(format).strip().lower() == 'ffv1'):
+                    forceFallBack = True
+                    print(f'Falling back to lsmas for FFV1 ({Path(filePath).name})')
+        except OSError:
+            print('pymediainfo could not find the mediainfo library! (it needs to be in path)')
+        except:
+            print('Parsing mediainfo failed. (Do you have pymediainfo installed?)')
+            
     if force_lsmas or forceFallBack:
         return core.lsmas.LWLibavSource(filePath, **kwargs)
 
     path = Path(filePath)
     dgiFile = path.with_suffix('.dgi')
 
     if dgiFile.exists():
```

### Comparing `vodesfunc-1.3.5/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.3.6/vodesfunc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.5
+Version: 1.3.6
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.5/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.3.6/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

