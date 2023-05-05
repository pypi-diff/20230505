# Comparing `tmp/pyaml-23.5.5.tar.gz` & `tmp/pyaml-23.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-23.5.5.tar", last modified: Fri May  5 00:42:12 2023, max compression
+gzip compressed data, was "pyaml-23.5.6.tar", last modified: Fri May  5 01:07:09 2023, max compression
```

## Comparing `pyaml-23.5.5.tar` & `pyaml-23.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.5/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.5/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9618 2023-05-05 00:42:12.326240 pyaml-23.5.5/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8914 2023-05-05 00:40:31.000000 pyaml-23.5.5/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     7428 2023-05-05 00:29:16.000000 pyaml-23.5.5/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.5/pyaml/__main__.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.5/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16678 2023-05-04 23:58:10.000000 pyaml-23.5.5/pyaml/tests/test_dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9618 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 00:41:09.000000 pyaml-23.5.5/pyproject.toml
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 00:42:12.326240 pyaml-23.5.5/setup.cfg
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.5/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.564579 pyaml-23.5.6/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.6/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.6/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9630 2023-05-05 01:07:09.564579 pyaml-23.5.6/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8926 2023-05-05 00:46:59.000000 pyaml-23.5.6/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.563579 pyaml-23.5.6/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     7503 2023-05-05 01:03:54.000000 pyaml-23.5.6/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.6/pyaml/__main__.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.564579 pyaml-23.5.6/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.6/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16678 2023-05-04 23:58:10.000000 pyaml-23.5.6/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.563579 pyaml-23.5.6/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9630 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 01:06:52.000000 pyaml-23.5.6/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 01:07:09.564579 pyaml-23.5.6/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.6/setup.py
```

### Comparing `pyaml-23.5.5/PKG-INFO` & `pyaml-23.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.5
+Version: 23.5.6
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
@@ -20,15 +20,15 @@
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -144,15 +144,15 @@
     - 45.67
     - 1:
       2: no
     - some text
 
   mb: *ma
 
-(force_embed enabled deduplication with ``&ma`` anchor,
+(force_embed=False enabled deduplication with ``&ma`` anchor,
 vspacing is adjusted to split even this tiny output)
 
 ----------
 
 Extended example::
 
   >>> pyaml.dump(data, vspacing=dict(split_lines=10))
```

### Comparing `pyaml-23.5.5/README.rst` & `pyaml-23.5.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -126,15 +126,15 @@
     - 45.67
     - 1:
       2: no
     - some text
 
   mb: *ma
 
-(force_embed enabled deduplication with ``&ma`` anchor,
+(force_embed=False enabled deduplication with ``&ma`` anchor,
 vspacing is adjusted to split even this tiny output)
 
 ----------
 
 Extended example::
 
   >>> pyaml.dump(data, vspacing=dict(split_lines=10))
```

### Comparing `pyaml-23.5.5/pyaml/__init__.py` & `pyaml-23.5.6/pyaml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,19 @@
 
 
 def dump( data, dst=str, safe=None, force_embed=True, vspacing=True,
 		string_val_style=None, sort_dicts=None, multiple_docs=False, **pyyaml_kws ):
 	'Serialize data as pretty-YAML to either specified dst file-like object, or str/bytes'
 	if safe is not None:
 		warnings.warn( 'pyaml module "safe" arg/keyword'
-			' is ignored as implicit safe=True, as of pyaml >= 23.x' )
+			' is ignored as implicit safe=False, as of pyaml >= 23.x', stacklevel=2 )
 	if sort_dicts is not None:
-		warnings.warn( 'pyaml module "sort_dicts" arg/keyword'
-			' is ignored as of pyaml >= 23.x - translated to sort_keys pyaml keyword' )
+		warnings.warn( 'pyaml module "sort_dicts" arg/keyword is deprecated as of'
+				' pyaml >= 23.x - translated to sort_keys PyYAML keyword, use that instead',
+			DeprecationWarning, stacklevel=2 )
 
 	buff = io.StringIO()
 	Dumper = lambda *a,**kw: PYAMLDumper( *a, **kw,
 		force_embed=force_embed, string_val_style=string_val_style, sort_dicts=sort_dicts )
 	if not multiple_docs: data = [data]
 	else: pyyaml_kws.setdefault('explicit_start', True)
 	yaml.dump_all( data, buff, Dumper=Dumper,
```

### Comparing `pyaml-23.5.5/pyaml/__main__.py` & `pyaml-23.5.6/pyaml/__main__.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.5/pyaml/tests/test_dump.py` & `pyaml-23.5.6/pyaml/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.5/pyaml.egg-info/PKG-INFO` & `pyaml-23.5.6/pyaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.5
+Version: 23.5.6
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
@@ -20,15 +20,15 @@
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -144,15 +144,15 @@
     - 45.67
     - 1:
       2: no
     - some text
 
   mb: *ma
 
-(force_embed enabled deduplication with ``&ma`` anchor,
+(force_embed=False enabled deduplication with ``&ma`` anchor,
 vspacing is adjusted to split even this tiny output)
 
 ----------
 
 Extended example::
 
   >>> pyaml.dump(data, vspacing=dict(split_lines=10))
```

### Comparing `pyaml-23.5.5/pyproject.toml` & `pyaml-23.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pyaml"
-version = "23.05.05"
+version = "23.05.06"
 
 description = "PyYAML-based module to produce a bit more pretty and readable YAML-serialized data"
 authors = [{name="Mike Kazantsev", email="mk.fraggod@gmail.com"}]
 license = {text="WTFPL"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
```

