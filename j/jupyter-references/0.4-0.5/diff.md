# Comparing `tmp/jupyter-references-0.4.tar.gz` & `tmp/jupyter-references-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-references-0.4.tar", last modified: Fri May  5 18:23:36 2023, max compression
+gzip compressed data, was "jupyter-references-0.5.tar", last modified: Fri May  5 18:44:54 2023, max compression
```

## Comparing `jupyter-references-0.4.tar` & `jupyter-references-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:23:36.360760 jupyter-references-0.4/
--rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.4/LICENSE
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:23:36.360303 jupyter-references-0.4/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.4/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:23:36.357192 jupyter-references-0.4/jupyter_references/
--rw-r--r--   0 kmt        (501) staff       (20)     3597 2023-05-05 18:22:33.000000 jupyter-references-0.4/jupyter_references/__init__.py
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:23:36.359968 jupyter-references-0.4/jupyter_references.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:23:36.000000 jupyter-references-0.4/jupyter_references.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 18:23:36.000000 jupyter-references-0.4/jupyter_references.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 18:23:36.000000 jupyter-references-0.4/jupyter_references.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 18:23:36.000000 jupyter-references-0.4/jupyter_references.egg-info/requires.txt
--rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 18:23:36.000000 jupyter-references-0.4/jupyter_references.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 18:23:36.360826 jupyter-references-0.4/setup.cfg
--rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 18:22:51.000000 jupyter-references-0.4/setup.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.335440 jupyter-references-0.5/
+-rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.5/LICENSE
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:44:54.335176 jupyter-references-0.5/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.5/README.md
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.327954 jupyter-references-0.5/jupyter_references/
+-rw-r--r--   0 kmt        (501) staff       (20)     3632 2023-05-05 18:44:11.000000 jupyter-references-0.5/jupyter_references/__init__.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.334792 jupyter-references-0.5/jupyter_references.egg-info/
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/SOURCES.txt
+-rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/dependency_links.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/requires.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/top_level.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 18:44:54.335494 jupyter-references-0.5/setup.cfg
+-rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 18:44:19.000000 jupyter-references-0.5/setup.py
```

### Comparing `jupyter-references-0.4/LICENSE` & `jupyter-references-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.4/PKG-INFO` & `jupyter-references-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.4
+Version: 0.5
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.4/README.md` & `jupyter-references-0.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.4/jupyter_references/__init__.py` & `jupyter-references-0.5/jupyter_references/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,25 +54,25 @@
             ref_list = {}
             url, year, title, author = match.groups()
             content = f'{author} et al. [({year})](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")'
             get_ipython().run_line_magic('replace_content', f"{content}") 
         else:
             print('clipboard is not bibtex:', cb)
         
-def reflist(file_name=None):
+def reflist(file_base_name=None):
     regex = re.compile(r'\d+\s+"([^"]+)"')
     references = {}
-    if file_name is None:
-        file_name = os.path.abspath(ipynbname.name()+'.ipynb')
-    if type(file_name) is not list:
-        file_names = [file_name]
+    if file_base_name is None:
+        file_base_name = ipynbname.name()
+    if type(file_base_name) is not list:
+        file_base_names = [file_base_name]
     else:
-        file_names = file_name
-    for file_name in file_names:
-        with open(file_name) as f:
+        file_base_names = file_base_name
+    for name in file_base_names:
+        with open(os.path.abspath(name+'.ipynb')) as f:
             notebook_json = json.load(f)
         for cell in notebook_json['cells']:
             if cell['cell_type'] == 'markdown':
                 source = ''.join(cell['source'])
                 for ref in regex.findall(source):
                     author, year, title, doi = ref.split('\n')
                     references[ref] = dict(author=author.strip(),
```

### Comparing `jupyter-references-0.4/jupyter_references.egg-info/PKG-INFO` & `jupyter-references-0.5/jupyter_references.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.4
+Version: 0.5
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.4/setup.py` & `jupyter-references-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 # package name must be the git repository name
 package_name = path.basename(this_directory)
 
 setuptools.setup(
     name=package_name,
-    version="0.4",
+    version="0.5",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Lightweight system for citing papers and making a reference list in jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f'https://github.com/kaspermunch/{package_name}',
     packages=setuptools.find_packages(),
```

