# Comparing `tmp/vodesfunc-1.3.4.tar.gz` & `tmp/vodesfunc-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.4.tar", last modified: Fri Apr 28 23:11:25 2023, max compression
+gzip compressed data, was "vodesfunc-1.3.5.tar", last modified: Thu May  4 22:52:46 2023, max compression
```

## Comparing `vodesfunc-1.3.4.tar` & `vodesfunc-1.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:11:25.605819 vodesfunc-1.3.4/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.4/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-04-28 23:11:25.604511 vodesfunc-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.4/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 23:11:25.605819 vodesfunc-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:11:25.593445 vodesfunc-1.3.4/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.4/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-04-28 23:10:34.000000 vodesfunc-1.3.4/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.4/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:11:25.604511 vodesfunc-1.3.4/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.4/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.4/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.4/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.4/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.4/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.4/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.4/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.4/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12477 2023-04-28 20:16:26.000000 vodesfunc-1.3.4/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.4/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.4/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    14121 2023-04-28 23:11:05.000000 vodesfunc-1.3.4/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.4/vodesfunc/types.py
--rw-rw-rw-   0        0        0     7542 2023-04-28 20:15:55.000000 vodesfunc-1.3.4/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:11:25.601510 vodesfunc-1.3.4/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-04-28 23:11:25.000000 vodesfunc-1.3.4/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-04-28 23:11:25.000000 vodesfunc-1.3.4/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:11:25.000000 vodesfunc-1.3.4/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-28 23:11:25.000000 vodesfunc-1.3.4/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 23:11:25.000000 vodesfunc-1.3.4/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.067706 vodesfunc-1.3.5/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-05-04 22:52:46.066706 vodesfunc-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/README.md
+-rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 22:52:46.067706 vodesfunc-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.051116 vodesfunc-1.3.5/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.5/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-05-04 22:52:33.000000 vodesfunc-1.3.5/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.5/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.066706 vodesfunc-1.3.5/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.5/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.5/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.5/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.5/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.5/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.5/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.5/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.5/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    12864 2023-05-04 21:46:43.000000 vodesfunc-1.3.5/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.5/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.5/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14121 2023-04-28 23:11:05.000000 vodesfunc-1.3.5/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.5/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     7612 2023-05-04 22:46:04.000000 vodesfunc-1.3.5/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:52:46.062658 vodesfunc-1.3.5/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 22:52:45.000000 vodesfunc-1.3.5/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.4/LICENSE` & `vodesfunc-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/PKG-INFO` & `vodesfunc-1.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.4
+Version: 1.3.5
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.4/setup.py` & `vodesfunc-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/aa.py` & `vodesfunc-1.3.5/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/convert.py` & `vodesfunc-1.3.5/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/download.py` & `vodesfunc-1.3.5/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/fonts.py` & `vodesfunc-1.3.5/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/muxing.py` & `vodesfunc-1.3.5/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/parsing.py` & `vodesfunc-1.3.5/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/auto/webhook.py` & `vodesfunc-1.3.5/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/automation.py` & `vodesfunc-1.3.5/vodesfunc/automation.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/denoise.py` & `vodesfunc-1.3.5/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/descale.py` & `vodesfunc-1.3.5/vodesfunc/descale.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,23 @@
                 ref_y = self.kernel.scale(base_height_desc, clip.width, clip.height)
             else:
                 ref_y = self.rescale
             
         if self.line_mask != False:
             if not isinstance(self.line_mask, vs.VideoNode):
                 try:
-                    from vsmask.edge import KirschTCanny
-                except:
                     from vsmasktools.edge import KirschTCanny
-                self.line_mask = KirschTCanny().edgemask(clip, lthr=80 << 8, hthr=150 << 8)
+                    try:
+                        # Scaling was changed so I abuse the new param to check if its the newer version
+                        self.line_mask = KirschTCanny().edgemask(clip, lthr=80 / 255, hthr=150 / 255, planes=(0, True))
+                    except:
+                        self.line_mask = KirschTCanny().edgemask(clip, lthr=80 << 8, hthr=150 << 8)
+                except:
+                    from vsmask.edge import KirschTCanny
+                    self.line_mask = KirschTCanny().edgemask(clip, lthr=80 << 8, hthr=150 << 8)
             
             if self.do_post_double is not None:
                 self.line_mask = self.line_mask.std.Inflate()
 
             self.line_mask = depth(self.line_mask, 16)
             
         if self.credit_mask != False or self.credit_mask_thr <= 0:
```

### Comparing `vodesfunc-1.3.4/vodesfunc/misc.py` & `vodesfunc-1.3.5/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/noise.py` & `vodesfunc-1.3.5/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/scale.py` & `vodesfunc-1.3.5/vodesfunc/scale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/types.py` & `vodesfunc-1.3.5/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.4/vodesfunc/util.py` & `vodesfunc-1.3.5/vodesfunc/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 class src_file:
 
     file: Path
     src: vs.VideoNode
     src_cut: vs.VideoNode
     trim: Trim = None
 
-    def __init__(self, file: PathLike, trim_start: int = 0, trim_end: int = 0, idx: Callable[[str], vs.VideoNode] = None, force_lsmas: bool = False) -> None:
+    def __init__(self, file: PathLike, trim_start: int = 0, trim_end: int = 0, idx: Callable[[str], vs.VideoNode] = None, force_lsmas: bool = False, **kwargs) -> None:
         """
             Custom `FileInfo` kind of thing for convenience
 
             :param file:            Either a string based filepath or a Path object
             :param trim_start:      At what frame the `src_cut` clip should start
             :param trim_end:        At what frame the `src_cut` clip should end
             :param idx:             Indexer for the input file. Pass a function that takes a string in and returns a vs.VideoNode.\nDefaults to `vodesfunc.src`
             :param force_lsmas:     Forces the use of lsmas inside of `vodesfunc.src`
         """
         self.file = file if isinstance(file, Path) else Path(file)
-        self.src = idx(str(self.file.resolve())) if idx else src(str(self.file.resolve()), force_lsmas)
+        self.src = idx(str(self.file.resolve())) if idx else src(str(self.file.resolve()), force_lsmas, **kwargs)
         if trim_start is None:
             trim_start = 0
         if trim_start != 0 or trim_end != 0:
             self.trim = (trim_start, trim_end)
             if trim_start != 0 and trim_end != 0 and trim_end != None:
                 self.src_cut = self.src[trim_start: trim_end]
             else:
@@ -54,26 +54,26 @@
             if self.file.with_suffix('.m2ts').exists():
                 self.file = self.file.with_suffix('.m2ts')
             else:
                 self.file = parse_m2ts_path(self.file)
 
 SRC_FILE = src_file
 
-def src(filePath: str = None, force_lsmas: bool = False, delete_dgi_log: bool = True) -> vs.VideoNode:
+def src(filePath: str = None, force_lsmas: bool = False, delete_dgi_log: bool = True, **kwargs) -> vs.VideoNode:
     """
         Uses dgindex as Source and requires dgindexnv in path
         to generate files if they don't exist.
 
         :param filepath:        Path to video or dgi file
         :param force_lsmas:     Skip dgsource entirely and use lsmas
         :param delete_dgi_log:  Delete the .log files dgindexnv creates
         :return:                Video Node
     """
     if filePath.lower().endswith('.dgi'):
-        return core.dgdecodenv.DGSource(filePath)
+        return core.dgdecodenv.DGSource(filePath, **kwargs)
 
     import shutil as sh
     from pathlib import Path
 
     forceFallBack = sh.which('dgindexnv') is None or not hasattr(core, "dgdecodenv")
 
     # I don't want that to be a hard dependency :trollhd:
@@ -92,30 +92,30 @@
                 print(f'Falling back to lsmas for FFV1 ({Path(filePath).name})')
     except OSError:
         print('pymediainfo could not find the mediainfo library! (it needs to be in path)')
     except:
         print('Parsing mediainfo failed. (Do you have pymediainfo installed?)')
 
     if force_lsmas or forceFallBack:
-        return core.lsmas.LWLibavSource(filePath)
+        return core.lsmas.LWLibavSource(filePath, **kwargs)
 
     path = Path(filePath)
     dgiFile = path.with_suffix('.dgi')
 
     if dgiFile.exists():
-        return core.dgdecodenv.DGSource(dgiFile.resolve(True))
+        return core.dgdecodenv.DGSource(dgiFile.resolve(True), **kwargs)
     else:
         print("Generating dgi file...")
         import os
         import subprocess as sub
         sub.Popen(f"dgindexnv -i \"{path.name}\" -h -o \"{dgiFile.name}\" -e",
                   shell=True, stdout=sub.DEVNULL, cwd=path.parent.resolve(True)).wait()
         if path.with_suffix('.log').exists() and delete_dgi_log:
             os.remove(path.with_suffix('.log').resolve(True))
-        return core.dgdecodenv.DGSource(dgiFile.resolve(True))
+        return core.dgdecodenv.DGSource(dgiFile.resolve(True), **kwargs)
 
 
 def set_output(clip: vs.VideoNode, name: str = None, frame_info: bool = False, allow_comp: bool = True) -> vs.VideoNode:
     """
     Outputs a clip. Less to type.
     Designed to be used with the good ol 'from vodesfunc import *' and the 'out' alias
     """
```

### Comparing `vodesfunc-1.3.4/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.3.5/vodesfunc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.4
+Version: 1.3.5
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.4/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.3.5/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

