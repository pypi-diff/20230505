# Comparing `tmp/CDSupdate-1.0.4.tar.gz` & `tmp/CDSupdate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDSupdate-1.0.4.tar", last modified: Thu May  4 07:13:54 2023, max compression
+gzip compressed data, was "CDSupdate-1.1.0.tar", last modified: Fri May  5 06:01:47 2023, max compression
```

## Comparing `CDSupdate-1.0.4.tar` & `CDSupdate-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 07:13:54.391754 CDSupdate-1.0.4/
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 07:13:54.388775 CDSupdate-1.0.4/CDSupdate/
--rw-r--r--   0 yrobin     (501) staff       (20)     9376 2023-05-04 07:07:59.000000 CDSupdate-1.0.4/CDSupdate/__CDSUParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/__CVarsParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.0.4/CDSupdate/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     3690 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)    12819 2023-05-03 12:54:20.000000 CDSupdate-1.0.4/CDSupdate/__extracvars.py
--rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.0.4/CDSupdate/__io.py
--rw-r--r--   0 yrobin     (501) staff       (20)     1912 2023-05-04 07:12:18.000000 CDSupdate-1.0.4/CDSupdate/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 07:13:54.391258 CDSupdate-1.0.4/CDSupdate/data/
--rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-dptas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1389 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-name.csv
--rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-pr-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-ps-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-psl-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-tas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-uas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-vas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/ERA5-zg-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/CDSupdate/data/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.0.4/CDSupdate/data/areas.csv
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 07:13:54.389550 CDSupdate-1.0.4/CDSupdate.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-04 07:13:54.000000 CDSupdate-1.0.4/CDSupdate.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      853 2023-05-04 07:13:54.000000 CDSupdate-1.0.4/CDSupdate.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-04 07:13:54.000000 CDSupdate-1.0.4/CDSupdate.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-04 07:13:54.000000 CDSupdate-1.0.4/CDSupdate.egg-info/requires.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-04 07:13:54.000000 CDSupdate-1.0.4/CDSupdate.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.0.4/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.0.4/MANIFEST.in
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-04 07:13:54.391606 CDSupdate-1.0.4/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     1568 2023-05-04 06:57:58.000000 CDSupdate-1.0.4/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 07:13:54.391400 CDSupdate-1.0.4/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.0.4/scripts/cdsupdate
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-04 07:13:54.391789 CDSupdate-1.0.4/setup.cfg
--rwxr-xr-x   0 yrobin     (501) staff       (20)     2417 2023-05-04 07:13:32.000000 CDSupdate-1.0.4/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.895380 CDSupdate-1.1.0/
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.891449 CDSupdate-1.1.0/CDSupdate/
+-rw-r--r--   0 yrobin     (501) staff       (20)     9376 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/CDSupdate/__CDSUParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__CVarsParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.1.0/CDSupdate/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    15304 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__extracvars.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.1.0/CDSupdate/__io.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1912 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.894758 CDSupdate-1.1.0/CDSupdate/data/
+-rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-dptas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1865 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-name.csv
+-rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-pr-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-ps-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-psl-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-rlds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-rsds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-tas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-uas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-vas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-zg-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.1.0/CDSupdate/data/areas.csv
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.892266 CDSupdate-1.1.0/CDSupdate.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/requires.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.1.0/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-05 06:01:47.895180 CDSupdate-1.1.0/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     1568 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.894959 CDSupdate-1.1.0/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/scripts/cdsupdate
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-05 06:01:47.895429 CDSupdate-1.1.0/setup.cfg
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     2417 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/setup.py
```

### Comparing `CDSupdate-1.0.4/CDSupdate/__CDSUParams.py` & `CDSupdate-1.1.0/CDSupdate/__CDSUParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__CVarsParams.py` & `CDSupdate-1.1.0/CDSupdate/__CVarsParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__curses_doc.py` & `CDSupdate-1.1.0/CDSupdate/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__doc.py` & `CDSupdate-1.1.0/CDSupdate/__doc.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 #############
 ## Imports ##
 #############
 
 from .__release import version
-from .__release import long_description
 from .__release import license
 from .__release import license_txt
 from .__release import src_url
 from .__release import authors_doc
 
 from .__CVarsParams import cvarsParams
 
@@ -39,15 +38,16 @@
 )
 
 doc = """\
 
 CDSupdate ({})
 {}
 
-{}
+CDSupdate is a tools to automatically download and update data from the Climate
+Data Store. Currently, only ERA5 is supported.
 
 Input parameters
 ----------------
 --log [LOGLEVEL FILE]
     Enable log, first optional is argument is the level (default is WARNING),
     the second is a file.
 --period t0/t1
@@ -90,15 +90,14 @@
 {}
 
 Sources and author(s)
 ---------------------
 Sources   : {}
 Author(s) : {}
 """.format( version , "=" * (12+len(version)) ,
-            long_description,
             ", ".join([f"'{s}'" for s in cvarsParams.all_cvars if cvarsParams.level(s) == "single"]),
             ", ".join([f"'{s}'" for s in cvarsParams.all_cvars if not cvarsParams.level(s) == "single"]),
             ", ".join([f"'{s}'" for s in cvarsParams._avail_levels]),
             area_description,
             license , "-" * ( 8 + len(license) ) , license_txt ,
             src_url , authors_doc )
```

### Comparing `CDSupdate-1.0.4/CDSupdate/__exceptions.py` & `CDSupdate-1.1.0/CDSupdate/__exceptions.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__exec.py` & `CDSupdate-1.1.0/CDSupdate/__exec.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__extracvars.py` & `CDSupdate-1.1.0/CDSupdate/__extracvars.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,14 +152,48 @@
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/sfcWind/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 	
 ##}}}
 
+def build_sfcWindmax():##{{{
+	
+	cvar = "sfcWindmax"
+	area_name = cdsuParams.area_name
+	
+	## files
+	cvar0   = "sfcWind"
+	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
+	ifiles0 = os.listdir(ipath0)
+	ifiles0.sort()
+	
+	
+	for ifile0 in ifiles0:
+		
+		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
+		
+		year  = idata0.time.dt.year[0].values
+		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
+		
+		## Build daily
+		odatad = idata0.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar0 : cvar } )
+		
+		## Save daily
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
+		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
+		odatad.to_netcdf( os.path.join( opath , ofile ) )
+##}}}
+
 def build_hurs():##{{{
 	
 	cvar = "hurs"
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathD  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "dptas" )
@@ -205,14 +239,48 @@
 		target = os.path.join( opath , ofile )
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 ##}}}
 
+def build_hursmax():##{{{
+	
+	cvar = "hursmax"
+	area_name = cdsuParams.area_name
+	
+	## files
+	cvar0   = "hurs"
+	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
+	ifiles0 = os.listdir(ipath0)
+	ifiles0.sort()
+	
+	
+	for ifile0 in ifiles0:
+		
+		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
+		
+		year  = idata0.time.dt.year[0].values
+		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
+		
+		## Build daily
+		odatad = idata0.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar0 : cvar } )
+		
+		## Save daily
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
+		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
+		odatad.to_netcdf( os.path.join( opath , ofile ) )
+##}}}
+
 def build_huss():##{{{
 	
 	cvar = "huss"
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathD  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "dptas" )
@@ -343,16 +411,20 @@
 		
 		if cvar == "tasmin":
 			build_tasmin()
 		if cvar == "tasmax":
 			build_tasmax()
 		if cvar == "sfcWind":
 			build_sfcWind()
+		if cvar == "sfcWindmax":
+			build_sfcWindmax()
 		if cvar == "hurs":
 			build_hurs()
+		if cvar == "hursmax":
+			build_hursmax()
 		if cvar == "huss":
 			build_huss()
 		if cvar == "heatIndex":
 			build_heatIndex()
 	
 ##}}}
```

### Comparing `CDSupdate-1.0.4/CDSupdate/__init__.py` & `CDSupdate-1.1.0/CDSupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__io.py` & `CDSupdate-1.1.0/CDSupdate/__io.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/__release.py` & `CDSupdate-1.1.0/CDSupdate/__release.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 ## GNU General Public License for more details.
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 
 version_major = "1"
-version_minor = "0"
-version_patch = "4"
+version_minor = "1"
+version_patch = "0"
 version_extra = ""
 version       = f"{version_major}.{version_minor}.{version_patch}{version_extra}"
 
 name = "CDSupdate"
 
 description = "Auto-updater of data from the Climate Data Store"
```

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-dptas-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-dptas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-name.csv` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-name.csv`

 * *Files 22% similar despite different names*

```diff
@@ -5,11 +5,15 @@
 single,2,tas,tasmax,,,air_temperature,Daily Max Near-Surface Air Temperature,K,
 single,0,,pr,mean_total_precipitation_rate,mtpr,precipitation_flux,Total Precipitation Flux,kg.m-2.s-1,
 single,0,,psl,mean_sea_level_pressure,msl,air_pressure_at_sea_level,Sea Level Pressure,Pa,
 single,0,,ps,surface_pressure,sp,surface_air_pressure,Surface Pressure,Pa,
 single,10,,uas,10m_u_component_of_wind,u10,eastward_wind,Eastward Near-Surface Wind,m.s-1,
 single,10,,vas,10m_v_component_of_wind,v10,northward_wind,Northward Near-Surface Wind,m.s-1,
 single,10,uas;vas,sfcWind,,,wind_speed,Near-Surface Wind Speed,m.s-1,
+single,10,sfcWind,sfcWindmax,,,wind_speed,Daily Max Near-Surface Wind Speed,m.s-1,
 single,2,tas;dptas,hurs,,,relative_humidity,Near-Surface Relative Humidity,%,
+single,2,hurs,hursmax,,,relative_humidity,Daily Max Near-Surface Relative Humidity,%,
 single,2,dptas;ps,huss,,,specific_humidity,Near-Surface Specific Humidity,kg.kg-1,
 single,2,tas;hurs,heatIndex,,,heat_index_of_air_temperature,Heat Index of Air Temperature,K,see Blazejczyk et al 2012 doi:10.1007/s00484-011-0453-2
 pressure,,,zg,geopotential,z,geopotential_height,Geopotential Height at __CHANGE__hPa,m,Multiply by 9.80665 to find the geopotential
+single,0,,rsds,mean_surface_downward_short_wave_radiation_flux,msdwswrf,surface_downwelling_shortwave_flux_in_air,Surface Downwelling Shortwave Radiation,
+single,0,,rlds,mean_surface_downward_long_wave_radiation_flux,msdwlwrf,surface_downwelling_longwave_flux_in_air,Surface Downwelling Longwave Radiation,
```

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-pr-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-pr-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-ps-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-ps-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-psl-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-psl-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-uas-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-uas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-vas-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-vas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/ERA5-zg-description.txt` & `CDSupdate-1.1.0/CDSupdate/data/ERA5-zg-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate/data/__init__.py` & `CDSupdate-1.1.0/CDSupdate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/CDSupdate.egg-info/PKG-INFO` & `CDSupdate-1.1.0/CDSupdate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.0.4
+Version: 1.1.0
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.0.4/CDSupdate.egg-info/SOURCES.txt` & `CDSupdate-1.1.0/CDSupdate.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 CDSupdate.egg-info/requires.txt
 CDSupdate.egg-info/top_level.txt
 CDSupdate/data/ERA5-dptas-description.txt
 CDSupdate/data/ERA5-name.csv
 CDSupdate/data/ERA5-pr-description.txt
 CDSupdate/data/ERA5-ps-description.txt
 CDSupdate/data/ERA5-psl-description.txt
+CDSupdate/data/ERA5-rlds-description.txt
+CDSupdate/data/ERA5-rsds-description.txt
 CDSupdate/data/ERA5-tas-description.txt
 CDSupdate/data/ERA5-uas-description.txt
 CDSupdate/data/ERA5-vas-description.txt
 CDSupdate/data/ERA5-zg-description.txt
 CDSupdate/data/__init__.py
 CDSupdate/data/areas.csv
 scripts/cdsupdate
```

### Comparing `CDSupdate-1.0.4/LICENSE` & `CDSupdate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/PKG-INFO` & `CDSupdate-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.0.4
+Version: 1.1.0
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.0.4/README.md` & `CDSupdate-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/scripts/cdsupdate` & `CDSupdate-1.1.0/scripts/cdsupdate`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.4/setup.py` & `CDSupdate-1.1.0/setup.py`

 * *Files identical despite different names*

