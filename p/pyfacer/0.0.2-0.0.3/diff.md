# Comparing `tmp/pyfacer-0.0.2-py3-none-any.whl.zip` & `tmp/pyfacer-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,30 @@
-Zip file size: 35342 bytes, number of entries: 29
+Zip file size: 33942 bytes, number of entries: 28
 -rw-r--r--  2.0 unx     1675 b- defN 23-May-04 10:32 facer/__init__.py
 -rw-r--r--  2.0 unx     7246 b- defN 23-May-04 10:46 facer/draw.py
 -rw-r--r--  2.0 unx      545 b- defN 23-Apr-27 08:30 facer/io.py
 -rw-r--r--  2.0 unx      962 b- defN 23-Apr-27 08:30 facer/show.py
 -rw-r--r--  2.0 unx    13358 b- defN 23-Apr-28 02:01 facer/transform.py
 -rw-r--r--  2.0 unx     5886 b- defN 23-May-04 10:53 facer/util.py
--rw-r--r--  2.0 unx       19 b- defN 23-May-05 02:43 facer/version.py
+-rw-r--r--  2.0 unx       19 b- defN 23-May-05 03:11 facer/version.py
 -rw-r--r--  2.0 unx       67 b- defN 23-May-04 07:21 facer/face_alignment/__init__.py
 -rw-r--r--  2.0 unx      738 b- defN 23-Apr-28 03:30 facer/face_alignment/base.py
 -rw-r--r--  2.0 unx     7113 b- defN 23-May-05 02:42 facer/face_alignment/farl.py
--rw-r--r--  2.0 unx     1486 b- defN 23-May-04 09:27 facer/face_alignment/network/__init__.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-05 03:08 facer/face_alignment/network/__init__.py
 -rw-r--r--  2.0 unx     2766 b- defN 23-May-04 07:34 facer/face_alignment/network/common.py
--rw-r--r--  2.0 unx     2466 b- defN 23-Apr-28 03:32 facer/face_alignment/network/geometry.py
+-rw-r--r--  2.0 unx     1374 b- defN 23-May-05 03:08 facer/face_alignment/network/geometry.py
 -rw-r--r--  2.0 unx      907 b- defN 23-May-04 08:33 facer/face_alignment/network/mmseg.py
 -rw-r--r--  2.0 unx     6315 b- defN 23-May-04 09:28 facer/face_alignment/network/transformers.py
--rw-r--r--  2.0 unx     5255 b- defN 23-Apr-28 03:32 facer/face_alignment/network/viz.py
 -rw-r--r--  2.0 unx      102 b- defN 23-Apr-28 03:32 facer/face_alignment/network/farl/__init__.py
 -rw-r--r--  2.0 unx    16648 b- defN 23-May-04 07:54 facer/face_alignment/network/farl/model.py
 -rw-r--r--  2.0 unx       73 b- defN 23-Apr-27 08:30 facer/face_detection/__init__.py
 -rw-r--r--  2.0 unx      372 b- defN 23-Apr-27 08:30 facer/face_detection/base.py
 -rw-r--r--  2.0 unx    20655 b- defN 23-Apr-28 02:01 facer/face_detection/retinaface.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Apr-27 08:30 facer/face_parsing/__init__.py
 -rw-r--r--  2.0 unx      732 b- defN 23-Apr-27 08:30 facer/face_parsing/base.py
 -rw-r--r--  2.0 unx     4005 b- defN 23-Apr-28 02:01 facer/face_parsing/farl.py
--rwxr-xr-x  2.0 unx     1070 b- defN 23-May-05 02:51 pyfacer-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3067 b- defN 23-May-05 02:51 pyfacer-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 02:51 pyfacer-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-05 02:51 pyfacer-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2427 b- defN 23-May-05 02:51 pyfacer-0.0.2.dist-info/RECORD
-29 files, 106114 bytes uncompressed, 31426 bytes compressed:  70.4%
+-rwxr-xr-x  2.0 unx     1070 b- defN 23-May-05 03:30 pyfacer-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5174 b- defN 23-May-05 03:30 pyfacer-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 03:30 pyfacer-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-05 03:30 pyfacer-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2335 b- defN 23-May-05 03:30 pyfacer-0.0.3.dist-info/RECORD
+28 files, 101766 bytes uncompressed, 30172 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -39,17 +39,14 @@
 
 Filename: facer/face_alignment/network/mmseg.py
 Comment: 
 
 Filename: facer/face_alignment/network/transformers.py
 Comment: 
 
-Filename: facer/face_alignment/network/viz.py
-Comment: 
-
 Filename: facer/face_alignment/network/farl/__init__.py
 Comment: 
 
 Filename: facer/face_alignment/network/farl/model.py
 Comment: 
 
 Filename: facer/face_detection/__init__.py
@@ -66,23 +63,23 @@
 
 Filename: facer/face_parsing/base.py
 Comment: 
 
 Filename: facer/face_parsing/farl.py
 Comment: 
 
-Filename: pyfacer-0.0.2.dist-info/LICENSE
+Filename: pyfacer-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyfacer-0.0.2.dist-info/METADATA
+Filename: pyfacer-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyfacer-0.0.2.dist-info/WHEEL
+Filename: pyfacer-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyfacer-0.0.2.dist-info/top_level.txt
+Filename: pyfacer-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfacer-0.0.2.dist-info/RECORD
+Filename: pyfacer-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## facer/version.py

```diff
@@ -1 +1 @@
-__version__="0.0.2"
+__version__="0.0.3"
```

## facer/face_alignment/network/__init__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 from .common import (load_checkpoint, Activation, MLP, Residual)
 from .geometry import (normalize_points, denormalize_points,
-                       points2heatmap, heatmap2points)
+                       heatmap2points)
 from .mmseg import MMSEG_UPerHead
 from .transformers import FaRLVisualFeatures
 from torch import nn
 from typing import Optional, List, Tuple
```

## facer/face_alignment/network/geometry.py

```diff
@@ -1,57 +1,27 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 from typing import Tuple, Union
 
 import torch
 
-from .ext.p2i_ops import p2i
-
 
 def normalize_points(points: torch.Tensor, h: int, w: int) -> torch.Tensor:
     """ Normalize coordinates to [0, 1].
     """
     return (points + 0.5) / torch.tensor([[[w, h]]]).to(points)
 
 
 def denormalize_points(normalized_points: torch.Tensor, h: int, w: int) -> torch.Tensor:
     """ Reverse normalize_points.
     """
     return normalized_points * torch.tensor([[[w, h]]]).to(normalized_points) - 0.5
 
 
-def points2heatmap(normalized_points, heatmap_size: Tuple[int, int], kernel_radius: float):
-    """ Normalized points [b x npoints x 2(XY)] -> heatmaps.
-    """
-    batch, npoints, _ = normalized_points.shape
-    out_h, out_w = heatmap_size
-
-    points = denormalize_points(normalized_points, out_h, out_w)
-
-    # (batch x npoints) x 1 x h x w
-    heatmap = torch.zeros(
-        batch * npoints, 1, out_h, out_w).to(points)
-    # (batch x npoints) x 2
-    points_flatten = points.view(-1, 2)
-    # (batch x npoints)
-    batch_inds = torch.arange(
-        batch * npoints, dtype=torch.int32).cuda()
-    # (batch x npoints) x 1
-    points_color = torch.ones(
-        points_flatten.size(0), 1).to(points_flatten)
-    # (batch x npoints) x 1 x h x w
-    heatmap = p2i(points_flatten, points_color, batch_inds=batch_inds, background=heatmap,
-                  kernel_radius=kernel_radius,
-                  kernel_kind_str='gaussian_awing', reduce='max')
-    # batch x npoints x h x w
-    heatmap = heatmap.reshape(batch, npoints, out_h, out_w)
-    return heatmap
-
-
 def heatmap2points(heatmap, t_scale: Union[None, float, torch.Tensor] = None):
     """ Heatmaps -> normalized points [b x npoints x 2(XY)].
     """
     dtype = heatmap.dtype
     _, _, h, w = heatmap.shape
 
     # 0 ~ h-1, 0 ~ w-1
```

## Comparing `pyfacer-0.0.2.dist-info/LICENSE` & `pyfacer-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfacer-0.0.2.dist-info/RECORD` & `pyfacer-0.0.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 facer/__init__.py,sha256=oz9_9tH_4ZcQowkMVDLwjrm7DxIxgOFGcHKMOF82uLA,1675
 facer/draw.py,sha256=vevNSN_wLXJG5wHzwwOzadsN-mq6DMdj3SxbKqkTkxM,7246
 facer/io.py,sha256=ynBWXy7illsGt1FtTOjZlqBW3Mv2IHrsbpmj32f3SiQ,545
 facer/show.py,sha256=jQEyk02d4gXfTsSDotzCGru5c3JmbMhzVAMSLBBlwww,962
 facer/transform.py,sha256=XHsqDdzItSJk7WekOmwNAH0D3BPz48ids6wltcvh9Pg,13358
 facer/util.py,sha256=57PR1TDx_3w8JUMa72QrowQNK-lwtjEIc-ZckRmGSWM,5886
-facer/version.py,sha256=HBhfINMXdfWYIApaqr1-ML8jjr202wq0tL7y497Ka5o,19
+facer/version.py,sha256=qHUqGJ1ETm11miieM-ePA1QGMQj4nWOr9giOoUt1H_A,19
 facer/face_alignment/__init__.py,sha256=DC1rYgBySHHD6FUCRKqWubyusox3lCWXVsuGdiNxFC4,67
 facer/face_alignment/base.py,sha256=d3lWu3deKWvIDChdl3GUQp4k8UiDyk6CxthCT-ypirQ,738
 facer/face_alignment/farl.py,sha256=9cHKd4yIolw321p2kUFuKIAGKuj_E3obUri3vEX6pGQ,7113
-facer/face_alignment/network/__init__.py,sha256=6-Hq7Nx1PNMmnOMNOEoO1ZrJ3WR62ZCrvRiroRpG78c,1486
+facer/face_alignment/network/__init__.py,sha256=ZrCsKOA3jTH9KVK0fJAOt3wCDT0Sxf1fEVH_-FMs2gg,1470
 facer/face_alignment/network/common.py,sha256=qiAtPYTH5eJMian_hiptf0naEiLNySctZblt4w2E-gM,2766
-facer/face_alignment/network/geometry.py,sha256=ShekBuArIrLC-j1uO7EeR_lCYK-ZCA-CWVp8GcRfQts,2466
+facer/face_alignment/network/geometry.py,sha256=UhfbTHNM8K7-qESLlqTLE30QR8p6LWUPSoiOe90bg_M,1374
 facer/face_alignment/network/mmseg.py,sha256=G5eHnIamwApCidTAkXxFCF836EDSy0Iuh9D5JCAMZFM,907
 facer/face_alignment/network/transformers.py,sha256=bTiZvnqfckBRq33lFUsKbcg6LRoUgcIKZMMZEcZDj1A,6315
-facer/face_alignment/network/viz.py,sha256=ut4fTRl9Z8cw-HLJOT-V1OROTaetMNcUrU6HVudexGk,5255
 facer/face_alignment/network/farl/__init__.py,sha256=MGKCdqBTL6OGKiS_b9ki8DTIA2zrM1p5DiFBPRnufFQ,102
 facer/face_alignment/network/farl/model.py,sha256=ZKp86to4p072a9N6XoATlI5BX7HjRjK8hM3KbAsIgZM,16648
 facer/face_detection/__init__.py,sha256=-uAQLsGBNY5fSilVYP6L3yg-fiS1FDUsJ9ltNKgGuQk,73
 facer/face_detection/base.py,sha256=ZQ55sccDDWLumxVWckAd8TjbUrcp9Q6eEEeW_eNNe6s,372
 facer/face_detection/retinaface.py,sha256=wmWlvFbfu_tlDJ033fMOoL_V_TVsTC6IlFTphgJwXHo,20655
 facer/face_parsing/__init__.py,sha256=TD6HvN1k_j-ea3ZqAK2ujHNZ9k-IT86Tm8iR4JnQh-g,61
 facer/face_parsing/base.py,sha256=NHp7zeZti5ziY6SCT1mOr3487P1PbsFLylQVwyftLaQ,732
 facer/face_parsing/farl.py,sha256=at7mRywm7JZZV1sHBBCe6GbEcbizbft5W1fZ1h5LceM,4005
-pyfacer-0.0.2.dist-info/LICENSE,sha256=41wcG5Hc62rg00AreChhWrFQeBz-st-PWTs8WZZRzbw,1070
-pyfacer-0.0.2.dist-info/METADATA,sha256=0fTfjr95VvQw8pxL5AcWvdpWwcZtgEEFglp5yRJEy78,3067
-pyfacer-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pyfacer-0.0.2.dist-info/top_level.txt,sha256=RI7cxPXuElyMHhoF-mhdJT0bHMvEGJc01hNFzhUY-78,6
-pyfacer-0.0.2.dist-info/RECORD,,
+pyfacer-0.0.3.dist-info/LICENSE,sha256=41wcG5Hc62rg00AreChhWrFQeBz-st-PWTs8WZZRzbw,1070
+pyfacer-0.0.3.dist-info/METADATA,sha256=mZLErv6CiGREyU7Rd57CSEoJ3ganGBoiAIuULSXGLV4,5174
+pyfacer-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyfacer-0.0.3.dist-info/top_level.txt,sha256=RI7cxPXuElyMHhoF-mhdJT0bHMvEGJc01hNFzhUY-78,6
+pyfacer-0.0.3.dist-info/RECORD,,
```

