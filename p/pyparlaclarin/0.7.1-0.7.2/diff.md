# Comparing `tmp/pyparlaclarin-0.7.1.tar.gz` & `tmp/pyparlaclarin-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparlaclarin-0.7.1.tar", max compression
+gzip compressed data, was "pyparlaclarin-0.7.2.tar", max compression
```

## Comparing `pyparlaclarin-0.7.1.tar` & `pyparlaclarin-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.7.1/README.md
--rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.7.1/pyparlaclarin/__init__.py
--rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.7.1/pyparlaclarin/create.py
--rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.7.1/pyparlaclarin/read.py
--rw-r--r--   0        0        0     5815 2023-05-05 12:56:54.925890 pyparlaclarin-0.7.1/pyparlaclarin/refine.py
--rw-r--r--   0        0        0      604 2023-05-05 12:57:02.682623 pyparlaclarin-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1332 2023-05-05 12:57:11.465326 pyparlaclarin-0.7.1/setup.py
--rw-r--r--   0        0        0     1495 2023-05-05 12:57:11.465489 pyparlaclarin-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.7.2/README.md
+-rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.7.2/pyparlaclarin/__init__.py
+-rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.7.2/pyparlaclarin/create.py
+-rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.7.2/pyparlaclarin/read.py
+-rw-r--r--   0        0        0     5880 2023-05-05 12:59:39.989246 pyparlaclarin-0.7.2/pyparlaclarin/refine.py
+-rw-r--r--   0        0        0      604 2023-05-05 13:02:10.201889 pyparlaclarin-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-05 13:02:15.959122 pyparlaclarin-0.7.2/setup.py
+-rw-r--r--   0        0        0     1495 2023-05-05 13:02:15.959292 pyparlaclarin-0.7.2/PKG-INFO
```

### Comparing `pyparlaclarin-0.7.1/README.md` & `pyparlaclarin-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.1/pyparlaclarin/create.py` & `pyparlaclarin-0.7.2/pyparlaclarin/create.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.1/pyparlaclarin/read.py` & `pyparlaclarin-0.7.2/pyparlaclarin/read.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.1/pyparlaclarin/refine.py` & `pyparlaclarin-0.7.2/pyparlaclarin/refine.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,17 +99,20 @@
     Args:
         paragraph: paragraph content, str.
         spaces: size of indentation as number of spaces.
     """
     s = "\n" + " " * spaces
     if preserve_lines:
         lines = [" ".join(line.split()) for line in paragraph.split("\n")]
-        for line in lines:
+        for line in lines[:-1]:
             s += line.strip() + "\n" + " " * spaces
-            s += "\n" + " " * (spaces - 2)
+        
+        if len(lines) >= 1:
+            s += lines[-1]
+        s += "\n" + " " * (spaces - 2)
     else:
         words = paragraph.replace("\n", "").strip().split()
         row = ""
 
         for word in words:
             if len(row) > 60:
                 s += row.strip() + "\n" + " " * spaces
```

### Comparing `pyparlaclarin-0.7.1/pyproject.toml` & `pyparlaclarin-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyparlaclarin"
-version = "0.7.1"
+version = "0.7.2"
 description = "Read, create, and modify Parla-Clarin XML files"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/pyparlaclarin"
 documentation = "https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/"
 readme = "README.md"
 license = "MIT"
 packages = [
```

### Comparing `pyparlaclarin-0.7.1/setup.py` & `pyparlaclarin-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['pyparlaclarin']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyparlaclarin',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'Read, create, and modify Parla-Clarin XML files',
     'long_description': '# Pyparlaclarin\n\nThis module includes functionality for reading, creating, and modifying Parla-Clarin XML files.\n\nFor instance, you can loop over all paragraphs in a Parla-Clarin file with a simple function:\n\n```python\nfrom pyparlaclarin.read import paragraph_iterator\n\nfor paragraph in paragraph_iterator(root):\n\tprint(paragraph)\n```\n\nor get all speeches by a speaker\n\n```python\nfrom pyparlaclarin.read import speeches_with_name\n\nfor speech in speeches_with_name(root, name="barack_obama_1961"):\n\tprint(speech)\n```\n\nFurther documentation is available on [GitHub pages](https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/).',
     'author': 'ninpnin',
     'author_email': 'vainoyrjanainen@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/welfare-state-analytics/pyparlaclarin',
```

### Comparing `pyparlaclarin-0.7.1/PKG-INFO` & `pyparlaclarin-0.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparlaclarin
-Version: 0.7.1
+Version: 0.7.2
 Summary: Read, create, and modify Parla-Clarin XML files
 Home-page: https://github.com/welfare-state-analytics/pyparlaclarin
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

