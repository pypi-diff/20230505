# Comparing `tmp/taskAutom-7.19.2.tar.gz` & `tmp/taskAutom-7.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-7.19.2.tar", last modified: Wed May  3 16:27:35 2023, max compression
+gzip compressed data, was "taskAutom-7.19.3.tar", last modified: Fri May  5 17:31:30 2023, max compression
```

## Comparing `taskAutom-7.19.2.tar` & `taskAutom-7.19.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.2/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-03 16:27:35.632553 taskAutom-7.19.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.2/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-03 16:27:35.632553 taskAutom-7.19.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-03 16:23:25.000000 taskAutom-7.19.2/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.628553 taskAutom-7.19.2/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-02 13:30:56.000000 taskAutom-7.19.2/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    64918 2023-05-03 14:19:43.000000 taskAutom-7.19.2/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.3/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-05 17:31:30.387546 taskAutom-7.19.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.3/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 17:31:30.387546 taskAutom-7.19.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-05 13:39:44.000000 taskAutom-7.19.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-05 13:39:49.000000 taskAutom-7.19.3/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    65612 2023-05-05 17:29:59.000000 taskAutom-7.19.3/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-7.19.2/LICENSE` & `taskAutom-7.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.2/PKG-INFO` & `taskAutom-7.19.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.2
+Version: 7.19.3
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-7.19.2/README.md` & `taskAutom-7.19.3/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.2/setup.py` & `taskAutom-7.19.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='7.19.2',
+    version='7.19.3',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-7.19.2/src/taskAutom/taskAutom.py` & `taskAutom-7.19.3/src/taskAutom/taskAutom.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
 #logging.basicConfig(level=logging.DEBUG,format='[%(levelname)s] (%(threadName)-10s) %(message)s')
 
+LATEST_VERSION = '7.19.3'
+
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
 	logsDirectory    = None,
@@ -52,15 +54,28 @@
 	logsDirTimestamp = None,
 	pluginFilename   = None,
 	cronTime         = dict(type=None),
 	jumpHosts        = dict(),
 	pluginType       = 'show',
 	cmdVerify        = True,
 	auxRetry         = 10,
-	inventoryFile    = None
+	inventoryFile    = None,
+	useSSHTunnel     = False,
+	useHeader        = True,
+	strictOrder      = False,
+	username         = None,
+	password         = None,
+	deviceType       = 'nokia_sros',
+	readTimeOut      = 10,
+	progNumThreads   = 1,
+	sshDebug         = False,
+	passByRow        = True,
+	genMop           = False,
+	dataGroupColumn  = 'ip',
+	version          = LATEST_VERSION
 )
 
 # - Parameters per vendor
 DICT_VENDOR = dict(
 	nokia_sros=dict(
 		START_SCRIPT     = "", 
 		FIRST_LINE       = "/environment no more\n",
@@ -234,15 +249,14 @@
 
 		with open(dictParam['logsDirectory'] + '00_log_console.txt','w') as f:
 			for k in LOG_CONSOLE:
 				f.write(k+'\n')
 			f.close()
 
 		with open(dictParam['logsDirectory'] + '00_report.json', 'w') as f:
-			dictParam['version'] = '7.19.2'
 			dictParam['password'] = '*****'
 			dictParam.pop('data')
 			dictParam.pop('mod')
 			dictParam['routersTotal'] = len(df)
 			dictParam['routersFailed'] = len(dfFailed)
 			if len(dictParam['jumpHosts']) > 0:
 				for srv in dictParam['jumpHosts']:
@@ -826,33 +840,42 @@
 			aluCliLine = mod.construir_cliLine(0, pluginData, 1, mop)
 		except Exception as e:
 			print('\nError: ' + str(e))
 			print('Row: ' + str(pluginData))
 			print(f'Error trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}. Quitting...\n')
 			quit()
 
-	try:
-		if len(aluCliLine) > 0:
-			if aluCliLine[-1] == "\n":
-				aluCliLine = aluCliLine[:-1]
-	except:
-		print(f'Error trying analyze the DATA file {dataFile}.\nVerify it and make sure that the table is consistent. Quitting...\n')
-		quit()		
+	return aluCliLine
 
-	if jobType == 2:	
 
-		if len(dictParam['cronTime']) == 0:
-			
-			pass
+def buildScripts(dictParam):
+	"""
+	This function builds scripts per router. This function must be used
+	when using taskAutom as a library (import)
 
-		return aluCliLine
+	Args:
+		dictParam
 
-	elif jobType == 0:
+	Returns:
+		_dict with results
+	"""
+
+	dictParam['data'] = verifyData(dictParam)
+	dictParam['mod']  = verifyPlugin(dictParam['pluginFilename'])
+	dictParam['pluginFileAlone'] = dictParam['pluginFilename'].split('/')[-1]
+	dictParam['listOfRouters'], _ = getListOfRouters(dictParam)
+
+	d = {}
+
+	for IPconnect in dictParam['listOfRouters']:
+		if IPconnect not in d.keys():
+			d[IPconnect] = {}
+		d[IPconnect][dictParam['pluginFileAlone']] = renderCliLine(IPconnect, dictParam, 1)
 
-		return aluCliLine
+	return d
 ###
 
 def run_mi_thread(i, routerInfo, dictParam):
 	"""[summary]
 
 	Args:
 		i ([type]): [description]
@@ -1695,15 +1718,15 @@
 		open(dictParam['logsCsvFilename'],'w').close()
 
 	return dictParam
 
 def getDictParam():
 
 	parser = argparse.ArgumentParser(description='taskAutom Parameters.', prog='taskAutom', usage='%(prog)s [options]')
-	parser.add_argument('-v'  ,'--version',     help='Version', action='version', version='Lucas Aimaretto - (c)2023 - laimaretto@gmail.com - Version: 7.19.2' )
+	parser.add_argument('-v'  ,'--version',     help='Version', action='version', version='Lucas Aimaretto - (c)2023 - laimaretto@gmail.com - Version: '+LATEST_VERSION )
 
 	groupJobTypes = parser.add_argument_group('JobTypes')
 	groupJobTypes.add_argument('-j'  ,'--jobType',       type=int, choices=[0,2,3], default=0, help='Type of job. j=0 to check data and plugin; j=2, to execute. j=3, to upload files via SCP/SFTP. Default=0')
 
 	groupPugin = parser.add_argument_group('Plugin')
 	groupPugin.add_argument('-pt' ,'--pluginType',      type=str, help='Type of plugin.', default='show', choices=['show','config'])
 	groupPugin.add_argument('-py' ,'--pluginFilename' , type=str, help='PY Template File. Optional if jobType=3.')
@@ -1741,14 +1764,15 @@
 	miscGroup.add_argument('-sd', '--sshDebug',      type=str, help='Enables debuging of SSH interaction with the network. Stored on debug.log. Default=no', default='no', choices=['no','yes'])
 
 	args = parser.parse_args()
 
 	### reading parameters
 
 	dictParam = dict(
+		version            = LATEST_VERSION,		
 		outputJob 		   = args.jobType,
 		dataFile           = args.dataFile,
 		xlsSheetName       = args.xlsSheetName,
 		useHeader          = True if args.useHeader == 'yes' else False,
 		passByRow          = True if args.passByRow == 'yes' else False,
 		pluginFilename     = args.pluginFilename,
 		username 		   = args.username,
```

### Comparing `taskAutom-7.19.2/taskAutom.egg-info/PKG-INFO` & `taskAutom-7.19.3/taskAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.2
+Version: 7.19.3
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

