# Comparing `tmp/cagen-0.2.0a9.tar.gz` & `tmp/cagen-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a9.tar", last modified: Mon Apr 24 07:50:58 2023, max compression
+gzip compressed data, was "cagen-0.2.0b1.tar", last modified: Fri May  5 15:25:29 2023, max compression
```

## Comparing `cagen-0.2.0a9.tar` & `cagen-0.2.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a9/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:50:58.233893 cagen-0.2.0a9/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3465 2023-04-17 09:01:49.000000 cagen-0.2.0a9/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-24 07:48:37.000000 cagen-0.2.0a9/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-24 07:50:58.233893 cagen-0.2.0a9/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a9/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4682 2023-04-24 07:50:44.000000 cagen-0.2.0a9/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8539 2023-04-24 07:42:52.000000 cagen-0.2.0a9/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0a9/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a9/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0a9/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a9/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.998355 cagen-0.2.0b1/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b1/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:25:28.998355 cagen-0.2.0b1/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b1/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-04-24 11:09:57.000000 cagen-0.2.0b1/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 15:25:28.998355 cagen-0.2.0b1/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b1/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     5291 2023-05-05 15:24:59.000000 cagen-0.2.0b1/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b1/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.998355 cagen-0.2.0b1/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b1/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b1/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b1/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b1/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 15:25:28.995021 cagen-0.2.0b1/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 15:25:28.000000 cagen-0.2.0b1/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a9/PKG-INFO` & `cagen-0.2.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a9
-Summary: A static site generator for cmpalgorithms project
+Version: 0.2.0b1
+Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
@@ -58,22 +58,24 @@
 
 If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
-cagen sourcefile.md generatedfile.html template.tmpl
+cagen generatedfile.html template.tmpl --source sourcefile.md
 ```
 where 
 
 - `sourcefile.md` is Markdown file
 - `generatedfile.html` is the HTML5 file
 - `template.tmpl` is Mako template file
 
+The `source` argument is optional. In the case it is omitted, `cagen` just renders the template to `generatedfile.html`
+
 See `cagen --help` for more options.
 
 This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
 ```
 cagen-make --init
 ```
```

### Comparing `cagen-0.2.0a9/README.md` & `cagen-0.2.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,22 +39,24 @@
 
 If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
-cagen sourcefile.md generatedfile.html template.tmpl
+cagen generatedfile.html template.tmpl --source sourcefile.md
 ```
 where 
 
 - `sourcefile.md` is Markdown file
 - `generatedfile.html` is the HTML5 file
 - `template.tmpl` is Mako template file
 
+The `source` argument is optional. In the case it is omitted, `cagen` just renders the template to `generatedfile.html`
+
 See `cagen --help` for more options.
 
 This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
 ```
 cagen-make --init
 ```
```

### Comparing `cagen-0.2.0a9/pyproject.toml` & `cagen-0.2.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-9"
+version = "0.2.0.beta-1"
 authors = [{'name'="Xavier B."}]
-description = "A static site generator for cmpalgorithms project"
+description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
```

### Comparing `cagen-0.2.0a9/src/cagen/cmd.py` & `cagen-0.2.0b1/src/cagen/cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 # SPDX-FileCopyrightText: 2023 Xavier Bordoy <somenxavier@posteo.net>
 #
 # SPDX-License-Identifier: GPL-2.0-only
 
 import cagen.libcagen as libcagen
 import argparse
 import os.path
+import shutil
 from mako.template import Template
+import pkgutil
 
 def cagen_cli():
     """Defines the `cagen` command line script function to call from pyproject.toml"""
 
-    parser = argparse.ArgumentParser(prog = "cagen", description="static site generator for cmpalgorithms project", epilog="For better processing, please put the options and the end of the call of the program.")
+    parser = argparse.ArgumentParser(prog = "cagen", description="static site generator for cmpalgorithms project", epilog="For better processing, please put the options at the end of the call of the program.")
     parser.add_argument("--source", type=str, help="the source markdown file. It could be None. In this case, it renders Template with --metadata fields to `to` path")
     parser.add_argument("to", type=str, help="destination file")
     parser.add_argument("template", type=str, help="Mako template file path")
     parser.add_argument("--syntax", type=str, default='html5', help="syntax of destination file. By default 'html5'")
-    parser.add_argument("--metadata", type=str, nargs='*', help="extra metadata provided to template. In the form variable=value variable2=value2 ...")
+    parser.add_argument("--metadata", type=str, nargs='*', help="extra metadata provided to template. In the form variable=value variable2=value2 ... . If you want to use cagen.libcagen.Collection invoke as Collection not full name")
     parser.add_argument("--evals", type=str, nargs='*', help="evals with `eval()` python function the specified metadata variables. Eg. if `--metadata foo=2.0` and `--eval foo`, then the foo variable is the float 2.0, not the string '2.0'.")
     args = parser.parse_args()
 
     # Conversion
+    entry = libcagen.Entry(args.source)
     if os.path.exists(args.template):
         with open(args.to, "w") as f:
             assignments=libcagen.extract_assignments(args.metadata)
             evals=args.evals
             eassignments=libcagen.evaluate_assignments(assignments, evals)
             f.write(entry.to(mytemplatepath=args.template, additionalsearchlist=eassignments, destsyntax=args.syntax))
             print("{} -> {} ({}) using {}".format(args.source, args.to, args.syntax, args.template))
@@ -95,14 +98,21 @@
 
 clean:
 \trm $(MARKDOWNS_HTML5)
 """
 
     parser = argparse.ArgumentParser(prog = "cagen-make", description="creates a Makefile file for using GNU Make to generate HTML5 files using cagen")
     parser.add_argument("--init", action='store_true', help="creates the Makefile")
+    parser.add_argument("--templates", action='store_true', help="creates the directory 'templates' in the current directory with the copy of basic cagen templates")
     args = parser.parse_args()
 
     if args.init:
         with open("Makefile", "w") as f:
             f.write(maketemplate)
+    elif args.templates
+        if not os.path.exists('templates'):
+            os.makedirs('templates')
+            # https://stackoverflow.com/a/58941536
+            original_template_dir = pkgutil.get_data(__name__, 'templates/')
+            shutil.copy(original_template_dir, 'templates')
     else:
         print("See --help for hints")
```

### Comparing `cagen-0.2.0a9/src/cagen/libcagen.py` & `cagen-0.2.0b1/src/cagen/libcagen.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,33 +50,46 @@
     def __init__(self, path: str):
         """Defines the `Entry` from `path`"""
         self.path = path
 
     @property
     def content(self) -> str:
         """Returns the content of the `Entry`"""
-        return frontmatter.load(self.path).content
+        if self.path != None:
+            return frontmatter.load(self.path).content
+        else:
+            return ""
 
     @property
     def metadata(self) -> dict:
         """Returns the YAML metadata header (as a `dict`) of the `Entry`"""
-        return frontmatter.load(self.path).metadata
+        if self.path != None:
+            return frontmatter.load(self.path).metadata
+        else:
+            return {}
 
     @property
     def to_dict(self) -> dict:
         """Returns the representation of `Entry` as a `dict`, containing metadata and content."""
-        return frontmatter.load(self.path).to_dict()
+        if self.path != None:
+            return frontmatter.load(self.path).to_dict()
+        else:
+            return {'content': ""}
 
     def __str__(self):
         """Defines a representation of `Entry` like `str`"""
-        post = frontmatter.load(self.path)
-        if 'title' in post.keys():
+
+        if self.path != None:
+            post = frontmatter.load(self.path)
+            if 'title' in post.keys():
                 return post['title']
-        else:
+            else:
                 return self.path
+        else:
+            return self.path
 
     def __repr__(self):
         """Defines object representation"""
         return self.path
 
     def __le__(self, other):
         """Returns when a <= b, where a and b are `Entry` instances."""
```

### Comparing `cagen-0.2.0a9/src/cagen/templates/schema.tmpl` & `cagen-0.2.0b1/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a9/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0b1/src/cagen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a9
-Summary: A static site generator for cmpalgorithms project
+Version: 0.2.0b1
+Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
@@ -58,22 +58,24 @@
 
 If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
-cagen sourcefile.md generatedfile.html template.tmpl
+cagen generatedfile.html template.tmpl --source sourcefile.md
 ```
 where 
 
 - `sourcefile.md` is Markdown file
 - `generatedfile.html` is the HTML5 file
 - `template.tmpl` is Mako template file
 
+The `source` argument is optional. In the case it is omitted, `cagen` just renders the template to `generatedfile.html`
+
 See `cagen --help` for more options.
 
 This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
 ```
 cagen-make --init
 ```
```

