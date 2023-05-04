# Comparing `tmp/vskernels-2.3.2.tar.gz` & `tmp/vskernels-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vskernels-2.3.2.tar", last modified: Sun Mar 26 17:38:21 2023, max compression
+gzip compressed data, was "vskernels-2.4.0.tar", last modified: Thu May  4 22:00:14 2023, max compression
```

## Comparing `vskernels-2.3.2.tar` & `vskernels-2.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:21.485987 vskernels-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-26 17:38:00.000000 vskernels-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-03-26 17:38:21.485987 vskernels-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-26 17:38:00.000000 vskernels-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-26 17:38:21.485987 vskernels-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-26 17:38:00.000000 vskernels-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:21.481987 vskernels-2.3.2/vskernels/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:21.485987 vskernels-2.3.2/vskernels/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/bicubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/fmtconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/placebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/kernels/various.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-26 17:38:00.000000 vskernels-2.3.2/vskernels/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:21.485987 vskernels-2.3.2/vskernels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-03-26 17:38:21.000000 vskernels-2.3.2/vskernels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-26 17:38:21.000000 vskernels-2.3.2/vskernels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:38:21.000000 vskernels-2.3.2/vskernels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 17:38:21.000000 vskernels-2.3.2/vskernels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-26 17:38:21.000000 vskernels-2.3.2/vskernels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 21:59:44.000000 vskernels-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-04 22:00:14.525055 vskernels-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 21:59:44.000000 vskernels-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 22:00:14.525055 vskernels-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 21:59:44.000000 vskernels-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.521055 vskernels-2.4.0/vskernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/vskernels/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/bicubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/fmtconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/placebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/various.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/vskernels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/top_level.txt
```

### Comparing `vskernels-2.3.2/LICENSE` & `vskernels-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/PKG-INFO` & `vskernels-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vskernels
-Version: 2.3.2
+Version: 2.4.0
 Summary: Kernel objects for scaling and format conversion within VapourSynth
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-kernels
 Project-URL: Documentation, https://vskernels.encode.moe/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vskernels Version: 2.3.2 Summary: Kernel objects
+Metadata-Version: 2.1 Name: vskernels Version: 2.4.0 Summary: Kernel objects
 for scaling and format conversion within VapourSynth Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev Project-URL: Source Code, https://
 github.com/Irrational-Encoding-Wizardry/vs-kernels Project-URL: Documentation,
 https://vskernels.encode.moe/en/latest/ Project-URL: Contact, https://
 discord.gg/qxTxVJGtst Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Other Audience
```

### Comparing `vskernels-2.3.2/README.md` & `vskernels-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/setup.cfg` & `vskernels-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/setup.py` & `vskernels-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/__init__.py` & `vskernels-2.4.0/vskernels/__init__.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/exceptions.py` & `vskernels-2.4.0/vskernels/exceptions.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/abstract.py` & `vskernels-2.4.0/vskernels/kernels/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from abc import abstractmethod
+from math import ceil
 from typing import Any, Sequence, Union, cast, overload
 
 from vstools import (
-    CustomValueError, FuncExceptT, GenericVSFunction, HoldsVideoFormatT, Matrix, MatrixT, T, VideoFormatT, core,
-    get_subclasses, get_video_format, inject_self, vs, vs_object
+    CustomValueError, FuncExceptT, GenericVSFunction, HoldsVideoFormatT, Matrix, MatrixT, T, VideoFormatT,
+    check_variable_resolution, core, get_subclasses, get_video_format, inject_self, vs, vs_object
 )
 
 from ..exceptions import UnknownDescalerError, UnknownKernelError, UnknownScalerError
 
 __all__ = [
     'Scaler', 'ScalerT',
     'Descaler',
@@ -99,14 +100,29 @@
 
     @classmethod
     def ensure_obj(
         cls: type[Scaler], scaler: ScalerT | None = None, func_except: FuncExceptT | None = None
     ) -> Scaler:
         return BaseScaler.ensure_obj(cls, Scaler, scaler, UnknownScalerError, [], func_except)  # type: ignore
 
+    @inject_self.cached
+    def multi(
+        self, clip: vs.VideoNode, multi: float = 2, shift: tuple[float, float] = (0, 0), **kwargs: Any
+    ) -> vs.VideoNode:
+        assert check_variable_resolution(clip, self.multi)
+
+        dst_width, dst_height = ceil(clip.width * multi), ceil(clip.height * multi)
+
+        if max(dst_width, dst_height) <= 0.0:
+            raise CustomValueError(
+                'Multiplying the resolution by "multi" must result in a positive resolution!', self.multi, multi
+            )
+
+        return self.scale(clip, dst_width, dst_height, shift, **kwargs)
+
 
 class Descaler(vs_object):
     @abstractmethod
     @inject_self.cached
     def descale(
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs: Any
     ) -> vs.VideoNode:
```

### Comparing `vskernels-2.3.2/vskernels/kernels/bicubic.py` & `vskernels-2.4.0/vskernels/kernels/bicubic.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
 class SetsuCubic(Bicubic):
     """
     Schizo (Setsugen's) values calculated from the legendary Pompo-san filterchain.
     Useful for heavy post processed content or ringing in general.
 
     Bicubic
-    strenght=200: b=-0.22582213942537233, c=0.06676658576029935
-    strenght=100: b=-0.26470935063297507, c=0.73588297801744030
+    strength=200: b=-0.22582213942537233, c=0.06676658576029935
+    strength=100: b=-0.26470935063297507, c=0.73588297801744030
     strength=50:  b=-0.24550548633321580, c=0.37020197611906490
     strength=1:   b=-0.32938660656063920, c=0.21245005943760129
     """
 
     def __init__(self, strength: float = 100.0, **kwargs: Any) -> None:
         super().__init__(
             asinh(.5) * acos(.5) * -abs(cos(strength * 4)),
```

### Comparing `vskernels-2.3.2/vskernels/kernels/docs.py` & `vskernels-2.4.0/vskernels/kernels/docs.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/fmtconv.py` & `vskernels-2.4.0/vskernels/kernels/fmtconv.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,23 +78,35 @@
         return Bicubic.resample(filtered, out_fmt)
 
     descale_function = scale_function
 
     _kernel: str
     """Name of the fmtconv kernel"""
 
+    _resize_fmtc_params_lut = {
+        'sw': 'src_width', 'sx': 'src_left',
+        'sh': 'src_height', 'sy': 'src_top'
+    }
+
     def __init__(self, taps: int = 4, **kwargs: Any) -> None:
         self.taps = taps
         super().__init__(**kwargs)
 
+    def _clean_args(self, **kwargs: Any) -> dict[str, Any]:
+        for fmtc_param, res_param in self._resize_fmtc_params_lut.items():
+            if res_param in kwargs:
+                kwargs[fmtc_param] = kwargs.pop(res_param)
+
+        return kwargs
+
     def get_scale_args(
         self, clip: vs.VideoNode, shift: tuple[float, float] = (0, 0),
         width: int | None = None, height: int | None = None, **kwargs: Any
     ) -> dict[str, Any]:
-        return dict(
+        return self._clean_args(
             sx=shift[1], sy=shift[0], kernel=self._kernel,
             **self.kwargs, **self.get_params_args(False, clip, width, height, **kwargs)
         )
 
     def get_descale_args(
         self, clip: vs.VideoNode, shift: tuple[float, float] = (0, 0),
         width: int | None = None, height: int | None = None, **kwargs: Any
@@ -102,15 +114,15 @@
         args = dict(
             invks=True, invkstaps=self.taps,
         ) | self.get_scale_args(
             clip, shift, width, height, **kwargs
         ) | self.get_params_args(
             True, clip, width, height, **kwargs
         )
-        return args
+        return self._clean_args(**args)
 
     def get_params_args(
         self, is_descale: bool, clip: vs.VideoNode, width: int | None = None, height: int | None = None, **kwargs: Any
     ) -> dict[str, Any]:
         if is_descale:
             return kwargs | dict(w=width, h=height, sw=width, sh=height)
         return kwargs | dict(w=width, h=height)
```

### Comparing `vskernels-2.3.2/vskernels/kernels/impulse.py` & `vskernels-2.4.0/vskernels/kernels/impulse.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/placebo.py` & `vskernels-2.4.0/vskernels/kernels/placebo.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/resize.py` & `vskernels-2.4.0/vskernels/kernels/resize.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/spline.py` & `vskernels-2.4.0/vskernels/kernels/spline.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/kernels/various.py` & `vskernels-2.4.0/vskernels/kernels/various.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels/util.py` & `vskernels-2.4.0/vskernels/util.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.3.2/vskernels.egg-info/PKG-INFO` & `vskernels-2.4.0/vskernels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vskernels
-Version: 2.3.2
+Version: 2.4.0
 Summary: Kernel objects for scaling and format conversion within VapourSynth
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-kernels
 Project-URL: Documentation, https://vskernels.encode.moe/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vskernels Version: 2.3.2 Summary: Kernel objects
+Metadata-Version: 2.1 Name: vskernels Version: 2.4.0 Summary: Kernel objects
 for scaling and format conversion within VapourSynth Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev Project-URL: Source Code, https://
 github.com/Irrational-Encoding-Wizardry/vs-kernels Project-URL: Documentation,
 https://vskernels.encode.moe/en/latest/ Project-URL: Contact, https://
 discord.gg/qxTxVJGtst Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Other Audience
```

### Comparing `vskernels-2.3.2/vskernels.egg-info/SOURCES.txt` & `vskernels-2.4.0/vskernels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

