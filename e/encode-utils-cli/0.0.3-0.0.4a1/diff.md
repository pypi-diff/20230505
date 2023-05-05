# Comparing `tmp/encode-utils-cli-0.0.3.tar.gz` & `tmp/encode_utils_cli-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encode-utils-cli-0.0.3.tar", max compression
+gzip compressed data, was "encode_utils_cli-0.0.4a1.tar", max compression
```

## Comparing `encode-utils-cli-0.0.3.tar` & `encode_utils_cli-0.0.4a1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1065 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/LICENSE
--rw-r--r--   0        0        0      828 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/README.md
--rw-r--r--   0        0        0     2874 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/__init__.py
--rw-r--r--   0        0        0      179 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/__main__.py
--rw-r--r--   0        0        0      941 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/_cli.py
--rw-r--r--   0        0        0     2067 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/chapt2bmqpyml.py
--rw-r--r--   0        0        0      664 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/frames_denum.py
--rwxr-xr-x   0        0        0     1218 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/mpls2chap.py
--rw-r--r--   0        0        0      437 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/num_frames.py
--rw-r--r--   0        0        0     1183 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/re_chapters.py
--rwxr-xr-x   0        0        0     1040 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/re_titles.py
--rwxr-xr-x   0        0        0      964 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/screens2bm.py
--rw-r--r--   0        0        0       22 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/util/__init__.py
--rw-r--r--   0        0        0     1963 2022-09-12 10:15:11.518948 encode-utils-cli-0.0.3/src/encode_utils_cli/util/load_mpls.py
--rw-r--r--   0        0        0      283 2022-09-12 10:15:11.522948 encode-utils-cli-0.0.3/src/encode_utils_cli/util/source.py
--rw-r--r--   0        0        0      708 2022-09-12 10:15:11.522948 encode-utils-cli-0.0.3/src/encode_utils_cli/util/timeconv.py
--rw-r--r--   0        0        0     2174 2022-09-12 10:15:11.522948 encode-utils-cli-0.0.3/src/encode_utils_cli/vs_screens.py
--rwxr-xr-x   0        0        0      768 2022-09-12 10:15:11.522948 encode-utils-cli-0.0.3/src/encode_utils_cli/zones_validator.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 encode-utils-cli-0.0.3/setup.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 encode-utils-cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/LICENSE
+-rw-r--r--   0        0        0      828 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/README.md
+-rw-r--r--   0        0        0     2599 2023-05-05 09:18:11.132545 encode_utils_cli-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__main__.py
+-rw-r--r--   0        0        0      970 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py
+-rw-r--r--   0        0        0     2087 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py
+-rw-r--r--   0        0        0      666 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py
+-rwxr-xr-x   0        0        0     1209 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py
+-rw-r--r--   0        0        0      427 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/num_frames.py
+-rw-r--r--   0        0        0     1163 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py
+-rwxr-xr-x   0        0        0     1042 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py
+-rwxr-xr-x   0        0        0      966 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py
+-rw-r--r--   0        0        0       35 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/__init__.py
+-rw-r--r--   0        0        0     2012 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py
+-rw-r--r--   0        0        0      312 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/source.py
+-rw-r--r--   0        0        0      672 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py
+-rw-r--r--   0        0        0     2203 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py
+-rwxr-xr-x   0        0        0      758 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 encode_utils_cli-0.0.4a1/PKG-INFO
```

### Comparing `encode-utils-cli-0.0.3/LICENSE` & `encode_utils_cli-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `encode-utils-cli-0.0.3/README.md` & `encode_utils_cli-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/_cli.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+"""Entrypoint for cli."""
 import click
 
 from encode_utils_cli.chapt2bmqpyml import chapt2bmqpyml
 from encode_utils_cli.frames_denum import frames_denum
 from encode_utils_cli.mpls2chap import mpls2chap
 from encode_utils_cli.num_frames import num_frames
 from encode_utils_cli.re_chapters import re_chapters
@@ -11,15 +12,15 @@
 from encode_utils_cli.vs_screens import vs_screens
 from encode_utils_cli.zones_validator import zones_validator
 
 
 @click.group(context_settings={"show_default": True, "help_option_names": ["-h", "--help"]})
 @click.version_option()
 def cli() -> None:
-    """Main entrypoint."""
+    """Entrypoint for cli."""
 
 
 cli.add_command(chapt2bmqpyml)
 cli.add_command(frames_denum)
 cli.add_command(mpls2chap)
 cli.add_command(num_frames)
 cli.add_command(re_chapters)
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/chapt2bmqpyml.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,34 @@
     "episodes",
     nargs=-1,
     required=True,
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
 )
 @click.option("-f", "--fps", type=str, default="24000/1001")
 @click.option(
-    "-v", "--vid-info", is_flag=True, default=False, help="Get corresponding videos info."
+    "-v",
+    "--vid-info",
+    is_flag=True,
+    default=False,
+    help="Get corresponding videos info.",
 )
 @click.option(
     "-c",
     "--custom-layout",
     is_flag=True,
     default=False,
     help="Custom layout.",
 )
 def chapt2bmqpyml(
     episodes: tuple[Path],
     fps: str,
     vid_info: bool,
     custom_layout: bool,
 ) -> None:
-    """
-    Convert chapters into yaml, corresponding bookmarks and qp files.
-    """
+    """Convert chapters into yaml, corresponding bookmarks and qp files."""
     for ep in episodes:
         chapters = ep.read_text()
 
         clip = source(Path(f"{ep.parents[1]}/{ep.stem}.mp4")) if vid_info else None
         fps_ = Fraction(fps if clip is None else clip.fps.numerator / clip.fps.denominator)
 
         names = [sub(r"[ ,]", "_", name) for name in findall(r"NAME=([^\n]+)", chapters)]
@@ -54,13 +56,13 @@
             bmk = Path(f"{ep.parent}/{ep.stem}.vpy.bookmarks")
             qpf = Path(f"{ep.parent}/{ep.stem}.qp")
             yml = Path(f"{ep.parent}/chapters.yaml")
 
         bmk.write_text(", ".join(f"{frame}" for frame in frames) + "\n")
         qpf.write_text("\n".join(f"{frame} I -1" for frame in frames) + "\n")
 
-        chap = {ep.stem: dict(zip(names, frames))}
+        chap = {ep.stem: dict(zip(names, frames, strict=True))}
         if clip is not None:
             chap[ep.stem]["EOF"] = clip.num_frames
 
         with yml.open("a") as stream:
             dump(data=chap, stream=stream, sort_keys=False)
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/frames_denum.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from pyperclip import copy
 
 
 @click.command()
 @click.argument("frames", nargs=-1, required=True, type=int)
 @click.option("-d", "--denum", type=float, default=2)
 def frames_denum(frames: tuple[int], denum: float) -> None:
-    """
+    r"""
     Sort frames and divide without remainder by the specified divisor.
+
     The result will be copied to the clipboard.
 
     \b
     >>> frames_denum((16886, 26280), denum=2)
     <<< "8443 13140"
     >>> frames_denum((16886, 26280), denum=.5)
     <<< "33772 52560"
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/mpls2chap.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 @click.option(
     "-d",
     "--out-dir",
     type=click.Path(file_okay=False, path_type=Path),
     help="Custom out dir.",
 )
 def mpls2chap(mpls: Path, start_ep: int, out_dir: Path) -> None:
-    """
-    Make .txt chapters from .mpls
-    """
+    """Make .txt chapters from .mpls."""
     out_dir = Path(mpls.parent) if out_dir is None else out_dir
 
     with mpls.open("rb") as data:
         chapterdata = load_mpls(data)[:-1]
 
     for number, ep in enumerate(chapterdata, start=start_ep):
         startpos = ep.times[0]
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/re_chapters.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     "-c",
     "--config",
     required=True,
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
     help="yaml config.",
 )
 def re_chapters(episodes: tuple[Path], config: Path) -> None:
-    """
-    Replace chapters names.
-    """
+    """Replace chapters names."""
     names = safe_load(config.read_text())
 
     for ep in episodes:
         chapters = ep.read_text()
         chap_count = len(findall(r"(NAME=)", chapters))
         zero_chap = findall(r"(CHAPTER00NAME=)", chapters)
         pad = 0 if zero_chap else 1
@@ -39,11 +37,9 @@
                 name=names[chap_count][i],
             )
 
         ep.write_text(chapters)
 
 
 def sub_chapter(chapters: str, num: int, name: str) -> str:
-    """
-    Replace chapter name.
-    """
+    """Replace chapter name."""
     return sub(rf"(CHAPTER{num:02d}NAME=)(.*)", rf"\1{name}", chapters)
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/re_titles.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     "-c",
     "--config",
     required=True,
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
     help="toml config.",
 )
 def re_titles(config: Path) -> None:
-    """
+    r"""
     Replace titles names from anidb.
+
     The result will be copied to the clipboard.
 
     \b
     >>> 1 	The Prince`s New Clothes
     <<< e1: EP1 «The Prince`s New Clothes»
     """
     titles = loads(config.read_text())["titles"]
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/screens2bm.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,17 @@
     "screens",
     nargs=-1,
     required=True,
     type=click.Path(dir_okay=False, path_type=PurePath),
 )
 @click.option("-f", "--fps", type=str, default="24000/1001")
 def screens2bm(screens: tuple[PurePath], fps: str) -> None:
-    """
+    r"""
     Parse screens timestamps hh:mm:ss.xxxx into bookmark format.
+
     The result will be copied to the clipboard.
 
     \b
     >>> 00000 (00:12:34.34) 01.png
     <<< 18086
     >>> 00000 (00_00_03.34) 02.png
     <<< 80
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/util/load_mpls.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 from io import SEEK_CUR
 from struct import unpack
 from typing import BinaryIO, NamedTuple
 
 
 class PlayList(NamedTuple):
+    """Represent playlist data."""
+
     name: str
     times: list[int]
 
 
 def load_mpls(f: BinaryIO, fix_overlap: bool = True) -> list[PlayList]:
     """
-        Parse blu-ray .mpls
-        https://gist.github.com/dk00/0a0634c5666cf1b8ab9f
+    Parse blu-ray `.mpls`.
+
+    https://gist.github.com/dk00/0a0634c5666cf1b8ab9f
 
     >>> [
     >>>     PlayList(name="00014", times=[189000000, 194469213, 225901239, 249525465, 253620806]),
     >>>     PlayList(name="00015", times=[189000000, 200779267, 223110326, 249510450, 253620806]),
     >>> ]
     """
 
@@ -61,11 +64,11 @@
 
     if fix_overlap:
         b = None
         for item in items:
             a, b = b, item.times
             if a and b[0] < a[-1] < b[-1]:
                 a[-1] = b[0]
-        if b is not None and len(b) > 1 and b[-1] - b[-2] < 90090:
+        if b is not None and len(b) > 1 and b[-1] - b[-2] < 90090:  # noqa: PLR2004
             b.pop()
 
     return items
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/util/timeconv.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 #!/usr/bin/env python
 from fractions import Fraction
 
 
 def seconds2ts(s: float) -> str:
-    """
-    Convert seconds in timestamp hh:mm:ss.xxx
-    """
+    """Convert seconds in timestamp hh:mm:ss.xxx."""
     m = s // 60
     s %= 60
     h = m // 60
     m %= 60
     return f"{h:02.0f}:{m:02.0f}:{s:06.3f}"
 
 
 def ts2seconds(ts: str) -> float:
-    """
-    Convert timestamp hh:mm:ss.xxxx to seconds
-    """
+    """Convert timestamp hh:mm:ss.xxxx to seconds."""
     h, m, s = map(float, ts.split(":"))
     return h * 3600 + m * 60 + s
 
 
 def seconds2f(s: float, fps: Fraction) -> int:
-    """
-    Convert seconds to frames
-    """
+    """Convert seconds to frames."""
     return round(s * fps)
 
 
 def ts2f(ts: str, fps: Fraction) -> int:
-    """
-    Convert a timestamp hh:mm:ss.xxxx in number of frames
-    """
+    """Convert a timestamp hh:mm:ss.xxxx in number of frames."""
     return seconds2f(s=ts2seconds(ts), fps=fps)
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/vs_screens.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     vids: tuple[Path],
     out_dir: Path,
     frames: str,
     offset: int,
     crop: int,
     drop_prop: bool,
 ) -> None:
-    """
-    Screens via Vapoursynth.
-    """
+    """Screens via Vapoursynth."""
     frames = frames or " ".join([f"{i}" for i in sample(range(100, 10000), k=5)])
     click.echo(f"Requesting frames: {frames!r}")
 
     for vid in vids:
         out_dir = Path(vid.parent) if out_dir is None else out_dir
         out_dir.mkdir(exist_ok=True)
         save_pattern = Path(f"{out_dir}/{vid.stem} %d.png")
@@ -49,25 +47,27 @@
 
         for frame in frames.split():
             click.echo(f"Writing: '{save_pattern}' {frame}")
             writer.get_frame(int(frame))
 
 
 def open_clip(video: Path, drop_prop: bool, offset: int, crop: int) -> VideoNode:
-    """
-    Prepare clip.
-    """
+    """Prepare clip."""
     clip = source(video)
+    sd_height = 576
 
     if drop_prop:
         clip = (
             clip.std.Setframe_prop(prop="_Matrix", delete=True)
             .std.Setframe_prop(prop="_Transfer", delete=True)
             .std.Setframe_prop(prop="_Primaries", delete=True)
         )
-    clip = clip.resize.Spline36(format=RGB24, matrix_in_s="709" if clip.height >= 576 else "601")
+    clip = clip.resize.Spline36(
+        format=RGB24,
+        matrix_in_s="709" if clip.height >= sd_height else "601",
+    )
     if offset:
         clip = clip.std.Trim(offset, clip.num_frames - 1)
     if crop:
         clip = clip.std.CropRel(top=crop, bottom=crop)
 
     return clip
```

### Comparing `encode-utils-cli-0.0.3/src/encode_utils_cli/zones_validator.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 @click.command()
 @click.argument(
     "zones_config",
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
 )
 def zones_validator(zones_config: Path) -> None:
-    """
-    Validate x264/x265 zones.
-    """
+    """Validate x264/x265 zones."""
     text = zones_config.read_text()
 
     targe_lines = [
         line
         for line in text.splitlines()
         if line and not line.isspace() and not line.lstrip().startswith("#")
     ]
```

### Comparing `encode-utils-cli-0.0.3/PKG-INFO` & `encode_utils_cli-0.0.4a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: encode-utils-cli
-Version: 0.0.3
+Version: 0.0.4a1
 Summary: Encode utils collection
 Home-page: https://github.com/DeadNews/encode-utils-cli
 License: MIT
 Keywords: cli,encode,vapoursynth,mpls
 Author: DeadNews
-Author-email: uhjnnn@gmail.com
+Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Video
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: click (>=8.0.2,<9.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: vapoursynth (>=59,<60)
+Requires-Dist: vapoursynth (>=60)
 Project-URL: Repository, https://github.com/DeadNews/encode-utils-cli
 Description-Content-Type: text/markdown
 
 # encode-utils-cli
 
 > Encode utils collection
```

