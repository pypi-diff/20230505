# Comparing `tmp/plot-antenna-1.1.tar.gz` & `tmp/plot-antenna-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.1.tar", last modified: Wed May  3 13:44:27 2023, max compression
+gzip compressed data, was "plot-antenna-1.2.tar", last modified: Fri May  5 19:04:30 2023, max compression
```

## Comparing `plot-antenna-1.1.tar` & `plot-antenna-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.677311 plot-antenna-1.1/
--rw-r--r--   0 ralf      (1000) priv      (1011)     9309 2023-05-03 13:44:27.677311 plot-antenna-1.1/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     7405 2023-05-03 13:41:51.000000 plot-antenna-1.1/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.649310 plot-antenna-1.1/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-03 13:44:00.000000 plot-antenna-1.1/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.1/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    47920 2023-05-03 13:32:42.000000 plot-antenna-1.1/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.669310 plot-antenna-1.1/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)     9309 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-03 13:44:27.677311 plot-antenna-1.1/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.1/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.673311 plot-antenna-1.1/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.1/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-05 19:04:30.617696 plot-antenna-1.2/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9911 2023-05-05 19:04:30.613696 plot-antenna-1.2/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7927 2023-05-05 19:01:31.000000 plot-antenna-1.2/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-05 19:04:30.585696 plot-antenna-1.2/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-05 19:03:56.000000 plot-antenna-1.2/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.2/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    48197 2023-05-05 18:55:35.000000 plot-antenna-1.2/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-05 19:04:30.605696 plot-antenna-1.2/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9911 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-05 19:04:30.000000 plot-antenna-1.2/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-05 19:04:30.617696 plot-antenna-1.2/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.2/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-05 19:04:30.609696 plot-antenna-1.2/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.2/test/test_plot.py
```

### Comparing `plot-antenna-1.1/PKG-INFO` & `plot-antenna-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.1
+Version: 1.2
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -25,15 +25,16 @@
         far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
         graphic that can be rotated and zoomed). It supports a local display
         program (using matplotlib_) and a HTML output version that displays
         everything using javascript (using plotly_). The program features a
         ``--help`` option. If the program called with ``--help`` does not
         display a ``-H`` or ``--export-html`` option, you most likely do not
         have a recent version of plotly_ installed. In that case only the
-        matplotlib_ variant is available.
+        matplotlib_ variant is available. For the plotly variant to work you
+        need both, a recent version of plotly_ as well as pandas_ installed.
         
         The program started out as a companion-program to my pymininec_
         project and is now an independent program.
         
         The plot program can also display output files of nec2c_, not only
         from pymininec_.
         
@@ -147,18 +148,27 @@
             http://on5au.be/Books/allmodnotes.zip
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
         .. _pymininec: https://github.com/schlatterbeck/pymininec
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
+        .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.2: Allow specification of title (legend) font size in plotly version
+        
+        - For some application (e.g. when using the plotly graphics inside a
+          html iframe) the title (or we may want to call it legend) of the
+          graphics may collide with the graphics itself. We can now specify the
+          font size with ``--title-font-size``. This option currently works only
+          with plotly graphics.
+        
         v1.1: Specification of azimuth / elevation angle
         
         - Now we can specify an azimuth angle for elevation plot and an
           elevation angle for azimuth plots
         - Bug-fix in computation of maximum gain azimuth direction: If the
           maximum gain in theta direction goes up or down, the azimuth angle
           would be computed incorrectly because all gain values at that theta
```

### Comparing `plot-antenna-1.1/README.rst` & `plot-antenna-1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
 graphic that can be rotated and zoomed). It supports a local display
 program (using matplotlib_) and a HTML output version that displays
 everything using javascript (using plotly_). The program features a
 ``--help`` option. If the program called with ``--help`` does not
 display a ``-H`` or ``--export-html`` option, you most likely do not
 have a recent version of plotly_ installed. In that case only the
-matplotlib_ variant is available.
+matplotlib_ variant is available. For the plotly variant to work you
+need both, a recent version of plotly_ as well as pandas_ installed.
 
 The program started out as a companion-program to my pymininec_
 project and is now an independent program.
 
 The plot program can also display output files of nec2c_, not only
 from pymininec_.
 
@@ -139,18 +140,27 @@
     http://on5au.be/Books/allmodnotes.zip
 .. _`Antenna modelling notes episode 48`:
     http://on5au.be/content/amod/amod48.html
 .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
 .. _pymininec: https://github.com/schlatterbeck/pymininec
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
+.. _pandas: https://pandas.pydata.org/
 
 Release Notes
 -------------
 
+v1.2: Allow specification of title (legend) font size in plotly version
+
+- For some application (e.g. when using the plotly graphics inside a
+  html iframe) the title (or we may want to call it legend) of the
+  graphics may collide with the graphics itself. We can now specify the
+  font size with ``--title-font-size``. This option currently works only
+  with plotly graphics.
+
 v1.1: Specification of azimuth / elevation angle
 
 - Now we can specify an azimuth angle for elevation plot and an
   elevation angle for azimuth plots
 - Bug-fix in computation of maximum gain azimuth direction: If the
   maximum gain in theta direction goes up or down, the azimuth angle
   would be computed incorrectly because all gain values at that theta
```

### Comparing `plot-antenna-1.1/plot_antenna/plot_antenna.py` & `plot-antenna-1.2/plot_antenna/plot_antenna.py`

 * *Files 0% similar despite different names*

```diff
@@ -795,14 +795,16 @@
             )
         fig.add_trace (go.Scatterpolar (**df))
         if self.plotly_lastfig:
             desc = '<br>'.join (self.desc [0:2] + self.desc [3:])
             # don't use fig.update_layout (title = desc) which will
             # delete title attributes
             fig.layout.title.text = desc
+            if self.args.title_font_size:
+                fig.layout.title.font.size = self.args.title_font_size
             lbl_deg = self.lbl_deg or 0
             tickangle = 90
             if lbl_deg > 180:
                 tickangle = -90
             fig.layout.polar.radialaxis.tickangle = tickangle
             fig.layout.polar.radialaxis.angle = lbl_deg
 # Trying to display 'X' and 'Y' on Azimuth plot
@@ -1241,14 +1243,19 @@
         )
     cmd.add_argument \
         ( '--plot-vswr', '--swr', '--vswr', '--plot-swr'
         , help    = 'Plot voltage standing wave ratio (VSWR)'
         , action  = 'store_true'
         )
     cmd.add_argument \
+        ( '--title-font-size'
+        , help    = 'Title/legend font size (currently only used in plotly)'
+        , type    = int
+        )
+    cmd.add_argument \
         ( '--wireframe'
         , help    = 'Show 3d plot as a wireframe (not solid)'
         , action  = 'store_true'
         )
     if px is not None:
         cmd.add_argument \
             ( "-H", "--export-html"
```

### Comparing `plot-antenna-1.1/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.2/plot_antenna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.1
+Version: 1.2
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -25,15 +25,16 @@
         far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
         graphic that can be rotated and zoomed). It supports a local display
         program (using matplotlib_) and a HTML output version that displays
         everything using javascript (using plotly_). The program features a
         ``--help`` option. If the program called with ``--help`` does not
         display a ``-H`` or ``--export-html`` option, you most likely do not
         have a recent version of plotly_ installed. In that case only the
-        matplotlib_ variant is available.
+        matplotlib_ variant is available. For the plotly variant to work you
+        need both, a recent version of plotly_ as well as pandas_ installed.
         
         The program started out as a companion-program to my pymininec_
         project and is now an independent program.
         
         The plot program can also display output files of nec2c_, not only
         from pymininec_.
         
@@ -147,18 +148,27 @@
             http://on5au.be/Books/allmodnotes.zip
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
         .. _pymininec: https://github.com/schlatterbeck/pymininec
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
+        .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.2: Allow specification of title (legend) font size in plotly version
+        
+        - For some application (e.g. when using the plotly graphics inside a
+          html iframe) the title (or we may want to call it legend) of the
+          graphics may collide with the graphics itself. We can now specify the
+          font size with ``--title-font-size``. This option currently works only
+          with plotly graphics.
+        
         v1.1: Specification of azimuth / elevation angle
         
         - Now we can specify an azimuth angle for elevation plot and an
           elevation angle for azimuth plots
         - Bug-fix in computation of maximum gain azimuth direction: If the
           maximum gain in theta direction goes up or down, the azimuth angle
           would be computed incorrectly because all gain values at that theta
```

### Comparing `plot-antenna-1.1/setup.py` & `plot-antenna-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `plot-antenna-1.1/test/test_plot.py` & `plot-antenna-1.2/test/test_plot.py`

 * *Files identical despite different names*

