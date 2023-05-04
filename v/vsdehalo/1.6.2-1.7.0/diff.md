# Comparing `tmp/vsdehalo-1.6.2.tar.gz` & `tmp/vsdehalo-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdehalo-1.6.2.tar", last modified: Sun Mar 26 17:40:23 2023, max compression
+gzip compressed data, was "vsdehalo-1.7.0.tar", last modified: Thu May  4 21:59:26 2023, max compression
```

## Comparing `vsdehalo-1.6.2.tar` & `vsdehalo-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:23.165032 vsdehalo-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-26 17:40:23.165032 vsdehalo-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:40:23.165032 vsdehalo-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:23.161032 vsdehalo-1.6.2/vsdehalo/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/vine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-26 17:39:59.000000 vsdehalo-1.6.2/vsdehalo/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:23.165032 vsdehalo-1.6.2/vsdehalo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-26 17:40:23.000000 vsdehalo-1.6.2/vsdehalo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-26 17:40:23.000000 vsdehalo-1.6.2/vsdehalo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:40:23.000000 vsdehalo-1.6.2/vsdehalo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-26 17:40:23.000000 vsdehalo-1.6.2/vsdehalo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 17:40:23.000000 vsdehalo-1.6.2/vsdehalo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/vsdehalo/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/vine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/vsdehalo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/top_level.txt
```

### Comparing `vsdehalo-1.6.2/LICENSE` & `vsdehalo-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.6.2/PKG-INFO` & `vsdehalo-1.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.6.2
+Version: 1.7.0
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

### Comparing `vsdehalo-1.6.2/setup.cfg` & `vsdehalo-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.6.2/setup.py` & `vsdehalo-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.6.2/vsdehalo/alpha.py` & `vsdehalo-1.7.0/vsdehalo/alpha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 
 from typing import Any, Sequence, final
 
 from vsaa import Nnedi3
 from vsexprtools import ExprOp, complexpr_available, combine, norm_expr
 from vskernels import BSpline, Lanczos, Mitchell, NoShift, Point, Scaler, ScalerT
-from vsmasktools import EdgeDetect, Morpho, Robinson3, XxpandMode, grow_mask
-from vsrgtools import box_blur, contrasharpening, contrasharpening_dehalo, repair
+from vsmasktools import EdgeDetect, Morpho, Robinson3, XxpandMode, grow_mask, retinex
+from vsrgtools import (
+    box_blur, contrasharpening, contrasharpening_dehalo, repair, RemoveGrainMode, RepairMode, gauss_blur, limit_filter
+)
 from vsrgtools.util import norm_rmode_planes
 from vsdenoise import Prefilter
 from vstools import (
-    ColorRange, ConvMode, CustomIndexError, CustomIntEnum, CustomValueError, FuncExceptT, InvalidColorFamilyError,
-    PlanesT, check_variable, clamp, cround, fallback, get_peak_value, join, mod4, normalize_planes, normalize_seq,
-    scale_value, split, to_arr, vs
+    ColorRange, ConvMode, CustomIndexError, CustomIntEnum, CustomValueError, FuncExceptT, FunctionUtil,
+    InvalidColorFamilyError, KwargsT, PlanesT, check_variable, clamp, cround, fallback, get_peak_value,
+    join, mod4, normalize_planes, normalize_seq, scale_value, split, to_arr, get_y, vs
 )
 
+
 __all__ = [
     'fine_dehalo',
     'fine_dehalo2',
     'dehalo_alpha',
-    'dehalo_sigma'
+    'dehalo_sigma',
+    'dehalomicron'
 ]
 
 
 FloatIterArr = float | list[float] | tuple[float | list[float], ...]
 
 
 def _limit_dehalo(
@@ -246,15 +250,15 @@
         # Final mask building #
 
         # Previous mask may be a bit weak on the pure edge side, so we ensure
         # that the main edges are really excluded. We do not want them to be
         # smoothed by the halo removal.
         shr_med = combine([strong, shrink], ExprOp.MAX, planes=planes) if exclude else strong
 
-        # Substracts masks and amplifies the difference to be sure we get 255
+        # Subtracts masks and amplifies the difference to be sure we get 255
         # on the areas to be processed.
         mask = norm_expr([large, shr_med], 'x y - 2 *', planes)
 
         # If edge processing is required, adds the edgemask
         if edgeproc > 0:
             mask = norm_expr([mask, strong], f'x y {edgeproc} 0.66 * * +', planes)
 
@@ -288,15 +292,15 @@
         if chroma:
             return join([y_merge, *chroma], clip.format.color_family)
 
         return y_merge
 
     def mask(
         self, clip: vs.VideoNode, dehaloed: vs.VideoNode | None = None,
-        rx: int = 1, ry: int | None = None, thmi: int = 50, thma: int = 100, thlimi: int = 80, thlima: int = 100,
+        rx: int = 1, ry: int | None = None, thmi: int = 50, thma: int = 100, thlimi: int = 50, thlima: int = 100,
         exclude: bool = True, edgeproc: float = 0.0, edgemask: EdgeDetect = Robinson3(),
         mask: int | FineDehaloMask = 1, planes: PlanesT = 0, first_plane: bool = False, func: FuncExceptT | None = None
     ) -> vs.VideoNode:
         """
         :param clip:                Source clip.
         :param dehaloed:            Optional dehaloed clip to mask. If this is specified, instead of returning
                                     the mask, the function will return the maskedmerged clip to this.
@@ -459,15 +463,15 @@
         dehaloed = norm_expr(d_clips, d_expr, planes)
     else:
         for fix, mask in [(fix_h, mask_v), (fix_v, mask_h)]:
             if mask:
                 dehaloed = dehaloed.std.MaskedMerge(fix, mask)
 
         if op:
-            dehaloed = combine([work_clip, dehaloed], ExprOp(op))
+            dehaloed = combine([work_clip, dehaloed], op)  # type: ignore
 
     if darkstr != brightstr != 1.0:
         dehaloed = _limit_dehalo(work_clip, dehaloed, darkstr, brightstr, planes)
 
     if not chroma:
         return dehaloed
 
@@ -640,7 +644,74 @@
     if (dehalo.width, dehalo.height) != (clip.width, clip.height):
         dehalo = pre_downscaler.scale(work_clip, clip.width, clip.height)
 
     if not chroma:
         return dehalo
 
     return join([dehalo, *chroma], clip.format.color_family)
+
+
+def dehalomicron(
+    clip: vs.VideoNode, brz: float = 0.75, sigma: float = 1.55, sigma0: float = 1.15, ss: float = 1.65,
+    pre_ss: bool = True, dampen: float | list[float] | tuple[float | list[float], bool | None] = 0.65,
+    sigma_ref: float = 4.3333, planes: PlanesT = 0, fdhealo_kwargs: KwargsT | None = None, **kwargs: Any
+) -> vs.VideoNode:
+    func = FunctionUtil(clip, dehalomicron, planes, (vs.GRAY, vs.YUV))
+
+    fdhealo_kwargs = KwargsT(edgeproc=0.5, ss=1.5 if pre_ss else 2.0) | (fdhealo_kwargs or {})
+
+    y = get_y(func.work_clip)
+
+    y_mask = retinex(y)
+
+    dehalo_ref0 = dehalo_sigma(func.work_clip, sigma=sigma0, planes=planes)
+    dehalo_ref0mask = dehalo_sigma(y_mask, sigma=sigma0 + sigma0 * 0.09)
+
+    ymask_ref0 = gauss_blur(y_mask, sigma=sigma_ref)
+
+    dehalo_mask = norm_expr([dehalo_ref0mask, y_mask], 'x y - abs 100 *')
+    dehalo_mask = RemoveGrainMode.CIRCLE_BLUR(dehalo_mask)
+    dehalo_mask = RemoveGrainMode.MINMAX_MEDIAN_OPP(dehalo_mask)
+
+    dmask_expr = 'x 2 *'
+
+    if brz != 0.0:
+        dmask_expr = f"x {scale_value(abs(brz) / 10, 32, y)} {'>' if brz < 0.0 else '>'} 0 {dmask_expr} ?"
+
+    dehalo_mask = norm_expr(dehalo_mask, dmask_expr, func.norm_planes)
+
+    fine_edge_mask = fine_dehalo.mask(norm_expr([y_mask, ymask_ref0], 'y x -'), planes=func.norm_planes)
+    dehalo_mask = norm_expr(
+        [dehalo_mask, y_mask, ymask_ref0, fine_edge_mask], 'y z + 2 / x < x and x abs a ?', func.norm_planes
+    )
+    dehalo_mask = RemoveGrainMode.EDGE_CLIP_STRONG(dehalo_mask)
+
+    actual_dehalo = dehalo_sigma(
+        func.work_clip, pre_ss=1 + pre_ss, sigma=sigma, ss=ss - 0.5 * pre_ss, planes=func.norm_planes, **kwargs
+    )
+    dehalo_ref = fine_dehalo(func.work_clip, planes=func.norm_planes, **fdhealo_kwargs)
+
+    dehalo_min = ExprOp.MIN(actual_dehalo, dehalo_ref, planes=func.norm_planes)
+
+    dehalo = limit_filter(actual_dehalo, func.work_clip, dehalo_ref, planes=func.norm_planes)
+    dehalo = dehalo.std.MaskedMerge(dehalo_min, dehalo_mask, func.norm_planes)
+
+    if isinstance(dampen, tuple):
+        dampen_amt, dampen_rev = dampen
+    else:
+        dampen_amt, dampen_rev = dampen, None
+
+    if dampen_rev is None:
+        dampen_rev = not pre_ss
+
+    dampen_amt = func.norm_seq(dampen_amt)
+
+    if max(dampen_amt) > 0.0:
+        dehalo_ref0 = dehalo.std.Merge(dehalo_ref0, dampen_amt)
+
+    rep = RepairMode.MINMAX_SQUARE_REF_CLOSE if pre_ss else RepairMode.MINMAX_SQUARE_REF1
+
+    clips = (dehalo, dehalo_ref0)
+
+    dehalo = rep(*(reversed(clips) if dampen_rev else clips), func.norm_planes)  # type: ignore
+
+    return func.return_clip(dehalo)
```

### Comparing `vsdehalo-1.6.2/vsdehalo/denoise.py` & `vsdehalo-1.7.0/vsdehalo/denoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 from math import ceil
 
 from vsaa import Nnedi3
 from vsdenoise import Prefilter
-from vsexprtools import ExprToken, norm_expr
+from vsexprtools import ExprOp, ExprToken, norm_expr
 from vskernels import NoShift, Point, Scaler, ScalerT
 from vsmasktools import Morpho, Prewitt
 from vsrgtools import LimitFilterMode, contrasharpening, contrasharpening_dehalo, limit_filter, repair
-from vstools import FunctionUtil, PlanesT, check_ref_clip, fallback, mod4, plane, scale_value, vs
+from vstools import FunctionUtil, PlanesT, check_ref_clip, fallback, mod4, plane, vs
 
 __all__ = [
     'smooth_dering'
 ]
 
 
 def smooth_dering(
     clip: vs.VideoNode,
     smooth: vs.VideoNode | Prefilter = Prefilter.MINBLUR1,
     ringmask: vs.VideoNode | None = None,
-    mrad: int = 1, msmooth: int = 1, minp: int = 1, mthr: int = 60, incedge: bool = False,
+    mrad: int = 1, msmooth: int = 1, minp: int = 1, mthr: float = 0.24, incedge: bool = False,
     thr: int = 12, elast: float = 2.0, darkthr: int | None = None,
     contra: int | float | bool = 1.2, drrep: int = 13, pre_ss: float = 1.0,
     pre_supersampler: ScalerT = Nnedi3(0, field=0, shifter=NoShift),
     pre_downscaler: ScalerT = Point, planes: PlanesT = 0, show_mask: bool = False
 ) -> vs.VideoNode:
     """
     :param clip:        Clip to process.
@@ -111,15 +111,15 @@
         repclp = work_clip
 
     limitclp = limit_filter(
         repclp, work_clip, None, LimitFilterMode.CLAMPING, planes, thr, elast, darkthr
     )
 
     if ringmask is None:
-        prewittm = Prewitt.edgemask(work_clip, scale_value(mthr, 8, work_clip))
+        prewittm = Prewitt.edgemask(work_clip, mthr)
 
         fmask = prewittm.std.Median(planes).misc.Hysteresis(prewittm, planes)
 
         omask = Morpho.expand(fmask, mrad, mrad, planes=planes) if mrad > 0 else fmask
 
         if msmooth > 0:
             omask = Morpho.inflate(omask, msmooth, planes)
@@ -130,15 +130,17 @@
             if minp <= 0:
                 imask = fmask
             elif minp % 2 == 0:
                 imask = Morpho.inpand(fmask, minp // 2, planes=planes)
             else:
                 imask = Morpho.inpand(Morpho.inflate(fmask, 1, planes), ceil(minp / 2), planes=planes)
 
-            ringmask = norm_expr([omask, imask], f'{ExprToken.RangeMax} {ExprToken.RangeMax} y - / x *')
+            ringmask = norm_expr(
+                [omask, imask], [f'{ExprToken.RangeMax} {ExprToken.RangeMax} y - / x *', ExprOp.clamp()]
+            )
 
     dering = work_clip.std.MaskedMerge(limitclp, ringmask, planes)
 
     if show_mask:
         return ringmask
 
     if (dering.width, dering.height) != (clip.width, clip.height):
```

### Comparing `vsdehalo-1.6.2/vsdehalo/vine.py` & `vsdehalo-1.7.0/vsdehalo/vine.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.6.2/vsdehalo/warp.py` & `vsdehalo-1.7.0/vsdehalo/warp.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.6.2/vsdehalo.egg-info/PKG-INFO` & `vsdehalo-1.7.0/vsdehalo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.6.2
+Version: 1.7.0
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

