# Comparing `tmp/pyparlaclarin-0.6.2.tar.gz` & `tmp/pyparlaclarin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparlaclarin-0.6.2.tar", max compression
+gzip compressed data, was "pyparlaclarin-0.7.0.tar", max compression
```

## Comparing `pyparlaclarin-0.6.2.tar` & `pyparlaclarin-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.6.2/README.md
--rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.6.2/pyparlaclarin/__init__.py
--rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.6.2/pyparlaclarin/create.py
--rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.6.2/pyparlaclarin/read.py
--rw-r--r--   0        0        0     5439 2023-02-14 11:59:28.135037 pyparlaclarin-0.6.2/pyparlaclarin/refine.py
--rw-r--r--   0        0        0      604 2023-02-14 11:59:47.790818 pyparlaclarin-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1332 2023-02-14 12:01:47.528951 pyparlaclarin-0.6.2/setup.py
--rw-r--r--   0        0        0     1495 2023-02-14 12:01:47.529311 pyparlaclarin-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.7.0/README.md
+-rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.7.0/pyparlaclarin/__init__.py
+-rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.7.0/pyparlaclarin/create.py
+-rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.7.0/pyparlaclarin/read.py
+-rw-r--r--   0        0        0     5731 2023-05-05 12:50:55.315484 pyparlaclarin-0.7.0/pyparlaclarin/refine.py
+-rw-r--r--   0        0        0      604 2023-05-05 12:51:20.320913 pyparlaclarin-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-05 12:52:33.067143 pyparlaclarin-0.7.0/setup.py
+-rw-r--r--   0        0        0     1495 2023-05-05 12:52:33.067568 pyparlaclarin-0.7.0/PKG-INFO
```

### Comparing `pyparlaclarin-0.6.2/README.md` & `pyparlaclarin-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.6.2/pyparlaclarin/create.py` & `pyparlaclarin-0.7.0/pyparlaclarin/create.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.6.2/pyparlaclarin/read.py` & `pyparlaclarin-0.7.0/pyparlaclarin/read.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.6.2/pyparlaclarin/refine.py` & `pyparlaclarin-0.7.0/pyparlaclarin/refine.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,35 +88,41 @@
             else:
                 prev_elem = elem
         else:
             prev_elem = elem
     return root
 
 
-def format_paragraph(paragraph, spaces=12):
+def format_paragraph(paragraph, spaces=12, preserve_lines=False):
     """
     Formats paragraphs to be equal in width.
 
     Args:
         paragraph: paragraph content, str.
         spaces: size of indentation as number of spaces.
     """
-    words = paragraph.replace("\n", "").strip().split()
     s = "\n" + " " * spaces
-    row = ""
-
-    for word in words:
-        if len(row) > 60:
-            s += row.strip() + "\n" + " " * spaces
-            row = word
-        else:
-            row += " " + word
+    if preserve_lines:
+        lines = [" ".join(line.split()) for line in paragraph.split("\n")]
+        for line in lines:
+            s += line.strip() + "\n" + " " * spaces
+            s += "\n" + " " * (spaces - 2)
+    else:
+        words = paragraph.replace("\n", "").strip().split()
+        row = ""
+
+        for word in words:
+            if len(row) > 60:
+                s += row.strip() + "\n" + " " * spaces
+                row = word
+            else:
+                row += " " + word
 
-    if len(row.strip()) > 0:
-        s += row.strip() + "\n" + " " * (spaces - 2)
+        if len(row.strip()) > 0:
+            s += row.strip() + "\n" + " " * (spaces - 2)
 
     if s.strip() == "":
         return None
     return s
 
 
 def format_texts(root, padding=12):
```

### Comparing `pyparlaclarin-0.6.2/pyproject.toml` & `pyparlaclarin-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyparlaclarin"
-version = "0.6.2"
+version = "0.7.0"
 description = "Read, create, and modify Parla-Clarin XML files"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/pyparlaclarin"
 documentation = "https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/"
 readme = "README.md"
 license = "MIT"
 packages = [
```

### Comparing `pyparlaclarin-0.6.2/setup.py` & `pyparlaclarin-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['pyparlaclarin']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyparlaclarin',
-    'version': '0.6.2',
+    'version': '0.7.0',
     'description': 'Read, create, and modify Parla-Clarin XML files',
     'long_description': '# Pyparlaclarin\n\nThis module includes functionality for reading, creating, and modifying Parla-Clarin XML files.\n\nFor instance, you can loop over all paragraphs in a Parla-Clarin file with a simple function:\n\n```python\nfrom pyparlaclarin.read import paragraph_iterator\n\nfor paragraph in paragraph_iterator(root):\n\tprint(paragraph)\n```\n\nor get all speeches by a speaker\n\n```python\nfrom pyparlaclarin.read import speeches_with_name\n\nfor speech in speeches_with_name(root, name="barack_obama_1961"):\n\tprint(speech)\n```\n\nFurther documentation is available on [GitHub pages](https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/).',
     'author': 'ninpnin',
     'author_email': 'vainoyrjanainen@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/welfare-state-analytics/pyparlaclarin',
```

### Comparing `pyparlaclarin-0.6.2/PKG-INFO` & `pyparlaclarin-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparlaclarin
-Version: 0.6.2
+Version: 0.7.0
 Summary: Read, create, and modify Parla-Clarin XML files
 Home-page: https://github.com/welfare-state-analytics/pyparlaclarin
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

