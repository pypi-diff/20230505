# Comparing `tmp/pyaml-23.5.6.tar.gz` & `tmp/pyaml-23.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-23.5.6.tar", last modified: Fri May  5 01:07:09 2023, max compression
+gzip compressed data, was "pyaml-23.5.7.tar", last modified: Fri May  5 17:04:11 2023, max compression
```

## Comparing `pyaml-23.5.6.tar` & `pyaml-23.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.564579 pyaml-23.5.6/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.6/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.6/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9630 2023-05-05 01:07:09.564579 pyaml-23.5.6/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8926 2023-05-05 00:46:59.000000 pyaml-23.5.6/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.563579 pyaml-23.5.6/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     7503 2023-05-05 01:03:54.000000 pyaml-23.5.6/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.6/pyaml/__main__.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.564579 pyaml-23.5.6/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.6/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16678 2023-05-04 23:58:10.000000 pyaml-23.5.6/pyaml/tests/test_dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 01:07:09.563579 pyaml-23.5.6/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9630 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 01:07:09.000000 pyaml-23.5.6/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 01:06:52.000000 pyaml-23.5.6/pyproject.toml
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 01:07:09.564579 pyaml-23.5.6/setup.cfg
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.6/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.7/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.7/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9729 2023-05-05 17:04:11.721541 pyaml-23.5.7/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9025 2023-05-05 13:06:24.000000 pyaml-23.5.7/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.720541 pyaml-23.5.7/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8951 2023-05-05 16:33:35.000000 pyaml-23.5.7/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.7/pyaml/__main__.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.7/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17672 2023-05-05 13:24:38.000000 pyaml-23.5.7/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9729 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 08:02:00.000000 pyaml-23.5.7/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 17:04:11.721541 pyaml-23.5.7/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.7/setup.py
```

### Comparing `pyaml-23.5.6/PKG-INFO` & `pyaml-23.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.6
+Version: 23.5.7
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
@@ -20,15 +20,18 @@
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+(side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there)
+
+It's a small module, and for projects that only need part of its functionality,
+I'd recommend copy-pasting that in, instead of adding janky dependency.
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -38,20 +41,16 @@
 - https://codeberg.org/mk-fg/pretty-yaml
 - https://fraggod.net/code/git/pretty-yaml
 
 
 Warning
 -------
 
-Prime goal of this module is to produce human-readable output that can be easily
-manipulated and re-used, but maybe with some occasional caveats.
-
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
-to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
-as an integer from that, but here it's a feature.
+Prime goal of this module is to produce human-readable output that can be
+easily diff'ed, manipulated and re-used, but maybe with occasional issues.
 
 So please do not rely on the thing to produce output that can always be
 deserialized exactly to what was exported, at least - use PyYAML directly
 for that (but maybe with options from the next section).
 
 
 What this module does and why
@@ -83,18 +82,19 @@
 
 * Most human-friendly representation options in PyYAML (that I know of)
   are used as defaults.
 
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
-* Use shorter and simplier yes/no for booleans.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
+  are represented as their safe YAML-compatible base (like int, list or mapping),
+  with mappings key-sorted by default for more diff-friendly output.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and key-sorted by default, for more diff-friendly output.
+* Use shorter and simplier yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -125,14 +125,16 @@
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
 * Add vertical spacing (empty lines) between keys on different depths,
   to separate long YAML sections in the output visually, make it more seekable.
 
+* Discard end-of-document "..." indicators for simple values.
+
 Result for the (rather meaningless) example above::
 
   >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
   a: |
     asldnsa
     asldpáknsa
@@ -212,18 +214,18 @@
         level: 0
 
     root:
       handlers:
         - console
       level: custom
 
-Note that unless there are many moderately wide and deep trees of data, which
-are expected to be read and edited by people, it might be preferrable to
-directly use PyYAML regardless, as it won't introduce another (rather pointless
-in that case) dependency and a point of failure.
+Note that unless there are many moderately wide and deep trees of data,
+which are expected to be read and edited by people, it might be preferrable
+to directly use PyYAML regardless, as it won't introduce another
+(rather pointless in that case) dependency and a point of failure.
 
 
 Some Tricks
 -----------
 
 * Pretty-print any yaml or json (yaml subset) file from the shell::
```

### Comparing `pyaml-23.5.6/README.rst` & `pyaml-23.5.7/pyaml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,37 @@
+Metadata-Version: 2.1
+Name: pyaml
+Version: 23.5.7
+Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
+Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
+License: WTFPL
+Keywords: yaml,serialization,pretty-print,formatter,human,readability
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: Public Domain
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: anchors
+
 pretty-yaml (or pyaml)
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+(side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there)
+
+It's a small module, and for projects that only need part of its functionality,
+I'd recommend copy-pasting that in, instead of adding janky dependency.
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -20,20 +41,16 @@
 - https://codeberg.org/mk-fg/pretty-yaml
 - https://fraggod.net/code/git/pretty-yaml
 
 
 Warning
 -------
 
-Prime goal of this module is to produce human-readable output that can be easily
-manipulated and re-used, but maybe with some occasional caveats.
-
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
-to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
-as an integer from that, but here it's a feature.
+Prime goal of this module is to produce human-readable output that can be
+easily diff'ed, manipulated and re-used, but maybe with occasional issues.
 
 So please do not rely on the thing to produce output that can always be
 deserialized exactly to what was exported, at least - use PyYAML directly
 for that (but maybe with options from the next section).
 
 
 What this module does and why
@@ -65,18 +82,19 @@
 
 * Most human-friendly representation options in PyYAML (that I know of)
   are used as defaults.
 
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
-* Use shorter and simplier yes/no for booleans.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
+  are represented as their safe YAML-compatible base (like int, list or mapping),
+  with mappings key-sorted by default for more diff-friendly output.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and key-sorted by default, for more diff-friendly output.
+* Use shorter and simplier yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -107,14 +125,16 @@
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
 * Add vertical spacing (empty lines) between keys on different depths,
   to separate long YAML sections in the output visually, make it more seekable.
 
+* Discard end-of-document "..." indicators for simple values.
+
 Result for the (rather meaningless) example above::
 
   >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
   a: |
     asldnsa
     asldpáknsa
@@ -194,18 +214,18 @@
         level: 0
 
     root:
       handlers:
         - console
       level: custom
 
-Note that unless there are many moderately wide and deep trees of data, which
-are expected to be read and edited by people, it might be preferrable to
-directly use PyYAML regardless, as it won't introduce another (rather pointless
-in that case) dependency and a point of failure.
+Note that unless there are many moderately wide and deep trees of data,
+which are expected to be read and edited by people, it might be preferrable
+to directly use PyYAML regardless, as it won't introduce another
+(rather pointless in that case) dependency and a point of failure.
 
 
 Some Tricks
 -----------
 
 * Pretty-print any yaml or json (yaml subset) file from the shell::
```

### Comparing `pyaml-23.5.6/pyaml/__init__.py` & `pyaml-23.5.7/pyaml/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os, sys, io, re, string, warnings, pathlib, collections as cs
 
 import yaml
 
 
 class PYAMLDumper(yaml.dumper.SafeDumper):
 
+	class str_ext(str): __slots__ = 'ext',
 	pyaml_anchor_decode = None # imported from unidecode module when needed
 
 	def __init__(self, *args, **kws):
 		self.pyaml_force_embed = kws.pop('force_embed', True)
 		self.pyaml_string_val_style = kws.pop('string_val_style', None)
 		if (sort_keys := kws.pop('sort_dicts', None)) is not None:
 			self.sort_keys = sort_keys # for compatibility with <23.x module options
@@ -54,42 +55,68 @@
 			self.write_indent()
 			self.write_indicator('-', True, indention=True)
 			self.states.append(self.expect_block_sequence_item)
 			self.expect_node(sequence=True)
 
 	def check_simple_key(self):
 		res = super().check_simple_key()
-		self.analysis.allow_flow_plain = False
+		if self.analysis: self.analysis.allow_flow_plain = False
 		return res
 
 	def choose_scalar_style(self, _re1=re.compile(r':(\s|$)')):
 		if self.states[-1] == self.expect_block_mapping_simple_value:
-			# Don't override string style for dict keys
+			# Mapping keys - disable overriding string style, strip comments
 			if self.pyaml_string_val_style: self.event.style = 'plain'
+			if isinstance(self.analysis.scalar, self.str_ext):
+				self.analysis.scalar = str(self.event.value)
 		# Do default thing for complicated stuff
 		if self.event.style != 'plain': return super().choose_scalar_style()
 		# Make sure style isn't overidden for strings like list/mapping items
 		if (s := self.event.value).startswith('- ') or _re1.search(s): return "'"
+		# Returned style=None picks write_plain in Emitter.process_scalar
+
+	def write_indicator(self, indicator, *args, **kws):
+		if indicator == '...': return # presumably it's useful somewhere, but don't care
+		super().write_indicator(indicator, *args, **kws)
 
 	def represent_str(self, data):
 		if not (style := self.pyaml_string_val_style):
 			if '\n' in data[:-1]:
 				style = 'literal'
 				for line in data.splitlines():
 					if len(line) > self.best_width: break
 				else: style = '|'
 		return yaml.representer.ScalarNode('tag:yaml.org,2002:str', data, style=style)
 
 	def represent_undefined(self, data):
 		if isinstance(data, tuple) and hasattr(data, '_make') and hasattr(data, '_asdict'):
 			return self.represent_dict(data._asdict()) # assuming namedtuple
-		elif isinstance(data, dict): return self.represent_dict(data) # some kind of dict
-		elif callable(getattr(data, 'tolist', None)):
-			return self.represent_data(data.tolist()) # numpy arrays
-		return super().represent_undefined(data)
+		if isinstance(data, cs.abc.Mapping): return self.represent_dict(data) # dict-like
+		if type(data).__class__.__module__ == 'enum':
+			node = self.represent_data(data.value)
+			node.value = self.str_ext(node.value)
+			node.value.ext = f'# {str(data)}'
+			return node
+		if hasattr(type(data), '__dataclass_fields__'):
+			try: import dataclasses as dcs
+			except ImportError: pass # can still be something else
+			else: return self.represent_dict(dcs.asdict(data))
+		try: # this is for numpy arrays, and the likes
+			if not callable(getattr(data, 'tolist', None)): raise AttributeError
+		except: pass # can raise other errors with custom types
+		else: return self.represent_data(data.tolist())
+		return super().represent_undefined(data) # will raise RepresenterError
+
+	def write_ext(self, func, text, *args, **kws):
+		# Emitter write-funcs extension to append comments to values
+		getattr(super(), f'write_{func}')(text, *args, **kws)
+		if ext := getattr(text, 'ext', None): super().write_plain(ext)
+	write_folded = lambda s,v,*a,**kw: s.write_ext('folded', v, *a, **kw)
+	write_literal = lambda s,v,*a,**kw: s.write_ext('literal', v, *a, **kw)
+	write_plain = lambda s,v,*a,**kw: s.write_ext('plain', v, *a, **kw)
 
 
 # Unsafe was a separate class in <23.x versions, left here for compatibility
 UnsafePYAMLDumper = PYAMLDumper
 
 add_representer = PYAMLDumper.add_representer
 
@@ -134,16 +161,17 @@
 	return re.sub(r'\n\n+', '\n\n', yaml_str.strip() + '\n')
 
 
 def dump( data, dst=str, safe=None, force_embed=True, vspacing=True,
 		string_val_style=None, sort_dicts=None, multiple_docs=False, **pyyaml_kws ):
 	'Serialize data as pretty-YAML to either specified dst file-like object, or str/bytes'
 	if safe is not None:
-		warnings.warn( 'pyaml module "safe" arg/keyword'
-			' is ignored as implicit safe=False, as of pyaml >= 23.x', stacklevel=2 )
+		cat = DeprecationWarning if not safe else UserWarning
+		warnings.warn( 'pyaml module "safe" arg/keyword is ignored as implicit'
+			' safe=maybe-true?, as of pyaml >= 23.x', category=cat, stacklevel=2 )
 	if sort_dicts is not None:
 		warnings.warn( 'pyaml module "sort_dicts" arg/keyword is deprecated as of'
 				' pyaml >= 23.x - translated to sort_keys PyYAML keyword, use that instead',
 			DeprecationWarning, stacklevel=2 )
 
 	buff = io.StringIO()
 	Dumper = lambda *a,**kw: PYAMLDumper( *a, **kw,
@@ -170,20 +198,22 @@
 	elif dst is str: return buff
 	else:
 		try: dst.write(b'') # tests if dst is str- or bytestream
 		except: dst.write(buff)
 		else: dst.write(buff.encode())
 
 
+# Simplier pyaml.dump() aliases
+
 def dump_all(data, *dump_args, **dump_kws):
 	return dump(data, *dump_args, multiple_docs=True, **dump_kws)
 
 def dumps(data, **dump_kws):
 	return dump(data, **dump_kws)
 
 def pprint(*data, **dump_kws):
 	dst = dump_kws.pop('file', dump_kws.pop('dst', sys.stdout))
 	if len(data) == 1: data, = data
 	dump(data, dst=dst, **dump_kws)
 
 p, _p = pprint, print
-print = pprint # pyaml.print() won't work without "from __future__ import print_function"
+print = pprint
```

### Comparing `pyaml-23.5.6/pyaml/__main__.py` & `pyaml-23.5.7/pyaml/__main__.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.6/pyaml/tests/test_dump.py` & `pyaml-23.5.7/pyaml/tests/test_dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, sys, io, unittest, json, collections as cs
+import os, sys, io, unittest, json, enum, collections as cs
 
 import yaml
 
 try: import pyaml
 except ImportError:
 	sys.path.insert(1, os.path.join(__file__, *['..']*3))
 	import pyaml
@@ -148,23 +148,27 @@
       handlers: [console]
       level: 0
   root:
     level: custom
     handlers: [console]
 '''
 
+class test_const(enum.IntEnum):
+	dispatch = 2455
+	heartbeat = 123
+
 data = dict(
 	path='/some/path',
 	query_dump=cs.OrderedDict([
 		('key1', 'тест1'),
 		('key2', 'тест2'),
 		('key3', 'тест3'),
 		('последний', None) ]),
 	ids=cs.OrderedDict(),
-	a=[1,None,'asd', 'не-ascii'], b=3.5, c=None,
+	a=[1,None,'asd', 'не-ascii'], b=3.5, c=None, d=test_const.dispatch,
 	asd=cs.OrderedDict([('b', 1), ('a', 2)]) )
 data['query_dump_clone'] = data['query_dump']
 data['ids']['id в уникоде'] = [4, 5, 6]
 data['ids']['id2 в уникоде'] = data['ids']['id в уникоде']
 # data["'asd'\n!\0\1"] =cs.OrderedDict([('b', 1), ('a', 2)]) <-- fails in many ways
 
 data_str_multiline = dict(cert=(
@@ -298,22 +302,36 @@
 	def test_print_args(self):
 		buff = io.BytesIO()
 		args = 1, 2, 3
 		b = pyaml.dump(args, dst=bytes)
 		pyaml.print(*args, file=buff)
 		self.assertEqual(b, buff.getvalue())
 
-	def test_str_style_pick(self):
+	def test_str_styles(self):
 		a = pyaml.dump(data_str_multiline)
 		b = pyaml.dump(data_str_multiline, string_val_style='|')
 		self.assertEqual(a, b)
 		b = pyaml.dump(data_str_multiline, string_val_style='plain')
 		self.assertNotEqual(a, b)
+		c = pyaml.dump(data_str_multiline, string_val_style='literal')
+		self.assertNotEqual(c, a)
+		self.assertNotEqual(c, b)
 		self.assertTrue(pyaml.dump('waka waka', string_val_style='|').startswith('|-\n'))
-		self.assertEqual(pyaml.dump(dict(a=1), string_val_style='|'), 'a: 1\n')
+
+		a = pyaml.dump(data_int := dict(a=123))
+		self.assertEqual(a, 'a: 123\n')
+		self.assertEqual(pyaml.dump(data_int, string_val_style='|'), a)
+		self.assertEqual(pyaml.dump(data_int, string_val_style='literal'), a)
+
+		a = pyaml.dump(data_str := dict(a='123'))
+		b = pyaml.dump(data_str, string_val_style='|')
+		self.assertEqual(a, "a: '123'\n")
+		self.assertEqual(self.flatten(data_str), self.flatten(yaml.safe_load(a)))
+		self.assertNotEqual(a, b)
+		self.assertEqual(self.flatten(data_str), self.flatten(yaml.safe_load(b)))
 
 	def test_colons_in_strings(self):
 		val1 = {'foo': ['bar:', 'baz', 'bar:bazzo', 'a: b'], 'foo:': 'yak:'}
 		val1_str = pyaml.dump(val1)
 		val2 = yaml.safe_load(val1_str)
 		val2_str = pyaml.dump(val2)
 		val3 = yaml.safe_load(val2_str)
@@ -365,14 +383,25 @@
 		self.assertEqual(val_str, u'y: 1\nx: 2\nz: 3\n') # namedtuple order was preserved
 
 	def test_ordereddict(self):
 		d = cs.OrderedDict((i, '') for i in reversed(range(10)))
 		lines = pyaml.dump(d, sort_keys=False).splitlines()
 		self.assertEqual(lines, list(reversed(sorted(lines))))
 
+	def test_enum(self):
+		c = test_const.heartbeat
+		d1 = {'a': c, 'b': c.value, c: 'testx'}
+		self.assertEqual(d1['a'], d1['b'])
+		s = pyaml.dump(d1)
+		d2 = yaml.safe_load(s)
+		self.assertEqual(d1['a'], d2['a'])
+		self.assertEqual(d1['a'], c)
+		self.assertEqual(d1[c], 'testx')
+		self.assertIn('a: 123 # test_const.heartbeat', s)
+
 	def test_pyyaml_params(self):
 		d = {'foo': 'lorem ipsum ' * 30} # 300+ chars
 		for w in 40, 80, 200:
 			lines = pyaml.dump(d, width=w, indent=10).splitlines()
 			for n, line in enumerate(lines, 1):
 				self.assertLess(len(line), w*1.2)
 				if n != len(lines): self.assertGreater(len(line), w*0.8)
```

### Comparing `pyaml-23.5.6/pyaml.egg-info/PKG-INFO` & `pyaml-23.5.7/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-Metadata-Version: 2.1
-Name: pyaml
-Version: 23.5.6
-Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
-Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
-License: WTFPL
-Keywords: yaml,serialization,pretty-print,formatter,human,readability
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: Public Domain
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-Provides-Extra: anchors
-
 pretty-yaml (or pyaml)
 ======================
 
 PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+(side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there)
+
+It's a small module, and for projects that only need part of its functionality,
+I'd recommend copy-pasting that in, instead of adding janky dependency.
 
 .. _PyYAML: http://pyyaml.org/
 .. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
@@ -38,20 +23,16 @@
 - https://codeberg.org/mk-fg/pretty-yaml
 - https://fraggod.net/code/git/pretty-yaml
 
 
 Warning
 -------
 
-Prime goal of this module is to produce human-readable output that can be easily
-manipulated and re-used, but maybe with some occasional caveats.
-
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
-to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
-as an integer from that, but here it's a feature.
+Prime goal of this module is to produce human-readable output that can be
+easily diff'ed, manipulated and re-used, but maybe with occasional issues.
 
 So please do not rely on the thing to produce output that can always be
 deserialized exactly to what was exported, at least - use PyYAML directly
 for that (but maybe with options from the next section).
 
 
 What this module does and why
@@ -83,18 +64,19 @@
 
 * Most human-friendly representation options in PyYAML (that I know of)
   are used as defaults.
 
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
-* Use shorter and simplier yes/no for booleans.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
+  are represented as their safe YAML-compatible base (like int, list or mapping),
+  with mappings key-sorted by default for more diff-friendly output.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and key-sorted by default, for more diff-friendly output.
+* Use shorter and simplier yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -125,14 +107,16 @@
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
 * Add vertical spacing (empty lines) between keys on different depths,
   to separate long YAML sections in the output visually, make it more seekable.
 
+* Discard end-of-document "..." indicators for simple values.
+
 Result for the (rather meaningless) example above::
 
   >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
   a: |
     asldnsa
     asldpáknsa
@@ -212,18 +196,18 @@
         level: 0
 
     root:
       handlers:
         - console
       level: custom
 
-Note that unless there are many moderately wide and deep trees of data, which
-are expected to be read and edited by people, it might be preferrable to
-directly use PyYAML regardless, as it won't introduce another (rather pointless
-in that case) dependency and a point of failure.
+Note that unless there are many moderately wide and deep trees of data,
+which are expected to be read and edited by people, it might be preferrable
+to directly use PyYAML regardless, as it won't introduce another
+(rather pointless in that case) dependency and a point of failure.
 
 
 Some Tricks
 -----------
 
 * Pretty-print any yaml or json (yaml subset) file from the shell::
```

### Comparing `pyaml-23.5.6/pyproject.toml` & `pyaml-23.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pyaml"
-version = "23.05.06"
+version = "23.05.07"
 
 description = "PyYAML-based module to produce a bit more pretty and readable YAML-serialized data"
 authors = [{name="Mike Kazantsev", email="mk.fraggod@gmail.com"}]
 license = {text="WTFPL"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
```

