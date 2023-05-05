# Comparing `tmp/dnfunc-0.0.2.tar.gz` & `tmp/dnfunc-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnfunc-0.0.2.tar", max compression
+gzip compressed data, was "dnfunc-0.0.3a2.tar", max compression
```

## Comparing `dnfunc-0.0.2.tar` & `dnfunc-0.0.3a2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2022-11-30 20:35:42.495870 dnfunc-0.0.2/LICENSE
--rw-r--r--   0        0        0      472 2022-11-30 20:35:42.495870 dnfunc-0.0.2/README.md
--rw-r--r--   0        0        0     2595 2022-11-30 20:35:42.495870 dnfunc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    49731 2022-11-30 20:35:42.495870 dnfunc-0.0.2/src/dnfunc/__init__.py
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 dnfunc-0.0.2/setup.py
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 dnfunc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/LICENSE
+-rw-r--r--   0        0        0      472 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/README.md
+-rw-r--r--   0        0        0     2663 2023-05-05 08:20:33.743370 dnfunc-0.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0    49969 2023-05-05 08:20:19.647066 dnfunc-0.0.3a2/src/dnfunc/__init__.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 dnfunc-0.0.3a2/PKG-INFO
```

### Comparing `dnfunc-0.0.2/LICENSE` & `dnfunc-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dnfunc-0.0.2/pyproject.toml` & `dnfunc-0.0.3a2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,106 @@
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
 [tool.poetry]
 name = "dnfunc"
-version = "0.0.2"
+version = "0.0.3-alpha.2"
 description = "A collection of Vapoursynth functions and wrapperspoetr"
-authors = ["DeadNews <uhjnnn@gmail.com>"]
+authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/dnfunc"
 repository = "https://github.com/DeadNews/dnfunc"
 keywords = ["vapoursynth", "vapoursynth-functions", "video-encoding"]
 classifiers = [
   "Operating System :: OS Independent",
   "Topic :: Multimedia :: Video",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+vapoursynth = ">=60"
 havsfunc = "^33"
+lvsfunc = "^0.7.1"
 pyyaml = "^6.0"
-vapoursynth = "^61"
+vstools = "^2.1.0"
 vsutil = "^0.8.0"
-vstools = "^1.6.2"
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
 
 [tool.poetry.group.ci.dependencies]
-bandit = "^1.7.4"
-black = "^22.10.0"
-flake8 = "^6.0.0"
-flake8-bugbear = "^22.10.27"
-flake8-builtins = "^2.0.1"
-flake8-comprehensions = "^3.10.1"
-flake8-implicit-str-concat = "^0.3.0"
-flake8-pie = "^0.16.0"
-flake8-pyproject = "^1.2.1"
-flake8-pytest-style = "^1.6.0"
-flake8-simplify = "^0.19.3"
-flake8-unused-arguments = "^0.0.12"
-flake8-use-pathlib = "^0.3.0"
-isort = "^5.10.1"
-mypy = "^0.991"
-pep8-naming = "^0.13.2"
-poethepoet = "^0.16.5"
-safety = "^2.3.3"
-types-pyyaml = "^6.0.12.2"
+black = "^23.3.0"
+mypy = "^1.2.0"
+poethepoet = "^0.20.0"
+ruff = "^0.0.264"
+types-pyyaml = "^6.0.12.9"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poe.tasks]
+ruff = "ruff check ."
+black = "black --check ."
+mypy = "mypy ."
+ci.sequence = ["ruff", "black", "mypy"]
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
 
 [tool.black]
 line-length = 99
 
-[tool.isort]
-line_length = 99
-profile = "black"
-
-[tool.flake8]
-max-line-length = 99
-max-complexity = 18
-show-source = true
-ignore = [
-  "E501",   # Line too long.
-  "PIE786", # Use precise exception handlers.
-  "PIE803", # Use lazy % formatting in logging functions.
-  "W503",   # Line break occurred before a binary operator.
-]
-
 [tool.mypy]
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
 show_column_numbers = true
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
-[tool.bandit]
-exclude_dirs = ["tests"]
-skips = [
-  "B404", # Importing subprocess.
-  "B603", # Calling subprocess.Popen without shell=True.
-]
-
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
-markers = ["docker", "slow"]
+markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if __name__ == .__main__.:"]
+exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
-[tool.poe.tasks]
-isort = "isort . --check-only --diff"
-black = "black . --check --diff"
-mypy = "mypy ."
-flake8 = "flake8 ."
-bandit = "bandit -r . -c pyproject.toml"
-safety = "safety check -r pyproject.toml -o bare"
-ci.sequence = ["isort", "black", "mypy", "flake8", "bandit", "safety"]
-pc = "pre-commit run -a"
+[tool.ruff]
+line-length = 99
+select = ["ALL"]
+ignore = [
+  "COM812", # Trailing comma missing
+  "D203",   # 1 blank line required before class docstring
+  "D212",   # Multi-line docstring summary should start at the first line
+  "E501",   # Line too long
+  "EXE001", # Shebang is present but file is not executable
+  "FBT001", # Boolean positional arg in function definition
+  "FBT002", # Boolean default value in function definition
+  #
+  "D101",    # Missing docstring in public class
+  "D102",    # Missing docstring in public method
+  "D103",    # Missing docstring in public function
+  "ERA001",  # Found commented-out code
+  "PLR2004", # Magic value used in comparison
+]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
+
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = false
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.flake8-annotations]
+allow-star-arg-any = true
+
+[tool.ruff.pylint]
+max-args = 7
```

### Comparing `dnfunc-0.0.2/src/dnfunc/__init__.py` & `dnfunc-0.0.3a2/src/dnfunc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 #!/usr/bin/env python
+"""A collection of Vapoursynth functions and wrappers."""
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass, field, replace
 from functools import partial
 from pathlib import Path, PurePath
 from shutil import which
-from typing import Any, NamedTuple, TypeAlias, TypeVar, Union
+from typing import Any, NamedTuple, TypeAlias, TypeVar
 
 import havsfunc as hav
 import insane_aa as iaa
 from kagefunc import adaptive_grain, kirsch, retinex_edgemask
 from vapoursynth import GRAY16, RGB, YUV420P10, VideoFrame, VideoNode, core
 from vstools import FrameRange, FrameRangeN, FrameRangesN, rfs
 from vsutil import depth, get_depth, get_y, iterate, join, split
 from yaml import safe_load
 
 T = TypeVar("T")
-Maps: TypeAlias = Union[FrameRangeN, FrameRangesN]
+Maps: TypeAlias = FrameRangeN | FrameRangesN
 VideoFunc1: TypeAlias = Callable[[VideoNode], VideoNode]
 VideoFunc2: TypeAlias = Callable[[VideoNode, VideoNode], VideoNode]
 
 PROC_DEPTH = 16  # processing_depth
 
 
 def load_yaml(file_path: str) -> dict | None:
-    """
-    Load yaml settings
-    """
+    """Load yaml settings."""
     f1 = Path(file_path)
 
     return safe_load(f1.read_text()) if f1.is_file() else None
 
 
 def override_dc(data_class: T, block: str, zone: str = "", **override: Any) -> T:
     """
-    Override default data_class params
+    Override default data_class params.
 
     Configuration preference order:
     1. func params
     2. yaml zone
     3. yaml main
     4. default
     """
     settings = load_yaml("./settings.yaml")
 
     if settings is not None:
         block_settings = settings.get(block)
 
         if block_settings is not None:
             # yaml main
-            data_class = replace(data_class, **block_settings["main"])
+            data_class = replace(data_class, **block_settings["main"])  # type: ignore[type-var]
 
             if zone and zone != "main":
                 # yaml zone
-                data_class = replace(data_class, **block_settings[zone])
+                data_class = replace(data_class, **block_settings[zone])  # type: ignore[type-var]
 
     # func params
-    return replace(data_class, **override)
+    return replace(data_class, **override)  # type: ignore[type-var]
 
 
 ######
 # aa #
 ######
 
 
@@ -76,20 +75,20 @@
 def get_edi3_mode() -> Edi3Mode:
     if which("nvidia-smi") is not None:
         return Edi3Mode(
             eedi3_mode=iaa.EEDI3Mode.OPENCL,
             device=0,
             nnedi3_mode=iaa.NNEDI3Mode.NNEDI3CL,
         )
-    else:
-        return Edi3Mode(
-            eedi3_mode=iaa.EEDI3Mode.CPU,
-            device=-1,
-            nnedi3_mode=iaa.NNEDI3Mode.ZNEDI3,
-        )
+
+    return Edi3Mode(
+        eedi3_mode=iaa.EEDI3Mode.CPU,
+        device=-1,
+        nnedi3_mode=iaa.NNEDI3Mode.ZNEDI3,
+    )
 
 
 @dataclass(frozen=True)
 class AASettings:
     desc_h: int = 0
     desc_str: float = 0.32
     kernel: str = "bicubic"
@@ -116,15 +115,14 @@
     clip: VideoNode,
     aaset: AASettings,
     out_mode: iaa.ClipMode,
     desc_h: int,
     desc_str: float,
     ext_mask: VideoNode | None = None,
 ) -> VideoNode:
-
     edi3set = get_edi3_mode()
     return iaa.insaneAA(
         clip=clip,
         eedi3_mode=edi3set.eedi3_mode,
         eedi3_device=edi3set.device,
         nnedi3_mode=edi3set.nnedi3_mode,
         nnedi3_device=edi3set.device,
@@ -177,41 +175,40 @@
 def aa(
     clip: VideoNode,
     zone: str = "",
     epname: str = "",
     ext_mask: VideoNode | None = None,
     **override: Any,
 ) -> VideoNode:
-    """
-    Anti-aliasing wrapper
-    """
+    """Anti-aliasing wrapper."""
     if epname:
         f1 = Path(f"./temp/{epname}_aa_lossless.mp4")
         if f1.is_file():
             aa_lossless = source(f1)
 
             if aa_lossless.num_frames != clip.num_frames:
-                raise NumFramesError(f"{aa_lossless.num_frames=}, {clip.num_frames=}")
+                msg = f"{aa_lossless.num_frames=}, {clip.num_frames=}"
+                raise NumFramesError(msg)
 
             return aa_lossless
 
     aaset = AASettings()
     aaset = override_dc(aaset, block="aa", zone=zone, **override)
 
     if aaset.uv_desc_h:
         return aa_yuv(clip=clip, aaset=aaset)
-    else:
-        return insane_aa(
-            clip=clip,
-            aaset=aaset,
-            out_mode=iaa.ClipMode.FULL,
-            desc_str=aaset.desc_str,
-            desc_h=clip.height if aaset.eedi3_only else aaset.desc_h,
-            ext_mask=ext_mask,
-        )
+
+    return insane_aa(
+        clip=clip,
+        aaset=aaset,
+        out_mode=iaa.ClipMode.FULL,
+        desc_str=aaset.desc_str,
+        desc_h=clip.height if aaset.eedi3_only else aaset.desc_h,
+        ext_mask=ext_mask,
+    )
 
 
 def diff_mask(clipa: VideoNode, clipb: VideoNode, mthr: int = 25) -> VideoNode:
     return (
         core.std.MakeDiff(clipa=get_y(clipa), clipb=get_y(clipb), planes=[0])
         .std.Prewitt()
         .std.Expr(f"x {mthr} < 0 x ?")
@@ -222,44 +219,41 @@
 
 
 def save_titles(
     oped_clip: VideoNode,
     ncoped: VideoNode,
     ncoped_aa: VideoNode,
 ) -> VideoNode:
-    """
-    Save OP/ED titles with expr and diff_mask
-    """
+    """Save OP/ED titles with expr and diff_mask."""
     oped_planes = split(oped_clip)
 
     oped_planes[0] = core.std.Expr(
-        [oped_planes[0], get_y(ncoped), get_y(ncoped_aa)], ["x y - z +"]
+        [oped_planes[0], get_y(ncoped), get_y(ncoped_aa)],
+        ["x y - z +"],
     )
 
     saved_titles = join(oped_planes)
     mask = diff_mask(oped_clip, ncoped)
 
     return masked_merge(saved_titles, oped_clip, mask=mask, yuv=False)
 
 
-def oped(
+def oped(  # noqa: PLR0913
     clip: VideoNode,
     name: str,
     offset: int,
     start: int,
     end: int,
     zone: str = "",
     ext_nc: VideoNode | None = None,
     input_aa: bool = False,
     edgefix: VideoFunc1 | None = None,
     filtr: VideoFunc2 | None = None,
 ) -> VideoNode:
-    """
-    Save OP/ED titles wrapper
-    """
+    """Save OP/ED titles wrapper."""
     ncoped_end = end - 1 - start + offset
 
     oped_clip = clip.std.Trim(start, end - 1)
     ncoped = source(f"./in/{name}.mp4").std.Trim(offset, ncoped_end)
 
     ncoped_aa_src = ext_nc.std.Trim(offset, ncoped_end) if ext_nc else ncoped
 
@@ -279,31 +273,28 @@
         f2 = Path(f"./temp/{name}_filt_lossless.mp4")
         if f2.is_file():
             ncoped_aa = source(f2).std.Trim(offset, ncoped_end)
         else:
             ncoped_aa = filtr(ncoped_aa, ncoped)
 
     if not (oped_clip.num_frames == ncoped.num_frames == ncoped_aa.num_frames):
-        raise NumFramesError(
-            f"{oped_clip.num_frames=}, {ncoped.num_frames=}, {ncoped_aa.num_frames=}"
-        )
+        msg = f"{oped_clip.num_frames=}, {ncoped.num_frames=}, {ncoped_aa.num_frames=}"
+        raise NumFramesError(msg)
 
     return save_titles(oped_clip=oped_clip, ncoped=ncoped, ncoped_aa=ncoped_aa)
 
 
 ##########
 # filter #
 ##########
 
 
 def gradfun_mask(source: VideoNode, thr_det: float = 1, mode: int = 3) -> VideoNode:
-    """
-    Stolen from fvsfunc
-    """
-    from muvsfunc import _Build_gf3_range_mask as gf3_range_mask  # noqa: N813
+    """Stolen from fvsfunc."""
+    from muvsfunc import _Build_gf3_range_mask as gf3_range_mask
 
     src_y = get_y(source)
     src_8 = depth(src_y, 8)
 
     tl = max(thr_det * 0.75, 1.0) - 0.0001
     th = max(thr_det, 1.0) + 0.0001
     mexpr = f"x {tl} - {th} {tl} - / 255 *"
@@ -313,36 +304,36 @@
         if mode > 1:
             deband_mask = deband_mask.std.Convolution([1, 2, 1, 2, 4, 2, 1, 2, 1])
             if mode > 2:
                 deband_mask = deband_mask.std.Convolution([1] * 9)
 
         return depth(deband_mask, PROC_DEPTH)
 
+    return None
+
 
 def adaptive_mix(
     clip: VideoNode,
     f1: VideoNode,
     f2: VideoNode,
     scaling: float,
     yuv: bool = False,
 ) -> VideoNode:
-
     adaptive_mask = adaptive_grain(clip=clip, luma_scaling=scaling, show_mask=True).std.Invert()
 
     return masked_merge(f1, f2, mask=adaptive_mask, yuv=yuv)
 
 
 def adaptive_debandmask(
     clip: VideoNode,
     source: VideoNode,
     db_mask: VideoNode,
     yaml: dict,
     db_expr: str = "",
 ) -> VideoNode:
-
     for zone in yaml:
         db_mode = yaml[zone]["db_mode"]
         thr_det = yaml[zone]["db_thr"]
         scaling = yaml[zone]["scaling"]
 
         db_n = gradfun_mask(source=source, thr_det=thr_det, mode=db_mode)
         db_mask = adaptive_mix(
@@ -356,15 +347,14 @@
     if db_expr:
         db_mask = db_mask.std.Expr(db_expr)
 
     return db_mask
 
 
 def adaptive_smdegrain(clip: VideoNode, smdegrain: VideoNode, yaml: dict) -> VideoNode:
-
     for zone in yaml:
         sm_thr = yaml[zone]["sm_thr"]
         sm_pref_mode = yaml[zone]["sm_pref_mode"]
         scaling = yaml[zone]["scaling"]
 
         dn_n = smdegrain_(clip=clip, sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
 
@@ -375,15 +365,14 @@
 
 def save_uv_unique_lines(
     clip: VideoNode,
     source: VideoNode,
     mode: str = "retinex",
     sigma: float = 1.0,
 ) -> VideoNode:
-
     clip_planes = split(clip)
     src_planes = split(source)
 
     if mode == "retinex":
         mask_u = retinex_edgemask(src_planes[1], sigma=sigma)
         mask_v = retinex_edgemask(src_planes[2], sigma=sigma)
     elif mode == "kirsch":
@@ -397,21 +386,22 @@
 
 
 def save_black(
     clip: VideoNode,
     filtered: VideoNode,
     threshold: float = 0.06276,
 ) -> VideoNode:
-    """
-    stolen from https://github.com/Irrational-Encoding-Wizardry/lvsfunc/blob/master/lvsfunc.py
-    return filtered when avg exceeds the threshold
-    """
+    """Return filtered when avg exceeds the threshold."""
 
     def _diff(
-        n: int, f: VideoFrame, clip: VideoNode, filtered: VideoNode, threshold: float  # noqa: U100
+        n: int,  # noqa: ARG001
+        f: VideoFrame,
+        clip: VideoNode,
+        filtered: VideoNode,
+        threshold: float,
     ) -> VideoNode:
         return filtered if f.props.PlaneStatsAverage > threshold else clip
 
     return core.std.FrameEval(
         clip=clip,
         eval=partial(_diff, clip=clip, filtered=filtered, threshold=threshold),
         prop_src=core.std.PlaneStats(clip),
@@ -421,17 +411,15 @@
 def f3kdb_deband(
     clip: VideoNode,
     det_y: int,
     grainy: int,
     drange: int,
     yuv: bool = False,
 ) -> VideoNode:
-    """
-    https://f3kdb.readthedocs.io/en/latest/presets.html
-    """
+    """https://f3kdb.readthedocs.io/en/latest/presets.html."""
     return core.f3kdb.Deband(
         clip=clip,
         range=drange,
         dither_algo=3,
         y=det_y,
         cb=det_y if yuv else 0,
         cr=det_y if yuv else 0,
@@ -447,15 +435,14 @@
 def contrasharp(
     clip: VideoNode,
     source: VideoNode,
     cs_mask: VideoNode,
     sm_thr: int,
     cs_val: float,
 ) -> tuple[VideoNode, VideoNode]:
-
     from CSMOD import CSMOD
 
     contrasharped = CSMOD(
         clip,
         source=source,
         preset="detail",
         edgemask=cs_mask,
@@ -467,49 +454,49 @@
 
 
 def _out_mask(mask: VideoNode) -> VideoNode:
     return core.resize.Point(mask, format=YUV420P10, matrix_s="709")
 
 
 def smdegrain_(clip: VideoNode, sm_thr: int = 48, sm_pref_mode: int = 1) -> VideoNode:
-
     sm_set = {
         "prefilter": sm_pref_mode,
         "tr": 4,
         "RefineMotion": True,
         "contrasharp": False,
     }
 
     if isinstance(sm_thr, int):
         return hav.SMDegrain(clip, thSAD=sm_thr, plane=4, chroma=True, **sm_set)
 
-    elif isinstance(sm_thr, list):
+    if isinstance(sm_thr, list):
         while len(sm_thr) < 3:
             sm_thr.append(sm_thr[len(sm_thr) - 1])
 
         if clip.format.num_planes == 1:
             return hav.SMDegrain(clip, thSAD=sm_thr[0], **sm_set)
 
         planes = split(clip)
 
         planes[0] = hav.SMDegrain(planes[0], thSAD=sm_thr[0], **sm_set)
         planes[1] = hav.SMDegrain(planes[1], thSAD=sm_thr[1], **sm_set)
         planes[2] = hav.SMDegrain(planes[2], thSAD=sm_thr[2], **sm_set)
 
         return join(planes)
 
+    return None
+
 
 def bm3d_(
     clip: VideoNode,
     bm_sigma: float = 2,
     bm_radius: float = 1,
     sm_thr: int = 48,
     sm_pref_mode: int = 1,
 ) -> VideoNode:
-
     from mvsfunc import BM3D
 
     planes = split(clip)
 
     planes[0] = BM3D(planes[0], sigma=bm_sigma, radius1=bm_radius)
     planes[1] = smdegrain_(planes[1], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
     planes[2] = smdegrain_(planes[2], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
@@ -550,22 +537,21 @@
     db_expr: str = ""
     ag_str: float = 0.0
     ag_scaling: float = 24.0
     ag_saveblack: int = 1
     ag_saveblack_tolerance: int = 2
 
 
-def filt(  # noqa: C901
+def filt(  # noqa: PLR0911, PLR0912, PLR0915, C901
     mrgc: VideoNode,
     zone: str = "",
     out_mode: int = 0,
     prefilt_func: VideoFunc2 | None = None,
     **override: Any,
 ) -> VideoNode:
-
     fset = FilterSettings()
     fset = override_dc(fset, block="filt", zone=zone, **override)
 
     clip16 = depth(mrgc, PROC_DEPTH)
 
     if prefilt_func:
         clip16 = prefilt_func(mrgc, clip16)
@@ -762,49 +748,49 @@
                 tolerance=fset.ag_saveblack_tolerance,
             )
         else:
             filtered = grained
 
     if out_mode == 0:
         return filtered
-    elif out_mode == 1:
+    if out_mode == 1:
         return _out_mask(ag_mask)
-    elif out_mode == 2:
+    if out_mode == 2:
         return _out_mask(db_mask_gradfun)
-    elif out_mode == 3:
+    if out_mode == 3:
         return _out_mask(db_mask)
-    elif out_mode == 4:
+    if out_mode == 4:
         return _out_mask(rt_mask_clip16)
-    elif out_mode == 5:
+    if out_mode == 5:
         return _out_mask(rt_mask_mix)
-    elif out_mode == 6:
+    if out_mode == 6:
         return _out_mask(rt_mask_denoised)
-    elif out_mode == 7:
+    if out_mode == 7:
         return _out_mask(rt_mask_denoised_x2)
 
+    return None
+
 
 #########
 # other #
 #########
 
 
 def chapt(epname: str, chaptname: str, fallback: str = "") -> int | None:
-
     chapters = load_yaml("./chapters.yaml")
 
     if chapters is None:
         return None
 
     epchaps = chapters[epname]
 
     return epchaps.get(chaptname, epchaps.get(fallback))
 
 
-def load_map(epname: str, mapname: str) -> Any:
-
+def load_map(epname: str, mapname: str) -> Any:  # noqa: ANN401
     maps = load_yaml("./maps.yaml")
 
     return None if maps is None else maps[mapname].get(epname)
 
 
 def fname(file: str, aa_mode: bool = False) -> str:
     f1 = PurePath(file)
@@ -814,15 +800,15 @@
 
 def source(
     file: str | Path | PurePath,
     bits: int = 0,
     fpsnum: int = 0,
     fpsden: int = 0,
 ) -> VideoNode:
-
+    """Load video source."""
     f1 = PurePath(file)
 
     if f1.suffix == ".mp4":
         src = core.lsmas.LibavSMASHSource(source=f1)
     else:
         src = core.lsmas.LWLibavSource(source=f1)
 
@@ -843,40 +829,38 @@
 
 def out(
     clip: VideoNode,
     epname: str,
     bits: int = 10,
     filtred: VideoFunc2 | None = None,
 ) -> VideoNode:
-
     if get_depth(clip) != bits:
         clip = depth(clip, bits)
 
     f1 = Path(f"./temp/{epname}_lossless.mp4")
 
     if f1.is_file():
         lossless = source(f1, bits=bits)
         if filtred:
             lossless = filtred(clip, lossless)
 
         return lossless
-    else:
-        return clip
+
+    return clip
 
 
 def pw(
     mrgc: VideoNode,
     masks: Iterable[int] = (3, 4),
     mask_zone: str = "",
     epis: VideoNode = None,
     clip: VideoNode = None,
     clip2_zone: str = "",
     ext_rip: VideoNode | None = None,
 ) -> VideoNode:
-
     pw_list = []
     if masks:
         for out_mode in masks:
             mask = filt(mrgc, zone=mask_zone, out_mode=out_mode)
             pw_list.append(mask)
 
     if epis:
@@ -888,15 +872,14 @@
     if ext_rip:
         pw_list.append(ext_rip)
 
     return core.std.Interleave(pw_list)
 
 
 def aa_pw(epis: VideoNode, zones: Iterable[str] = ("main", "test")) -> VideoNode:
-
     pw_list = []
     if epis:
         pw_list.append(epis)
 
     for zone in zones:
         aaep = aa(epis, zone=zone)
         pw_list.append(aaep)
@@ -916,19 +899,22 @@
         mask=mask,
         planes=[0, 1, 2] if yuv else [0],
     )
 
 
 def check_num_frames(epis: VideoNode, clip: VideoNode) -> None:
     if epis.num_frames != clip.num_frames:
-        raise NumFramesError(f"{epis.num_frames=}, {clip.num_frames=}")
+        msg = f"{epis.num_frames=}, {clip.num_frames=}"
+        raise NumFramesError(msg)
 
 
-def _mask_resize(mask: VideoNode, format_src: VideoNode | None = None) -> VideoNode:  # noqa: U100
-
+def _mask_resize(
+    mask: VideoNode,
+    format_src: VideoNode | None = None,  # noqa: ARG001
+) -> VideoNode:
     # if format_src:
     #     mask_format = format_src.format.replace(color_family=GRAY, subsampling_w=0, subsampling_h=0)
     # else:
     #     mask_format = GRAY16
 
     mask_format = GRAY16
 
@@ -941,15 +927,14 @@
 
 def color_mask(
     mask_src: VideoNode,
     format_src: VideoNode,
     color: str = "$000000",
     tolerance: int = 2,
 ) -> VideoNode:
-
     if get_depth(mask_src) != 8:
         mask_src = depth(mask_src, 8)
 
     mask = mask_src.tcm.TColorMask(colors=color, tolerance=tolerance)
 
     return _mask_resize(mask, format_src)
 
@@ -959,15 +944,14 @@
     f1: VideoNode | None = None,
     f2: VideoNode | None = None,
     color: str = "$000000",
     tolerance: int = 2,
     out_mask: bool = False,
     maps: Maps | None = None,
 ) -> VideoNode:
-
     mask = color_mask(mask_src=mask_src, format_src=f1, color=color, tolerance=tolerance)
     if out_mask:
         return mask
 
     replaced = masked_merge(f1, f2, mask=mask, yuv=False)
 
     return rfs(f1, replaced, maps) if maps else replaced
@@ -981,43 +965,42 @@
 def rfs_image(
     mrgc: VideoNode,
     epis: VideoNode,
     maskname: str = "",
     yuv: bool = False,
     maps: Maps | None = None,
 ) -> VideoNode:
-
     mask = image_mask(maskname, format_src=mrgc)
     replaced = masked_merge(mrgc, epis, mask=mask, yuv=yuv)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
 def rfs_diff(
     mrgc: VideoNode,
     epis: VideoNode,
     maps: Maps | None = None,
     mthr: int = 25,
     yuv: bool = True,
     out_mask: bool = False,
 ) -> VideoNode:
-
     mask = diff_mask(mrgc, epis, mthr=mthr)
     if out_mask:
         return mask
 
     replaced = masked_merge(mrgc, epis, mask=mask, yuv=yuv)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
 def diff_rescale_mask(source: VideoNode, dset: AASettings) -> VideoNode:
     """
-    Builds mask from difference of original and re-upscales clips;
-    based on atomchtools
+    Build mask from difference of original and re-upscales clips.
+
+    Based on atomchtools.
     """
     from descale import Descale
     from fvsfunc import Resize
 
     clip = get_y(source) if source.format.num_planes != 1 else source
 
     desc = Descale(
@@ -1067,15 +1050,14 @@
     epis: VideoNode = None,
     zone: str = "",
     maps: Maps | None = None,
     filt: VideoFunc1 | None = None,
     out_mask: bool = False,
     **override: Any,
 ) -> VideoNode:
-
     dset = AASettings()
     dset = override_dc(dset, block="aa", zone=zone, **override)
 
     mask = diff_rescale_mask(epis, dset=dset)
     if filt:
         mask = filt(mask)
     if out_mask:
@@ -1095,15 +1077,14 @@
         mthr=mthr,
         LumaOnly=not yuv,
         useCL=get_edi3_mode().device != -1,
     )
 
 
 def hard(clip: VideoNode, mthr: int, zone: str = "", **override: Any) -> VideoNode:
-
     yuv = yuv if (yuv := override.get("yuv")) is not None else False
 
     if zone is None and override.get("desc_h") is None:
         return _hard(clip, mthr=mthr, yuv=yuv)
 
     revset = AASettings()
     revset = override_dc(revset, block="aa", zone=zone, **override)
@@ -1125,15 +1106,14 @@
     mrgc: VideoNode,
     src: VideoNode,
     mthr: int,
     maps: Maps,
     zone: str = "",
     **override: Any,
 ) -> VideoNode:
-
     hard_ = hard(src, mthr=mthr, zone=zone, **override)
 
     return rfs(mrgc, hard_, maps)
 
 
 @dataclass(frozen=True)
 class QTGMCSettings:
@@ -1147,14 +1127,16 @@
     preset: str = "placebo"
     match_enhance: float = 0.95
     sharp: float = 0.2
 
 
 def qtgmc(clip: VideoNode, zone: str = "", **override: Any) -> VideoNode:
     """
+    QTGMC.
+
     InputType — 0 for interlaced input. Mode 1 is for general progressive material.
     Modes 2 & 3 are designed for badly deinterlaced material.
     Sharpness — The default 1.0 is fairly sharp. If using source-match the default is 0.2
     """
     qset = QTGMCSettings()
     qset = override_dc(qset, block="qtgmc", zone=zone, **override)
 
@@ -1186,15 +1168,14 @@
 def rfs_qtgmc(
     mrgc: VideoNode,
     src: VideoNode,
     maps: Maps,
     zone: str = "",
     **override: Any,
 ) -> VideoNode:
-
     stabilize = qtgmc(src, zone=zone, **override)
 
     return rfs(mrgc, stabilize, maps)
 
 
 def get_kirsch2_mask(clip_y: VideoNode) -> VideoNode:
     n = core.std.Convolution(clip_y, [5, 5, 5, -3, 0, -3, -3, -3, -3], divisor=3, saturate=False)
@@ -1229,15 +1210,14 @@
 def outerline_mask(
     clip: VideoNode,
     mode: str = "kirsch",
     max_c: int = 3,
     min_c: int = 1,
     ext_mask: VideoNode | None = None,
 ) -> VideoNode:
-
     mask = ext_mask or edge_detect(clip, mode=mode)
 
     mask_outer = iterate(mask, function=core.std.Maximum, count=max_c)
     mask_inner = mask.std.Inflate()
     mask_inner = iterate(mask_inner, function=core.std.Minimum, count=min_c)
 
     return core.std.Expr([mask_outer, mask_inner], "x y -")
@@ -1259,15 +1239,14 @@
     ext_dehalo: VideoNode | None = None,
     zone: str = "",
     ext_mask: VideoNode | None = None,
     maps: Maps | None = None,
     out_mask: bool = False,
     **override: Any,
 ) -> VideoNode:
-
     dehset = DehaloSettings()
     dehset = override_dc(dehset, block="dehalo", zone=zone, **override)
 
     if ext_dehalo:
         dehalo = ext_dehalo
         mask_src = dehalo
     else:
@@ -1295,45 +1274,43 @@
 
     replaced = masked_merge(clip, dehalo, mask=mask, yuv=False)
 
     return rfs(clip, replaced, maps) if maps else replaced
 
 
 def dehalo_chroma(clip: VideoNode, zone: str = "") -> VideoNode:
-
     planes = split(clip)
     planes[1] = rfs_dehalo(planes[1], zone=zone)
     planes[2] = rfs_dehalo(planes[2], zone=zone)
 
     return join(planes)
 
 
 @dataclass(frozen=True)
 class RepairSettings:
     edgclr_args: dict[str, int] = field(
-        default_factory=lambda: ({"strength": 10, "rmode": 13, "smode": 1})
+        default_factory=lambda: ({"strength": 10, "rmode": 13, "smode": 1}),
     )
     dering_args: dict[str, int] = field(
-        default_factory=lambda: ({"mrad": 2, "mthr": 70, "thr": 12, "darkthr": 3})
+        default_factory=lambda: ({"mrad": 2, "mthr": 70, "thr": 12, "darkthr": 3}),
     )
     mode: str = "kirsch"
     max_c: int = 3
     min_c: int = 1
     mask_from_filtred: bool = False
 
 
 def rfs_repair(
     clip: VideoNode,
     zone: str = "",
     out_mask: bool = False,
     maps: Maps | None = None,
     **override: Any,
 ) -> VideoNode:
-    """ """
-
+    """Applay `Repair` filters."""
     repset = RepairSettings()
     repset = override_dc(repset, block="repair", zone=zone, **override)
 
     if repset.edgclr_args:
         repair = hav.EdgeCleaner(clip, **repset.edgclr_args)
     if repset.dering_args:
         repair = hav.HQDeringmod(clip, **repset.dering_args)
@@ -1355,15 +1332,14 @@
 
 def rfs_linedark(
     clip: VideoNode,
     zone: str = "",
     maps: Maps | None = None,
     **override: Any,
 ) -> VideoNode:
-
     ldset = LineDarkSettings()
     ldset = override_dc(ldset, block="linedark", zone=zone, **override)
 
     replaced = hav.FastLineDarkenMOD(clip, **ldset.linedark_args)
 
     return rfs(clip, replaced, maps) if maps else replaced
 
@@ -1380,15 +1356,14 @@
 def rfs_sharp(
     clip: VideoNode,
     zone: str = "",
     maps: Maps = None,
     out_mask: bool = False,
     **override: Any,
 ) -> VideoNode:
-
     shset = SsharpSettings()
     shset = override_dc(shset, block="sharp", zone=zone, **override)
 
     mask = edge_detect(clip, mode=shset.mask_mode, expr=shset.mask_expr)
     if out_mask:
         return mask
 
@@ -1414,27 +1389,27 @@
     radius: int | list[int] = 0
     yuv: bool = False
 
     @staticmethod
     def to_list(val: int | list[int]) -> list[int]:
         return val if isinstance(val, list) else [val, 0, 0]
 
-    def check_yuv(self) -> None:
+    def check_yuv(self: "EdgeFixSettings") -> None:
         self.yuv = any(
             isinstance(val, list)
             for val in (self.top, self.bottom, self.left, self.right, self.radius)
         )
 
 
 def edgefix(
     epis: VideoNode,
     zone: str = "",
     **override: Any,
 ) -> tuple[VideoNode, VideoNode, VideoFunc1]:
-    """ """
+    """Fix edges."""
 
     def _edgefixer(epis: VideoNode) -> VideoNode:
         if not edset.yuv or not edset.crop_args:
             # luma
             return core.edgefixer.Continuity(
                 epis,
                 top=edset.top,
@@ -1518,17 +1493,15 @@
 
 
 def crop(
     epis: VideoNode,
     zone: str = "",
     **override: Any,
 ) -> tuple[VideoNode, VideoFunc1]:
-    """
-    Crop wrapper
-    """
+    """Crop wrapper."""
 
     def _crop(epis: VideoNode) -> VideoNode:
         return core.std.CropRel(
             epis,
             top=crset.top,
             bottom=crset.bottom,
             left=crset.left,
@@ -1540,17 +1513,15 @@
 
     epis = _crop(epis)
 
     return (epis, _crop)
 
 
 def to60fps_mv(clip: VideoNode) -> VideoNode:
-    """
-    http://avisynth.org.ru/mvtools/mvtools2.html
-    """
+    """http://avisynth.org.ru/mvtools/mvtools2.html."""
     sup = core.mv.Super(clip, pel=2, sharp=2, rfilter=4)
     bvec = core.mv.Analyse(
         sup,
         blksize=8,
         isb=True,
         chroma=True,
         search=3,
@@ -1592,39 +1563,41 @@
         smoothfps_params,
     )
 
 
 def to60fps(clip: VideoNode, mode: str = "svp") -> VideoNode:
     if mode == "mv":
         return to60fps_mv(clip)
-    elif mode == "svp":
+    if mode == "svp":
         return to60fps_svp(clip)
 
+    return None
+
 
 def chromashift(clip: VideoNode, cx: int = 0, cy: int = 0) -> VideoNode:
     """
+    Shift hroma.
+
     cx — Horizontal chroma shift. Positive value shifts chroma to left, negative value shifts chroma to right.
     cy — Vertical chroma shift. Positive value shifts chroma upwards, negative value shifts chroma downwards.
     """
     planes = split(clip)
 
     planes[1] = core.resize.Spline36(planes[1], src_left=cx, src_top=cy)
     planes[2] = core.resize.Spline36(planes[2], src_left=cx, src_top=cy)
 
     return join(planes)
 
 
-def adaptive_chromashift(
+def adaptive_chromashift(  # noqa: PLR0915
     clip: VideoNode,
     fix: VideoNode,
     pw_mode: int = 0,
 ) -> VideoNode:
-    """
-    Chromashift with comparisons for floating chromashift
-    """
+    """Chromashift with comparisons for floating chromashift."""
 
     def make_diff(clip: VideoNode) -> VideoNode:
         from fvsfunc import Downscale444
 
         desc_h = 720
         desc_w = hav.m4((clip.width * desc_h) / clip.height)
         descale = Downscale444(clip, w=desc_w, h=desc_h)
@@ -1640,15 +1613,14 @@
 
     def frame_diff_eval(
         n: int,
         f: VideoFrame,
         f1: VideoNode,
         f2: VideoNode,
     ) -> VideoNode:
-
         c0 = f[1].props.PlaneStatsAverage > f[0].props.PlaneStatsAverage
         p1 = f[3].props.PlaneStatsAverage > f[2].props.PlaneStatsAverage
         n1 = f[5].props.PlaneStatsAverage > f[4].props.PlaneStatsAverage
         p2 = f[7].props.PlaneStatsAverage > f[6].props.PlaneStatsAverage
         n2 = f[9].props.PlaneStatsAverage > f[8].props.PlaneStatsAverage
         p3 = f[11].props.PlaneStatsAverage > f[10].props.PlaneStatsAverage
         n3 = f[13].props.PlaneStatsAverage > f[12].props.PlaneStatsAverage
@@ -1668,22 +1640,21 @@
 
     def add_caption(
         n: int,
         f: VideoFrame,
         out: VideoNode,
         condition: bool,
     ) -> VideoNode:
-
         lines: list[str] = []
         if pw_mode == 2:
             lines.extend(
                 (
                     f"Frame avg: {f[0].props.PlaneStatsAverage}",
                     f"Frame avg: {f[1].props.PlaneStatsAverage}",
-                )
+                ),
             )
         lines.append("fix" if condition else "clip")
 
         style = "Fira Code,20,&H0000FFFF,&H00000000,&H00000000,&H00000000,1,0,0,0,100,100,0,0,1,2,0,7,10,10,10,1"
         return out.sub.Subtitle("\n".join(lines), start=n, end=n + 1, style=style)
 
     def _adaptive_chromashift(clip: VideoNode, fix: VideoNode) -> VideoNode:
@@ -1719,15 +1690,15 @@
     mode: str = "insane_aa",
     ref_clip: VideoNode | None = None,
     width: int = 0,
     height: int = 0,
     zone: str = "",
     **override: Any,
 ) -> VideoNode:
-
+    """Upcale clip to the new size."""
     if ref_clip is not None:
         dx = ref_clip.width
         dy = ref_clip.height
     elif width and height:
         dx = width
         dy = height
     elif height:
@@ -1754,22 +1725,24 @@
             nsize=4,
             mdis=20,
             nrad=aaset.nrad,
             alpha=aaset.alpha,
             beta=aaset.beta,
             gamma=aaset.gamma,
         )
-    elif mode == "jinc":
+    if mode == "jinc":
         return clip.jinc.JincResize(dx, dy)
-    elif mode == "lanczos":
+    if mode == "lanczos":
         return clip.resize.Lanczos(dx, dy, filter_param_a=2)
 
+    return None
 
-def downscale(clip: VideoNode, desc_h: int = 720, to420: bool = False) -> VideoNode:
 
+def downscale(clip: VideoNode, desc_h: int = 720, to420: bool = False) -> VideoNode:
+    """Downcale clip to the new size."""
     if clip.height == desc_h:
         return clip
 
     desc_w = hav.m4((clip.width * desc_h) / clip.height)
 
     if not to420:
         return clip.resize.Spline36(desc_w, desc_h)
@@ -1785,15 +1758,14 @@
 
 def rfs_black_crop(
     clip: VideoNode,
     maps: Maps,
     top: int = 0,
     bot: int = 0,
 ) -> VideoNode:
-
     fixed_black = clip.std.CropRel(top=top, bottom=bot).std.AddBorders(top=top, bottom=bot)
 
     return rfs(clip, fixed_black, maps)
 
 
 def get_list(ranges: list[FrameRange]) -> list[int]:
     frames = []
```

### Comparing `dnfunc-0.0.2/PKG-INFO` & `dnfunc-0.0.3a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: dnfunc
-Version: 0.0.2
+Version: 0.0.3a2
 Summary: A collection of Vapoursynth functions and wrapperspoetr
 Home-page: https://github.com/DeadNews/dnfunc
 License: MIT
 Keywords: vapoursynth,vapoursynth-functions,video-encoding
 Author: DeadNews
-Author-email: uhjnnn@gmail.com
+Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Video
 Requires-Dist: havsfunc (>=33,<34)
+Requires-Dist: lvsfunc (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: vapoursynth (>=61,<62)
-Requires-Dist: vstools (>=1.6.2,<2.0.0)
+Requires-Dist: vapoursynth (>=60)
+Requires-Dist: vstools (>=2.1.0,<3.0.0)
 Requires-Dist: vsutil (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/DeadNews/dnfunc
 Description-Content-Type: text/markdown
 
 # dnfunc
 
 > A collection of Vapoursynth functions and wrappers
```

