# Comparing `tmp/betweens-0.2.0.tar.gz` & `tmp/betweens-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.2.0.tar", last modified: Fri May  5 10:23:09 2023, max compression
+gzip compressed data, was "betweens-0.2.3.tar", last modified: Fri May  5 10:33:49 2023, max compression
```

## Comparing `betweens-0.2.0.tar` & `betweens-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.829221 betweens-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1180 2023-05-05 10:23:09.828220 betweens-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.819219 betweens-0.2.0/betweens/
--rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.2.0/betweens/__init__.py
--rw-rw-rw-   0        0        0     2025 2023-05-05 10:17:07.000000 betweens-0.2.0/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.2.0/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:23:09.827220 betweens-0.2.0/betweens.egg-info/
--rw-rw-rw-   0        0        0     1180 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 10:23:09.000000 betweens-0.2.0/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      270 2023-05-05 10:18:48.000000 betweens-0.2.0/new.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 10:23:09.829221 betweens-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-05-05 10:22:43.000000 betweens-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.170697 betweens-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1180 2023-05-05 10:33:49.169696 betweens-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.158696 betweens-0.2.3/betweens/
+-rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-0.2.3/betweens/__init__.py
+-rw-rw-rw-   0        0        0     2565 2023-05-05 10:31:57.000000 betweens-0.2.3/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.2.3/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.167695 betweens-0.2.3/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1180 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      355 2023-05-05 10:32:39.000000 betweens-0.2.3/new.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:33:49.170697 betweens-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-05-05 10:32:45.000000 betweens-0.2.3/setup.py
```

### Comparing `betweens-0.2.0/LICENSE` & `betweens-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.2.0/PKG-INFO` & `betweens-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.2.0
+Version: 0.2.3
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `betweens-0.2.0/betweens/betweens.py` & `betweens-0.2.3/betweens/betweens.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,20 +36,32 @@
     if type(s1) != type(str()) and type(s2) != type(str()):
         raise TypeError('Must be string.')
     result = []
     if len(s1) != len(s2):
         raise TypeError('s1 and s2 must be same type.')
     if len(s1)==2:
         try:
-            for i in l1[l1.index(s1)-1:l1.index(s2)]:
-                result.append(i)
+            if l1.index(s1)>l1.index(s2):
+                for i in l1[l1.index(s1)-1:l1.index(s2)]:
+                    result.append(i)
+            elif l1.index(s1)<l1.index(s2):
+                for i in l1[l1.index(s1)-1:l1.index(s2):-1]:
+                    result.append(i)
+            else:
+                print('s1 and s2 must be different!')
         except ValueError:
             raise ValueError('s1 and s2 must be units of length or area.')
     elif len(s1)==3:
         try:
-            for i in l2[l2.index(s1)-1:l2.index(s2)]:
-                result.append(i)
+            if l2.index(s1)>l2.index(s2):
+                for i in l1[l2.index(s1)-1:l2.index(s2)]:
+                    result.append(i)
+            elif l1.index(s1)<l1.index(s2):
+                for i in l2[l2.index(s1)-1:l2.index(s2):-1]:
+                    result.append(i)
+            else:
+                print('s1 and s2 must be different!')
         except ValueError:
             raise ValueError('s1 and s2 must be units of length or area.')
     else:
         raise ValueError('s1 and s2 must be units of length or area.')
     return result
```

### Comparing `betweens-0.2.0/betweens.egg-info/PKG-INFO` & `betweens-0.2.3/betweens.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.2.0
+Version: 0.2.3
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `betweens-0.2.0/setup.py` & `betweens-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 long_description = None
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='0.2.0', # 版本
+      version='0.2.3', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Operating System :: MacOS :: MacOS X',
           'Operating System :: Microsoft :: Windows :: Windows 10',
```

