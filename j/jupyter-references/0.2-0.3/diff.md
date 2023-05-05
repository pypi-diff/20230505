# Comparing `tmp/jupyter-references-0.2.tar.gz` & `tmp/jupyter-references-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-references-0.2.tar", last modified: Fri May  5 17:14:13 2023, max compression
+gzip compressed data, was "jupyter-references-0.3.tar", last modified: Fri May  5 17:50:28 2023, max compression
```

## Comparing `jupyter-references-0.2.tar` & `jupyter-references-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.047169 jupyter-references-0.2/
--rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.2/LICENSE
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:14:13.046932 jupyter-references-0.2/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.2/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.041507 jupyter-references-0.2/jupyter_references/
--rw-r--r--   0 kmt        (501) staff       (20)     3275 2023-05-05 17:06:41.000000 jupyter-references-0.2/jupyter_references/__init__.py
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.046074 jupyter-references-0.2/jupyter_references.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/requires.txt
--rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 17:14:13.047228 jupyter-references-0.2/setup.cfg
--rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 17:14:08.000000 jupyter-references-0.2/setup.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:50:28.174537 jupyter-references-0.3/
+-rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.3/LICENSE
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:50:28.174234 jupyter-references-0.3/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.3/README.md
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:50:28.160442 jupyter-references-0.3/jupyter_references/
+-rw-r--r--   0 kmt        (501) staff       (20)     3349 2023-05-05 17:49:56.000000 jupyter-references-0.3/jupyter_references/__init__.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:50:28.173103 jupyter-references-0.3/jupyter_references.egg-info/
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:50:28.000000 jupyter-references-0.3/jupyter_references.egg-info/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 17:50:28.000000 jupyter-references-0.3/jupyter_references.egg-info/SOURCES.txt
+-rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 17:50:28.000000 jupyter-references-0.3/jupyter_references.egg-info/dependency_links.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 17:50:28.000000 jupyter-references-0.3/jupyter_references.egg-info/requires.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 17:50:28.000000 jupyter-references-0.3/jupyter_references.egg-info/top_level.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 17:50:28.174602 jupyter-references-0.3/setup.cfg
+-rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 17:50:05.000000 jupyter-references-0.3/setup.py
```

### Comparing `jupyter-references-0.2/LICENSE` & `jupyter-references-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.2/PKG-INFO` & `jupyter-references-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.2
+Version: 0.3
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.2/README.md` & `jupyter-references-0.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.2/jupyter_references/__init__.py` & `jupyter-references-0.3/jupyter_references/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     @line_magic
     def replace_content(self, line):
         self.shell.set_next_input(line, replace=True)
         
 ip = get_ipython()
 ip.register_magics(MyMagics)
 
-def cite(cb=clipboard.osx_clipboard_get()):
+def cite(cb=None):
+    if cb is None:
+        cb = clipboard.osx_clipboard_get()
     bibtex_entries = re.findall(r'\@[^\@]+', cb)
     cite_list = []
     for i, entry in enumerate(bibtex_entries):
 
         match = re.search(r'@\w+{([^,]+).*year = {(\d+)}.*title = {{(.*)}}.*author = {([^,]+)', entry, re.DOTALL)
         if match:
             url, year, title, author = match.groups()
@@ -35,15 +37,17 @@
                     cite_list.append(f'[{author} {year},](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")')
     content = ' '.join(cite_list)
     if content:
         get_ipython().run_line_magic('replace_content', f"{content}") 
     else:
         print('clipboard is not bibtex:', cb)
         
-def incite(cb=clipboard.osx_clipboard_get()):
+def incite(cb=None):
+    if cb is None:
+        cb = clipboard.osx_clipboard_get()
     bibtex_entries = re.findall(r'\@[^\@]+', cb)
     if len(bibtex_entries) > 1:
         print('clipboard has bibtex entries:', cb)
     else:
         match = re.search(r'@\w+{([^,]+).*year = {(\d+)}.*title = {{(.*)}}.*author = {([^,]+)',
             cb, re.DOTALL)
         if match:
```

### Comparing `jupyter-references-0.2/jupyter_references.egg-info/PKG-INFO` & `jupyter-references-0.3/jupyter_references.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.2
+Version: 0.3
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.2/setup.py` & `jupyter-references-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 # package name must be the git repository name
 package_name = path.basename(this_directory)
 
 setuptools.setup(
     name=package_name,
-    version="0.2",
+    version="0.3",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Lightweight system for citing papers and making a reference list in jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f'https://github.com/kaspermunch/{package_name}',
     packages=setuptools.find_packages(),
```

