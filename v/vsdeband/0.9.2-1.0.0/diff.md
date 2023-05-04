# Comparing `tmp/vsdeband-0.9.2.tar.gz` & `tmp/vsdeband-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdeband-0.9.2.tar", last modified: Sun Mar 26 17:40:14 2023, max compression
+gzip compressed data, was "vsdeband-1.0.0.tar", last modified: Thu May  4 21:59:35 2023, max compression
```

## Comparing `vsdeband-0.9.2.tar` & `vsdeband-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:14.013246 vsdeband-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-26 17:39:53.000000 vsdeband-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-26 17:40:14.013246 vsdeband-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-26 17:39:53.000000 vsdeband-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-26 17:40:14.013246 vsdeband-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-26 17:39:53.000000 vsdeband-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:14.013246 vsdeband-0.9.2/vsdeband/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/f3kdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/grainers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/placebo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-26 17:39:53.000000 vsdeband-0.9.2/vsdeband/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:14.013246 vsdeband-0.9.2/vsdeband.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-26 17:40:14.000000 vsdeband-0.9.2/vsdeband.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-26 17:40:14.000000 vsdeband-0.9.2/vsdeband.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:40:14.000000 vsdeband-0.9.2/vsdeband.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-26 17:40:14.000000 vsdeband-0.9.2/vsdeband.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 17:40:14.000000 vsdeband-0.9.2/vsdeband.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.128878 vsdeband-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 21:59:08.000000 vsdeband-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 21:59:35.128878 vsdeband-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 21:59:08.000000 vsdeband-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 21:59:35.128878 vsdeband-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-04 21:59:08.000000 vsdeband-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.124879 vsdeband-1.0.0/vsdeband/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/f3kdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/placebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.128878 vsdeband-1.0.0/vsdeband.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/top_level.txt
```

### Comparing `vsdeband-0.9.2/LICENSE` & `vsdeband-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdeband-0.9.2/PKG-INFO` & `vsdeband-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 0.9.2
+Version: 1.0.0
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

### Comparing `vsdeband-0.9.2/setup.cfg` & `vsdeband-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdeband-0.9.2/setup.py` & `vsdeband-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsdeband-0.9.2/vsdeband/f3kdb.py` & `vsdeband-1.0.0/vsdeband/f3kdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,34 +100,29 @@
 
 @dataclass
 class F3kdb(Debander):
     """Debander wrapper around the f3kdb plugin."""
 
     radius: int | None = None
     thr: int | list[int] | None = None
-    grains: int | list[int] | None = None
+    grain: int | list[int] | None = None
 
     sample_mode: SampleModeT | None = None
 
     seed: int | None = None
     dynamic_grain: int | None = None
 
     blur_first: bool | None = None
 
-    def __post_init__(self) -> None:
-        super().__post_init__()
-
-        self.config = Debander.SupportsConfig(True, True, False)
-
     @inject_self
     def deband(  # type: ignore[override]
         self, clip: vs.VideoNode,
         radius: int = 16,
         thr: int | list[int] = 96,
-        grains: int | list[int] = 0,
+        grain: float | list[float] = 0.0,
         sample_mode: SampleModeT = SampleMode.SQUARE,
         dynamic_grain: int | None = None,
         blur_first: bool | None = None,
         color_range: ColorRangeT | None = None,
         seed: int | None = None,
         planes: PlanesT = None,
         _func: FuncExceptT | None = None
@@ -139,15 +134,15 @@
 
         if 'y_2' not in core.neo_f3kdb.Deband.__signature__.parameters:  # type: ignore
             raise CustomRuntimeError('You are using an outdated version of neo_f3kdb, upgrade now!', func.func)
 
         radius = fallback(self.radius, radius)
 
         y, cb, cr = func.norm_seq(fallback(self.thr, thr))
-        gry, grc = normalize_seq(fallback(self.grains, grains), 2)
+        gry, grc = normalize_seq(fallback(self.grain, grain), 2)
 
         sample_mode = fallback(self.sample_mode, sample_mode)  # type: ignore
 
         color_range = ColorRange.from_param(
             color_range, self.deband
         ) or ColorRange.from_video(func.work_clip, func=func.func)
 
@@ -165,25 +160,14 @@
             y1, cb1, cr1 = func.norm_seq(sample_mode.thr_mid)
             y2, cb2, cr2 = func.norm_seq(sample_mode.thr_max)
             sample_mode = sample_mode.sample_mode
 
         blur_first = fallback(self.blur_first or blur_first, max(y, cb, cr) < 2048)  # type: ignore
 
         debanded = core.neo_f3kdb.Deband(
-            func.work_clip, radius, y, cb, cr, gry, grc,  # type: ignore
+            func.work_clip, radius, y, cb, cr, gry * 255 * 0.8, grc * 255 * 0.8,  # type: ignore
             sample_mode.value, self.seed or seed, blur_first, self.dynamic_grain or dynamic_grain,
             None, None, None, color_range.is_limited, 16, random_algo_ref, random_algo_ref,
             random_param_ref, random_param_grain, None, y1, cb1, cr1, y2, cb2, cr2, True
         )
 
         return func.return_clip(debanded)
-
-    @inject_self
-    def grain(  # type: ignore[override]
-        self, clip: vs.VideoNode, strength: int | tuple[int, int] = 4, dynamic: bool | int = True,
-        radius: int = 16, sample_mode: SampleMode = SampleMode.SQUARE,
-        color_range: ColorRangeT | None = None, seed: int | None = None, planes: PlanesT = None
-    ) -> vs.VideoNode:
-        return self.deband(
-            clip, radius, [1, 1, 1],
-            strength, sample_mode, dynamic, None, color_range, seed, planes  # type: ignore
-        )
```

### Comparing `vsdeband-0.9.2/vsdeband/filters.py` & `vsdeband-1.0.0/vsdeband/filters.py`

 * *Files identical despite different names*

### Comparing `vsdeband-0.9.2/vsdeband/funcs.py` & `vsdeband-1.0.0/vsdeband/funcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,29 +29,29 @@
 
     'guided_deband'
 ]
 
 
 def mdb_bilateral(
     clip: vs.VideoNode, radius: int = 16,
-    thr: int | list[int] = 260, grains: int | tuple[int, int] = 0,
+    thr: int | list[int] = 260, grain: float | tuple[float, float] = 0.0,
     lthr: int | tuple[int, int] = (153, 0), elast: float = 3.0,
     bright_thr: int | None = None,
     debander: type[Debander] | Debander = F3kdb
 ) -> vs.VideoNode:
     """
     Multi stage debanding, bilateral-esque filter.
 
     This function is more of a last resort for extreme banding.
     Recommend values are ~40-60 for luma and chroma strengths.
 
     :param clip:        Input clip.
     :param radius:      Banding detection range.
     :param thr:         Banding detection thr(s) for planes.
-    :param grains:      Specifies amount of grains added in the last debanding stage.
+    :param grain:       Specifies amount of grain added in the last debanding stage.
                         It happens after `vsrgtools.limit_filter`.
     :param lthr:        Threshold of the limiting. Refer to `vsrgtools.limit_filter`.
     :param elast:       Elasticity of the limiting. Refer to `vsrgtools.limit_filter`.
     :param bright_thr:  Limiting over the bright areas. Refer to `vsrgtools.limit_filter`.
     :param debander:    Specify what Debander to use. You can pass an instance with custom arguments.
 
     :return:            Debanded clip.
@@ -62,63 +62,63 @@
     if not isinstance(debander, Debander):
         debander = debander()
 
     clip, bits = expect_bits(clip, 16)
 
     rad1, rad2, rad3 = round(radius * 4 / 3), round(radius * 2 / 3), round(radius / 3)
 
-    db1 = debander.deband(clip, radius=rad1, thr=[max(1, th // 2) for th in to_arr(thr)], grains=0)
-    db2 = debander.deband(db1, radius=rad2, thr=thr, grains=0)
-    db3 = debander.deband(db2, radius=rad3, thr=thr, grains=0)
+    db1 = debander.deband(clip, radius=rad1, thr=[max(1, th // 2) for th in to_arr(thr)], grain=0.0)
+    db2 = debander.deband(db1, radius=rad2, thr=thr, grain=0)
+    db3 = debander.deband(db2, radius=rad3, thr=thr, grain=0)
 
     limit = limit_filter(db3, db2, clip, thr=lthr, elast=elast, bright_thr=bright_thr)
 
-    if grains:
-        limit = debander.grain(limit, strength=grains)
+    if grain:
+        limit = debander.grain(limit, strength=grain)
 
     return depth(limit, bits)
 
 
 def masked_deband(
     clip: vs.VideoNode, radius: int = 16,
-    thr: int | list[int] = 96, grains: int | list[int] = [12, 0],
+    thr: float | list[float] = 96, grain: float | list[float] = [0.23, 0],
     sigma: float = 1.25, rxsigma: list[int] = [50, 220, 300],
-    pf_sigma: float | None = 1.25, brz: tuple[int, int] = (2500, 4500),
+    pf_sigma: float | None = 1.25, brz: tuple[int, int] = (0.38, 0.68),
     rg_mode: RemoveGrainModeT = RemoveGrainMode.MINMAX_MEDIAN_OPP,
     debander: type[Debander] | Debander = F3kdb, **kwargs: Any
 ) -> vs.VideoNode:
     clip, bits = expect_bits(clip, 16)
 
     if not isinstance(debander, Debander):
         debander = debander()
 
     deband_mask = deband_detail_mask(clip, sigma, rxsigma, pf_sigma, brz, rg_mode)
 
-    deband = debander.deband(clip, radius=radius, thr=thr, grains=grains, **kwargs)
+    deband = debander.deband(clip, radius=radius, thr=thr, grain=grain, **kwargs)
 
     masked = deband.std.MaskedMerge(clip, deband_mask)
 
     return depth(masked, bits)
 
 
 def pfdeband(
     clip: vs.VideoNode, radius: int = 16,
-    thr: int | list[int] = 120, grains: int | list[int] = 0,
+    thr: float | list[float] = 120, grain: float | list[float] = 0.0,
     lthr: int | tuple[int, int] = (76, 0), elast: float = 2.5,
     bright_thr: int | None = None, scaler: ScalerT = Spline64,
     prefilter: Prefilter | VSFunction = partial(Prefilter.SCALEDBLUR, scale=1, radius=2),
     debander: type[Debander] | Debander = F3kdb, **kwargs: Any
 ) -> vs.VideoNode:
     """
     Prefilter and deband a clip.
 
     :param clip:        Input clip.
     :param radius:      Banding detection range.
     :param thr:         Banding detection thr(s) for planes.
-    :param grains:      Specifies amount of grains added in the last debanding stage.
+    :param grain:       Specifies amount of grain added in the last debanding stage.
                         It happens after `vsrgtools.limit_filter`.
     :param lthr:        Threshold of the limiting. Refer to `vsrgtools.limit_filter`.
     :param elast:       Elasticity of the limiting. Refer to `vsrgtools.limit_filter`.
     :param bright_thr:  Limiting over the bright areas. Refer to `vsrgtools.limit_filter`.
     :param prefilter:   Prefilter used to blur the clip before debanding.
     :param debander:    Specify what Debander to use. You can pass an instance with custom arguments.
 
@@ -133,15 +133,15 @@
     scaler = Scaler.ensure_obj(scaler, pfdeband)
 
     clip, bits = expect_bits(clip, 16)
 
     blur = prefilter(clip, **kwargs)
     change_res = (blur.width, blur.height) != (clip.width, clip.height)
 
-    deband = debander.deband(blur, radius=radius, thr=thr, grains=grains)
+    deband = debander.deband(blur, radius=radius, thr=thr, grain=grain)
 
     out = deband if change_res else clip
 
     diff = out.std.MakeDiff(blur)
 
     if change_res:
         diff = scaler.scale(diff, clip.width, clip.height)
```

### Comparing `vsdeband-0.9.2/vsdeband/mask.py` & `vsdeband-1.0.0/vsdeband/mask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from __future__ import annotations
 
-from vsexprtools import ExprOp, combine
-from vsmasktools import Morpho, retinex
+from vsexprtools import ExprOp
+from vsmasktools import Morpho, Prewitt, retinex
 from vsrgtools import RemoveGrainMode, RemoveGrainModeT, gauss_blur, removegrain
-from vstools import core, depth, expect_bits, get_y, iterate, vs
+from vstools import get_y, vs
 
 __all__ = [
     'deband_detail_mask'
 ]
 
 
 def deband_detail_mask(
-    clip: vs.VideoNode,
-    sigma: float = 1.0, rxsigma: list[int] = [50, 200, 350],
-    pf_sigma: float | None = 1.0, brz: tuple[int, int] = (2500, 4500),
+    clip: vs.VideoNode, sigma: float = 1.0, rxsigma: list[int] = [50, 200, 350],
+    pf_sigma: float | None = 1.0, brz: tuple[float, float] = (0.38, 0.68),
     rg_mode: RemoveGrainModeT = RemoveGrainMode.MINMAX_MEDIAN_OPP
 ) -> vs.VideoNode:
-    clip_y, bits = expect_bits(get_y(clip), 16)
+    clip_y = get_y(clip)
 
-    pf = gauss_blur(clip_y, pf_sigma) if pf_sigma else clip_y
-    ret = retinex(pf, rxsigma, upper_thr=0.005)
+    ret = retinex(
+        clip_y if pf_sigma is None else gauss_blur(clip_y, pf_sigma), rxsigma, upper_thr=0.005
+    )
+
+    brz0, brz1 = (br / 10 for br in brz)
 
     blur_ret = gauss_blur(ret, sigma)
-    blur_ret_diff = combine([blur_ret, ret], ExprOp.SUB).std.Deflate()
-    blur_ret_brz = iterate(blur_ret_diff, core.std.Inflate, 4)
-    blur_ret_brz = Morpho.closing(blur_ret_brz.std.Binarize(brz[0]), coords=8)
+    blur_ret_diff = Morpho.deflate(ExprOp.SUB(blur_ret, ret))
+
+    blur_ret_brz = Morpho.inflate(blur_ret_diff, 4)
+    blur_ret_brz = Morpho.closing(Morpho.binarize(blur_ret_brz, brz0), coords=8)
 
-    prewitt_mask = clip_y.std.Prewitt().std.Binarize(brz[1]).std.Deflate().std.Inflate()
-    prewitt_brz = Morpho.closing(prewitt_mask.std.Binarize(brz[1]), coords=4)
+    prewitt_mask = Morpho.inflate(Morpho.deflate(Prewitt.edgemask(clip_y, brz1, brz1)))
+    prewitt_brz = Morpho.closing(Morpho.binarize(prewitt_mask, brz1), coords=4)
 
-    merged = combine([blur_ret_brz, prewitt_brz], ExprOp.ADD)
-    rm_grain = removegrain(merged, rg_mode)
+    merged = ExprOp.ADD(blur_ret_brz, prewitt_brz)
 
-    return depth(rm_grain, bits)
+    return removegrain(merged, rg_mode)
```

### Comparing `vsdeband-0.9.2/vsdeband/placebo.py` & `vsdeband-1.0.0/vsdeband/placebo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any
 
-from vstools import (
-    CustomIntEnum, KwargsT, check_variable, fallback, inject_self, join, kwargs_fallback, normalize_seq, split, vs
-)
+from vstools import CustomIntEnum, KwargsT, check_variable, fallback, inject_self, join, normalize_seq, split, vs
 
 from .abstract import Debander
 
 __all__ = [
     'PlaceboDither',
     'Placebo'
 ]
@@ -26,15 +23,15 @@
     very slow, however this only needs to be performed once. Even so, using
     this with a `lut_size` greater than 6 is generally ill-advised. This is
     the preferred/default dither method.
     """
 
     DEFAULT = BLUE_NOISE
 
-    ORDERED_LU = 1
+    ORDERED_LUT = 1
     """
     Dither with an ordered (bayer) dither matrix, using a LUT. Low quality,
     and since this also uses a LUT, there's generally no advantage to picking
     this instead of `BLUE_NOISE`. It's mainly there for testing.
     """
 
     ORDERED_FIXED = 2
@@ -64,29 +61,24 @@
 
 @dataclass
 class Placebo(Debander):
     """Debander wrapper around libplacebo plugin's Deband function."""
 
     radius: float | None = None
     thr: float | list[float] | None = None
-    grains: float | list[float] | None = None
+    grain: float | list[float] | None = None
 
     iterations: int | None = None
 
     dither: PlaceboDither | None = None
 
-    def __post_init__(self) -> None:
-        super().__post_init__()
-
-        self.config = Debander.SupportsConfig(False, True, False)
-
     @inject_self
     def deband(  # type: ignore[override]
         self, clip: vs.VideoNode, radius: float = 16.0, thr: float | list[float] = 4.0,
-        iterations: int = 1, grains: float | list[float] = 6.0, dither: PlaceboDither = PlaceboDither.DEFAULT
+        iterations: int = 1, grain: float | list[float] = 0.0, dither: PlaceboDither = PlaceboDither.DEFAULT
     ) -> vs.VideoNode:
         """
         Main deband function, wrapper for `placebo.Deband <https:/github.com/Lypheo/vs-placebo#vs-placebo>`_
 
         :param clip:            Source clip
         :param radius:          The debanding filter's initial radius.
                                 The radius increases linearly for each iteration.
@@ -112,44 +104,19 @@
         """
 
         assert check_variable(clip, self.__class__.deband)
 
         radius = fallback(self.radius, radius)
         thr = normalize_seq(fallback(self.thr, thr))  # type: ignore[arg-type]
         iterations = fallback(self.iterations, iterations)
-        grains = normalize_seq(fallback(self.grains, grains))  # type: ignore[arg-type]
+        grain = normalize_seq(fallback(self.grain, grain))  # type: ignore[arg-type]
         dither = fallback(self.dither, dither)
 
         debs = [
-            p.placebo.Deband(1, iterations, thr, radius, gra, **dither.placebo_args)
-            for p, thr, gra in zip(split(clip), thr, grains)
+            p.placebo.Deband(1, iterations, thr, radius, gra * (1 << 5) * 0.8, **dither.placebo_args)
+            for p, thr, gra in zip(split(clip), thr, grain)
         ]
 
         if len(debs) == 1:
             return debs[0]
 
         return join(debs, clip.format.color_family)
-
-    @inject_self
-    def grain(  # type: ignore[override]
-        self, clip: vs.VideoNode, strength: float | tuple[int, int],
-        dynamic: bool | int = True, **kwargs: Any
-    ) -> vs.VideoNode:
-        """
-        Add Placebo grain to a clip.
-
-        :param clip:            Source clip
-        :param strength:        Strength of the grain per plane.
-        :param dynamic:         Graining mode. Static means no changes per frame, dynamic means changes every frame.
-
-        :return:                Grained clip
-        """
-        assert check_variable(clip, self.__class__.grain)
-
-        radius = kwargs_fallback(self.radius, (kwargs, 'radius'), 0)
-        thr = normalize_seq(kwargs_fallback(self.thr, (kwargs, 'thr'), 0))
-        grains = normalize_seq(strength)
-
-        if not dynamic:
-            raise NotImplementedError
-
-        return self.deband(clip, radius, thr, grains=grains, **kwargs)  # type: ignore
```

### Comparing `vsdeband-0.9.2/vsdeband.egg-info/PKG-INFO` & `vsdeband-1.0.0/vsdeband.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 0.9.2
+Version: 1.0.0
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

