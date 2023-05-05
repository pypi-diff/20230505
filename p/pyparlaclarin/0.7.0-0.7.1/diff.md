# Comparing `tmp/pyparlaclarin-0.7.0.tar.gz` & `tmp/pyparlaclarin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparlaclarin-0.7.0.tar", max compression
+gzip compressed data, was "pyparlaclarin-0.7.1.tar", max compression
```

## Comparing `pyparlaclarin-0.7.0.tar` & `pyparlaclarin-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.7.0/README.md
--rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.7.0/pyparlaclarin/__init__.py
--rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.7.0/pyparlaclarin/create.py
--rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.7.0/pyparlaclarin/read.py
--rw-r--r--   0        0        0     5731 2023-05-05 12:50:55.315484 pyparlaclarin-0.7.0/pyparlaclarin/refine.py
--rw-r--r--   0        0        0      604 2023-05-05 12:51:20.320913 pyparlaclarin-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1332 2023-05-05 12:52:33.067143 pyparlaclarin-0.7.0/setup.py
--rw-r--r--   0        0        0     1495 2023-05-05 12:52:33.067568 pyparlaclarin-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.7.1/README.md
+-rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.7.1/pyparlaclarin/__init__.py
+-rw-r--r--   0        0        0     3595 2021-10-25 14:50:08.220709 pyparlaclarin-0.7.1/pyparlaclarin/create.py
+-rw-r--r--   0        0        0     5031 2021-11-29 17:34:22.618350 pyparlaclarin-0.7.1/pyparlaclarin/read.py
+-rw-r--r--   0        0        0     5815 2023-05-05 12:56:54.925890 pyparlaclarin-0.7.1/pyparlaclarin/refine.py
+-rw-r--r--   0        0        0      604 2023-05-05 12:57:02.682623 pyparlaclarin-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-05 12:57:11.465326 pyparlaclarin-0.7.1/setup.py
+-rw-r--r--   0        0        0     1495 2023-05-05 12:57:11.465489 pyparlaclarin-0.7.1/PKG-INFO
```

### Comparing `pyparlaclarin-0.7.0/README.md` & `pyparlaclarin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.0/pyparlaclarin/create.py` & `pyparlaclarin-0.7.1/pyparlaclarin/create.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.0/pyparlaclarin/read.py` & `pyparlaclarin-0.7.1/pyparlaclarin/read.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.7.0/pyparlaclarin/refine.py` & `pyparlaclarin-0.7.1/pyparlaclarin/refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,43 +121,43 @@
             s += row.strip() + "\n" + " " * (spaces - 2)
 
     if s.strip() == "":
         return None
     return s
 
 
-def format_texts(root, padding=12):
+def format_texts(root, padding=12, preserve_lines=False):
     """
     Formats all text elements in a Parla-Clarin document.
 
     Args:
         root: Parla-Clarin document as an lxml tree root.
     """
     for tag, elem in _iter(root):
 
         # Format notes' text content
         # Remove notes with no text content
         if tag == "note":
             if type(elem.text) == str:
-                elem.text = format_paragraph(elem.text, spaces=padding)
+                elem.text = format_paragraph(elem.text, spaces=padding, preserve_lines=preserve_lines)
             else:
                 elem.text = None
             if elem.text is None:
                 elem.getparent().remove(elem)
 
         # Remove u's with no children
         elif tag == "u":
             if len("".join(elem.itertext())) == 0:
                 elem.getparent().remove(elem)
             elif len(list(elem)) > 0:
                 # Format segs' text content
                 # Remove segs with no text content
                 for seg in elem:
                     if type(seg.text) == str:
-                        seg.text = format_paragraph(seg.text, spaces=padding+2)
+                        seg.text = format_paragraph(seg.text, spaces=padding+2, preserve_lines=preserve_lines)
                     else:
                         seg.text = None
                     if seg.text is None:
                         seg.getparent().remove(seg)
                 elem.text = None
             else:
                 elem.getparent().remove(elem)
```

### Comparing `pyparlaclarin-0.7.0/pyproject.toml` & `pyparlaclarin-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyparlaclarin"
-version = "0.7.0"
+version = "0.7.1"
 description = "Read, create, and modify Parla-Clarin XML files"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/pyparlaclarin"
 documentation = "https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/"
 readme = "README.md"
 license = "MIT"
 packages = [
```

### Comparing `pyparlaclarin-0.7.0/setup.py` & `pyparlaclarin-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['pyparlaclarin']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyparlaclarin',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Read, create, and modify Parla-Clarin XML files',
     'long_description': '# Pyparlaclarin\n\nThis module includes functionality for reading, creating, and modifying Parla-Clarin XML files.\n\nFor instance, you can loop over all paragraphs in a Parla-Clarin file with a simple function:\n\n```python\nfrom pyparlaclarin.read import paragraph_iterator\n\nfor paragraph in paragraph_iterator(root):\n\tprint(paragraph)\n```\n\nor get all speeches by a speaker\n\n```python\nfrom pyparlaclarin.read import speeches_with_name\n\nfor speech in speeches_with_name(root, name="barack_obama_1961"):\n\tprint(speech)\n```\n\nFurther documentation is available on [GitHub pages](https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/).',
     'author': 'ninpnin',
     'author_email': 'vainoyrjanainen@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/welfare-state-analytics/pyparlaclarin',
```

### Comparing `pyparlaclarin-0.7.0/PKG-INFO` & `pyparlaclarin-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparlaclarin
-Version: 0.7.0
+Version: 0.7.1
 Summary: Read, create, and modify Parla-Clarin XML files
 Home-page: https://github.com/welfare-state-analytics/pyparlaclarin
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

