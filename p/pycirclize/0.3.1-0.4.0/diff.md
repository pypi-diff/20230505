# Comparing `tmp/pycirclize-0.3.1.tar.gz` & `tmp/pycirclize-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-0.3.1.tar", max compression
+gzip compressed data, was "pycirclize-0.4.0.tar", max compression
```

## Comparing `pycirclize-0.3.1.tar` & `pycirclize-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1062 2023-04-09 08:06:37.002844 pycirclize-0.3.1/LICENSE
--rw-r--r--   0        0        0     4783 2023-04-09 08:06:37.002844 pycirclize-0.3.1/README.md
--rw-r--r--   0        0        0     1216 2023-04-09 08:06:37.158843 pycirclize-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       89 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    29406 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/circos.py
--rw-r--r--   0        0        0     2921 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/config.py
--rw-r--r--   0        0        0      232 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    18161 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    15424 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     7996 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0    12582 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/patches.py
--rw-r--r--   0        0        0    15864 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/sector.py
--rw-r--r--   0        0        0    45503 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/track.py
--rw-r--r--   0        0        0      534 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     6869 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     3774 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     9955 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/images/python_logo.png
--rw-r--r--   0        0        0     2314 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0     4991 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/tree.py
--rw-r--r--   0        0        0        0 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1941 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     1839 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_gff.py
--rw-r--r--   0        0        0     2090 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     2751 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_circos.py
--rw-r--r--   0        0        0    20534 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_plot.py
--rw-r--r--   0        0        0     2811 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_sector.py
--rw-r--r--   0        0        0      925 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_track.py
--rw-r--r--   0        0        0      755 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0   580710 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
--rw-r--r--   0        0        0    58530 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
--rw-r--r--   0        0        0        0 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/test_helper.py
--rw-r--r--   0        0        0     5743 1970-01-01 00:00:00.000000 pycirclize-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-05 12:51:25.158812 pycirclize-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4721 2023-05-05 12:51:25.158812 pycirclize-0.4.0/README.md
+-rw-r--r--   0        0        0     1436 2023-05-05 12:51:25.298814 pycirclize-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    30836 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     2921 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/config.py
+-rw-r--r--   0        0        0      232 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    18100 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    17331 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     7996 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0    12582 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    16431 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    46811 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/track.py
+-rw-r--r--   0        0        0      534 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     6869 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     3774 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     9955 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/images/python_logo.png
+-rw-r--r--   0        0        0     2314 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0     4991 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/tree.py
+-rw-r--r--   0        0        0        0 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1941 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/__init__.py
+-rw-r--r--   0        0        0     1752 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     1839 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     2090 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_matrix.py
+-rw-r--r--   0        0        0     2765 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_circos.py
+-rw-r--r--   0        0        0    20530 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_plot.py
+-rw-r--r--   0        0        0     2811 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_sector.py
+-rw-r--r--   0        0        0      925 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_track.py
+-rw-r--r--   0        0        0      755 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
+-rw-r--r--   0        0        0    30808 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
+-rw-r--r--   0        0        0   283582 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
+-rw-r--r--   0        0        0   148834 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
+-rw-r--r--   0        0        0    36204 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff
+-rw-r--r--   0        0        0   580710 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
+-rw-r--r--   0        0        0    58530 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
+-rw-r--r--   0        0        0        0 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2025 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/test_dataset.py
+-rw-r--r--   0        0        0     1839 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/test_helper.py
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 pycirclize-0.4.0/PKG-INFO
```

### Comparing `pycirclize-0.3.1/LICENSE` & `pycirclize-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/README.md` & `pycirclize-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -61,30 +61,30 @@
 # Initialize Circos sectors
 sectors = {"A": 10, "B": 15, "C": 12, "D": 20, "E": 15}
 circos = Circos(sectors, space=5)
 
 for sector in circos.sectors:
     # Plot sector name
     sector.text(f"Sector: {sector.name}", r=110, size=15)
-    # Create x positions & randomized y values
+    # Create x positions & random y values
     x = np.arange(sector.start, sector.end) + 0.5
     y = np.random.randint(0, 100, len(x))
-    # Plot line track
-    line_track = sector.add_track((80, 100), r_pad_ratio=0.1)
-    line_track.xticks_by_interval(interval=1)
-    line_track.axis()
-    line_track.line(x, y)
-    # Plot points track
-    points_track = sector.add_track((55, 75), r_pad_ratio=0.1)
-    points_track.axis()
-    points_track.scatter(x, y)
-    # Plot bar track
-    bar_track = sector.add_track((30, 50), r_pad_ratio=0.1)
-    bar_track.axis()
-    bar_track.bar(x, y)
+    # Plot lines
+    track1 = sector.add_track((80, 100), r_pad_ratio=0.1)
+    track1.xticks_by_interval(interval=1)
+    track1.axis()
+    track1.line(x, y)
+    # Plot points 
+    track2 = sector.add_track((55, 75), r_pad_ratio=0.1)
+    track2.axis()
+    track2.scatter(x, y)
+    # Plot bars
+    track3 = sector.add_track((30, 50), r_pad_ratio=0.1)
+    track3.axis()
+    track3.bar(x, y)
 
 # Plot links 
 circos.link(("A", 0, 3), ("B", 15, 12))
 circos.link(("B", 0, 3), ("C", 7, 11), color="skyblue")
 circos.link(("C", 2, 5), ("E", 15, 12), color="chocolate", direction=1)
 circos.link(("D", 3, 5), ("D", 18, 15), color="lime", ec="black", lw=0.5, hatch="//", direction=2)
 circos.link(("D", 8, 10), ("E", 2, 8), color="violet", ec="red", lw=1.0, ls="dashed")
```

### Comparing `pycirclize-0.3.1/src/pycirclize/circos.py` & `pycirclize-0.4.0/src/pycirclize/circos.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         self,
         sectors: dict[str, int] | dict[str, float],
         start: float = 0,
         end: float = 360,
         *,
         space: float | list[float] = 0,
         endspace: bool = True,
-        sectors_start_pos: dict[str, int] | dict[str, float] = {},
+        sectors_start_pos: dict[str, int] | dict[str, float] | None = None,
+        sector2clockwise: dict[str, bool] | None = None,
         show_axis_for_debug: bool = False,
     ):
         """
         Parameters
         ----------
         sectors : dict[str, int] | dict[str, float]
             Sector name & size dict
@@ -47,19 +48,24 @@
             Plot start degree (`-360 <= start < end <= 360`)
         end : float, optional
             Plot end degree (`-360 <= start < end <= 360`)
         space : float | list[float], optional
             Space degree(s) between sector
         endspace : bool, optional
             If True, insert space after the end sector
-        sectors_start_pos : dict[str, int] | dict[str, float], optional
+        sectors_start_pos : dict[str, int] | dict[str, float] | None, optional
             Sector name & start position dict. By default, `start_pos=0`.
+        sector2clockwise : dict[str, bool] | None, optional
+            Sector name & clockwise bool dict. By default, `clockwise=True`.
         show_axis_for_debug : bool, optional
             Show axis for position check debugging (Developer option)
         """
+        sectors_start_pos = {} if sectors_start_pos is None else sectors_start_pos
+        sector2clockwise = {} if sector2clockwise is None else sector2clockwise
+
         # Check start-end degree range
         self._check_degree_range(start, end)
 
         # Calculate sector region & add sector
         whole_deg_size = end - start
         space_num = len(sectors) if endspace else len(sectors) - 1
         if isinstance(space, (list, tuple)):
@@ -80,15 +86,16 @@
         for idx, (sector_name, sector_size) in enumerate(sectors.items()):
             sector_size_ratio = sector_size / sector_total_size
             deg_size = whole_deg_size_without_space * sector_size_ratio
             rad_size = math.radians(deg_size)
             rad_lim = (rad_pos, rad_pos + rad_size)
             rad_pos += rad_size + math.radians(space_list[idx])
             start_pos = sectors_start_pos.get(sector_name, 0)
-            sector = Sector(sector_name, sector_size, rad_lim, start_pos)
+            clockwise = sector2clockwise.get(sector_name, True)
+            sector = Sector(sector_name, sector_size, rad_lim, start_pos, clockwise)
             self._sectors.append(sector)
 
         self._deg_lim = (start, end)
         self._rad_lim = (math.radians(start), math.radians(end))
         self._patches: list[Patch] = []
         self._plot_funcs: list[Callable[[PolarAxes], None]] = []
         self._ax: PolarAxes | None = None
@@ -153,20 +160,20 @@
         *,
         start: float = 0,
         end: float = 360,
         space: float | list[float] = 0,
         endspace: bool = True,
         r_lim: tuple[float, float] = (97, 100),
         cmap: str | dict[str, str] = "viridis",
-        link_cmap: list[tuple[str, str, str]] = [],
+        link_cmap: list[tuple[str, str, str]] | None = None,
         ticks_interval: int | None = None,
         order: str | list[str] | None = None,
-        label_kws: dict[str, Any] = {},
-        ticks_kws: dict[str, Any] = {},
-        link_kws: dict[str, Any] = {},
+        label_kws: dict[str, Any] | None = None,
+        ticks_kws: dict[str, Any] | None = None,
+        link_kws: dict[str, Any] | None = None,
         link_kws_handler: Callable[[str, str], dict[str, Any] | None] | None = None,
     ) -> Circos:
         """Initialize Circos instance from Matrix
 
         Circos tracks and links are auto-defined by Matrix (For plotting Chord Diagram)
 
         Parameters
@@ -183,44 +190,49 @@
             If True, insert space after the end sector
         r_lim : tuple[float, float], optional
             Outer track radius limit region (0 - 100)
         cmap : str | dict[str, str], optional
             Colormap assigned to each outer track and link.
             User can set matplotlib's colormap (e.g. `viridis`, `jet`, `tab10`) or
             label_name -> color dict (e.g. `dict(A="red", B="blue", C="green", ...)`)
-        link_cmap : list[tuple[str, str, str]], optional
+        link_cmap : list[tuple[str, str, str]] | None, optional
             Link colormap to overwrite link colors automatically set by cmap.
             User can set list of `from_label`, `to_label`, `color` tuple
             (e.g. `[("A", "B", "red"), ("A", "C", "#ffff00), ...]`)
         ticks_interval : int | None, optional
             Ticks interval. If None, ticks are not plotted.
         order : str | list[str] | None, optional
             Sort order of matrix for plotting Chord Diagram. If `None`, no sorting.
             If `asc`|`desc`, sort in ascending(or descending) order by node size.
             If node name list is set, sort in user specified node order.
-        label_kws : dict[str, Any], optional
+        label_kws : dict[str, Any] | None, optional
             Keyword arguments passed to `sector.text()` method
             (e.g. `dict(r=110, orientation="vertical", size=15, ...)`)
-        ticks_kws : dict[str, Any], optional
+        ticks_kws : dict[str, Any] | None, optional
             Keyword arguments passed to `track.xticks_by_interval()` method
             (e.g. `dict(label_size=10, label_orientation="vertical", ...)`)
-        link_kws : dict[str, Any], optional
+        link_kws : dict[str, Any] | None, optional
             Keyword arguments passed to `circos.link()` method
             (e.g. `dict(direction=1, ec="black", lw=0.5, alpha=0.8, ...)`)
         link_kws_handler : Callable[[str, str], dict[str, Any] | None] | None, optional
             User-defined function to handle keyword arguments for each link.
             This option allows user to set or override properties such as
             `fc`, `alpha`, `zorder`, etc... on each link.
             Handler function arguments `[str, str]` means `[from_label, to_label]`.
 
         Returns
         -------
         circos : Circos
             Circos instance initialized from Matrix
         """
+        link_cmap = [] if link_cmap is None else deepcopy(link_cmap)
+        label_kws = {} if label_kws is None else deepcopy(label_kws)
+        ticks_kws = {} if ticks_kws is None else deepcopy(ticks_kws)
+        link_kws = {} if link_kws is None else deepcopy(link_kws)
+
         # If input matrix is file path, convert to Matrix instance
         if isinstance(matrix, (str, Path, pd.DataFrame)):
             matrix = Matrix(matrix)
 
         # Sort matrix if order is set
         if order is not None:
             matrix = matrix.sort(order)
@@ -274,14 +286,15 @@
     def initialize_from_bed(
         bed_file: str | Path,
         start: float = 0,
         end: float = 360,
         *,
         space: float | list[float] = 0,
         endspace: bool = True,
+        sector2clockwise: dict[str, bool] | None = None,
     ) -> Circos:
         """Initialize Circos instance from BED file
 
         Circos sectors are auto-defined by BED chromosomes
 
         Parameters
         ----------
@@ -291,30 +304,34 @@
             Plot start degree (-360 <= start < end <= 360)
         end : float, optional
             Plot end degree (-360 <= start < end <= 360)
         space : float | list[float], optional
             Space degree(s) between sector
         endspace : bool, optional
             If True, insert space after the end sector
+        sector2clockwise : dict[str, bool] | None, optional
+            Sector name & clockwise bool dict. By default, `clockwise=True`.
 
         Returns
         -------
         circos : Circos
             Circos instance initialized from BED file
         """
+        sector2clockwise = {} if sector2clockwise is None else sector2clockwise
         records = Bed(bed_file).records
         sectors = {rec.chr: rec.size for rec in records}
         sectors_start_pos = {rec.chr: rec.start for rec in records}
         return Circos(
             sectors,
             start,
             end,
             space=space,
             endspace=endspace,
             sectors_start_pos=sectors_start_pos,
+            sector2clockwise=sector2clockwise,
         )
 
     def add_cytoband_tracks(
         self,
         r_lim: tuple[float, float],
         cytoband_file: str | Path,
         *,
@@ -593,16 +610,16 @@
         self,
         bounds: tuple[float, float, float, float] = (1.02, 0.3, 0.02, 0.4),
         *,
         vmin: float = 0,
         vmax: float = 1,
         cmap: str | Colormap = "bwr",
         orientation: str = "vertical",
-        colorbar_kws: dict[str, Any] = {},
-        tick_kws: dict[str, Any] = {},
+        colorbar_kws: dict[str, Any] | None = None,
+        tick_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot colorbar
 
         Parameters
         ----------
         bounds : tuple[float, float, float, float], optional
             Colorbar bounds tuple (`x`, `y`, `width`, `height`)
@@ -611,21 +628,23 @@
         vmax : float, optional
             Colorbar max value
         cmap : str | Colormap, optional
             Colormap (e.g. `viridis`, `Spectral`, `Reds`, `Greys`)
             <https://matplotlib.org/stable/tutorials/colors/colormaps.html>
         orientation : str, optional
             Colorbar orientation (`vertical`|`horizontal`)
-        colorbar_kws : dict[str, Any], optional
+        colorbar_kws : dict[str, Any] | None, optional
             Colorbar properties (e.g. `dict(label="name", format="%.1f", ...)`)
             <https://matplotlib.org/stable/api/colorbar_api.html>
-        tick_kws : dict[str, Any], optional
+        tick_kws : dict[str, Any] | None, optional
             Axes.tick_params properties (e.g. `dict(labelsize=12, colors="red", ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.tick_params.html>
         """
+        colorbar_kws = {} if colorbar_kws is None else deepcopy(colorbar_kws)
+        tick_kws = {} if tick_kws is None else deepcopy(tick_kws)
 
         def plot_colorbar(ax: PolarAxes) -> None:
             axin: Axes = ax.inset_axes(bounds)
             norm = Normalize(vmin=vmin, vmax=vmax)
             Colorbar(
                 axin,
                 cmap=cmap,
@@ -691,14 +710,19 @@
         savefile: str | Path,
         *,
         dpi: int = 100,
         pad_inches: float = 0.5,
     ) -> None:
         """Save figure to file
 
+        `circos.savefig("result.png")` is alias for the following code
+
+        >>> fig = circos.plotfig()
+        >>> fig.savefig("result.png")
+
         Parameters
         ----------
         savefile : str | Path
             Save file
         dpi : int, optional
             DPI
         pad_inches : float, optional
```

### Comparing `pycirclize-0.3.1/src/pycirclize/config.py` & `pycirclize-0.4.0/src/pycirclize/config.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/parser/bed.py` & `pycirclize-0.4.0/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/parser/genbank.py` & `pycirclize-0.4.0/src/pycirclize/parser/genbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import bz2
 import gzip
 import zipfile
 from collections import defaultdict
-from functools import lru_cache
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
 from Bio.SeqFeature import FeatureLocation, Seq, SeqFeature
@@ -130,15 +129,14 @@
 
     @property
     def genome_seq(self) -> str:
         """Range genome sequence"""
         seq = "".join(str(r.seq) for r in self.records)
         return seq[self.min_range : self.max_range]
 
-    @lru_cache(maxsize=None)
     def calc_genome_gc_content(self) -> float:
         """Calculate genome GC content"""
         try:
             gc_content = SeqUtils.gc_fraction(self.genome_seq) * 100
         except AttributeError:
             # For backward compatibility, biopython <= 1.79
             gc_content = SeqUtils.GC(self.genome_seq)
```

### Comparing `pycirclize-0.3.1/src/pycirclize/parser/gff.py` & `pycirclize-0.4.0/src/pycirclize/parser/gff.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,43 +106,54 @@
             GFF target seqid
 
         Returns
         -------
         gff_records, start, end : tuple[list[GffRecord], int, int]
             GFF record list, start, end
         """
+        # Parse GFF lines
         gff_all_lines = handle.read().splitlines()
         gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
         gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
         if len(gff_records) == 0:
             err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
             raise ValueError(err_msg)
 
+        # Get target seqid & GFF records
         seqid_list = list(dict.fromkeys([rec.seqid for rec in gff_records]))
-        self._seqid_list = seqid_list
         if target_seqid is None:
             target_seqid = seqid_list[0]
-        self._target_seqid = target_seqid
         if target_seqid not in seqid_list:
             err_msg = f"Not found {target_seqid=} in '{self._gff_file}'"
             raise ValueError(err_msg)
-        gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
+        target_gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
 
         # Try to get start-end region from '##sequence-region' annotation line
-        start, end = None, None
-        for line in gff_all_lines:
-            if line.startswith("##sequence-region") and target_seqid in line:
-                if len(line.split()) == 4:
-                    start, end = line.split()[2:4]
-                    start, end = int(start) - 1, int(end)
-                    break
-        if start is None or end is None:
-            start, end = 0, max([r.end for r in gff_records])
+        # If not found, (0, max_coordinate) is set as start-end
+        seqid2start_end: dict[str, tuple[int, int]] = {}
+        for seqid in seqid_list:
+            start, end = None, None
+            for line in gff_all_lines:
+                if line.startswith("##sequence-region") and seqid in line:
+                    if len(line.split()) == 4:
+                        start, end = line.split()[2:4]
+                        start, end = int(start) - 1, int(end)
+                        break
+            if start is None or end is None:
+                start, end = 0, max([r.end for r in target_gff_records])
+            seqid2start_end[seqid] = (start, end)
+        seqid2size = {seqid: e - s for seqid, (s, e) in seqid2start_end.items()}
+
+        # Set properties
+        self._target_seqid = target_seqid
+        self._seqid_list = seqid_list
+        self._all_records = gff_records
+        self._seqid2size = seqid2size
 
-        return gff_records, start, end
+        return target_gff_records, *seqid2start_end[target_seqid]
 
     @property
     def name(self) -> str:
         """Name"""
         if self._name is not None:
             return self._name
         if self._gff_file.suffix in (".gz", ".bz2", ".zip"):
@@ -156,18 +167,23 @@
 
         If `##sequence-region` pragma is not found, seq_region=`(0, max_coords_value)`
         """
         return self._seq_region
 
     @property
     def records(self) -> list[GffRecord]:
-        """GFF records"""
+        """GFF records (target seqid only)"""
         return self._records
 
     @property
+    def all_records(self) -> list[GffRecord]:
+        """All GFF records"""
+        return self._all_records
+
+    @property
     def records_within_range(self) -> list[GffRecord]:
         """GFF records within min-max range"""
         target_gff_records: list[GffRecord] = []
         for rec in self.records:
             if rec.is_within_range(self.min_range, self.max_range):
                 target_gff_records.append(rec)
         return target_gff_records
@@ -191,19 +207,15 @@
         """Get seqid & complete/contig/scaffold genome size dict
 
         Returns
         -------
         seqid2size : dict[str, int]
             seqid & genome size dict
         """
-        seqid2size: dict[str, int] = {}
-        for seqid in self.seqid_list:
-            gff = Gff(self._gff_file, target_seqid=seqid)
-            seqid2size[seqid] = gff.range_size
-        return seqid2size
+        return self._seqid2size
 
     def get_seqid2features(
         self,
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
         pseudogene: bool | None = False,
     ) -> dict[str, list[SeqFeature]]:
@@ -222,20 +234,25 @@
             If None, extract regardless of pseudogene tag.
 
         Returns
         -------
         seqid2features : dict[str, list[SeqFeature]]
             seqid & features dict
         """
-        seqid2features = {}
+        gff_records = GffRecord.filter_records(
+            self.all_records,
+            feature_type=feature_type,
+            target_strand=target_strand,
+            pseudogene=pseudogene,
+        )
+        seqid2features: dict[str, list[SeqFeature]] = {}
         for seqid in self.seqid_list:
-            gff = Gff(self._gff_file, target_seqid=seqid)
-            seqid2features[seqid] = gff.extract_features(
-                feature_type, target_strand, pseudogene
-            )
+            seqid2features[seqid] = []
+        for rec in gff_records:
+            seqid2features[rec.seqid].append(rec.to_seq_feature())
         return seqid2features
 
     def extract_features(
         self,
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
         pseudogene: bool | None = False,
@@ -255,28 +272,21 @@
             If None, extract all regardless of pseudogene tag.
 
         Returns
         -------
         features : list[SeqFeature]
             Feature list
         """
-        features: list[SeqFeature] = []
-        for rec in self.records_within_range:
-            if feature_type is not None and rec.type != feature_type:
-                continue
-            if target_strand is not None and rec.strand != target_strand:
-                continue
-            has_pseudo_attr = "pseudo" in rec.attrs or "pseudogene" in rec.attrs
-            if (
-                pseudogene is None
-                or (pseudogene is True and has_pseudo_attr)
-                or (pseudogene is False and not has_pseudo_attr)
-            ):
-                features.append(rec.to_seq_feature())
-        return features
+        gff_records = GffRecord.filter_records(
+            self.records_within_range,
+            feature_type=feature_type,
+            target_strand=target_strand,
+            pseudogene=pseudogene,
+        )
+        return [rec.to_seq_feature() for rec in gff_records]
 
     def extract_exon_features(self, feature_type: str = "mRNA") -> list[SeqFeature]:
         """Extract exon structure features within min-max range
 
         Extract exons based on `parent feature` and `exon` ID-Parent relation
 
         Parameters
@@ -461,7 +471,49 @@
         for attr in attrs:
             if attr != "" and "=" in attr:
                 key, value = attr.split("=")
                 attr_dict[key] = value.split(",")
         gff_elms[8] = attr_dict
 
         return GffRecord(*gff_elms)
+
+    @staticmethod
+    def filter_records(
+        gff_records: list[GffRecord],
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> list[GffRecord]:
+        """Filter GFF records (feature_type, strand, pseudogene)
+
+        Parameters
+        ----------
+        gff_records : list[GffRecord]
+            GFF records to be filterd
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...). If None, no filter.
+        target_strand : int | None, optional
+            Target strand. If None, no filter.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only filter.
+            If False, `pseudo=`, `pseudogene=` not tagged record only filter.
+            If None, no filter.
+
+        Returns
+        -------
+        filter_gff_records : list[SeqFeature]
+            Filtered GFF records
+        """
+        filter_gff_records = []
+        for rec in gff_records:
+            if feature_type is not None and rec.type != feature_type:
+                continue
+            if target_strand is not None and rec.strand != target_strand:
+                continue
+            has_pseudo_attr = "pseudo" in rec.attrs or "pseudogene" in rec.attrs
+            if (
+                pseudogene is None
+                or (pseudogene is True and has_pseudo_attr)
+                or (pseudogene is False and not has_pseudo_attr)
+            ):
+                filter_gff_records.append(rec)
+        return filter_gff_records
```

### Comparing `pycirclize-0.3.1/src/pycirclize/parser/matrix.py` & `pycirclize-0.4.0/src/pycirclize/parser/matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/patches.py` & `pycirclize-0.4.0/src/pycirclize/patches.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/sector.py` & `pycirclize-0.4.0/src/pycirclize/sector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import math
+from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 import numpy as np
 from matplotlib.patches import Patch
@@ -22,31 +23,35 @@
 
     def __init__(
         self,
         name: str,
         size: float,
         rad_lim: tuple[float, float],
         start_pos: float = 0,
+        clockwise: bool = True,
     ):
         """
         Parameters
         ----------
         name : str
             Sector name
         size : float
             Sector size
         rad_lim : tuple[float, float]
             Sector radian limit region
         start_pos : float, optional
             Sector start position
+        clockwise : bool, optional
+            Sector coordinate direction (clockwise or anti-clockwise).
         """
         self._name = name
         self._size = size
         self._rad_lim = rad_lim
         self._start_pos = start_pos
+        self._clockwise = clockwise
         self._tracks: list[Track] = []
 
         # Plot data and functions
         self._patches: list[Patch] = []
         self._plot_funcs: list[Callable[[PolarAxes], None]] = []
 
     ############################################################
@@ -90,14 +95,19 @@
 
     @property
     def deg_lim(self) -> tuple[float, float]:
         """Sector degree limit"""
         return tuple(map(math.degrees, self.rad_lim))
 
     @property
+    def clockwise(self) -> bool:
+        """Sector coordinate direction"""
+        return self._clockwise
+
+    @property
     def tracks(self) -> list[Track]:
         """Tracks in sector"""
         return self._tracks
 
     @property
     def patches(self) -> list[Patch]:
         """Plot patches"""
@@ -186,14 +196,16 @@
         -------
         rad : float
             Radian coordinate
         """
         if not self.start <= x <= self.end and not ignore_range_error:
             err_msg = f"{x=} is invalid range of '{self.name}' sector.\n{self}"
             raise ValueError(err_msg)
+        if not self.clockwise:
+            x = (self.start + self.end) - x
         size_ratio = self.rad_size / self.size
         x_from_start = x - self.start
         rad_from_start = x_from_start * size_ratio
         rad = min(self.rad_lim) + rad_from_start
         return rad
 
     def axis(self, **kwargs) -> None:
@@ -345,16 +357,16 @@
         x: float | None = None,
         r: float = 105,
         rotation: int | float | str | None = None,
         border_width: int = 0,
         label: str | None = None,
         label_pos: str = "bottom",
         label_margin: float = 0.1,
-        imshow_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        imshow_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot raster image
 
         This method is experimental. API may change in the future release.
 
         Parameters
         ----------
@@ -375,21 +387,24 @@
             Border width in pixel. By default, 0 is set (no border shown).
         label : str | None, optional
             Image label. If None, no label shown.
         label_pos : str, optional
             Label plot position (`bottom` or `top`)
         label_margin : float, optional
             Label margin
-        imshow_kws : dict[str, Any], optional
+        imshow_kws : dict[str, Any] | None, optional
             Axes.imshow properties
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(size=10, color="red", ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        imshow_kws = {} if imshow_kws is None else deepcopy(imshow_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Load image data
         if isinstance(img, str) and urlparse(img).scheme in ("http", "https"):
             im = Image.open(urlopen(img))
         elif isinstance(img, (str, Path)):
             im = Image.open(str(img))
         else:
             im = img
```

### Comparing `pycirclize-0.3.1/src/pycirclize/track.py` & `pycirclize-0.4.0/src/pycirclize/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
 
     @property
     def parent_sector(self) -> Sector:
         """Parent sector"""
         return self._parent_sector
 
     @property
+    def clockwise(self) -> bool:
+        """Track coordinate direction"""
+        return self.parent_sector.clockwise
+
+    @property
     def patches(self) -> list[Patch]:
         """Plot patches"""
         return self._patches
 
     @property
     def plot_funcs(self) -> list[Callable[[PolarAxes], None]]:
         """Plot functions"""
@@ -263,15 +268,15 @@
             If `r_lim` param is set by user, this option not works.
         **kwargs : dict, optional
             Patch properties (e.g. `fc="red", ec="blue", lw=1.0, ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
         """
         rad_rect_start = self.x_to_rad(start)
         rad_rect_end = self.x_to_rad(end)
-        rad = rad_rect_start if start < end else rad_rect_end
+        rad = min(rad_rect_start, rad_rect_end)
         width = abs(rad_rect_end - rad_rect_start)
         if r_lim is not None:
             if not min(self.r_lim) <= min(r_lim) < max(r_lim) <= max(self.r_lim):
                 raise ValueError(f"{r_lim=} is invalid track range.\n{self}")
             radr, height = (rad, min(r_lim)), max(r_lim) - min(r_lim)
         elif ignore_pad:
             radr, height = (rad, min(self.r_lim)), self.r_size
@@ -334,16 +339,16 @@
         *,
         tick_length: float = 2,
         outer: bool = True,
         show_bottom_line: bool = False,
         label_size: float = 8,
         label_margin: float = 0.5,
         label_orientation: str = "horizontal",
-        line_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        line_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot xticks & labels on user-specified position
 
         If you want to plot xticks and their position labels at regular intervals,
         it is recommended to use `track.xticks_by_interval()` instead.
 
         Parameters
@@ -360,21 +365,24 @@
             If True, show bottom line.
         label_size : float, optional
             Label size
         label_margin : float, optional
             Label margin size
         label_orientation : str, optional
             Label orientation (`horizontal` or `vertical`)
-        line_kws : dict[str, Any], optional
+        line_kws : dict[str, Any] | None, optional
             Patch properties (e.g. `dict(ec="red", lw=1, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(color="red", alpha=0.5, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        line_kws = {} if line_kws is None else deepcopy(line_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Check list length of x & labels
         labels = [""] * len(x) if labels is None else labels
         if len(x) != len(labels):
             err_msg = f"List length is not match ({len(x)=}, {len(labels)=})"
             raise ValueError(err_msg)
 
         # Plot xticks & labels
@@ -409,16 +417,16 @@
         outer: bool = True,
         show_bottom_line: bool = False,
         show_label: bool = True,
         label_size: float = 8,
         label_margin: float = 0.5,
         label_orientation: str = "horizontal",
         label_formatter: Callable[[float], str] | None = None,
-        line_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        line_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot xticks & position labels by user-specified interval
 
         `track.xticks_by_interval()` is high-level API function of `track.xticks()`.
         If you want to plot xticks and their labels in any position you like,
         use `track.xticks()` instead.
 
@@ -438,21 +446,24 @@
             Label size
         label_margin : float, optional
             Label margin size
         label_orientation : str, optional
             Label orientation (`horizontal` or `vertical`)
         label_formatter : Callable[[float], str] | None, optional
             User-defined function for label format. (e.g. `1000 -> '1.0 Kb'`)
-        line_kws : dict[str, Any], optional
+        line_kws : dict[str, Any] | None, optional
             Patch properties (e.g. `dict(ec="red", lw=1, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(color="red", alpha=0.5, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        line_kws = {} if line_kws is None else deepcopy(line_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Setup xtick positions
         x_list = []
         start_pos, end_pos = self.start - (self.start % interval), self.end + interval
         for x in np.arange(start_pos, end_pos, interval):
             if self.start <= x <= self.end:
                 x = int(x) if isinstance(interval, int) else float(x)
                 x_list.append(x)
@@ -484,16 +495,16 @@
         *,
         vmin: float = 0,
         vmax: float | None = None,
         side: str = "right",
         tick_length: float = 1,
         label_size: float = 8,
         label_margin: float = 0.5,
-        line_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        line_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot yticks & labels on user-specified position
 
         Parameters
         ----------
         y : list[int] | list[float] | np.ndarray
             Y coordinates
@@ -507,32 +518,38 @@
             Ticks side position (`right` or `left`)
         tick_length : float, optional
             Tick length (Degree unit)
         label_size : float, optional
             Label size
         label_margin : float, optional
             Label margin size
-        line_kws : dict[str, Any], optional
+        line_kws : dict[str, Any] | None, optional
             Patch properties (e.g. `dict(ec="red", lw=1, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(color="red", alpha=0.5, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        line_kws = {} if line_kws is None else deepcopy(line_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Check y, labels list length
         labels = [""] * len(y) if labels is None else labels
         if len(y) != len(labels):
             err_msg = f"List length is not match ({len(y)=}, {len(labels)=})"
             raise ValueError(err_msg)
         # Check side value
         if side not in ("right", "left"):
             raise ValueError(f"{side=} is invalid ('right' or 'left').")
         # Set vmax & check if y is in min-max range
         vmax = max(y) if vmax is None else vmax
         self._check_value_min_max(y, vmin, vmax)
+        # Temporarily set clockwise=True in this method
+        original_clockwise = self.clockwise
+        self.parent_sector._clockwise = True
 
         # Plot yticks & labels
         r = [self._y_to_r(v, vmin, vmax) for v in y]
         for r_pos, label in zip(r, labels):
             # Set plot properties
             x_tick_length = (self.size / self.deg_size) * tick_length
             x_label_margin = (self.size / self.deg_size) * label_margin
@@ -556,14 +573,17 @@
                 va = "center_baseline"
                 _text_kws = deepcopy(text_kws)
                 _text_kws.update(
                     dict(ha=ha, va=va, rotation_mode="anchor", size=label_size)
                 )
                 self.text(label, x_text, r_pos, ignore_range_error=True, **_text_kws)
 
+        # Restore clockwise to original value
+        self.parent_sector._clockwise = original_clockwise
+
     def grid(
         self,
         y_grid_num: int | None = 6,
         x_grid_interval: float | None = None,
         **kwargs,
     ) -> None:
         """Plot grid
@@ -820,16 +840,16 @@
         *,
         vmin: float | None = None,
         vmax: float | None = None,
         start: float | None = None,
         end: float | None = None,
         cmap: str | Colormap = "bwr",
         show_value: bool = False,
-        rect_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        rect_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot heatmap
 
         Parameters
         ----------
         data : np.ndarray
             Numpy 2d array matrix values
@@ -844,21 +864,24 @@
             End position for heatmap plot (x coordinate).
             If None, `track.end` is set.
         cmap : str | Colormap, optional
             Colormap (e.g. `viridis`, `Spectral`, `Reds`, `Greys`)
             <https://matplotlib.org/stable/tutorials/colors/colormaps.html>
         show_value : bool, optional
             If True, show data value on heatmap rectangle
-        rect_kws : dict[str, Any], optional
+        rect_kws : dict[str, Any] | None, optional
             Patch properties (e.g. `dict(ec="black", lw=0.5, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(size=6, color="red", ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        rect_kws = {} if rect_kws is None else deepcopy(rect_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Set default value for None properties
         vmin = np.min(data) if vmin is None else vmin
         vmax = np.max(data) if vmax is None else vmax
         start = self.start if start is None else start
         end = self.end if end is None else end
 
         # Calculate radius & x position range list of heatmap rectangle
@@ -904,17 +927,17 @@
         format: str = "newick",
         outer: bool = True,
         use_branch_length: bool = False,
         leaf_label_size: float = 0,
         innode_label_size: float = 0,
         leaf_label_margin: float = 0.5,
         label_formatter: Callable[[Clade], str] | None = None,
-        node_color_list: list[tuple[list[str], str]] = [],
-        line_kws: dict[str, Any] = {},
-        text_kws: dict[str, Any] = {},
+        node_color_list: list[tuple[list[str], str]] | None = None,
+        line_kws: dict[str, Any] | None = None,
+        text_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot tree
 
         It is recommended that the track(sector) size be the same as the number of
         leaf nodes in the tree, to make it easier to combine with `bar` and `heatmap`.
 
         Parameters
@@ -933,26 +956,30 @@
         innode_label_size : float, optional
             Internal node label size. By default, `size=0` (No display).
         leaf_label_margin : float, optional
             leaf node label margin size (Radius unit)
         label_formatter : Callable[[Clade], str] | None, optional
             User-defined label format function.
             (e.g. `lambda node: node.name.replace("_", " ")`)
-        node_color_list : list[tuple[list[str], str]]
+        node_color_list : list[tuple[list[str], str]] | None, optional
             Tree node & color setting list.
             If multi nodes are set, MRCA(Most Recent Common Ancestor) node of
             target nodes is set.
             (e.g. `[(["node1"], "red"), (["taxa1", "taxa2"], "blue"), ...]`)
-        line_kws : dict[str, Any], optional
+        line_kws : dict[str, Any] | None, optional
             Patch properties (e.g. `dict(ec="red", lw=1, ls="dashed", ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
-        text_kws : dict[str, Any], optional
+        text_kws : dict[str, Any] | None, optional
             Text properties (e.g. `dict(color="red", ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
+        node_color_list = [] if node_color_list is None else deepcopy(node_color_list)
+        line_kws = {} if line_kws is None else deepcopy(line_kws)
+        text_kws = {} if text_kws is None else deepcopy(text_kws)
+
         # Load tree data, set node names, set node colors
         tree = utils.TreeUtil.load_tree(treedata, format)
         tree = utils.TreeUtil.set_unique_node_name(tree)
         tree = utils.TreeUtil.set_node_color(tree, node_color_list)
         utils.TreeUtil.check_node_name_dup(tree)
         # If not `use_branch_length` or not branch length exists
         # Convert tree to ultrametric tree
```

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/__init__.py` & `pycirclize-0.4.0/src/pycirclize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/dataset.py` & `pycirclize-0.4.0/src/pycirclize/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/helper.py` & `pycirclize-0.4.0/src/pycirclize/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/images/python_logo.png` & `pycirclize-0.4.0/src/pycirclize/utils/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/plot.py` & `pycirclize-0.4.0/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/src/pycirclize/utils/tree.py` & `pycirclize-0.4.0/src/pycirclize/utils/tree.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/conftest.py` & `pycirclize-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/parser/test_genbank.py` & `pycirclize-0.4.0/tests/parser/test_genbank.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/parser/test_gff.py` & `pycirclize-0.4.0/tests/parser/test_gff.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/parser/test_matrix.py` & `pycirclize-0.4.0/tests/parser/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/test_circos.py` & `pycirclize-0.4.0/tests/test_circos.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,10 +82,10 @@
 
 def test_ax_property():
     """Test `circos.ax` property"""
     sectors = {"A": 10, "B": 20, "C": 15}
     circos = Circos(sectors)
     # Raise error before calling `circos.plotfig()` method
     with pytest.raises(ValueError):
-        circos.ax
+        assert circos.ax
     circos.plotfig()
-    circos.ax
+    assert circos.ax
```

### Comparing `pycirclize-0.3.1/tests/test_plot.py` & `pycirclize-0.4.0/tests/test_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,19 +323,19 @@
     assert fig_outfile.exists()
 
 
 def test_track_xticks_by_interval_plot(fig_outfile: Path):
     """Test `track.xticks_by_interval()`"""
     sectors = {"A": 10000000, "B": 20000000, "C": 15000000}
     circos = Circos(sectors, space=5)
+    mb_size = 1000000
     for sector in circos.sectors:
         # Major & Minor xticks
         track1 = sector.add_track((90, 100))
         track1.axis()
-        mb_size = 1000000
         track1.xticks_by_interval(mb_size, label_orientation="vertical")
         track1.xticks_by_interval(mb_size / 5, tick_length=1, show_label=False)
         # Mb formatted xticks
         track2 = sector.add_track((80, 90))
         track2.xticks_by_interval(
             mb_size,
             outer=False,
```

### Comparing `pycirclize-0.3.1/tests/test_sector.py` & `pycirclize-0.4.0/tests/test_sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/test_track.py` & `pycirclize-0.4.0/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_chr.bed` & `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv` & `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv` & `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gbk` & `pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gff` & `pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz` & `pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz` & `pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/tests/utils/test_dataset.py` & `pycirclize-0.4.0/tests/utils/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 
 @pytest.mark.skipif(
     condition=not check_network_conn(),
     reason="No network connection.",
 )
 def test_fetch_genbank_by_accid(tmp_path: Path):
+    """Test `fetch_genbank_by_accid()`"""
     accid = "JX128258.1"
     # Case1. Download as textio
     _ = fetch_genbank_by_accid(accid)
     # Case2. Download as file
     gbk_outfile = tmp_path / "out.gbk"
     fetch_genbank_by_accid(accid, gbk_outfile=gbk_outfile)
     assert gbk_outfile.exists()
```

### Comparing `pycirclize-0.3.1/tests/utils/test_helper.py` & `pycirclize-0.4.0/tests/utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.1/PKG-INFO` & `pycirclize-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycirclize
-Version: 0.3.1
+Version: 0.4.0
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
@@ -86,30 +86,30 @@
 # Initialize Circos sectors
 sectors = {"A": 10, "B": 15, "C": 12, "D": 20, "E": 15}
 circos = Circos(sectors, space=5)
 
 for sector in circos.sectors:
     # Plot sector name
     sector.text(f"Sector: {sector.name}", r=110, size=15)
-    # Create x positions & randomized y values
+    # Create x positions & random y values
     x = np.arange(sector.start, sector.end) + 0.5
     y = np.random.randint(0, 100, len(x))
-    # Plot line track
-    line_track = sector.add_track((80, 100), r_pad_ratio=0.1)
-    line_track.xticks_by_interval(interval=1)
-    line_track.axis()
-    line_track.line(x, y)
-    # Plot points track
-    points_track = sector.add_track((55, 75), r_pad_ratio=0.1)
-    points_track.axis()
-    points_track.scatter(x, y)
-    # Plot bar track
-    bar_track = sector.add_track((30, 50), r_pad_ratio=0.1)
-    bar_track.axis()
-    bar_track.bar(x, y)
+    # Plot lines
+    track1 = sector.add_track((80, 100), r_pad_ratio=0.1)
+    track1.xticks_by_interval(interval=1)
+    track1.axis()
+    track1.line(x, y)
+    # Plot points 
+    track2 = sector.add_track((55, 75), r_pad_ratio=0.1)
+    track2.axis()
+    track2.scatter(x, y)
+    # Plot bars
+    track3 = sector.add_track((30, 50), r_pad_ratio=0.1)
+    track3.axis()
+    track3.bar(x, y)
 
 # Plot links 
 circos.link(("A", 0, 3), ("B", 15, 12))
 circos.link(("B", 0, 3), ("C", 7, 11), color="skyblue")
 circos.link(("C", 2, 5), ("E", 15, 12), color="chocolate", direction=1)
 circos.link(("D", 3, 5), ("D", 18, 15), color="lime", ec="black", lw=0.5, hatch="//", direction=2)
 circos.link(("D", 8, 10), ("E", 2, 8), color="violet", ec="red", lw=1.0, ls="dashed")
```

