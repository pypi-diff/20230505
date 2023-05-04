# Comparing `tmp/vsmasktools-0.9.3.tar.gz` & `tmp/vsmasktools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmasktools-0.9.3.tar", last modified: Sun Mar 26 17:38:58 2023, max compression
+gzip compressed data, was "vsmasktools-1.0.0.tar", last modified: Thu May  4 22:00:45 2023, max compression
```

## Comparing `vsmasktools-0.9.3.tar` & `vsmasktools-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/vsmasktools/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/vsmasktools/edge/
--rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/_2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/_3x3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/_5x5.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14311 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/edge_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/hardsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/morpho.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-03-26 17:38:37.000000 vsmasktools-0.9.3/vsmasktools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:58.091611 vsmasktools-0.9.3/vsmasktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-26 17:38:58.000000 vsmasktools-0.9.3/vsmasktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-26 17:38:58.000000 vsmasktools-0.9.3/vsmasktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:38:58.000000 vsmasktools-0.9.3/vsmasktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-26 17:38:58.000000 vsmasktools-0.9.3/vsmasktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-26 17:38:58.000000 vsmasktools-0.9.3/vsmasktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.262222 vsmasktools-1.0.0/vsmasktools/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/vsmasktools/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_3x3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_5x5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/hardsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/morpho.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/spat_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/vsmasktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/top_level.txt
```

### Comparing `vsmasktools-0.9.3/LICENSE` & `vsmasktools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/PKG-INFO` & `vsmasktools-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 0.9.3
+Version: 1.0.0
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-0.9.3/README.md` & `vsmasktools-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/setup.cfg` & `vsmasktools-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/setup.py` & `vsmasktools-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/abstract.py` & `vsmasktools-1.0.0/vsmasktools/abstract.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/details.py` & `vsmasktools-1.0.0/vsmasktools/details.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/diff.py` & `vsmasktools-1.0.0/vsmasktools/diff.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     mask = Morpho.expand(mask, 2 + expand, mode=XxpandMode.ELLIPSE).std.Deflate()
 
     return depth(mask, bits)
 
 
 def diff_creditless(
-    credit_clip: vs.VideoNode, nc_clip: vs.VideoNode, thr: float,
+    credit_clip: vs.VideoNode, nc_clip: vs.VideoNode, thr: float = 0.1,
     start_frame: int = 0, expand: int = 2, *, prefilter: bool | int = False,
     ep_clip: vs.VideoNode | None = None, func: FuncExceptT | None = None, **kwargs: Any
 ) -> vs.VideoNode:
     func = func or diff_creditless
 
     assert check_variable(credit_clip, func)
 
@@ -68,42 +68,42 @@
     diff_fmt = dst_fmt.replace(color_family=vs.GRAY)
 
     diff = ExprOp.mae(dst_fmt)(
         (Bicubic.resample(c, dst_fmt) for c in clips),
         format=diff_fmt, split_planes=True
     )
 
-    mask = Morpho.binarize(ExLaplacian4.edgemask(diff), thr)
+    mask = Morpho.binarize(ExLaplacian4.edgemask(diff), thr / 10)
     mask = Morpho.expand(mask, 2 + expand, mode=XxpandMode.ELLIPSE)
 
     if not ep_clip or ep_clip.num_frames == mask.num_frames:
         return mask
 
     blank = ep_clip.std.BlankClip(format=diff_fmt.id, keep=True)
 
     return insert_clip(blank, mask, start_frame)
 
 
 def diff_creditless_oped(
-    ep: vs.VideoNode, ncop: vs.VideoNode, nced: vs.VideoNode,
+    ep: vs.VideoNode, ncop: vs.VideoNode, nced: vs.VideoNode, thr: float = 0.1,
     opstart: int | None = None, opend: int | None = None,
     edstart: int | None = None, edend: int | None = None,
     func: FuncExceptT | None = None, **kwargs: Any
 ) -> vs.VideoNode:
     func = func or diff_creditless_oped
 
     op_mask = ed_mask = None
 
-    kwargs |= KwargsT(thr=25, expand=4, prefilter=False, func=func, ep_clip=ep) | kwargs
+    kwargs |= KwargsT(expand=4, prefilter=False, func=func, ep_clip=ep) | kwargs
 
     if opstart is not None and opend is not None:
-        op_mask = diff_creditless(ep[opstart:opend + 1], ncop[:opend - opstart + 1], opstart, **kwargs)
+        op_mask = diff_creditless(ep[opstart:opend + 1], ncop[:opend - opstart + 1], thr, opstart, **kwargs)
 
     if edstart is not None and edend is not None:
-        ed_mask = diff_creditless(ep[edstart:edend + 1], nced[:edend - edstart + 1], edstart, **kwargs)
+        ed_mask = diff_creditless(ep[edstart:edend + 1], nced[:edend - edstart + 1], thr, edstart, **kwargs)
 
     if op_mask and ed_mask:
         return ExprOp.ADD.combine(op_mask, ed_mask)
     elif op_mask or ed_mask:
         return op_mask or ed_mask  # type: ignore
 
     raise CustomValueError(
```

### Comparing `vsmasktools-0.9.3/vsmasktools/edge/_1d.py` & `vsmasktools-1.0.0/vsmasktools/edge/_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from abc import ABC
 from typing import Any, Sequence
 
 from vstools import ColorRange, depth, vs
 
-from ._abstract import EdgeDetect, EuclidianDistance
+from ._abstract import EdgeDetect, EuclideanDistance
 
 __all__ = [
     'Matrix1D',
     'TEdge', 'TEdgeTedgemask',
     #
     'SavitzkyGolay',
     #
@@ -119,15 +119,15 @@
 ]
 
 
 class Matrix1D(EdgeDetect, ABC):
     ...
 
 
-class TEdge(EuclidianDistance, Matrix1D):
+class TEdge(EuclideanDistance, Matrix1D):
     """(TEdgeMasktype=2) Avisynth plugin."""
 
     matrices = [
         [12, -74, 0, 74, -12],
         [-12, 74, 0, -74, 12]
     ]
     divisors = [62, 62]
@@ -137,24 +137,24 @@
 class TEdgeTedgemask(Matrix1D, EdgeDetect):
     """(tedgemask.TEdgeMask(threshold=0.0, type=2)) Vapoursynth plugin."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         return clip.tedgemask.TEdgeMask(threshold=0, type=2)  # type: ignore
 
 
-class SavitzkyGolay(EuclidianDistance, Matrix1D):
+class SavitzkyGolay(EuclideanDistance, Matrix1D):
     mode_types = ['h', 'v']
 
 
 class SavitzkyGolayNormalise(SavitzkyGolay):
     def _preprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
         return depth(clip, 32)
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
-        return depth(clip, self._bits, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
+        return depth(clip, input_bits, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
 
     def _get_matrices(self) -> Sequence[Sequence[float]]:
         assert self.divisors
         return [[c / div for c in mat] for mat, div in zip(self.matrices, self.divisors)]
 
     def _get_divisors(self) -> Sequence[float]:
         return [0.0] * len(self._get_matrices())
```

### Comparing `vsmasktools-0.9.3/vsmasktools/edge/_3x3.py` & `vsmasktools-1.0.0/vsmasktools/edge/_3x3.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 import math
 from abc import ABC
 from dataclasses import dataclass
 from typing import Any, NoReturn, Sequence
 
 from vsexprtools import ExprOp
-from vstools import ColorRange, depth, get_depth, join, split, vs
+from vstools import ColorRange, KwargsT, depth, get_depth, join, split, vs
 
 from ..morpho import Morpho
 from ..types import XxpandMode
-from ._abstract import EdgeDetect, EuclidianDistance, MatrixEdgeDetect, Max, RidgeDetect, SingleMatrix
+from ._abstract import EdgeDetect, EuclideanDistance, MagnitudeMatrix, MatrixEdgeDetect, Max, RidgeDetect, SingleMatrix
 
 __all__ = [
     'Matrix3x3',
     # Single matrix
     'Laplacian1', 'Laplacian2', 'Laplacian3', 'Laplacian4',
     'Kayyali',
-    # Euclidian Distance
+    # Euclidean Distance
     'Tritical', 'TriticalTCanny',
     'Cross',
     'Prewitt', 'PrewittStd', 'PrewittTCanny',
     'Sobel', 'SobelStd', 'SobelTCanny', 'ASobel',
     'Scharr', 'RScharr', 'ScharrTCanny',
     'Kroon', 'KroonTCanny',
     'FreyChenG41', 'FreyChen',
@@ -66,16 +66,16 @@
 
 class Kayyali(SingleMatrix, Matrix3x3):
     """Kayyali operator."""
 
     matrices = [[6, 0, -6, 0, 0, 0, -6, 0, 6]]
 
 
-# Euclidian Distance
-class Tritical(RidgeDetect, EuclidianDistance, Matrix3x3):
+# Euclidean Distance
+class Tritical(RidgeDetect, EuclideanDistance, Matrix3x3):
     """
     Operator used in Tritical's original TCanny filter.
     Plain and simple orthogonal first order derivative.
     """
 
     matrices = [
         [0, 0, 0, -1, 0, 1, 0, 0, 0],
@@ -86,30 +86,30 @@
 class TriticalTCanny(Matrix3x3, EdgeDetect):
     """
     Operator used in Tritical's original TCanny filter.
     Plain and simple orthogonal first order derivative.
     """
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=0, **kwargs)
+        return clip.tcanny.TCanny(op=0, **(KwargsT(sigma=0, mode=1) | kwargs))
 
 
-class Cross(RidgeDetect, EuclidianDistance, Matrix3x3):
+class Cross(RidgeDetect, EuclideanDistance, Matrix3x3):
     """
     "HotDoG" Operator from AVS ExTools by Dogway.
     Plain and simple cross first order derivative.
     """
 
     matrices = [
         [1, 0, 0, 0, 0, 0, 0, 0, -1],
         [0, 0, -1, 0, 0, 0, 1, 0, 0]
     ]
 
 
-class Prewitt(RidgeDetect, EuclidianDistance, Matrix3x3):
+class Prewitt(RidgeDetect, EuclideanDistance, Matrix3x3):
     """Judith M. S. Prewitt operator."""
 
     matrices = [
         [1, 0, -1, 1, 0, -1, 1, 0, -1],
         [1, 1, 1, 0, 0, 0, -1, -1, -1]
     ]
 
@@ -121,18 +121,18 @@
         return clip.std.Prewitt(**kwargs)
 
 
 class PrewittTCanny(Matrix3x3, EdgeDetect):
     """Judith M. S. Prewitt TCanny plugin operator."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=1, scale=2, **kwargs)
+        return clip.tcanny.TCanny(op=1, **(KwargsT(sigma=0, mode=1, scale=2) | kwargs))
 
 
-class Sobel(RidgeDetect, EuclidianDistance, Matrix3x3):
+class Sobel(RidgeDetect, EuclideanDistance, Matrix3x3):
     """Sobel–Feldman operator."""
 
     matrices = [
         [1, 0, -1, 2, 0, -2, 1, 0, -1],
         [1, 2, 1, 0, 0, 0, -1, -2, -1]
     ]
 
@@ -144,40 +144,40 @@
         return clip.std.Sobel(**kwargs)
 
 
 class SobelTCanny(Matrix3x3, EdgeDetect):
     """Sobel–Feldman Vapoursynth plugin operator."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=2, scale=2, **kwargs)
+        return clip.tcanny.TCanny(op=2, **(KwargsT(sigma=0, mode=1, scale=2) | kwargs))
 
 
 class ASobel(Matrix3x3, EdgeDetect):
     """Modified Sobel–Feldman operator from AWarpSharp."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         return (vs.core.warp.ASobel if get_depth(clip) < 32 else vs.core.warpsf.ASobel)(  # type: ignore
             clip, 255, **kwargs
         )
 
 
-class Scharr(RidgeDetect, EuclidianDistance, Matrix3x3):
+class Scharr(RidgeDetect, EuclideanDistance, Matrix3x3):
     """
     Original H. Scharr optimised operator which attempts
     to achieve the perfect rotational symmetry with coefficients 3 and 10.
     """
 
     matrices = [
         [-3, 0, 3, -10, 0, 10, -3, 0, 3],
         [-3, -10, -3, 0, 0, 0, 3, 10, 3]
     ]
     divisors = [3, 3]
 
 
-class RScharr(RidgeDetect, EuclidianDistance, Matrix3x3):
+class RScharr(RidgeDetect, EuclideanDistance, Matrix3x3):
     """
     Refined H. Scharr operator to more accurately calculate
     1st derivatives for a 3x3 kernel with coeffs 47 and 162.
     """
 
     matrices = [
         [-47, 0, 47, -162, 0, 162, -47, 0, 47],
@@ -186,32 +186,32 @@
     divisors = [47, 47]
 
 
 class ScharrTCanny(Matrix3x3, EdgeDetect):
     """H. Scharr optimised TCanny Vapoursynth plugin operator."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=2, scale=4 / 3, **kwargs)
+        return clip.tcanny.TCanny(op=2, **(KwargsT(sigma=0, mode=1, scale=4 / 3) | kwargs))  # type: ignore
 
 
-class Kroon(RidgeDetect, EuclidianDistance, Matrix3x3):
+class Kroon(RidgeDetect, EuclideanDistance, Matrix3x3):
     """Dirk-Jan Kroon operator."""
 
     matrices = [
         [-17, 0, 17, -61, 0, 61, -17, 0, 17],
         [-17, -61, -17, 0, 0, 0, 17, 61, 17]
     ]
     divisors = [17, 17]
 
 
 class KroonTCanny(Matrix3x3, EdgeDetect):
     """Dirk-Jan Kroon TCanny Vapoursynth plugin operator."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=4, scale=1 / 17, **kwargs)
+        return clip.tcanny.TCanny(op=4, **(KwargsT(mode=1, scale=1 / 17) | kwargs))  # type: ignore
 
 
 class FreyChen(MatrixEdgeDetect):
     """Chen Frei operator. 3x3 matrices properly implemented."""
 
     sqrt2 = math.sqrt(2)
     matrices = [
@@ -236,27 +236,27 @@
         6,
         3
     ]
 
     def _preprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
         return depth(clip, 32)
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
-        return depth(clip, self._bits, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
+        return depth(clip, input_bits, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
 
     def _merge_edge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode:
         M = 'x x * y y * + z z * + a a * +'
         S = f'b b * c c * + d d * + e e * + f f * + {M} +'
         return vs.core.std.Expr(clips, f'{M} {S} / sqrt')
 
     def _merge_ridge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode | NoReturn:
         raise NotImplementedError
 
 
-class FreyChenG41(RidgeDetect, EuclidianDistance, Matrix3x3):
+class FreyChenG41(RidgeDetect, EuclideanDistance, Matrix3x3):
     """"Chen Frei" operator. 3x3 matrices from G41Fun."""
 
     matrices = [
         [-7, 0, 7, -10, 0, 10, -7, 0, 7],
         [-7, -10, -7, 0, 0, 0, 7, 10, 7]
     ]
     divisors = [7, 7]
@@ -293,34 +293,34 @@
         [10, 5, 0, 5, 0, -5, 0, -5, -10],
         [5, 0, -5, 10, 0, -10, 5, 0, -5],
         [0, -5, -10, 5, 0, -5, 10, 5, 0]
     ]
     divisors = [4] * 4
 
 
-class Kirsch(Max, Matrix3x3):
+class Kirsch(MagnitudeMatrix, Max, Matrix3x3):
     """Russell Kirsch compass operator."""
 
     matrices = [
-        [5, 5, 5, -3, 0, -3, -3, -3, -3],
-        [5, 5, -3, 5, 0, -3, -3, -3, -3],
-        [5, -3, -3, 5, 0, -3, 5, -3, -3],
-        [-3, -3, -3, 5, 0, -3, 5, 5, -3],
-        [-3, -3, -3, -3, 0, -3, 5, 5, 5],
-        [-3, -3, -3, -3, 0, 5, -3, 5, 5],
-        [-3, -3, 5, -3, 0, 5, -3, -3, 5],
-        [-3, 5, 5, -3, 0, 5, -3, -3, -3]
+        [5, 5, 5, -3, 0, -3, -3, -3, -3],  # N
+        [5, 5, -3, 5, 0, -3, -3, -3, -3],  # NW
+        [5, -3, -3, 5, 0, -3, 5, -3, -3],  # W
+        [-3, -3, -3, 5, 0, -3, 5, 5, -3],  # SW
+        [-3, -3, -3, -3, 0, -3, 5, 5, 5],  # S
+        [-3, -3, -3, -3, 0, 5, -3, 5, 5],  # SE
+        [-3, -3, 5, -3, 0, 5, -3, -3, 5],  # E
+        [-3, 5, 5, -3, 0, 5, -3, -3, -3],  # NE
     ]
 
 
 class KirschTCanny(Matrix3x3, EdgeDetect):
     """Russell Kirsch compass TCanny Vapoursynth plugin operator."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
-        return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=5, **kwargs)
+        return clip.tcanny.TCanny(op=5, **(KwargsT(sigma=0, mode=1) | kwargs))
 
 
 # Misc
 @dataclass
 class MinMax(EdgeDetect):
     """Min/max mask with separate luma/chroma radii."""
```

### Comparing `vsmasktools-0.9.3/vsmasktools/edge/_5x5.py` & `vsmasktools-1.0.0/vsmasktools/edge/_5x5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from abc import ABC
 from typing import Any, Sequence
 
 from vstools import ColorRange, depth, vs
 
-from ._abstract import EdgeDetect, EuclidianDistance, Max, RidgeDetect, SingleMatrix
+from ._abstract import EdgeDetect, EuclideanDistance, Max, RidgeDetect, SingleMatrix
 
 __all__ = [
     'Matrix5x5',
     # Single matrix
     'ExLaplacian1', 'ExLaplacian2', 'ExLaplacian3', 'ExLaplacian4',
     'LoG',
-    # Euclidian distance
+    # Euclidean distance
     'ExPrewitt',
     'ExSobel',
     'FDoG', 'FDoGTCanny',
     'DoG',
     'Farid',
     # Max
     'ExKirsch'
@@ -54,34 +54,34 @@
 
 class LoG(SingleMatrix, Matrix5x5):
     """Laplacian of Gaussian operator."""
 
     matrices = [[0, 0, -1, 0, 0, 0, -1, -2, -1, 0, -1, -2, 16, -2, -1, 0, -1, -2, -1, 0, 0, 0, -1, 0, 0]]
 
 
-# Euclidian distance
-class ExPrewitt(RidgeDetect, EuclidianDistance, Matrix5x5):
+# Euclidean distance
+class ExPrewitt(RidgeDetect, EuclideanDistance, Matrix5x5):
     """Extended Judith M. S. Prewitt operator."""
 
     matrices = [
         [2, 1, 0, -1, -2, 2, 1, 0, -1, -2, 2, 1, 0, -1, -2, 2, 1, 0, -1, -2, 2, 1, 0, -1, -2],
         [2, 2, 2, 2, 2, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, -1, -1, -1, -1, -1, -2, -2, -2, -2, -2]
     ]
 
 
-class ExSobel(RidgeDetect, EuclidianDistance, Matrix5x5):
+class ExSobel(RidgeDetect, EuclideanDistance, Matrix5x5):
     """Extended Sobel–Feldman operator."""
 
     matrices = [
         [2, 1, 0, -1, -2, 2, 1, 0, -1, -2, 4, 2, 0, -2, -4, 2, 1, 0, -1, -2, 2, 1, 0, -1, -2],
         [2, 2, 4, 2, 2, 1, 1, 2, 1, 1, 0, 0, 0, 0, 0, -1, -1, -2, -1, -1, -2, -2, -4, -2, -2]
     ]
 
 
-class FDoG(RidgeDetect, EuclidianDistance, Matrix5x5):
+class FDoG(RidgeDetect, EuclideanDistance, Matrix5x5):
     """Flow-based Difference of Gaussian"""
 
     matrices = [
         [1, 1, 0, -1, -1, 2, 2, 0, -2, -2, 3, 3, 0, -3, -3, 2, 2, 0, -2, -2, 1, 1, 0, -1, -1],
         [1, 2, 3, 2, 1, 1, 2, 3, 2, 1, 0, 0, 0, 0, 0, -1, -2, -3, -2, -1, -1, -2, -3, -2, -1]
     ]
     divisors = [2, 2]
@@ -90,34 +90,34 @@
 class FDoGTCanny(Matrix5x5, EdgeDetect):
     """Flow-based Difference of Gaussian TCanny Vapoursynth plugin."""
 
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         return clip.tcanny.TCanny(kwargs.pop('sigma', 0), mode=1, op=6, scale=0.5, **kwargs)
 
 
-class DoG(EuclidianDistance, Matrix5x5):
+class DoG(EuclideanDistance, Matrix5x5):
     """Zero-cross (of the 2nd derivative) of a Difference of Gaussians"""
 
     matrices = [
         [0, 0, 5, 0, 0, 0, 5, 10, 5, 0, 5, 10, 20, 10, 5, 0, 5, 10, 5, 0, 0, 0, 5, 0, 0],
         [0, 25, 0, 25, 50, 25, 0, 25, 0],
     ]
     divisors = [4, 6]
 
     def _preprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
         return depth(clip, 32)
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
-        return depth(clip, self._bits, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
+        return depth(clip, input_bits, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
 
     def _merge_edge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode:
         return vs.core.std.Expr(clips, 'x y -')
 
 
-class Farid(RidgeDetect, EuclidianDistance, Matrix5x5):
+class Farid(RidgeDetect, EuclideanDistance, Matrix5x5):
     """Farid & Simoncelli operator."""
 
     matrices = [[
         0.004127602875174862, 0.027308149775363867, 0.04673225765917656, 0.027308149775363867, 0.004127602875174862,
         0.010419993699470744, 0.06893849946536831, 0.11797400212587895, 0.06893849946536831, 0.010419993699470744,
         0.0, 0.0, 0.0, 0.0, 0.0,
         -0.010419993699470744, -0.06893849946536831, -0.11797400212587895, -0.06893849946536831, -0.010419993699470744,
@@ -129,16 +129,16 @@
         -0.010419993699470744, -0.06893849946536831, -0.11797400212587895, -0.06893849946536831, -0.010419993699470744,
         -0.004127602875174862, -0.027308149775363867, -0.04673225765917656, -0.027308149775363867, -0.004127602875174862
     ]]
 
     def _preprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
         return depth(clip, 32)
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
-        return depth(clip, self._bits, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
+        return depth(clip, input_bits, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
 
 
 # Max
 class ExKirsch(Max):
     """Extended Russell Kirsch compass operator. 5x5 matrices."""
 
     matrices = [
```

### Comparing `vsmasktools-0.9.3/vsmasktools/edge/_abstract.py` & `vsmasktools-1.0.0/vsmasktools/edge/_abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,76 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from enum import Enum, auto
+from enum import Enum, IntFlag, auto
 from typing import Any, ClassVar, NoReturn, Sequence, TypeAlias
 
 from vsexprtools import ExprOp, ExprToken, norm_expr
 from vstools import (
     ColorRange, CustomRuntimeError, CustomValueError, FuncExceptT, PlanesT, T, check_variable, core, get_lowest_values,
-    get_peak_value, get_peak_values, get_subclasses, inject_self, join, normalize_planes, plane, vs
+    get_peak_value, get_peak_values, get_subclasses, inject_self, join, normalize_planes, plane, scale_value, vs
 )
 
 from ..exceptions import UnknownEdgeDetectError, UnknownRidgeDetectError
 
 __all__ = [
     'EdgeDetect', 'EdgeDetectT',
     'RidgeDetect', 'RidgeDetectT',
 
-    'MatrixEdgeDetect', 'SingleMatrix', 'EuclidianDistance',
+    'MatrixEdgeDetect', 'SingleMatrix', 'EuclideanDistance', 'MagnitudeMatrix',
 
     'Max',
 
+    'MagDirection',
+
     'get_all_edge_detects',
     'get_all_ridge_detect',
 ]
 
 
 class _Feature(Enum):
     EDGE = auto()
     RIDGE = auto()
 
 
+class MagDirection(IntFlag):
+    """Direction of magnitude calculation."""
+
+    N = auto()
+    NW = auto()
+    W = auto()
+    SW = auto()
+    S = auto()
+    SE = auto()
+    E = auto()
+    NE = auto()
+
+    ALL = N | NW | W | SW | S | SE | E | NE
+
+    AXIS = N | W | S | E
+    CORNERS = NW | SW | SE | NE
+
+    NORTH = N | NW | NE
+    WEAST = W | NW | SW
+    EAST = E | NE | SE
+    SOUTH = S | SW | SE
+
+    def select_matrices(self, matrices: Sequence[T]) -> Sequence[T]:
+        # In Python <3.11, composite flags are included in MagDirection's
+        # collection and iteration interfaces.
+        primary_flags = [
+            flag for flag in MagDirection if flag != 0 and flag & (flag - 1) == 0
+        ]
+        assert len(matrices) == len(primary_flags) and self
+
+        return [
+            matrix for flag, matrix in zip(primary_flags, matrices) if self & flag
+        ]
+
+
 class BaseDetect:
     @staticmethod
     def from_param(
         cls: type[T],
         value: str | type[T] | T | None,
         exception_cls: type[CustomValueError],
         excluded: Sequence[type[T]] = [],
@@ -87,15 +124,18 @@
 
         return new_edge_detect
 
 
 class EdgeDetect(ABC):
     """Abstract edge detection interface."""
 
-    _bits: int
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__()
+
+        self.kwargs = kwargs
 
     @classmethod
     def from_param(
         cls: type[EdgeDetect], edge_detect: EdgeDetectT | None = None, func_except: FuncExceptT | None = None
     ) -> type[EdgeDetect]:
         return BaseDetect.from_param(cls, edge_detect, UnknownEdgeDetectError, [], func_except)
 
@@ -104,16 +144,16 @@
         cls: type[EdgeDetect], edge_detect: EdgeDetectT | None = None, func_except: FuncExceptT | None = None
     ) -> EdgeDetect:
         return BaseDetect.ensure_obj(cls, edge_detect, UnknownEdgeDetectError, [], func_except)
 
     @inject_self
     def edgemask(
         self, clip: vs.VideoNode, lthr: float = 0.0, hthr: float | None = None, multi: float = 1.0,
-        clamp: bool | tuple[float, float] | list[tuple[float, float]] = False, planes: PlanesT = None,
-        **kwargs: Any
+        clamp: bool | tuple[float, float] | list[tuple[float, float]] = False,
+        planes: PlanesT | tuple[PlanesT, bool] = None, **kwargs: Any
     ) -> vs.VideoNode:
         """
         Makes edge mask based on convolution kernel.
         The resulting mask can be thresholded with lthr, hthr and multiplied with multi.
 
         :param clip:            Source clip
         :param lthr:            Low threshold. Anything below lthr will be set to 0
@@ -127,23 +167,30 @@
 
     def _mask(
         self,
         clip: vs.VideoNode,
         lthr: float = 0.0, hthr: float | None = None,
         multi: float = 1.0,
         clamp: bool | tuple[float, float] | list[tuple[float, float]] = False,
-        feature: _Feature = _Feature.EDGE, planes: PlanesT = None, **kwargs: Any
+        feature: _Feature = _Feature.EDGE, planes: PlanesT | tuple[PlanesT, bool] = None, **kwargs: Any
     ) -> vs.VideoNode:
         assert check_variable(clip, self.__class__)
 
-        self._bits = clip.format.bits_per_sample
+        kwargs = self.kwargs | kwargs
+
         peak = get_peak_value(clip)
-        hthr = peak if hthr is None else hthr
+        hthr = 1.0 if hthr is None else hthr
+
+        lthr, hthr = scale_value(lthr, 32, clip), scale_value(hthr, 32, clip)
 
-        planes = normalize_planes(clip, planes)
+        discard_planes = False
+        if isinstance(planes, tuple):
+            planes, discard_planes = planes
+
+        planes = normalize_planes(clip, planes)  # type: ignore
 
         wclip = plane(clip, planes[0]) if len(planes) == 1 else clip
 
         clip_p = self._preprocess(wclip)
 
         try:
             if feature == _Feature.EDGE:
@@ -151,20 +198,22 @@
             elif feature == _Feature.RIDGE:
                 if not isinstance(self, RidgeDetect):
                     raise RuntimeError
                 mask = self._compute_ridge_mask(clip_p, **kwargs)
         except Exception as e:
             raise CustomRuntimeError('There was an error processing the mask! Are you using an abstract class?') from e
 
-        mask = self._postprocess(mask)
+        mask = self._postprocess(mask, clip.format.bits_per_sample)
 
         if multi != 1:
             mask = ExprOp.MUL(mask, suffix=str(multi), planes=planes)
 
-        if lthr > 0 and hthr < peak:
+        if lthr == hthr:
+            mask = norm_expr(mask, f'x {hthr} >= {ExprToken.RangeMax} 0 ?', planes)
+        elif lthr > 0 and hthr < peak:
             mask = norm_expr(mask, f'x {hthr} > {ExprToken.RangeMax} x {lthr} < 0 x ? ?', planes)
         elif lthr > 0:
             mask = norm_expr(mask, f'x {lthr} < 0 x ?', planes)
         elif hthr < peak:
             mask = norm_expr(mask, f'x {hthr} > {ExprToken.RangeMax} x ?', planes)
 
         if clamp:
@@ -175,27 +224,27 @@
             if isinstance(clamp, list):
                 mask = norm_expr(mask, [ExprOp.clamp(*c, c='x') for c in clamp], planes)
             elif isinstance(clamp, tuple):
                 mask = ExprOp.clamp(*clamp, c='x')(mask, planes=planes)
 
         assert mask.format
 
-        if mask.format.num_planes != clip.format.num_planes:
+        if mask.format.num_planes != clip.format.num_planes and not discard_planes:
             return join({None: clip.std.BlankClip(color=[0] * clip.format.num_planes, keep=True), planes[0]: mask})
 
         return mask
 
     @abstractmethod
     def _compute_edge_mask(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         raise NotImplementedError
 
     def _preprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
         return clip
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
         return clip
 
 
 class MatrixEdgeDetect(EdgeDetect):
     matrices: ClassVar[Sequence[Sequence[float]]]
     divisors: ClassVar[Sequence[float] | None] = None
     mode_types: ClassVar[Sequence[str] | None] = None
@@ -233,22 +282,32 @@
 
     def _get_divisors(self) -> Sequence[float]:
         return self.divisors if self.divisors else [0.0] * len(self._get_matrices())
 
     def _get_mode_types(self) -> Sequence[str]:
         return self.mode_types if self.mode_types else ['s'] * len(self._get_matrices())
 
-    def _postprocess(self, clip: vs.VideoNode) -> vs.VideoNode:
+    def _postprocess(self, clip: vs.VideoNode, input_bits: int) -> vs.VideoNode:
         if len(self.matrices[0]) > 9 or (self.mode_types and self.mode_types[0] != 's'):
             clip = clip.std.Crop(
                 right=clip.format.subsampling_w * 2 if clip.format and clip.format.subsampling_w != 0 else 2
             ).resize.Point(clip.width, src_width=clip.width)
         return clip
 
 
+class MagnitudeMatrix(MatrixEdgeDetect):
+    def __init__(self, mag_directions: MagDirection = MagDirection.ALL, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+
+        self.mag_directions = mag_directions
+
+    def _get_matrices(self) -> Sequence[Sequence[float]]:
+        return self.mag_directions.select_matrices(self.matrices)
+
+
 class RidgeDetect(MatrixEdgeDetect):
     @classmethod
     def from_param(  # type: ignore
         cls: type[RidgeDetect], edge_detect: RidgeDetectT | None = None, func_except: FuncExceptT | None = None
     ) -> type[RidgeDetect]:
         return BaseDetect.from_param(cls, edge_detect, UnknownRidgeDetectError, [], func_except)
 
@@ -257,43 +316,44 @@
         cls: type[RidgeDetect], edge_detect: RidgeDetectT | None = None, func_except: FuncExceptT | None = None
     ) -> RidgeDetect:
         return BaseDetect.ensure_obj(cls, edge_detect, UnknownRidgeDetectError, [], func_except)
 
     @inject_self
     def ridgemask(
         self, clip: vs.VideoNode, lthr: float = 0.0, hthr: float | None = None, multi: float = 1.0,
-        clamp: bool | tuple[float, float] | list[tuple[float, float]] = False, **kwargs: Any
+        clamp: bool | tuple[float, float] | list[tuple[float, float]] = False,
+        planes: PlanesT | tuple[PlanesT, bool] = None, **kwargs: Any
     ) -> vs.VideoNode | NoReturn:
         """
         Makes ridge mask based on convolution kernel.
         The resulting mask can be thresholded with lthr, hthr and multiplied with multi.
 
         :param clip:            Source clip
         :param lthr:            Low threshold. Anything below lthr will be set to 0
         :param hthr:            High threshold. Anything above hthr will be set to the range max
         :param multi:           Multiply all pixels by this before thresholding
         :param clamp:           Clamp to TV or full range if True or specified range `(low, high)`
 
         :return:                Mask clip
         """
-        return self._mask(clip, lthr, hthr, multi, clamp, _Feature.RIDGE, **kwargs)
+        return self._mask(clip, lthr, hthr, multi, clamp, _Feature.RIDGE, planes, **kwargs)
 
     def _merge_ridge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode:
         return core.std.Expr(clips, 'x y * 2 * -1 * x dup * z dup * 4 * + y dup * + + sqrt x y + +')
 
 
 class SingleMatrix(MatrixEdgeDetect, ABC):
     def _merge_edge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode:
         return clips[0]
 
     def _merge_ridge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode | NoReturn:
         raise NotImplementedError
 
 
-class EuclidianDistance(MatrixEdgeDetect, ABC):
+class EuclideanDistance(MatrixEdgeDetect, ABC):
     def _merge_edge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode:
         return core.std.Expr(clips, 'x x * y y * + sqrt')
 
     def _merge_ridge(self, clips: Sequence[vs.VideoNode]) -> vs.VideoNode | NoReturn:
         raise NotImplementedError
 
 
@@ -328,15 +388,15 @@
     """
     def _all_subclasses(cls: type[EdgeDetect] = EdgeDetect) -> set[type[EdgeDetect]]:
         return set(cls.__subclasses__()).union(s for c in cls.__subclasses__() for s in _all_subclasses(c))
 
     all_subclasses = {
         s for s in _all_subclasses()
         if s.__name__ not in {
-            'MatrixEdgeDetect', 'RidgeDetect', 'SingleMatrix', 'EuclidianDistance', 'Max',
+            'MatrixEdgeDetect', 'RidgeDetect', 'SingleMatrix', 'EuclideanDistance', 'Max',
             'Matrix1D', 'SavitzkyGolay', 'SavitzkyGolayNormalise',
             'Matrix2x2', 'Matrix3x3', 'Matrix5x5'
         }
     }
     return [
         edge_detect().edgemask(clip, lthr, hthr, multi, clamp).text.Text(edge_detect.__name__)
         for edge_detect in sorted(all_subclasses, key=lambda x: x.__name__)
@@ -360,15 +420,15 @@
     """
     def _all_subclasses(cls: type[RidgeDetect] = RidgeDetect) -> set[type[RidgeDetect]]:
         return set(cls.__subclasses__()).union(s for c in cls.__subclasses__() for s in _all_subclasses(c))
 
     all_subclasses = {
         s for s in _all_subclasses()
         if s.__name__ not in {
-            'MatrixEdgeDetect', 'RidgeDetect', 'SingleMatrix', 'EuclidianDistance', 'Max',
+            'MatrixEdgeDetect', 'RidgeDetect', 'SingleMatrix', 'EuclideanDistance', 'Max',
             'Matrix1D', 'SavitzkyGolay', 'SavitzkyGolayNormalise',
             'Matrix2x2', 'Matrix3x3', 'Matrix5x5'
         }
     }
     return [
         edge_detect().ridgemask(clip, lthr, hthr, multi, clamp).text.Text(edge_detect.__name__)
         for edge_detect in sorted(all_subclasses, key=lambda x: x.__name__)
```

### Comparing `vsmasktools-0.9.3/vsmasktools/edge_funcs.py` & `vsmasktools-1.0.0/vsmasktools/edge_funcs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from __future__ import annotations
 
 from functools import partial
-from typing import Any, Sequence
+from typing import Any, Literal, Sequence, cast, overload
 
 from vsexprtools import ExprOp, ExprToken, norm_expr
 from vsrgtools import gauss_blur
 from vsrgtools.util import wmean_matrix
-from vstools import check_variable, core, get_peak_value, get_y, iterate, plane, scale_value, vs
+from vstools import (
+    ColorRange, CustomEnum, VSFunctionAllArgs, check_variable, core, depth, get_peak_value, get_y, iterate, plane,
+    scale_value, vs
+)
 
 from .details import multi_detail_mask
-from .edge import FDoGTCanny, Kirsch, Prewitt
-from .funcs import retinex
+from .edge import FDoGTCanny, Kirsch, MagDirection, Prewitt, PrewittTCanny
 from .morpho import Morpho
+from .spat_funcs import retinex
 from .types import Coordinates, GenericMaskT
 from .utils import normalize_mask
 
 __all__ = [
     'ringing_mask',
 
     'luma_mask', 'luma_credit_mask',
 
     'tcanny_retinex',
 
-    'limited_linemask'
+    'limited_linemask',
+
+    'dre_edgemask'
 ]
 
 
 def ringing_mask(
     clip: vs.VideoNode,
     rad: int = 2, brz: float = 0.35,
     thmi: float = 0.315, thma: float = 0.5,
@@ -108,7 +113,61 @@
     clip_y = plane(clip, 0)
 
     return ExprOp.ADD(
         (normalize_mask(edge, clip_y, **kwargs) for edge in edgemasks),
         (tcanny_retinex(clip_y, s) for s in sigmas),
         (multi_detail_mask(clip_y, s) for s in detail_sigmas)
     )
+
+
+class _dre_edgemask(CustomEnum):
+    """Edgemask with dynamic range enhancement prefiltering."""
+
+    RETINEX = cast(VSFunctionAllArgs, object())
+    CLAHE = cast(VSFunctionAllArgs, object())
+
+    def _prefilter(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
+        if self is self.RETINEX:  # type: ignore
+            sigmas = kwargs.get('sigmas', [50, 200, 350])
+
+            return retinex(clip, sigmas, 0.001, 0.005)
+
+        if self is self.CLAHE:  # type: ignore
+            limit, tile = kwargs.get('limit', 0.305), kwargs.get('tile', 5)
+
+            return depth(depth(clip, 16).ehist.CLAHE(scale_value(limit / 10, 32, 16), tile), clip)
+
+        return clip
+
+    @overload
+    def __call__(  # type: ignore
+        self: Literal[RETINEX], src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122,
+        *, sigmas: Sequence[float] = [50, 200, 350]
+    ) -> vs.VideoNode:
+        ...
+
+    @overload
+    def __call__(  # type: ignore
+        self: Literal[CLAHE], src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122,
+        *, limit: float = 0.305, tile: int = 5
+    ) -> vs.VideoNode:
+        ...
+
+    def __call__(self, src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122, **kwargs: Any) -> vs.VideoNode:
+        luma = get_y(src)
+
+        dreluma = self._prefilter(luma, **kwargs)
+
+        tcanny = PrewittTCanny.edgemask(dreluma, sigma=tsigma, scale=1)
+        tcanny = Morpho.minimum(tcanny, coords=Coordinates.CORNERS)
+
+        kirsch = Kirsch(MagDirection.N | MagDirection.EAST).edgemask(luma)
+
+        add_clip = ExprOp.ADD(tcanny, kirsch)
+
+        if brz > 0:
+            add_clip = Morpho.binarize(add_clip, brz)
+
+        return ColorRange.FULL.apply(add_clip)
+
+
+dre_edgemask = _dre_edgemask.RETINEX
```

### Comparing `vsmasktools-0.9.3/vsmasktools/exceptions.py` & `vsmasktools-1.0.0/vsmasktools/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/hardsub.py` & `vsmasktools-1.0.0/vsmasktools/hardsub.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/masks.py` & `vsmasktools-1.0.0/vsmasktools/masks.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/morpho.py` & `vsmasktools-1.0.0/vsmasktools/morpho.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/types.py` & `vsmasktools-1.0.0/vsmasktools/types.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools/utils.py` & `vsmasktools-1.0.0/vsmasktools/utils.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-0.9.3/vsmasktools.egg-info/PKG-INFO` & `vsmasktools-1.0.0/vsmasktools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 0.9.3
+Version: 1.0.0
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-0.9.3/vsmasktools.egg-info/SOURCES.txt` & `vsmasktools-1.0.0/vsmasktools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 vsmasktools/__init__.py
 vsmasktools/_metadata.py
 vsmasktools/abstract.py
 vsmasktools/details.py
 vsmasktools/diff.py
 vsmasktools/edge_funcs.py
 vsmasktools/exceptions.py
-vsmasktools/funcs.py
 vsmasktools/hardsub.py
 vsmasktools/masks.py
 vsmasktools/morpho.py
 vsmasktools/py.typed
+vsmasktools/spat_funcs.py
 vsmasktools/types.py
 vsmasktools/utils.py
 vsmasktools.egg-info/PKG-INFO
 vsmasktools.egg-info/SOURCES.txt
 vsmasktools.egg-info/dependency_links.txt
 vsmasktools.egg-info/requires.txt
 vsmasktools.egg-info/top_level.txt
```

