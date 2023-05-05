# Comparing `tmp/Omar_Style_sel-0.3.tar.gz` & `tmp/Omar_Style_sel-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Omar_Style_sel-0.3.tar", last modified: Thu May  4 21:39:28 2023, max compression
+gzip compressed data, was "Omar_Style_sel-0.4.tar", last modified: Fri May  5 18:14:28 2023, max compression
```

## Comparing `Omar_Style_sel-0.3.tar` & `Omar_Style_sel-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 21:39:28.045427 Omar_Style_sel-0.3/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-04 21:39:27.864258 Omar_Style_sel-0.3/Omar_Style_sel/
--rw-rw-rw-   0        0        0     2756 2023-05-04 21:36:01.000000 Omar_Style_sel-0.3/Omar_Style_sel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 21:39:28.038272 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/
--rw-rw-rw-   0        0        0     1833 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1833 2023-05-04 21:39:28.041269 Omar_Style_sel-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-04-25 18:53:37.000000 Omar_Style_sel-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 21:39:28.048269 Omar_Style_sel-0.3/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-05-04 21:37:22.000000 Omar_Style_sel-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 18:14:28.150616 Omar_Style_sel-0.4/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-05 18:14:28.033608 Omar_Style_sel-0.4/Omar_Style_sel/
+-rw-rw-rw-   0        0        0     4764 2023-05-05 18:10:52.000000 Omar_Style_sel-0.4/Omar_Style_sel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 18:14:28.145616 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/
+-rw-rw-rw-   0        0        0     1833 2023-05-05 18:14:27.000000 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-05 18:14:27.000000 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 18:14:27.000000 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-05 18:14:27.000000 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-05 18:14:27.000000 Omar_Style_sel-0.4/Omar_Style_sel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1833 2023-05-05 18:14:28.149616 Omar_Style_sel-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2023-04-25 18:53:37.000000 Omar_Style_sel-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 18:14:28.151617 Omar_Style_sel-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-05-05 18:13:02.000000 Omar_Style_sel-0.4/setup.py
```

### Comparing `Omar_Style_sel-0.3/Omar_Style_sel.egg-info/PKG-INFO` & `Omar_Style_sel-0.4/Omar_Style_sel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Omar-Style-sel
-Version: 0.3
+Version: 0.4
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Omar_Style_sel-0.3/PKG-INFO` & `Omar_Style_sel-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Omar_Style_sel
-Version: 0.3
+Version: 0.4
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Omar_Style_sel-0.3/README.md` & `Omar_Style_sel-0.4/README.md`

 * *Files identical despite different names*

### Comparing `Omar_Style_sel-0.3/setup.py` & `Omar_Style_sel-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='Omar_Style_sel',
-    version="0.3",
+    version="0.4",
     author='omar Style',
     author_email='omarllStyle@gmail.com',
     description='Omar_Style _ 〄🇵🇸',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['Omar_Style_sel'],
```

