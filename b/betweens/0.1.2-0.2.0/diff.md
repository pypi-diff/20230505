# Comparing `tmp/betweens-0.1.2.tar.gz` & `tmp/betweens-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.1.2.tar", last modified: Thu May  4 10:36:45 2023, max compression
+gzip compressed data, was "betweens-0.2.0.tar", last modified: Fri May  5 10:23:09 2023, max compression
```

## Comparing `betweens-0.1.2.tar` & `betweens-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:36:45.512720 betweens-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1180 2023-05-04 10:36:45.512720 betweens-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:36:45.497071 betweens-0.1.2/betweens/
--rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.1.2/betweens/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-05-04 10:35:09.000000 betweens-0.1.2/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-03 10:18:54.000000 betweens-0.1.2/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:36:45.512720 betweens-0.1.2/betweens.egg-info/
--rw-rw-rw-   0        0        0     1180 2023-05-04 10:36:45.000000 betweens-0.1.2/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-04 10:36:45.000000 betweens-0.1.2/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:36:45.000000 betweens-0.1.2/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 10:36:45.000000 betweens-0.1.2/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2023-05-04 10:36:02.000000 betweens-0.1.2/new.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 10:36:45.512720 betweens-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-05-04 10:36:17.000000 betweens-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.829221 betweens-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1180 2023-05-05 10:23:09.828220 betweens-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.819219 betweens-0.2.0/betweens/
+-rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.2.0/betweens/__init__.py
+-rw-rw-rw-   0        0        0     2025 2023-05-05 10:17:07.000000 betweens-0.2.0/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.2.0/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.827220 betweens-0.2.0/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1180 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      270 2023-05-05 10:18:48.000000 betweens-0.2.0/new.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:23:09.829221 betweens-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-05-05 10:22:43.000000 betweens-0.2.0/setup.py
```

### Comparing `betweens-0.1.2/LICENSE` & `betweens-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.1.2/PKG-INFO` & `betweens-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.1.2
+Version: 0.2.0
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `betweens-0.1.2/betweens/betweens.py` & `betweens-0.2.0/betweens/betweens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 def between1(a,b):
     '''Print numbers between a and b'''
     if type(a) != type(int()) and type(b) != type(int()):
         raise TypeError('Must be integer.')
     result = []
-    for i in range(a-1,b):
-        result.append(i)
+    if a>b:
+        for i in range(a-1,b):
+            result.append(i)
+    elif a<b:
+        for i in range(a-1,b,-1):
+            result.append(i)
+    else:
+        print('a and b must be different!')
     return result
 
 def between2(l1,l2,a,b):
     '''Print numbers between l1[a] and l2[b]'''
     if type(l1) != type(list()) and type(l1) != type(tuple()) and type(l1) != type(dict()) and type(l2) != type(list()) and type(l2) != type(tuple()) and type(l1) != type(dict()):
         raise TypeError('l1, l2 must be list, dict or tuple.')
     if type(a) != type(int()) and type(b) != type(int()):
         raise TypeError('a, b must be integer.')
     result = []
-    for i in range(l1[a-1],l2[b]):
-        result.append(i)
+    if l1[a]>l2[b]: 
+        for i in range(l1[a-1],l2[b]):
+            result.append(i)
+    elif l1[a]<l2[b]:
+        for i in range(l1[a-1],l2[b],-1):
+            result.append(i)
+    else:
+        print('l1[a] and l2[b] must be different!')
     return result
 
 def between3(s1,s2):
     l1 = ['nm','um','mm','cm','dm','m','km']
     l2 = ['nm2','um2','mm2','cm2','dm2','m2','hm2','km2']
     if type(s1) != type(str()) and type(s2) != type(str()):
         raise TypeError('Must be string.')
```

### Comparing `betweens-0.1.2/betweens.egg-info/PKG-INFO` & `betweens-0.2.0/betweens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.1.2
+Version: 0.2.0
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `betweens-0.1.2/setup.py` & `betweens-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 long_description = None
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='0.1.2', # 版本
+      version='0.2.0', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Operating System :: MacOS :: MacOS X',
           'Operating System :: Microsoft :: Windows :: Windows 10',
```

