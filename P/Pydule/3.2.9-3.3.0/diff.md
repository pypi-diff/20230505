# Comparing `tmp/Pydule-3.2.9.tar.gz` & `tmp/Pydule-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.2.9.tar", last modified: Mon May  1 07:45:24 2023, max compression
+gzip compressed data, was "Pydule-3.3.0.tar", last modified: Thu May  4 16:04:19 2023, max compression
```

## Comparing `Pydule-3.2.9.tar` & `Pydule-3.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.964952 Pydule-3.2.9/
--rw-rw-rw-   0        0        0     2419 2023-05-01 07:45:24.949329 Pydule-3.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1631 2023-04-30 15:24:02.000000 Pydule-3.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 07:45:24.964952 Pydule-3.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1399 2023-04-30 15:23:25.000000 Pydule-3.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.839980 Pydule-3.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.949329 Pydule-3.2.9/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2419 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12126 2023-05-01 04:34:10.000000 Pydule-3.2.9/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:04:19.581991 Pydule-3.3.0/
+-rw-rw-rw-   0        0        0     2452 2023-05-04 16:04:19.568028 Pydule-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1649 2023-05-04 14:22:20.000000 Pydule-3.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:04:19.584015 Pydule-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2023-05-04 15:08:06.000000 Pydule-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:04:19.465304 Pydule-3.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 16:04:19.520156 Pydule-3.3.0/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2452 2023-05-04 16:04:18.000000 Pydule-3.3.0/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-04 16:04:19.000000 Pydule-3.3.0/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:04:19.000000 Pydule-3.3.0/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-05-04 16:04:19.000000 Pydule-3.3.0/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 16:04:19.000000 Pydule-3.3.0/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14262 2023-05-04 15:50:14.000000 Pydule-3.3.0/src/Pydule.py
```

### Comparing `Pydule-3.2.9/PKG-INFO` & `Pydule-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.9
-Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
+Version: 3.3.0
+Summary: Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Access ChatGPT
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
```

### Comparing `Pydule-3.2.9/README.md` & `Pydule-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Access ChatGPT
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
```

### Comparing `Pydule-3.2.9/setup.py` & `Pydule-3.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.2.9',
-	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
+	version='3.3.0',
+	description="Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
@@ -37,11 +37,12 @@
 		'numpy',
 		'pyperclip',
 		'soundfile',
 		'soundcard',
 		'pyautogui',
 		'pyaudio',
 		'wave',
-		'opencv-python'
+		'opencv-python',
+		'openai'
 	]
 
 )
```

### Comparing `Pydule-3.2.9/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.3.0/src/Pydule.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.9
-Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
+Version: 3.3.0
+Summary: Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Access ChatGPT
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
```

### Comparing `Pydule-3.2.9/src/Pydule.py` & `Pydule-3.3.0/src/Pydule.py`

 * *Files 18% similar despite different names*

```diff
@@ -144,14 +144,23 @@
 	for i in string:
 		s+=d[i]
 	for i in d:
 		n=ord(i)
 		e[n]=d[i]	
 	return s,e
 
+def ChatGPT(prompt,engine="text-davinci-003",max_tokens=1024,temperature=0.7):
+	import openai
+
+	openai.api_key = dcodestr('@#@_%%+^-+*%+*#+_%&*@^-^&&*%_!*%-=*$^-_@%=$#^*=%#&-&#-@@=^%@=_#^-^=$=&^+_**-!@+$!#@#+%_*!*+_!@=-#^!_^@$+#-#$==!-*_$!@@=@+$!#@#_**&+@%*!_^+$-!=*#$+-_**&+@%-$!-*&&^+#+#+__!%@*#&_+^*&^_$&*=%@*@@*%%#%^-+*%+*^-^&&*%%=#$==%%!$#=$%*_$!@@=%!$#=$%@@*%%#%@@*%%#%$&*=%@*%$&*++#^#-%#_^*!_^+$-^-^&&*%&-&#-@@#*_@$%*_**&+@%-=_+*##%$&*++#-=*-_!&%$&*++##*_@$%*_!*%-=*-^%@*^@',swapdict({65: '%$&*++#', 66: '_+^*&^_', 67: '-_$!!#=', 68: '-=_+*##', 69: '$^-_@%=', 70: '^-^&&*%', 71: '=^%@=_#', 72: '$+%%!&@', 73: '!=*#$+-', 74: '%=#$==%', 75: '$#^*=%#', 76: '!@-*^-&', 77: '__%!-^^', 78: '^_@%^=%', 79: '^+@!@*^', 80: '+^*^!%$', 81: '&-&#-@@', 82: '$%^*+^+', 83: '_**&+@%', 84: '^+#+#+_', 85: '^#-%#_^', 86: '-^%@*^@', 87: '%#_&#*!', 88: '&%&_#_$', 89: '_@+-+^&', 90: '-=*-_!&', 97: '$==-^%%', 98: '@@*%%#%', 99: '$^&!%!@', 100: '_!*%-=*', 101: '#*_@$%*', 102: '$=%*=-%', 103: '+%_*!*+', 104: '%!+@%_+', 105: '*_$!@@=', 106: '-**^^^-', 107: '^-+*%+*', 108: '$&*=%@*', 109: '-=#^^^^', 110: '-$!-*&&', 111: '*^^*_!*', 112: '_!@=-#^', 113: '+*&=&+=', 114: '^%%=+=&', 115: '@#@_%%+', 116: '@+$!#@#', 117: '-=-@!&!', 118: '^+_**-!', 119: '==@^%_+', 120: '-#$==!-', 121: '^*_$%=^', 122: '%!$#=$%', 49: '@!%+^#_', 50: '^%!^_--', 51: '_!%@*#&', 52: '*!_^+$-', 53: '^@_+#%&', 54: '*@-!_#%', 55: '!&$=-%$', 56: '!_^@$+#', 57: '^-^=$=&', 48: '&^&!##=', 33: '=-$_=^!', 64: '*$-*++-', 35: '@##+*!$', 36: '_%%+%$*', 37: '_*=@@*$', 94: '_%*_*$_', 38: '!___=-_', 42: '^+$&@=-', 95: '--$&@+-', 61: '#!^=&&&', 45: '#+_%&*@', 43: '=^-!%_&', 40: '%=-=!_=', 41: '%&@$$@$', 91: '+#_&@-_', 93: '_=!&-#*', 96: '-#_*%!=', 126: '-&@*$*@', 123: '++*&**!', 125: '^_&**!=', 63: '$-#-&-^', 92: '-=-++*-', 39: '$#@-^$+', 47: '$@!$=*_', 59: '-*&^^%@', 58: '#@_-&$^', 34: '^_@!#^!', 60: '%%@_#__', 62: '-&%+-+#', 46: '%%^!+!=', 44: '_!%@*_#', 32: '&!_@^&!'}))
+
+	completions = openai.Completion.create(engine=engine,prompt=prompt,max_tokens=max_tokens,n=1,stop=None,temperature=temperature)
+
+	return completions.choices[0].text.strip()
+
 def wjson(data,path):
 	import json
 	with open(path,'w') as json_file:
 		json.dump(data,json_file)
 
 def deljsonele(path):
 	import json
@@ -212,15 +221,15 @@
 				else:
 					new+=j
 		return new
 	else:
 		print(err)			
 
 def functions():
-	l=['recintaudio(<seconds>)','recmic(<seconds>)','recscreen()','mulmatrix(<matrix a>,<matrix b>)','codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
+	l=['ChatGPT(<content>)','recintaudio(<seconds>)','recmic(<seconds>)','recscreen()','mulmatrix(<matrix a>,<matrix b>)','codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
 	print('Available Functions : \n')
 	for i in l:
 		print(f'\t{i}')
 
 def summatrix(x,y):
 	import numpy as np
 	result = np.array(x) + np.array(y)
```

