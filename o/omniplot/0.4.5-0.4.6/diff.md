# Comparing `tmp/omniplot-0.4.5.tar.gz` & `tmp/omniplot-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.4.5.tar", last modified: Fri Apr 28 23:49:20 2023, max compression
+gzip compressed data, was "omniplot-0.4.6.tar", last modified: Fri May  5 07:34:25 2023, max compression
```

## Comparing `omniplot-0.4.5.tar` & `omniplot-0.4.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/
--rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.5/LICENSE
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-28 23:49:20.878973 omniplot-0.4.5/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-04-22 04:16:47.000000 omniplot-0.4.5/README.md
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/
--rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/_adjustText.py
--rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-28 23:42:17.000000 omniplot-0.4.5/omniplot/_version.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/chipseq_utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/cython_utils/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/cython_utils/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/data.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   102103 2023-04-28 23:42:02.000000 omniplot-0.4.5/omniplot/heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/igraph_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/networkplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    20850 2023-04-28 23:24:22.000000 omniplot-0.4.5/omniplot/plot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/plot_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    73070 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/proportion.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/regressionplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scatter.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/scripts/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scripts/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scripts/gff2tss.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/statistics.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.5/omniplot/utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot.egg-info/
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)      711 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/SOURCES.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/dependency_links.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/requires.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/top_level.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-28 23:49:20.882972 omniplot-0.4.5/setup.cfg
--rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.5/setup.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/tests/
--rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.4.5/tests/test_chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.4.5/tests/test_network.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     5410 2023-04-28 23:42:02.000000 omniplot-0.4.5/tests/tests heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    13863 2023-04-28 23:22:23.000000 omniplot-0.4.5/tests/tests.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/
+-rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.6/LICENSE
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-05 07:34:25.484147 omniplot-0.4.6/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3392 2023-04-30 04:35:53.000000 omniplot-0.4.6/README.md
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/_adjustText.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-05-04 03:46:52.000000 omniplot-0.4.6/omniplot/_version.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/chipseq_utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/cython_utils/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/cython_utils/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/data.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   101567 2023-05-05 07:29:10.000000 omniplot-0.4.6/omniplot/heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/igraph_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/networkplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    24258 2023-04-30 04:35:53.000000 omniplot-0.4.6/omniplot/plot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/plot_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    74812 2023-05-04 02:23:00.000000 omniplot-0.4.6/omniplot/proportion.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/regressionplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scatter.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot/scripts/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scripts/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/scripts/gff2tss.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.6/omniplot/statistics.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.6/omniplot/utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/omniplot.egg-info/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)      711 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/requires.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-05-05 07:34:25.000000 omniplot-0.4.6/omniplot.egg-info/top_level.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-05-05 07:34:25.484147 omniplot-0.4.6/setup.cfg
+-rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.6/setup.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-05-05 07:34:25.484147 omniplot-0.4.6/tests/
+-rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.4.6/tests/test_chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.4.6/tests/test_network.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     5410 2023-04-29 06:16:08.000000 omniplot-0.4.6/tests/tests heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    14530 2023-05-05 07:21:22.000000 omniplot-0.4.6/tests/tests.py
```

### Comparing `omniplot-0.4.5/LICENSE` & `omniplot-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/PKG-INFO` & `omniplot-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.5
+Version: 0.4.6
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.5/README.md` & `omniplot-0.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 Known issues:<br>
 If you get errors saying "error: invalid command 'bdist_wheel'", please try pip install --upgrade pip wheel setuptools
 
 ## How to use
 I created jupyter notebooks to demonstrate the usage of omniplot [Link](https://github.com/koonimaru/omniplot/tree/main/ipynb).
 You can open jupyter notebooks with [jupyter lab](https://jupyterlab.readthedocs.io/en/stable/) or [VScode](https://code.visualstudio.com/).
 
-And you may want to visit an auto-generated [API](https://koonimaru.github.io/omniplot/). 
+And, I also write articles in [medium](https://medium.com/@koh.onimaru).
+
+A formal documation is under development, but you may want to visit an auto-generated [API](https://koonimaru.github.io/omniplot/). 
 
 ## Example usage
 ```python
 import pandas as pd
 from omniplot import plot as op
 import seaborn as  sns
 import matplotlib.pyplot as plt
```

### Comparing `omniplot-0.4.5/omniplot/__init__.py` & `omniplot-0.4.6/omniplot/__init__.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/_adjustText.py` & `omniplot-0.4.6/omniplot/_adjustText.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/chipseq.py` & `omniplot-0.4.6/omniplot/chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/chipseq_utils.py` & `omniplot-0.4.6/omniplot/chipseq_utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/heatmap.py` & `omniplot-0.4.6/omniplot/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1146,15 +1146,16 @@
                 size_format: str="",
                 rowplot_format: str="{x:.1f}",
                 colplot_format:  str="{x:.1f}",
                 
                 boxlabels: bool=False,
                 box_textwidth: Optional[int]=None,
                 box_max_lines: Optional[int]=None,
-                n_jobs=-1,
+                n_jobs: int=-1,
+                show_values: bool=False
                 ):
     """
     Drawing a heatmap. The function is mostly overlapping with the complex_clustermap, but has more flexibility, but may be slower.
     The main difference is this heatmap uses patch collections instead of pcolormech.  
     
     Parameters
     ----------
@@ -1325,18 +1326,15 @@
         return size_scale*((x-smin)/(smax-smin))
     def _reverse_size(x, size_scale, smin, smax):
         return (x/size_scale-0.01)*(smax-smin)+smin
     
     margin=0.00
     sns.set_theme(style="white",font="Arial",font_scale=1.1)
     TBLR=['top','bottom','left','right']
-
-
-    # Separating values into heatmap colors, sizes, ans category
-    
+    # Separating values into heatmap colors, sizes, ans category    
     lut={}
     if dtype=="numerical":
         (df, X, category, rowlabels, collabels, 
         Xsize, size_title, cunit, lut)=_process_vdata(df, variables, category,
                                                         row,  col,rowlabels, 
                                                         sizes, size_title, 
                                                         colors, lut,fillna,ztranform,cunit)
@@ -1360,36 +1358,32 @@
     colplot_num=len(col_colors)+len(col_plot)+\
         len(col_scatter)+len(col_bar)+col_axis+\
         int(clustering_method=="kmeans" and col_cluster==True)+int(clustering_method=="kmodes" and col_cluster==True)
     Xshape=X.shape
     if np.sum(Xshape)>200:
         edgecolor=None
     show_legend=int(rowplot_num>0 or type(Xsize)!=type(None))
-    
 
     if len(figsize)==0:
         figure_height=np.amin([np.amax([X.shape[0]/5, 3]), 10])
         if show_legend>0:
-            # figure_width=np.amax([figure_height*X.shape[1]/X.shape[0], 4])+1
             figure_width=figure_height*X.shape[1]/X.shape[0]+1
             figure_width=np.amin([np.amax([figure_height*X.shape[1]/X.shape[0]+1+int(boxlabels)*6, 5]), 10])
         else:
-            # figure_width=np.amax([figure_height*X.shape[1]/X.shape[0], 4])
             figure_width=figure_height*X.shape[1]/X.shape[0]+int(boxlabels)*6
         figsize=[figure_width,figure_height,]
     print("figsize: ", figsize)
     fig=plt.figure(figsize=figsize, layout='constrained')
     
     # determining the size and positionn of axes
     if col_ticklabels==True:
         lmax = float(np.amax(list(map(len, list(collabels.astype(str)))))) 
         lmax=np.amin([lmax/150, 0.3])
     else:
         lmax=0
-    # print(lmax)
 
     if boxlabels==True:
         row_ticklabels=False
 
     xori=0.05
     yori=0.11+lmax
     lcatw=0.04
@@ -1409,28 +1403,27 @@
     if col_cluster==True:
         ltreeh=0.75-lmax
         ttreeh=0.05
     else:
         ltreeh=0.8-lmax
         ttreeh=0
     if ttreew<0:
-        raise Exception("Too many things to plot. Please reduce the number of row-wise plots.")
+        raise Exception("Too many things to plot. \
+                        Please reduce the number of \
+                        row-wise plots.")
     hmapw=ttreew
     hmaph=ltreeh
     lcatx=xori+ltreew
     tcaty=yori+ltreeh
     tcath=0.025
 
     hmapx=xori+ltreew+lcatw*rowplot_num
     ttreey=yori+ltreeh+tcath*colplot_num
     legendh=(3/Xshape[0])*hmaph
     
-    # print([xori,ltreew,hmapw,legendw])
-    
-
     size_legend_num=3
     size_legend_elements=[]
     if type(Xsize)!=type(None):
         smin=np.amin(Xsize)
         smax=np.amax(Xsize)
         _scaled=_scale_size(Xsize,1, smin, smax)
         vmin, vmax=np.amin(_scaled), np.amax(_scaled)
@@ -1442,26 +1435,24 @@
                 size_format="{x:.2f}"
             elif 0<np.abs(vmax)<=1 or 1000<np.abs(vmax):
                 size_format="{x:.3E}"
         sx=1
         _sx=vmax*(hmaph/legendw)*size_legend_num/Xshape[1]
         _sy=vmax*(hmaph/legendh)*size_legend_num/Xshape[0]
         _sy=200
-        # print("_sy", _sy)
         size_legend_elements.append(Rectangle((0 -0.5,0-0.5), 1, size_legend_num))
 
         size_labels=[]
         prev_top=0
         for _i in range(size_legend_num):
             s=vmin+_i*vinterval
             if s <0.1:
                 s=0.1
             sx=s*(hmapw/legendw)/Xshape[1]
             sy=s*(hmaph/legendh)*size_legend_num/Xshape[0]
-            # print(sx, sy)
             
             if prev_top==0:
                 _yh=0
             else:
                 _yh=prev_top+sy
             if shape=="by_category":
                 size_legend_elements.append(_create_polygon("circle", 0, _i, sx,ry=sy))
@@ -1530,14 +1521,15 @@
             for i, (kclass, label) in enumerate(zip(_klabels, rowlabels)):
                 if not kclass in rclusters:
                     rclusters[kclass]=[]
                 rclusters[kclass].append(label)
 
     else:
         sortindexr=np.arange(len(rowlabels))
+
     # Column-wise clustering 
     if col_cluster==True:
         
         if clustering_method=="hierarchical":
             ax1=fig.add_axes([hmapx,ttreey,ttreew,ttreeh])
             X, Xsize, Zt, collabels, cclusters,=_dendrogram(X, 
                                                                     Xsize, ax1,collabels,
@@ -1611,17 +1603,15 @@
                                            plotkw, scatterkw, barkw, catnum, ax_dict,row_axis=row_axis)
     legend_elements_dict, catnum, axis_dict=_col_plot(sortindexc, fig, col_colors, col_plot, 
                                             col_scatter, col_bar, 
                                             colplot_format,
                                             legend_elements_dict, 
                                             Xshape, tcaty,tcath,hmapx,
                                             hmapw, margin, plotkw, scatterkw, barkw, catnum, axis_dict, col_axis=col_axis)
-    
     # Creating the heatmap
-
     # Calculating the maximum and minum values of the data if the data is numerical.
     if dtype=="numerical":
         cmap=plt.get_cmap(palette)
         Xmin=np.amin(X)
         Xmax=np.amax(X)
     if len(shape_colors)>0:
         cmap=plt.get_cmap(palette)
@@ -1644,17 +1634,14 @@
                 _shape_legend_elements={"ao":[],"labels":[],"handler":{}}
                 for _cat, _shape in _shape_lut.items():
                     ao=_AnyObject()
                     obshape=_AnyObjectHandler(facecolor="black", shape=_shape,label=_cat)
                     _shape_legend_elements["ao"].append(ao)
                     _shape_legend_elements["labels"].append(_cat)
                     _shape_legend_elements["handeler"][ao]=obshape
-                    # legend_elements.append(Line2D([0], [0], marker="s", linewidth=0, markeredgecolor="darkgray",
-                                        # label=_cat,
-                                        # markerfacecolor=_color))
                 shape_legend_elements["categorical"]=_shape_legend_elements
             else:
                 _uniq_labels=np.unique(X.flatten())
                 _cmap=plt.get_cmap(cpalette, len(_uniq_labels)+2)
                 _color_lut={u: _cmap(i+1) for i, u in enumerate(_uniq_labels)}
                 
                 legend_elements=[]
@@ -1663,16 +1650,14 @@
                                         label=_cat,
                                         markerfacecolor=_color))
                 legend_elements_dict["categorical"]=legend_elements
         else:
             for i in range(Xshape[1]):
                 __X=X[:,i]
                 _uniq_labels=np.unique(__X)
-                # print(colormap_list[i+int(row_cluster)+int(col_cluster)], _uniq_labels)
-                
                 if shape=="by_category":
                     _shape_legend_elements={"ao":[],"labels":[],"handler":{}}
                     _shape_tmp_lut={u: shape_list[i] for i, u in enumerate(_uniq_labels)}
                     for _cat, _shape in _shape_tmp_lut.items():
                         ao=_AnyObject()
                         obshape=_AnyObjectHandler(facecolor="black", shape=_shape)
                         _shape_legend_elements["ao"].append(ao)
```

### Comparing `omniplot-0.4.5/omniplot/igraph_classes.py` & `omniplot-0.4.6/omniplot/igraph_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/networkplot.py` & `omniplot-0.4.6/omniplot/networkplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/plot.py` & `omniplot-0.4.6/omniplot/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -556,20 +556,105 @@
             
         elif orientation=="vertical":
             _yl=np.concatenate([[minx], xinterval, [maxx]])
             _yr=np.concatenate([[minx], xinterval, [maxx]])
             xr=np.concatenate([[i], i+estimate, [i]])
             xl=np.concatenate([[i], i-estimate, [i]])
             ax.fill(xl, _yl, xr,_yr, color=vc )
-            ax.plot([i,i], [q1, q3], lw=10,color=box_color)
+            #ax.plot([i,i], [q1, q3], lw=10,color=box_color)
+            ax.fill([i, i-0.05, i-0.05, i+0.05, i+0.05,i], [q1, q1, q3, q3,q1,q1], lw=10,color=box_color)
             
             ax.plot([i,i], [q1-iqr*1.5, q3+iqr*1.5],  lw=1,color=box_color)
             ax.plot([i-0.05,i+0.05], [q2, q2],  color="w")
             if show_points==True:
                 ax.scatter(i+0.5*np.random.uniform(size=X.shape[0])-0.25, X, color=point_color, **point_kw)
     if orientation=="horizontal":
         ax.set_yticks(np.arange(len(mat)), labels=xlabels)
     elif orientation=="vertical":
         ax.set_xticks(np.arange(len(mat)), labels=xlabels, rotation=90)
         plt.subplots_adjust(bottom=0.2)
+
+def _boxplot(df: Union[pd.DataFrame, np.ndarray], 
+                 x: str="", 
+                 y: str="", 
+                 xlabels: list=[],
+                 order: list=[], 
+                 ax: plt.Axes=None,
+                 orientation: str="vertical",
+                 show_points: bool=True,
+                 point_color: str="blue",
+                 box_color: str="black",
+                 violine_color: Union[str,list, dict]="gray",
+                 point_kw={"s":10},
+                 scale_prop=False):
+    if ax==None:
+        fig, ax=plt.subplots()
+    if type(df)==pd.DataFrame:
+        if len(order)!=0:
+            dfs = {_s: _x[y].values for _s, _x in df.groupby(x)}
+            mat=[dfs[_s] for _s in order]
+            xlabels=order
+        else:
+            mat = []
+            xlabels=[]
+            for _s, _x in df.groupby(x):
+                mat.append(_x[y].values)
+                xlabels.append(_s)
+    else:
+        mat=np.array(df)
+    
+    proportion=np.array([np.sum(mat[i]) for i in range(len(mat))])
+    proportion=proportion/np.sum(proportion)
+    for i in range(len(mat)):
+        X=mat[i]
+        # print(X)
+        kde=stats.gaussian_kde(X)
+        q3, q1=np.quantile(X, 0.75), np.quantile(X, 0.25)
+        q2=np.quantile(X, 0.5)
+        iqr=q3-q1
+
+        minx, maxx=q1-iqr*1.5, q3+iqr*1.5
+        xinterval=np.linspace(minx,maxx, 100)
+        estimate=kde(xinterval)
+        if scale_prop==True:
+            estimate=proportion[i]*estimate/np.amax(estimate)
+        else:
+            estimate=0.5*estimate/np.amax(estimate)
+
+
+        if type(violine_color)==list:
+            vc=violine_color[i]
+        elif type(violine_color)==dict:
+            vc=xlabels[violine_color[i]]
+        elif type(violine_color)==str:
+            vc=violine_color
+        if orientation=="horizontal":
+            ax.fill_between(xinterval,i+estimate, i-estimate, color=vc)
+            ax.fill_between([q1, q3], [i-0.05,i-0.05], [i+0.05,i+0.05],color=box_color)
+            
+            ax.plot([q1-iqr*1.5, q3+iqr*1.5], [i,i], lw=1,color=box_color)
+            ax.plot([q2, q2], [i-0.05,i+0.05], color="w")
+            if show_points==True:
+                ax.scatter(X, i+0.5*np.random.uniform(size=X.shape[0])-0.25, color=point_color, **point_kw)
+            
+        elif orientation=="vertical":
+            _yl=np.concatenate([[minx], xinterval, [maxx]])
+            _yr=np.concatenate([[minx], xinterval, [maxx]])
+            xr=np.concatenate([[i], i+estimate, [i]])
+            xl=np.concatenate([[i], i-estimate, [i]])
+            ax.fill(xl, _yl, xr,_yr, color=vc )
+            #ax.plot([i,i], [q1, q3], lw=10,color=box_color)
+            ax.fill([i, i-0.05, i-0.05, i+0.05, i+0.05,i], [q1, q1, q3, q3,q1,q1], lw=10,color=box_color)
+            
+            ax.plot([i,i], [q1-iqr*1.5, q3+iqr*1.5],  lw=1,color=box_color)
+            ax.plot([i-0.05,i+0.05], [q2, q2],  color="w")
+            if show_points==True:
+                ax.scatter(i+0.5*np.random.uniform(size=X.shape[0])-0.25, X, color=point_color, **point_kw)
+    if orientation=="horizontal":
+        ax.set_yticks(np.arange(len(mat)), labels=xlabels)
+    elif orientation=="vertical":
+        ax.set_xticks(np.arange(len(mat)), labels=xlabels, rotation=90)
+        plt.subplots_adjust(bottom=0.2)
+
+
 if __name__=="__main__":
     pass
```

### Comparing `omniplot-0.4.5/omniplot/plot_classes.py` & `omniplot-0.4.6/omniplot/plot_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/proportion.py` & `omniplot-0.4.6/omniplot/proportion.py`

 * *Files 6% similar despite different names*

```diff
@@ -328,14 +328,15 @@
                     show_values_intact: bool=False,
                     show: bool=False,
                     figsize: List[int]=[],
                     xunit: str="",
                     yunit: str="",
                     title: str="",
                     hatch: bool=False,
+                    orientation: str="vertical",
                     rotation: int=90,
                     ax: Optional[plt.Axes]=None,
                     show_legend:bool=True,
                     bin_num: Union[dict, int]=10,
                     ylim: Optional[int]=None)-> Dict:
     
     """
@@ -525,21 +526,26 @@
     if type(palette)==str:
         cmap=plt.get_cmap(palette)
         
     ncols=len(x)*len(hue)-len(set(x)&set(hue))
     if ncols<1:
         ncols=1
     if len(figsize)==0:
-        figsize=[(4+0.1*meankey_len)*ncols, 6]
+        if orientation=="vertical":
+            figsize=[(4+0.1*meankey_len)*ncols, 6]
+        else:
+            figsize=[6, (3+0.1*meankey_len)*ncols]
     if ax!=None:
         axes=ax
         fig=None
     else:
-        fig, axes=plt.subplots(figsize=figsize,ncols=ncols)
-    
+        if orientation=="vertical":
+            fig, axes=plt.subplots(figsize=figsize,ncols=ncols)
+        else:
+            fig, axes=plt.subplots(figsize=figsize,nrows=ncols)
     if ncols==1:
         axes=[axes]
     else:
         axes=axes.flatten()
     
     if scale=="absolute":
         unit=""
@@ -561,90 +567,124 @@
             bottom=np.zeros([len(keys)])
             for i, h in enumerate(hues):
                 ax=axes[axindex]
                 
                 heights=np.array([data[_x][_hue][key][i] for key in keys])
                 
                 if type(palette)==dict:
-                    if hatch==True:
-                        ax.bar(keys, heights,width=0.5, bottom=bottom, color=palette[h], label=h, hatch=hatch_list[i])
-                    else:
-                        ax.bar(keys, heights,width=0.5, bottom=bottom, color=palette[h], label=h)
+                    _color=palette[h]
                 else:
-                    if hatch==True:
-                        ax.bar(keys, heights,width=0.5, bottom=bottom, color=cmap(i/len(hues)), label=h, hatch=hatch_list[i])
-                    else:
-                        ax.bar(keys, heights,width=0.5, bottom=bottom, color=cmap(i/len(hues)), label=h)
+                    _color=cmap(i/len(hues))
+                if hatch==True:
+                    _hatch=hatch_list[i]
+                else:
+                    _hatch=None
+                if orientation=="vertical":                    
+                    ax.bar(keys, heights,width=0.5, 
+                        bottom=bottom, 
+                        color=_color, 
+                        label=h, 
+                            hatch=_hatch)
+                elif orientation=="horizontal":
+                    ax.barh(keys, width=heights,height=0.5, 
+                        left=bottom, 
+                        color=_color, 
+                        label=h, 
+                            hatch=_hatch)
+                    
                 if show_values==True:
                     for j in range(len(keys)):
+                        if orientation=="vertical":        
+                            _tmpx, _tmpy=j,bottom[j]+heights[j]/2
+                        elif orientation=="horizontal":
+                            _tmpy, _tmpx=j,bottom[j]+heights[j]/2
+
                         if scale=="absolute":
-                            ax.text(j,bottom[j]+heights[j]/2,"{}{}".format(heights[j],unit), 
+                            ax.text(_tmpx, _tmpy,"{}{}".format(heights[j],unit), 
                                  bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
                         else:
-                            ax.text(j,bottom[j]+heights[j]/2,"{:.2f}{}".format(heights[j],unit), 
+                            ax.text(_tmpx, _tmpy,"{:.2f}{}".format(heights[j],unit), 
                                  bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
                 
                 pos[_x][_hue][h]={key: [he, bo] for key, he, bo in zip(keys, heights, bottom)}
                 bottom+=heights
             if len(keys)==1:
-                ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
-                ax.margins(x=1)
+                if orientation=="vertical":
+                    ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+                    ax.margins(x=1)
+                    ax.set_xlabel(_x)
+                elif orientation=="horizontal":
+                    ax.set_xticks(ax.get_yticks(), labels=keys, rotation=0)
+                    ax.margins(y=1)
+                    ax.set_ylabel(_x)
+
             else:
-                ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+                if orientation=="vertical":
+
+                    ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+                    ax.set_xlabel(_x)
+
+                elif orientation=="horizontal":
+                    ax.set_yticks(ax.get_yticks(), labels=keys, rotation=0)
+                    ax.set_ylabel(_x)
+
             #ax.set_xticklabels(ax.get_xticklabels(), rotation=90)
             if show_legend==True:
                 ax.legend(title=_hue,loc=[1.01,0])
-            ax.set_xlabel(_x)
+            
             if scale=="absolute":
                 ylabel="Counts"
             elif scale=="fraction":
                 ylabel="Fraction"
             elif scale=="percentage":
                 ylabel="Percentage"
-            ax.set_ylabel(ylabel)
+            if orientation=="vertical": 
+                ax.set_ylabel(ylabel)
+            elif orientation=="horizontal":
+                ax.set_xlabel(ylabel)
+            
             axindex+=1
             if len(pvals)>0 and _x in pvals:
                 
-                for _hue in hue:
-                    if _x==_hue:
-                        continue
-                    if not _hue in pos[_x]:
-                        continue
-                    hues=huekeys[_hue]
-                    for i, h in enumerate(hues):
-                        #print(pos)
-                        #print(pos[_x])
-                        _pos=pos[_x][_hue][h]
-                        for idx1, idx2, pval in pvals[_x][_hue][h]:
-                            
-                            he1, bot1=_pos[keys[idx1]]
-                            he2, bot2=_pos[keys[idx2]]
+                # for _hue in hue:
+
+                if _x==_hue:
+                    continue
+                if not _hue in pos[_x]:
+                    continue
+                hues=huekeys[_hue]
+                print(axindex,_hue, hues)
+                for i, h in enumerate(hues):
+                    _pos=pos[_x][_hue][h]
+                    for idx1, idx2, pval in pvals[_x][_hue][h]:
+                        he1, bot1=_pos[keys[idx1]]
+                        he2, bot2=_pos[keys[idx2]]
+                        if orientation=="vertical":
                             line, =ax.plot([idx1,idx2],[he1/2+bot1,he2/2+bot2],color="gray")
-                            # r1=ax.transData.transform([idx1, he1/2+bot1])
-                            # r2=ax.transData.transform([idx2, he2/2+bot2])
-                            r1=np.array([idx1, he1/2+bot1])
-                            r2=np.array([idx2, he2/2+bot2])
-                            r=r2-r1
-                            #print(ax.get_xlim(),ax.get_ylim())
-                            r=np.array([1,3])*r/np.array([ax.get_xlim()[1]-ax.get_xlim()[0],ax.get_ylim()[1]-ax.get_ylim()[0]])
-                            #r=ax.transData.transform(r)
-                            if idx2<idx1:
-                                r=-r
-                            #print(r)
-                            r=r*(r @ r)**(-0.5)
-                            #print(h,r)
-                            angle=np.arccos(r[0])
-                            if r[1]<0:
-                                angle= -angle
-                            #print(angle)
-                            if pval < 0.05:
-                                pval_str=str(np.round(-np.log10(pval), decimals=1))
-                            else:
-                                pval_str="ns"
+                        else:
+                            line, =ax.plot([he1/2+bot1,he2/2+bot2],[idx1,idx2],color="gray")
+                        # r1=np.array([idx1, he1/2+bot1])
+                        # r2=np.array([idx2, he2/2+bot2])
+                        # r=r2-r1
+                        # r=np.array([1,3])*r/np.array([ax.get_xlim()[1]-ax.get_xlim()[0],ax.get_ylim()[1]-ax.get_ylim()[0]])
+                        # if idx2<idx1:
+                        #     r=-r
+                        # r=r*(r @ r)**(-0.5)
+                        # angle=np.arccos(r[0])
+                        # if r[1]<0:
+                        #     angle= -angle
+                        #print(angle)
+                        if pval < 0.05:
+                            pval_str=str(np.round(-np.log10(pval), decimals=1))
+                        else:
+                            pval_str="ns"
+                        if orientation=="vertical":
                             _line_annotate( "mlp="+pval_str, line, (idx1+idx2)/2, color="magenta")
+                        else:
+                            _line_annotate( "mlp="+pval_str, line, (he1/2+bot1+he2/2+bot2)/2, color="magenta")
             if scale=="absolute" and ylim !=None:
                 ax.set_ylim(0, ylim)
 
     if len(x)==1 and len(hue)==1:
         plt.subplots_adjust(top=0.93,left=0.1,right=0.7, bottom=0.17)                            
     else:
         plt.tight_layout(w_pad=2)
@@ -669,20 +709,21 @@
                     unit: Union[str, List, Dict]="",
                     title: str="",
                     hatch: bool=False,
                     rotation: Optional[int]=None,
                     ax: Optional[plt.Axes]=None,
                     show_legend:bool=True,
                     ylim: Optional[int]=None,
+                    orientation: str="vertical",
                     horizontal: bool=False,
                     margins: dict={},
                     gridspec_kw: dict={},
                     legend_row_num: int=2,
-                    bar_width: float=0.75
-                    )-> Dict:
+                    bar_width: float=0.75,
+                    show_ticklabels: bool=True)-> Dict:
     
     """
     Drawing a stacked barplot by taking values as an input with or without the fisher's exact test. 
     
     Parameters
     ----------
     df : pandas DataFrame
@@ -743,14 +784,17 @@
     References
     ----------
     See Also
     --------
     Examples
     --------
     """
+    if horizontal==True:
+        orientation="horizontal"
+
     if type(df)==Dict:
         df=pd.DataFrame(df)
    
     pvals={}
     # if len(test_pairs) >0:
     #     print("mlp stands for -log10(p value)")
     #     for _hue in hue:
@@ -766,28 +810,28 @@
     #                 [yes_total-yes_and_hue, no_total-no_and_hue]]
 
     #         odd, pval=fisher_exact(table)
     #         pvals[_x][_hue][h].append([idx1, idx2, pval])
     
     
     if len(gridspec_kw)==0:
-        if horizontal==True:
+        if orientation=="horizontal":
             gridspec_kw=dict(top=0.75,left=0.25,right=0.9, bottom=0.17)
         else:
             gridspec_kw=dict(top=0.93,left=0.1,right=0.7, bottom=0.17)
 
     if len(margins)==0:
-        if horizontal==True and scale!="absolute":
+        if orientation=="horizontal" and scale!="absolute":
             margins=dict(x=0)
         else:
             margins=dict(x=0.1)
 
 
     if len(figsize)==0:
-        if horizontal==True:
+        if orientation=="horizontal":
             figsize=[6, len(df.index)/2]
         else:
             figsize=[len(df.columns)+1, 6]
     if ax!=None:
         fig=None
     else:
         fig, ax=plt.subplots(figsize=figsize,gridspec_kw=gridspec_kw)
@@ -820,15 +864,15 @@
     bottom=np.zeros([len(keys)])
     
     for i, col in enumerate(_df.columns):
         # print(col)
         heights=_df[col].values
         # print(heights,bottom)
         originalval=df[col].values
-        if horizontal==True:
+        if orientation=="horizontal":
             if type(palette)==dict:
                 if hatch==True:
                     ax.barh(keys, width=heights,height=bar_width, left=bottom, color=palette[col], label=col, hatch=hatch_list[i])
                 else:
                     ax.barh(keys, width=heights,height=bar_width, left=bottom, color=palette[col], label=col)
             else:
                 if hatch==True:
@@ -856,15 +900,15 @@
                         u=unit[k]
                     else:
                         u=""
                 elif type(unit)==list:
                     u=unit[j]
                 else:
                     u=unit
-                if horizontal==True:
+                if orientation=="horizontal":
                     if show_values_intact==True:
                         ax.text(bottom[j]+heights[j]/2, j,"{}{}".format(originalval[j],u), va="center",ha="center",
                                 bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
                     else:
                         ax.text(bottom[j]+heights[j]/2,j,"{:.2f}{}".format(heights[j],u), va="center",ha="center",
                                 bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
                 else:
@@ -877,46 +921,53 @@
                     
             
         pos[col]={key: [he, bo] for key, he, bo in zip(keys, heights, bottom)}
         bottom+=heights
     
     #ax.set_xticklabels(ax.get_xticklabels(), rotation=90)
     if show_legend==True:
-        if horizontal==True:
+        if orientation=="horizontal":
             ax.legend(loc=[0,1.01], ncols=len(_df.columns)//legend_row_num+int(len(_df.columns)%legend_row_num!=0))
         else:
             ax.legend(loc=[1.01,0])
-    if horizontal==True:
+    if orientation=="horizontal":
         if rotation==None:
             rotation=0
-
-        if len(keys)==1:
-            ax.set_yticks(ax.get_yticks(), labels=keys, rotation=rotation)
-            ax.margins(x=1)
+        if show_ticklabels==True:
+            if len(keys)==1:
+                ax.set_yticks(np.arange(len(keys)), labels=keys, rotation=rotation)
+                ax.margins(x=1)
+            else:
+                print(ax.get_yticks())
+                ax.set_yticks(np.arange(len(keys)), labels=keys, rotation=rotation)
         else:
-            ax.set_yticks(ax.get_yticks(), labels=keys, rotation=rotation)
+            ax.set_yticks([])
         ax.set_ylabel(ylabel)
         if xlabel =="":
             if show_values_intact==False:
                 if scale=="absolute":
                     xlabel="Counts"
                 elif scale=="fraction":
                     xlabel="Fraction"
                 elif scale=="percentage":
                     xlabel="Percentage"
         
         ax.set_xlabel(xlabel)
     else:
         if rotation==None:
             rotation=90
-        if len(keys)==1:
-            ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
-            ax.margins(x=1)
+        if show_ticklabels==True:
+
+            if len(keys)==1:
+                ax.set_xticks(np.arange(len(keys)), labels=keys, rotation=rotation)
+                ax.margins(x=1)
+            else:
+                ax.set_xticks(np.arange(len(keys)), labels=keys, rotation=rotation)
         else:
-            ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+            ax.set_xticks([])
         ax.set_xlabel(xlabel)
         if ylabel =="":
             if show_values_intact==False:
                 if scale=="absolute":
                     ylabel="Counts"
                 elif scale=="fraction":
                     ylabel="Fraction"
@@ -961,19 +1012,22 @@
     #                 if pval < 0.05:
     #                     pval_str=str(np.round(-np.log10(pval), decimals=1))
     #                 else:
     #                     pval_str="ns"
     #                 _line_annotate( "mlp="+pval_str, line, (idx1+idx2)/2, color="magenta")
     if scale=="absolute" and ylim !=None:
         ax.set_ylim(0, ylim)
-    if horizontal==True:
+    if orientation=="horizontal":
         ax.invert_yaxis()
 
-    if title !="" and fig !=None:
-        fig.suptitle(title)
+    if title !="":
+        if fig !=None:
+            fig.suptitle(title)
+        else:
+            plt.title(title)
     if show:
         plt.show()
     return {"pval":pvals,"axes":ax}
 
 def nice_piechart(df: pd.DataFrame, 
                   category: Union[str, List[str]],
                   palette: str="tab20c",
```

### Comparing `omniplot-0.4.5/omniplot/regressionplot.py` & `omniplot-0.4.6/omniplot/regressionplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/scatter.py` & `omniplot-0.4.6/omniplot/scatter.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/scripts/gff2tss.py` & `omniplot-0.4.6/omniplot/scripts/gff2tss.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/statistics.py` & `omniplot-0.4.6/omniplot/statistics.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot/utils.py` & `omniplot-0.4.6/omniplot/utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/omniplot.egg-info/PKG-INFO` & `omniplot-0.4.6/omniplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.5
+Version: 0.4.6
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.5/omniplot.egg-info/SOURCES.txt` & `omniplot-0.4.6/omniplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/setup.py` & `omniplot-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/tests/test_chipseq.py` & `omniplot-0.4.6/tests/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/tests/test_network.py` & `omniplot-0.4.6/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.5/tests/tests heatmap.py` & `omniplot-0.4.6/tests/tests heatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"],
     row_split=True, clustering_method="kmeans",
                category=["species", "island"],
                col_colors={"colors": ["bill","bill","flipper"]}, 
                row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3)
     op.heatmap(df=df, dtype="categorical", variables=["species", "island", "sex"],
                row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3,column_wise_color=True) 
-    # _df=df.sample(n=25, replace=False, random_state=1)
+    # _df=df.sample(n=50, replace=False, random_state=1)
     # _df=_df.reset_index(drop=True)
     # op.heatmap(df=_df, 
     # dtype="categorical", 
     # variables=["species", "island", "sex"],
     #            row_plot=["body_mass_g"], 
     #            shape="by_category", shape_colors=np.arange(25*3).reshape([25,3]),
     #            row_ticklabels=False,
```

### Comparing `omniplot-0.4.5/tests/tests.py` & `omniplot-0.4.6/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 test="decomp"
 test="manifold"
 test="triangle_heatmap"
 test="radialtree"
 test="violinplot"
 test="cluster"
 test="regression"
-
 test="dotplot"
 test="regression"
 test="nice_piechart_num"
 test="pie_scatter"
 test="correlation"
 test="manifold"
 test="stacked"
@@ -28,15 +27,16 @@
 test="cluster"
 test="nested_piechart"
 test="radialtree"
 test="scatterplot"
 test="stacked_num"
 test="complex_clustermap"
 test="volcanoplot"
-test="violinplot2"
+test="stacked_num"
+
 if test=="stackedlines":
     f="/media/koh/grasnas/home/data/omniplot/energy/owid-energy-data.csv"
     df=pd.read_csv(f)
     _df=df.loc[df["country"]=="Japan"]
     cols=['biofuel_consumption',
             'coal_consumption',
             'gas_consumption',
@@ -107,42 +107,58 @@
     #                                                                 ["Chinstrap","Gentoo","Adelie"],
     #                                                                 ["Dream","Biscoe","Torgersen"]],
     #                     test_pairs=[["Adelie","Gentoo"]], hatch=True)
     # op.stacked_barplot(df, x="species",
     #                     hue="sex", scale="percentage", hatch=True)
 
     df=sns.load_dataset("titanic")
-    op.stacked_barplot(df=df,x=["sex"],hue=["age","alone"], bin_num=10)
+    op.stacked_barplot(df=df,x=["sex"],
+                       hue=["age","alone"], 
+                       bin_num=10, 
+                       test_pairs=[["male", "female"]],
+                       orientation="vertical",
+                       scale="absolute")
 
     plt.show()
 elif test=="stacked_num": 
     """          　Bournemouth    Brighton
         Possession         36          64
         Shots              14          16
         Shots on Target     3           6
         Corners             5           5
         Fouls              11           5
     """
-    df=pd.DataFrame({"Bournemouth":[36,14,3,5,11],"Brighton":[64,16,6,5,5]}, index=["Possession","Shots","Shots on Target","Corners","Fouls"])
-    op.stacked_barplot_num(df=df,show_values_intact=True, 
-                           unit={"Possession":"%"}, 
-                           horizontal=True)
-    df=pd.read_csv("/media/koh/grasnas/home/data/omniplot/energy/owid-energy-data_curated_with_continents.csv")
-    df=df.loc[df["year"]==2021]
-    cols=["country","coal_consumption","gas_consumption","hydro_consumption","oil_consumption",
-          "nuclear_consumption","biofuel_consumption","solar_consumption","wind_consumption"]
-    df=df[cols]
-    df=df.reindex()
+    # fig, ax=plt.subplots()
+    # df=pd.DataFrame({"Bournemouth":[36,14,3,5,11],
+    # "Brighton":[64,16,6,5,5]}, 
+    # index=["Possession","Shots","Shots on Target","Corners","Fouls"])
+    # op.stacked_barplot_num(df=df,
+    # show_values_intact=True, 
+    #                        unit={"Possession":"%"}, 
+    #                        horizontal=True,
+    # ax=ax)
     
-    srt=np.argsort(np.array(df.sum(axis=1)))[::-1]
-    df=df.iloc[srt[:10]]
-    print(df)
-    op.stacked_barplot_num(df=df,x="country",show_values=False,# show_values_intact=True, 
-                           #unit={"Possession":"%"}, 
-                           horizontal=True,scale="absolute",xlabel="kwh",legend_row_num=4)
+    mat=np.concatenate([0.25*np.random.uniform(0,1,size=[10, 25]),0.5*np.random.uniform(0,1,size=[15, 25]),
+    np.random.uniform(0,1,size=[15, 25])])
+    mat=np.concatenate([mat, np.random.uniform(0,1,size=[40, 15])], axis=1)
+    _df=pd.DataFrame({"less":np.sum(mat<0.5, axis=1),"more":np.sum(mat>=0.5, axis=1)})
+    op.stacked_barplot_num(df=_df,orientation="horizontal")
+    # df=pd.read_csv("/media/koh/grasnas/home/data/omniplot/energy/owid-energy-data_curated_with_continents.csv")
+    # df=df.loc[df["year"]==2021]
+    # cols=["country","coal_consumption","gas_consumption","hydro_consumption","oil_consumption",
+    #       "nuclear_consumption","biofuel_consumption","solar_consumption","wind_consumption"]
+    # df=df[cols]
+    # df=df.reindex()
+    
+    # srt=np.argsort(np.array(df.sum(axis=1)))[::-1]
+    # df=df.iloc[srt[:10]]
+    # print(df)
+    # op.stacked_barplot_num(df=df,x="country",show_values=False,# show_values_intact=True, 
+    #                        #unit={"Possession":"%"}, 
+    #                        horizontal=True,scale="absolute",xlabel="kwh",legend_row_num=4)
     plt.show()
 
 elif test=="nice_piechart_num":
     f="/home/koh/ews/omniplot/data/energy_vs_gdp.csv"
     df=pd.read_csv(f, comment='#')
     df=df.set_index("country")
     op.nice_piechart_num(df, hue=['biofuel_electricity',
```

