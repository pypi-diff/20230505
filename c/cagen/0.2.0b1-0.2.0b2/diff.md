# Comparing `tmp/cagen-0.2.0b1.tar.gz` & `tmp/cagen-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0b1.tar", last modified: Fri May  5 15:25:29 2023, max compression
+gzip compressed data, was "cagen-0.2.0b2.tar", last modified: Fri May  5 15:30:07 2023, max compression
```

## Comparing `cagen-0.2.0b1.tar` & `cagen-0.2.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.998355 cagen-0.2.0b1/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b1/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:25:28.998355 cagen-0.2.0b1/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b1/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-04-24 11:09:57.000000 cagen-0.2.0b1/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 15:25:28.998355 cagen-0.2.0b1/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b1/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     5291 2023-05-05 15:24:59.000000 cagen-0.2.0b1/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b1/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.998355 cagen-0.2.0b1/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b1/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b1/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b1/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b1/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:30:07.358648 cagen-0.2.0b2/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b2/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:30:07.358648 cagen-0.2.0b2/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b2/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-05 15:29:58.000000 cagen-0.2.0b2/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 15:30:07.358648 cagen-0.2.0b2/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:30:07.355315 cagen-0.2.0b2/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:30:07.355315 cagen-0.2.0b2/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b2/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     5292 2023-05-05 15:29:44.000000 cagen-0.2.0b2/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b2/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:30:07.358648 cagen-0.2.0b2/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b2/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b2/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b2/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b2/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:30:07.358648 cagen-0.2.0b2/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 15:30:07.000000 cagen-0.2.0b2/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0b1/PKG-INFO` & `cagen-0.2.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0b1/README.md` & `cagen-0.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b1/pyproject.toml` & `cagen-0.2.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.beta-1"
+version = "0.2.0.beta-2"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0b1/src/cagen/cmd.py` & `cagen-0.2.0b2/src/cagen/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     parser.add_argument("--init", action='store_true', help="creates the Makefile")
     parser.add_argument("--templates", action='store_true', help="creates the directory 'templates' in the current directory with the copy of basic cagen templates")
     args = parser.parse_args()
 
     if args.init:
         with open("Makefile", "w") as f:
             f.write(maketemplate)
-    elif args.templates
+    elif args.templates:
         if not os.path.exists('templates'):
             os.makedirs('templates')
             # https://stackoverflow.com/a/58941536
             original_template_dir = pkgutil.get_data(__name__, 'templates/')
             shutil.copy(original_template_dir, 'templates')
     else:
         print("See --help for hints")
```

### Comparing `cagen-0.2.0b1/src/cagen/libcagen.py` & `cagen-0.2.0b2/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b1/src/cagen/templates/schema.tmpl` & `cagen-0.2.0b2/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b1/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0b2/src/cagen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

