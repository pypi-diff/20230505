# Comparing `tmp/DTCO-0.1.1.tar.gz` & `tmp/DTCO-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DTCO-0.1.1.tar", last modified: Fri Dec  9 10:48:32 2022, max compression
+gzip compressed data, was "DTCO-0.1.2.tar", last modified: Fri May  5 10:48:04 2023, max compression
```

## Comparing `DTCO-0.1.1.tar` & `DTCO-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 10:48:32.000000 DTCO-0.1.1/
-drwxrwxrwx   0        0        0        0 2022-12-09 10:48:32.000000 DTCO-0.1.1/DTCO.egg-info/
--rw-rw-rw-   0        0        0        1 2022-12-09 10:48:32.000000 DTCO-0.1.1/DTCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4273 2022-12-09 10:48:32.000000 DTCO-0.1.1/DTCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2022-12-09 10:48:32.000000 DTCO-0.1.1/DTCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2022-12-09 10:48:32.000000 DTCO-0.1.1/DTCO.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-09 10:48:32.000000 DTCO-0.1.1/GRO/
--rw-rw-rw-   0        0        0    37339 2022-12-09 09:18:25.000000 DTCO-0.1.1/GRO/classGRO.py
--rw-rw-rw-   0        0        0       51 2022-12-09 10:45:03.000000 DTCO-0.1.1/GRO/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 10:48:32.000000 DTCO-0.1.1/libMetric/
--rw-rw-rw-   0        0        0    48880 2022-12-09 07:56:38.000000 DTCO-0.1.1/libMetric/classLiberty.py
--rw-rw-rw-   0        0        0       63 2022-12-09 10:44:53.000000 DTCO-0.1.1/libMetric/__init__.py
--rw-rw-rw-   0        0        0     4273 2022-12-09 10:48:32.000000 DTCO-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2962 2022-12-09 09:23:17.000000 DTCO-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2022-12-09 10:48:32.000000 DTCO-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2022-12-09 10:48:12.000000 DTCO-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.144781 DTCO-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/DTCO.egg-info/
+-rw-rw-rw-   0        0        0     3478 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-05 10:48:04.000000 DTCO-0.1.2/DTCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/GRO/
+-rw-rw-rw-   0        0        0       51 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/__init__.py
+-rw-rw-rw-   0        0        0    37339 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/classGRO.py
+-rw-rw-rw-   0        0        0     2068 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/gro.py
+-rw-rw-rw-   0        0        0     1113 2023-05-05 05:23:41.000000 DTCO-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3478 2023-05-05 10:48:04.144781 DTCO-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3051 2023-05-05 09:10:11.000000 DTCO-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/copernic/
+-rw-rw-rw-   0        0        0       63 2023-05-05 07:07:04.000000 DTCO-0.1.2/copernic/__init__.py
+-rw-rw-rw-   0        0        0    29038 2023-05-05 07:45:01.000000 DTCO-0.1.2/copernic/classCPAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/libMetric/
+-rw-rw-rw-   0        0        0       63 2023-05-05 05:23:41.000000 DTCO-0.1.2/libMetric/__init__.py
+-rw-rw-rw-   0        0        0    48880 2023-05-05 05:23:41.000000 DTCO-0.1.2/libMetric/classLiberty.py
+-rw-rw-rw-   0        0        0       86 2023-05-05 10:48:04.144781 DTCO-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-05 10:46:14.000000 DTCO-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DTCO-0.1.1/DTCO.egg-info/PKG-INFO` & `DTCO-0.1.2/DTCO.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,136 @@
 Metadata-Version: 2.1
 Name: DTCO
-Version: 0.1.1
+Version: 0.1.2
 Summary: DTCO Utility
 Home-page: https://github.com/dipsci/DTCO
 Author: hockchen
 Author-email: hock.chen@dipsci.com
-License: UNKNOWN
-Description: **Liberty Metric Package**
-        
-        ```
-        from libMetric import liberty as lutil
-        import numpy as np
-        ```
-        
-        
-        Liberty conversion
-        ```
-        # load & convert CCS to JSON
-        lnode = lutil.read_lib('ccs.lib')
-        lutil.dump_json(lnode,out='ccs.json')
-        lnode.keys()
-        
-        # load liberty from JSON
-        lnode = lutil.load_json('ccs.json')
-        lnode.keys()
-        ```
-        
-        Timing & power operation
-        ```
-        # list cells in the liberary
-        [v for v in lnode['cell']]
-        
-        # grab cell node by cell-name, e.g., 'ND2D1LVT'
-        cnode = lnode['cell']['ND2D1LVT']
-        
-        # encapsulate all timing/power tables by timing-arc into a dataframe
-        lutT = lutil.get_cell_timing(cnode,todf=True)
-        lutP = lutil.get_cell_power(cnode,todf=True)
-        lutT.index # enumerate all lookup tables encapsulated by timing-arc
-        lutP.index # enumerate all lookup tables encapsulated by timing-arc
-        ```
-        
-        Lookup table, interpolation & regression
-        ```
-        # lookup table interpolation, e.g., timing-arc ('A1,ZN,', 'combinational', 'cell_rise')
-        lut = lutT.loc[('A1,ZN,', 'combinational', 'cell_rise')]
-        y,x,v = map(np.array,lut.values) # unpack values as numpy array
-        
-        # timing interpolation based on the specified transition & load
-        lutil.table_lookup(lut,trans=0.0207,load=0.0010072,dflag=True)
-        
-        # LS regression & prediction
-        lutil.lut2lsCoeff(lut.to_dict(),trans=0.03,load=0.0017,dflag=True)
-        ```
-        
-        
-        Data visualization API
-        ```
-        cnode = lnode['cell']['DFCNQD1LVT']
-        
-        lutT = lutil.get_cell_timing(cnode,todf=False) # grab all timing tables in JSON
-        lutil.plot_lut(lutT,keys=[('CP,Q,', 'rising_edge', 'cell_rise'),
-                    ('CP,Q,', 'rising_edge', 'cell_fall')],xylabel=('load','trans'))
-        
-        lutil.plot_lut(lutT,keys=[('CP,D,CDN', 'setup_rising', 'rise_constraint'),
-                    ('CP,D,CDN', 'hold_rising', 'rise_constraint')],xylabel=('clock','data'))
-        ```
-        
-        
-        ---
-        
-        **GRO Compiler Package**
-        
-        
-        ```
-        from GRO import ROCompiler 
-        import sys
-        
-        if __name__ == '__main__':
-            argv = sys.argv
-        else: # test mode
-            argv = ['C:/Home/Projects/Pypi/DTCO/GRO/gro.py',
-                    '-config','C:/Home/Projects/Pypi/DTCO/GRO/demo/config_demo.f',
-                    '-outDir','C:/Home/Projects/Pypi/DTCO/GRO/demo/RO_demo',
-                    '-target','TT']
-        
-        # init GRO instance
-        gro = ROCompiler()
-        
-        # parse command line
-        code,pdata = gro.parseArguments(argv)
-        
-        # update pdata from config
-        if pdata.get('configFile')!=None:
-            cfg = gro.loadConfig(pdata['configFile'])
-        if pdata.get('initProj')==True: # create RO project directory
-            gro.initProjectDirectory()
-            gro.initMakefile()
-        if pdata.get('initLib')==True:
-            gro.initLibJSON() # build library JSON DB
-        if pdata.get('buildRO')==True: # generate RO design and the successive DC, synthesis, vsim, SPICE environments
-            gro.commitConfig() # start from liberty JSON without initLibJSON
-            gro.compileGRO()
-        if pdata.get('lpe')!=None:
-            gro.genSPICESim()
-        ```
-        
-        ---
-        
-        **Design & Technology C-optimization**
-        
-        Process Uniformity & OCV Analysis
-        
-        Machine-learning Framework
-        
-        
-        
-Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design
-Platform: UNKNOWN
+Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design,WAT,CP,Binning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**Liberty Metric Package**
+
+```
+from libMetric import liberty as lutil
+import numpy as np
+```
+
+
+Liberty conversion
+```
+# load & convert CCS to JSON
+lnode = lutil.read_lib('ccs.lib')
+lutil.dump_json(lnode,out='ccs.json')
+lnode.keys()
+
+# load liberty from JSON
+lnode = lutil.load_json('ccs.json')
+lnode.keys()
+```
+
+Timing & power operation
+```
+# list cells in the liberary
+[v for v in lnode['cell']]
+
+# grab cell node by cell-name, e.g., 'ND2D1LVT'
+cnode = lnode['cell']['ND2D1LVT']
+
+# encapsulate all timing/power tables by timing-arc into a dataframe
+lutT = lutil.get_cell_timing(cnode,todf=True)
+lutP = lutil.get_cell_power(cnode,todf=True)
+lutT.index # enumerate all lookup tables encapsulated by timing-arc
+lutP.index # enumerate all lookup tables encapsulated by timing-arc
+```
+
+Lookup table, interpolation & regression
+```
+# lookup table interpolation, e.g., timing-arc ('A1,ZN,', 'combinational', 'cell_rise')
+lut = lutT.loc[('A1,ZN,', 'combinational', 'cell_rise')]
+y,x,v = map(np.array,lut.values) # unpack values as numpy array
+
+# timing interpolation based on the specified transition & load
+lutil.table_lookup(lut,trans=0.0207,load=0.0010072,dflag=True)
+
+# LS regression & prediction
+lutil.lut2lsCoeff(lut.to_dict(),trans=0.03,load=0.0017,dflag=True)
+```
+
+Data visualization API
+```
+cnode = lnode['cell']['DFCNQD1LVT']
+
+lutT = lutil.get_cell_timing(cnode,todf=False) # grab all timing tables in JSON
+lutil.plot_lut(lutT,keys=[('CP,Q,', 'rising_edge', 'cell_rise'),
+            ('CP,Q,', 'rising_edge', 'cell_fall')],xylabel=('load','trans'))
+
+lutil.plot_lut(lutT,keys=[('CP,D,CDN', 'setup_rising', 'rise_constraint'),
+            ('CP,D,CDN', 'hold_rising', 'rise_constraint')],xylabel=('clock','data'))
+```
+
+
+
+
+
+
+---
+
+
+
+**GRO Compiler Package**
+
+```
+from GRO import ROCompiler 
+import sys
+
+if __name__ == '__main__':
+    argv = sys.argv
+else: # test mode
+    argv = ['C:/Home/Projects/Pypi/DTCO/GRO/gro.py',
+            '-config','C:/Home/Projects/Pypi/DTCO/GRO/demo/config_demo.f',
+            '-outDir','C:/Home/Projects/Pypi/DTCO/GRO/demo/RO_demo',
+            '-target','TT']
+
+# init GRO instance
+gro = ROCompiler()
+
+# parse command line
+code,pdata = gro.parseArguments(argv)
+
+# update pdata from config
+if pdata.get('configFile')!=None:
+    cfg = gro.loadConfig(pdata['configFile'])
+if pdata.get('initProj')==True: # create RO project directory
+    gro.initProjectDirectory()
+    gro.initMakefile()
+if pdata.get('initLib')==True:
+    gro.initLibJSON() # build library JSON DB
+if pdata.get('buildRO')==True: # generate RO design and the successive DC, synthesis, vsim, SPICE environments
+    gro.commitConfig() # start from liberty JSON without initLibJSON
+    gro.compileGRO()
+if pdata.get('lpe')!=None:
+    gro.genSPICESim()
+```
+
+---
+
+
+**Copernic System**
+WAT Analysis
+
+CP Analysis
+
+Binning Strategy
+
+
+---
+
+**Design & Technology C-optimization**
+
+Process Uniformity & OCV Analysis
+
+Machine-learning Framework
+
```

### Comparing `DTCO-0.1.1/GRO/classGRO.py` & `DTCO-0.1.2/GRO/classGRO.py`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.1/libMetric/classLiberty.py` & `DTCO-0.1.2/libMetric/classLiberty.py`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.1/PKG-INFO` & `DTCO-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,136 @@
 Metadata-Version: 2.1
 Name: DTCO
-Version: 0.1.1
+Version: 0.1.2
 Summary: DTCO Utility
 Home-page: https://github.com/dipsci/DTCO
 Author: hockchen
 Author-email: hock.chen@dipsci.com
-License: UNKNOWN
-Description: **Liberty Metric Package**
-        
-        ```
-        from libMetric import liberty as lutil
-        import numpy as np
-        ```
-        
-        
-        Liberty conversion
-        ```
-        # load & convert CCS to JSON
-        lnode = lutil.read_lib('ccs.lib')
-        lutil.dump_json(lnode,out='ccs.json')
-        lnode.keys()
-        
-        # load liberty from JSON
-        lnode = lutil.load_json('ccs.json')
-        lnode.keys()
-        ```
-        
-        Timing & power operation
-        ```
-        # list cells in the liberary
-        [v for v in lnode['cell']]
-        
-        # grab cell node by cell-name, e.g., 'ND2D1LVT'
-        cnode = lnode['cell']['ND2D1LVT']
-        
-        # encapsulate all timing/power tables by timing-arc into a dataframe
-        lutT = lutil.get_cell_timing(cnode,todf=True)
-        lutP = lutil.get_cell_power(cnode,todf=True)
-        lutT.index # enumerate all lookup tables encapsulated by timing-arc
-        lutP.index # enumerate all lookup tables encapsulated by timing-arc
-        ```
-        
-        Lookup table, interpolation & regression
-        ```
-        # lookup table interpolation, e.g., timing-arc ('A1,ZN,', 'combinational', 'cell_rise')
-        lut = lutT.loc[('A1,ZN,', 'combinational', 'cell_rise')]
-        y,x,v = map(np.array,lut.values) # unpack values as numpy array
-        
-        # timing interpolation based on the specified transition & load
-        lutil.table_lookup(lut,trans=0.0207,load=0.0010072,dflag=True)
-        
-        # LS regression & prediction
-        lutil.lut2lsCoeff(lut.to_dict(),trans=0.03,load=0.0017,dflag=True)
-        ```
-        
-        
-        Data visualization API
-        ```
-        cnode = lnode['cell']['DFCNQD1LVT']
-        
-        lutT = lutil.get_cell_timing(cnode,todf=False) # grab all timing tables in JSON
-        lutil.plot_lut(lutT,keys=[('CP,Q,', 'rising_edge', 'cell_rise'),
-                    ('CP,Q,', 'rising_edge', 'cell_fall')],xylabel=('load','trans'))
-        
-        lutil.plot_lut(lutT,keys=[('CP,D,CDN', 'setup_rising', 'rise_constraint'),
-                    ('CP,D,CDN', 'hold_rising', 'rise_constraint')],xylabel=('clock','data'))
-        ```
-        
-        
-        ---
-        
-        **GRO Compiler Package**
-        
-        
-        ```
-        from GRO import ROCompiler 
-        import sys
-        
-        if __name__ == '__main__':
-            argv = sys.argv
-        else: # test mode
-            argv = ['C:/Home/Projects/Pypi/DTCO/GRO/gro.py',
-                    '-config','C:/Home/Projects/Pypi/DTCO/GRO/demo/config_demo.f',
-                    '-outDir','C:/Home/Projects/Pypi/DTCO/GRO/demo/RO_demo',
-                    '-target','TT']
-        
-        # init GRO instance
-        gro = ROCompiler()
-        
-        # parse command line
-        code,pdata = gro.parseArguments(argv)
-        
-        # update pdata from config
-        if pdata.get('configFile')!=None:
-            cfg = gro.loadConfig(pdata['configFile'])
-        if pdata.get('initProj')==True: # create RO project directory
-            gro.initProjectDirectory()
-            gro.initMakefile()
-        if pdata.get('initLib')==True:
-            gro.initLibJSON() # build library JSON DB
-        if pdata.get('buildRO')==True: # generate RO design and the successive DC, synthesis, vsim, SPICE environments
-            gro.commitConfig() # start from liberty JSON without initLibJSON
-            gro.compileGRO()
-        if pdata.get('lpe')!=None:
-            gro.genSPICESim()
-        ```
-        
-        ---
-        
-        **Design & Technology C-optimization**
-        
-        Process Uniformity & OCV Analysis
-        
-        Machine-learning Framework
-        
-        
-        
-Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design
-Platform: UNKNOWN
+Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design,WAT,CP,Binning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**Liberty Metric Package**
+
+```
+from libMetric import liberty as lutil
+import numpy as np
+```
+
+
+Liberty conversion
+```
+# load & convert CCS to JSON
+lnode = lutil.read_lib('ccs.lib')
+lutil.dump_json(lnode,out='ccs.json')
+lnode.keys()
+
+# load liberty from JSON
+lnode = lutil.load_json('ccs.json')
+lnode.keys()
+```
+
+Timing & power operation
+```
+# list cells in the liberary
+[v for v in lnode['cell']]
+
+# grab cell node by cell-name, e.g., 'ND2D1LVT'
+cnode = lnode['cell']['ND2D1LVT']
+
+# encapsulate all timing/power tables by timing-arc into a dataframe
+lutT = lutil.get_cell_timing(cnode,todf=True)
+lutP = lutil.get_cell_power(cnode,todf=True)
+lutT.index # enumerate all lookup tables encapsulated by timing-arc
+lutP.index # enumerate all lookup tables encapsulated by timing-arc
+```
+
+Lookup table, interpolation & regression
+```
+# lookup table interpolation, e.g., timing-arc ('A1,ZN,', 'combinational', 'cell_rise')
+lut = lutT.loc[('A1,ZN,', 'combinational', 'cell_rise')]
+y,x,v = map(np.array,lut.values) # unpack values as numpy array
+
+# timing interpolation based on the specified transition & load
+lutil.table_lookup(lut,trans=0.0207,load=0.0010072,dflag=True)
+
+# LS regression & prediction
+lutil.lut2lsCoeff(lut.to_dict(),trans=0.03,load=0.0017,dflag=True)
+```
+
+Data visualization API
+```
+cnode = lnode['cell']['DFCNQD1LVT']
+
+lutT = lutil.get_cell_timing(cnode,todf=False) # grab all timing tables in JSON
+lutil.plot_lut(lutT,keys=[('CP,Q,', 'rising_edge', 'cell_rise'),
+            ('CP,Q,', 'rising_edge', 'cell_fall')],xylabel=('load','trans'))
+
+lutil.plot_lut(lutT,keys=[('CP,D,CDN', 'setup_rising', 'rise_constraint'),
+            ('CP,D,CDN', 'hold_rising', 'rise_constraint')],xylabel=('clock','data'))
+```
+
+
+
+
+
+
+---
+
+
+
+**GRO Compiler Package**
+
+```
+from GRO import ROCompiler 
+import sys
+
+if __name__ == '__main__':
+    argv = sys.argv
+else: # test mode
+    argv = ['C:/Home/Projects/Pypi/DTCO/GRO/gro.py',
+            '-config','C:/Home/Projects/Pypi/DTCO/GRO/demo/config_demo.f',
+            '-outDir','C:/Home/Projects/Pypi/DTCO/GRO/demo/RO_demo',
+            '-target','TT']
+
+# init GRO instance
+gro = ROCompiler()
+
+# parse command line
+code,pdata = gro.parseArguments(argv)
+
+# update pdata from config
+if pdata.get('configFile')!=None:
+    cfg = gro.loadConfig(pdata['configFile'])
+if pdata.get('initProj')==True: # create RO project directory
+    gro.initProjectDirectory()
+    gro.initMakefile()
+if pdata.get('initLib')==True:
+    gro.initLibJSON() # build library JSON DB
+if pdata.get('buildRO')==True: # generate RO design and the successive DC, synthesis, vsim, SPICE environments
+    gro.commitConfig() # start from liberty JSON without initLibJSON
+    gro.compileGRO()
+if pdata.get('lpe')!=None:
+    gro.genSPICESim()
+```
+
+---
+
+
+**Copernic System**
+WAT Analysis
+
+CP Analysis
+
+Binning Strategy
+
+
+---
+
+**Design & Technology C-optimization**
+
+Process Uniformity & OCV Analysis
+
+Machine-learning Framework
+
```

### Comparing `DTCO-0.1.1/README.md` & `DTCO-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,33 +42,37 @@
 # timing interpolation based on the specified transition & load
 lutil.table_lookup(lut,trans=0.0207,load=0.0010072,dflag=True)
 
 # LS regression & prediction
 lutil.lut2lsCoeff(lut.to_dict(),trans=0.03,load=0.0017,dflag=True)
 ```
 
-
 Data visualization API
 ```
 cnode = lnode['cell']['DFCNQD1LVT']
 
 lutT = lutil.get_cell_timing(cnode,todf=False) # grab all timing tables in JSON
 lutil.plot_lut(lutT,keys=[('CP,Q,', 'rising_edge', 'cell_rise'),
             ('CP,Q,', 'rising_edge', 'cell_fall')],xylabel=('load','trans'))
 
 lutil.plot_lut(lutT,keys=[('CP,D,CDN', 'setup_rising', 'rise_constraint'),
             ('CP,D,CDN', 'hold_rising', 'rise_constraint')],xylabel=('clock','data'))
 ```
 
 
+
+
+
+
 ---
 
-**GRO Compiler Package**
 
 
+**GRO Compiler Package**
+
 ```
 from GRO import ROCompiler 
 import sys
 
 if __name__ == '__main__':
     argv = sys.argv
 else: # test mode
@@ -96,14 +100,24 @@
     gro.compileGRO()
 if pdata.get('lpe')!=None:
     gro.genSPICESim()
 ```
 
 ---
 
+
+**Copernic System**
+WAT Analysis
+
+CP Analysis
+
+Binning Strategy
+
+
+---
+
 **Design & Technology C-optimization**
 
 Process Uniformity & OCV Analysis
 
 Machine-learning Framework
 
-
```

