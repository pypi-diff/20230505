# Comparing `tmp/phot2lc-1.7.6.tar.gz` & `tmp/phot2lc-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phot2lc-1.7.6.tar", last modified: Tue May  2 21:53:35 2023, max compression
+gzip compressed data, was "phot2lc-1.7.7.tar", last modified: Thu May  4 22:31:15 2023, max compression
```

## Comparing `phot2lc-1.7.6.tar` & `phot2lc-1.7.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.6/LICENSE
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-02 21:53:35.460662 phot2lc-1.7.6/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.6/README.md
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-05-02 21:53:35.460662 phot2lc-1.7.6/setup.cfg
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-05-02 21:52:36.000000 phot2lc-1.7.6/setup.py
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/phot2lc/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.6/src/phot2lc/__init__.py
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2333 2023-05-02 21:50:55.000000 phot2lc-1.7.6/src/phot2lc/addstar
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.6/src/phot2lc/config.dat
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83856 2023-04-29 00:22:15.000000 phot2lc-1.7.6/src/phot2lc/phot2lc
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.6/src/phot2lc/photconfig
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.6/src/phot2lc/photfunc.py
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.6/src/phot2lc/quicklook
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.6/src/phot2lc/teledat.py
--rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.6/src/phot2lc/ucm_utils.py
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21475 2023-05-02 21:51:26.000000 phot2lc-1.7.6/src/phot2lc/version_history.txt
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.6/src/phot2lc/weldlc
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/phot2lc.egg-info/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/SOURCES.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/dependency_links.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/top_level.txt
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.7/LICENSE
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-04 22:31:15.757616 phot2lc-1.7.7/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.7/README.md
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-05-04 22:31:15.757616 phot2lc-1.7.7/setup.cfg
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-05-04 22:30:00.000000 phot2lc-1.7.7/setup.py
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/phot2lc/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.7/src/phot2lc/__init__.py
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2362 2023-05-04 22:29:04.000000 phot2lc-1.7.7/src/phot2lc/addstar
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.7/src/phot2lc/config.dat
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83643 2023-05-04 22:29:21.000000 phot2lc-1.7.7/src/phot2lc/phot2lc
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.7/src/phot2lc/photconfig
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.7/src/phot2lc/photfunc.py
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.7/src/phot2lc/quicklook
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.7/src/phot2lc/teledat.py
+-rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.7/src/phot2lc/ucm_utils.py
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21673 2023-05-04 22:30:42.000000 phot2lc-1.7.7/src/phot2lc/version_history.txt
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.7/src/phot2lc/weldlc
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/phot2lc.egg-info/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/top_level.txt
```

### Comparing `phot2lc-1.7.6/LICENSE` & `phot2lc-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/PKG-INFO` & `phot2lc-1.7.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.6
+Version: 1.7.7
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `phot2lc-1.7.6/README.md` & `phot2lc-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/setup.py` & `phot2lc-1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phot2lc",
-    version="1.7.6",
+    version="1.7.7",
     author="Zach Vanderbosch",
     author_email="zvanderbosch@gmail.com",
     description="Light curve extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zvanderbosch/phot2lc",
     packages=setuptools.find_packages('src'),
```

### Comparing `phot2lc-1.7.6/src/phot2lc/addstar` & `phot2lc-1.7.7/src/phot2lc/addstar`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 if len(match_idx) > 0:
     match_dat = star_dat.loc[match_idx].values[0]
     print('Object already in stars.dat file:')
     print(' ',*match_dat)
     exit()
 
 # If no match, add to file
-print(coord.to_string('hmsdms',sep=" "))
 ra_string = coord.to_string('hmsdms',sep=" ",precision=2)[0:11]
 de_string = coord.to_string('hmsdms',sep=" ",precision=2)[12:]
 new_line = "{}  {} {}\n".format(objectname,ra_string, de_string)
-print(new_line)
 with open(star_dat_file, 'a') as file:
-    file.write(new_line)
+    file.write(new_line)
+print('\nAdded "{:s}" entry to stars.dat file.\n'.format(
+    new_line.strip("\n"))
+)
```

### Comparing `phot2lc-1.7.6/src/phot2lc/phot2lc` & `phot2lc-1.7.7/src/phot2lc/phot2lc`

 * *Files 1% similar despite different names*

```diff
@@ -297,16 +297,26 @@
             if 'Start of column name definitions' in l:
                 start_row = i
             if (i == start_row+2):
                 colnames = l.split("=")[1].strip().split(" ")
             if l[0] == "#":
                 skip_rows.append(i)
 
-    df = pd.read_csv(phot_names[0],header=None,delim_whitespace=True,
-        names=colnames,skiprows=skip_rows)
+    df = pd.read_csv(
+        phot_names[0],
+        header=None,
+        delim_whitespace=True,
+        names=colnames,
+        skiprows=skip_rows
+    )
+
+    # Remove any rows containing NaN-valued counts
+    check_columns = [c for c in df.columns if "counts_" in c]
+    df = df.dropna(subset=check_columns).reset_index(drop=True)
+
     phot_data = [df]
 
 elif psource == 'ucm':
 
     # Load in the data
     skip_rows = []
     with open(phot_names[0]) as f:
@@ -324,14 +334,18 @@
     objColnames = ['naper','x','y','xm','ym','exm','eym','counts','countse',
     'sky','nsky','nrej','worst','flag']
 
     allobjColnames = [['{}_{}'.format(cname,x+1) for cname in objColnames] for x in range(Nphotobj)]
     colnames = baseColnames + list(itertools.chain.from_iterable(allobjColnames))
     df.columns = colnames
 
+    # Remove any rows containing NaN-valued counts
+    check_columns = [c for c in df.columns if "counts_" in c]
+    df = df.dropna(subset=check_columns).reset_index(drop=True)
+
     phot_data = [df]
 
 
 
           
 if psource == 'hsp':
     Nobj = len(phot_data[0].columns) - 1  # Number of stars (last column is sky)
@@ -805,16 +819,22 @@
     keep_ind = [i for i,x in enumerate(log_data[:,1]) if x == 1]
 
 # Create one version of the divided light curve without any deleted points
 dlc_init_all,_,_,_ = div_lc(time_stamps,phot_target,phot_comps,
                             polypack,list(range(Ndat)),[])
 
 # Create version with points deleted if specified
-dlc_init,dellc_init,draw_init,mod_init = div_lc(time_stamps,phot_target,phot_comps,
-                                                polypack,keep_ind,dele_ind)
+dlc_init, dellc_init, draw_init, mod_init = div_lc(
+    time_stamps,
+    phot_target,
+    phot_comps,
+    polypack,
+    keep_ind,
+    dele_ind
+)
 
 
 # Plot Light Curve
 p0, = bx_LC.plot(time_stamps[keep_ind],dlc_init,ls='-',c='w',lw=0.5,
                  marker='o',ms=3,mew=0.75,mec='w',mfc='w')
 # Show deleted points
 p1, = bx_LC.plot(time_stamps[dele_ind],dellc_init,ls='None',
@@ -1495,41 +1515,56 @@
         sys.exit(1)
 
     # Option to reprint the command list
     if event.key == '?':
         print_commands()
 
 # Setup the rectangle selectors, start them off as deactivated
-rect_garbage = dict(facecolor='#FFFF00',edgecolor = '#FFFF00',
-                    alpha=0.4, fill=True)
-rect_zoom = dict(facecolor='#6DA1F0',edgecolor = '#6DA1F0',
-                 alpha=0.4, fill=True)
-toggle_garbage.RS = RectangleSelector(bx_LC, garbage_select, 
-                                       props=rect_garbage,
-                                       useblit=True,
-                                       button=[1],  # Left click only
-                                       minspanx=5, minspany=5,
-                                       spancoords='pixels',
-                                       interactive=False)
-
-toggle_reverse_garbage.RS = RectangleSelector(bx_LC, reverse_garbage_select, 
-                                       props=rect_garbage,
-                                       useblit=True,
-                                       button=[1],  # Left click only
-                                       minspanx=5, minspany=5,
-                                       spancoords='pixels',
-                                       interactive=False)
-
-toggle_zoom.RS = RectangleSelector(bx_LC, zoom_select, 
-                                       props=rect_zoom,
-                                       useblit=True,
-                                       button=[1],  # Left click only
-                                       minspanx=5, minspany=5,
-                                       spancoords='pixels',
-                                       interactive=False)
+rect_garbage = dict(
+    facecolor='#FFFF00',
+    edgecolor = '#FFFF00',
+    alpha=0.4, 
+    fill=True
+)
+rect_zoom = dict(
+    facecolor='#6DA1F0',
+    edgecolor = '#6DA1F0',
+    alpha=0.4, 
+    fill=True
+)
+toggle_garbage.RS = RectangleSelector(
+    bx_LC, garbage_select, 
+    props=rect_garbage,
+    useblit=True,
+    button=[1],  # Left click only
+    minspanx=5, 
+    minspany=5,
+    spancoords='pixels',
+    interactive=False
+)
+toggle_reverse_garbage.RS = RectangleSelector(
+    bx_LC, reverse_garbage_select, 
+    props=rect_garbage,
+    useblit=True,
+    button=[1],  # Left click only
+    minspanx=5, 
+    minspany=5,
+    spancoords='pixels',
+    interactive=False
+)
+toggle_zoom.RS = RectangleSelector(
+    bx_LC, zoom_select, 
+    props=rect_zoom,
+    useblit=True,
+    button=[1],  # Left click only
+    minspanx=5, 
+    minspany=5,
+    spancoords='pixels',
+    interactive=False
+)
 toggle_garbage.RS.set_active(False)
 toggle_reverse_garbage.RS.set_active(False)
 toggle_zoom.RS.set_active(False)
 
 # Connect incoming events to event handlers
 cidb1 = figb.canvas.mpl_connect('key_press_event', on_event_b)
 plt.show()
```

### Comparing `phot2lc-1.7.6/src/phot2lc/photfunc.py` & `phot2lc-1.7.7/src/phot2lc/photfunc.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/src/phot2lc/quicklook` & `phot2lc-1.7.7/src/phot2lc/quicklook`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/src/phot2lc/teledat.py` & `phot2lc-1.7.7/src/phot2lc/teledat.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/src/phot2lc/ucm_utils.py` & `phot2lc-1.7.7/src/phot2lc/ucm_utils.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/src/phot2lc/version_history.txt` & `phot2lc-1.7.7/src/phot2lc/version_history.txt`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,20 @@
 
 
  Version 1.7.6 (2023-05-02)
 ---------------------------
 > Minor bug fixes in addstar
 
 
+ Version 1.7.7 (2023 May 4)
+---------------------------
+> Better handling of NaN values in HiPERCAM and 
+  ULTRACAM output.
+> Better information print out from the addstar 
+  command line function.
```

### Comparing `phot2lc-1.7.6/src/phot2lc/weldlc` & `phot2lc-1.7.7/src/phot2lc/weldlc`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.6/src/phot2lc.egg-info/PKG-INFO` & `phot2lc-1.7.7/src/phot2lc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.6
+Version: 1.7.7
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

