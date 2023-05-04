# Comparing `tmp/datafiles-2.1b4.tar.gz` & `tmp/datafiles-2.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafiles-2.1b4.tar", max compression
+gzip compressed data, was "datafiles-2.1b5.tar", max compression
```

## Comparing `datafiles-2.1b4.tar` & `datafiles-2.1b5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1088 2020-10-23 18:26:12.919187 datafiles-2.1b4/LICENSE.md
--rw-r--r--   0        0        0     3587 2022-08-20 19:54:08.509269 datafiles-2.1b4/README.md
--rw-r--r--   0        0        0      230 2022-03-07 22:22:01.280577 datafiles-2.1b4/datafiles/__init__.py
--rw-r--r--   0        0        0      929 2021-05-22 20:25:09.696998 datafiles-2.1b4/datafiles/config.py
--rw-r--r--   0        0        0     6817 2022-12-22 17:25:22.931529 datafiles-2.1b4/datafiles/converters/__init__.py
--rw-r--r--   0        0        0     1605 2022-03-07 22:22:01.282152 datafiles-2.1b4/datafiles/converters/_bases.py
--rw-r--r--   0        0        0     1369 2022-03-07 22:22:01.282572 datafiles-2.1b4/datafiles/converters/builtins.py
--rw-r--r--   0        0        0     7651 2022-07-28 22:23:18.880690 datafiles-2.1b4/datafiles/converters/containers.py
--rw-r--r--   0        0        0      605 2022-03-07 22:22:01.283437 datafiles-2.1b4/datafiles/converters/enumerations.py
--rw-r--r--   0        0        0     1038 2022-03-07 22:22:01.284256 datafiles-2.1b4/datafiles/converters/extensions.py
--rw-r--r--   0        0        0     1481 2023-02-11 22:50:48.180296 datafiles-2.1b4/datafiles/decorators.py
--rw-r--r--   0        0        0     3643 2022-03-07 22:22:01.285760 datafiles-2.1b4/datafiles/formats.py
--rw-r--r--   0        0        0     4688 2022-06-30 21:39:29.057831 datafiles-2.1b4/datafiles/hooks.py
--rw-r--r--   0        0        0     6011 2023-02-11 22:50:48.180679 datafiles-2.1b4/datafiles/manager.py
--rw-r--r--   0        0        0    10496 2023-02-11 22:50:48.182618 datafiles-2.1b4/datafiles/mapper.py
--rw-r--r--   0        0        0     2381 2023-02-11 22:50:48.184347 datafiles-2.1b4/datafiles/model.py
--rw-r--r--   0        0        0     1206 2022-12-22 17:25:22.933989 datafiles-2.1b4/datafiles/plugins.py
--rw-r--r--   0        0        0      133 2021-06-01 21:23:07.659224 datafiles-2.1b4/datafiles/settings.py
--rw-r--r--   0        0        0      362 2022-07-28 22:23:18.881053 datafiles-2.1b4/datafiles/tests/__init__.py
--rw-r--r--   0        0        0    16339 2022-08-20 19:54:08.510731 datafiles-2.1b4/datafiles/tests/test_converters.py
--rw-r--r--   0        0        0      923 2020-10-23 18:26:12.922512 datafiles-2.1b4/datafiles/tests/test_decorators.py
--rw-r--r--   0        0        0     1789 2022-03-07 22:22:01.290202 datafiles-2.1b4/datafiles/tests/test_formats.py
--rw-r--r--   0        0        0     2006 2022-03-07 22:22:01.290605 datafiles-2.1b4/datafiles/tests/test_generics.py
--rw-r--r--   0        0        0     1585 2022-03-07 22:22:01.291486 datafiles-2.1b4/datafiles/tests/test_hooks.py
--rw-r--r--   0        0        0     5555 2023-02-11 22:50:48.185274 datafiles-2.1b4/datafiles/tests/test_manager.py
--rw-r--r--   0        0        0     3849 2022-04-10 21:45:32.239091 datafiles-2.1b4/datafiles/tests/test_mapper.py
--rw-r--r--   0        0        0      609 2023-02-11 22:50:48.185663 datafiles-2.1b4/datafiles/tests/test_model.py
--rw-r--r--   0        0        0     2790 2022-03-07 22:22:01.293345 datafiles-2.1b4/datafiles/tests/test_utils.py
--rw-r--r--   0        0        0      743 2022-06-30 21:39:29.058486 datafiles-2.1b4/datafiles/types.py
--rw-r--r--   0        0        0     4242 2022-03-07 22:22:01.294612 datafiles-2.1b4/datafiles/utils.py
--rw-r--r--   0        0        0     2093 2023-02-11 22:51:02.959785 datafiles-2.1b4/pyproject.toml
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 datafiles-2.1b4/setup.py
--rw-r--r--   0        0        0     5193 1970-01-01 00:00:00.000000 datafiles-2.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-06-09 21:33:24.000000 datafiles-2.1b5/LICENSE.md
+-rw-r--r--   0        0        0     3587 2022-08-20 17:08:29.834288 datafiles-2.1b5/README.md
+-rw-r--r--   0        0        0      230 2022-03-05 04:25:20.295998 datafiles-2.1b5/datafiles/__init__.py
+-rw-r--r--   0        0        0      929 2022-10-11 11:26:59.042300 datafiles-2.1b5/datafiles/config.py
+-rw-r--r--   0        0        0     6817 2022-11-23 17:08:26.552083 datafiles-2.1b5/datafiles/converters/__init__.py
+-rw-r--r--   0        0        0     1605 2022-02-02 22:35:04.726189 datafiles-2.1b5/datafiles/converters/_bases.py
+-rw-r--r--   0        0        0     1369 2022-02-02 22:35:04.726539 datafiles-2.1b5/datafiles/converters/builtins.py
+-rw-r--r--   0        0        0     7651 2022-07-29 16:35:41.392675 datafiles-2.1b5/datafiles/converters/containers.py
+-rw-r--r--   0        0        0      605 2022-02-02 22:35:04.727351 datafiles-2.1b5/datafiles/converters/enumerations.py
+-rw-r--r--   0        0        0     1038 2022-02-02 22:35:04.727646 datafiles-2.1b5/datafiles/converters/extensions.py
+-rw-r--r--   0        0        0     1481 2023-03-26 19:07:40.583195 datafiles-2.1b5/datafiles/decorators.py
+-rw-r--r--   0        0        0     3643 2022-11-09 21:15:25.993928 datafiles-2.1b5/datafiles/formats.py
+-rw-r--r--   0        0        0     4688 2022-04-22 23:18:12.443625 datafiles-2.1b5/datafiles/hooks.py
+-rw-r--r--   0        0        0     6011 2023-02-13 17:48:23.609765 datafiles-2.1b5/datafiles/manager.py
+-rw-r--r--   0        0        0    10496 2023-02-13 17:48:23.611367 datafiles-2.1b5/datafiles/mapper.py
+-rw-r--r--   0        0        0     2381 2023-02-13 17:48:23.612399 datafiles-2.1b5/datafiles/model.py
+-rw-r--r--   0        0        0     1206 2022-11-23 17:06:22.694080 datafiles-2.1b5/datafiles/plugins.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:40:43.756929 datafiles-2.1b5/datafiles/py.typed
+-rw-r--r--   0        0        0      133 2021-05-26 11:50:47.865164 datafiles-2.1b5/datafiles/settings.py
+-rw-r--r--   0        0        0      362 2022-07-29 16:35:41.394659 datafiles-2.1b5/datafiles/tests/__init__.py
+-rw-r--r--   0        0        0    16339 2022-08-20 17:08:29.835977 datafiles-2.1b5/datafiles/tests/test_converters.py
+-rw-r--r--   0        0        0      923 2020-05-02 16:10:37.000000 datafiles-2.1b5/datafiles/tests/test_decorators.py
+-rw-r--r--   0        0        0     1789 2022-02-02 22:35:04.730640 datafiles-2.1b5/datafiles/tests/test_formats.py
+-rw-r--r--   0        0        0     2006 2022-02-02 22:35:04.730913 datafiles-2.1b5/datafiles/tests/test_generics.py
+-rw-r--r--   0        0        0     1585 2022-04-22 23:06:52.609396 datafiles-2.1b5/datafiles/tests/test_hooks.py
+-rw-r--r--   0        0        0     5555 2023-02-11 00:35:02.076274 datafiles-2.1b5/datafiles/tests/test_manager.py
+-rw-r--r--   0        0        0     3849 2022-10-11 11:26:59.046450 datafiles-2.1b5/datafiles/tests/test_mapper.py
+-rw-r--r--   0        0        0      609 2023-02-13 17:48:23.612872 datafiles-2.1b5/datafiles/tests/test_model.py
+-rw-r--r--   0        0        0     2790 2022-03-07 14:07:43.245444 datafiles-2.1b5/datafiles/tests/test_utils.py
+-rw-r--r--   0        0        0      743 2022-04-16 23:56:46.724770 datafiles-2.1b5/datafiles/types.py
+-rw-r--r--   0        0        0     4242 2022-04-16 23:57:40.170785 datafiles-2.1b5/datafiles/utils.py
+-rw-r--r--   0        0        0     2015 2023-03-26 19:40:43.757150 datafiles-2.1b5/pyproject.toml
+-rw-r--r--   0        0        0     5193 1970-01-01 00:00:00.000000 datafiles-2.1b5/PKG-INFO
```

### Comparing `datafiles-2.1b4/LICENSE.md` & `datafiles-2.1b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/README.md` & `datafiles-2.1b5/README.md`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/config.py` & `datafiles-2.1b5/datafiles/config.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/__init__.py` & `datafiles-2.1b5/datafiles/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/_bases.py` & `datafiles-2.1b5/datafiles/converters/_bases.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/builtins.py` & `datafiles-2.1b5/datafiles/converters/builtins.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/containers.py` & `datafiles-2.1b5/datafiles/converters/containers.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/enumerations.py` & `datafiles-2.1b5/datafiles/converters/enumerations.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/converters/extensions.py` & `datafiles-2.1b5/datafiles/converters/extensions.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/decorators.py` & `datafiles-2.1b5/datafiles/decorators.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/formats.py` & `datafiles-2.1b5/datafiles/formats.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/hooks.py` & `datafiles-2.1b5/datafiles/hooks.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/manager.py` & `datafiles-2.1b5/datafiles/manager.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/mapper.py` & `datafiles-2.1b5/datafiles/mapper.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/model.py` & `datafiles-2.1b5/datafiles/model.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/plugins.py` & `datafiles-2.1b5/datafiles/plugins.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_converters.py` & `datafiles-2.1b5/datafiles/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_decorators.py` & `datafiles-2.1b5/datafiles/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_formats.py` & `datafiles-2.1b5/datafiles/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_generics.py` & `datafiles-2.1b5/datafiles/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_hooks.py` & `datafiles-2.1b5/datafiles/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_manager.py` & `datafiles-2.1b5/datafiles/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_mapper.py` & `datafiles-2.1b5/datafiles/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_model.py` & `datafiles-2.1b5/datafiles/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/tests/test_utils.py` & `datafiles-2.1b5/datafiles/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/types.py` & `datafiles-2.1b5/datafiles/types.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/datafiles/utils.py` & `datafiles-2.1b5/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.1b4/pyproject.toml` & `datafiles-2.1b5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "datafiles"
-version = "2.1b4"
+version = "2.1b5"
 description = "File-based ORM for dataclasses."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -77,18 +77,16 @@
 pytest-cov = "^2.8.1"
 pytest-profiling = "*"
 
 # Coverage
 coveragespace = "^6.0"
 
 # Documentation
-mkdocs = "^1.3"
+mkdocs = "^1.4"
 pygments = "^2.10"
-jinja2 = "~3.0.3" # fix for 'mkdocs' incompatiblity
-importlib-metadata = "<5"
 
 # Notebooks
 idna = "^3.3" # papermill dependency
 ipython = "^8.10"
 jupyter = { version = "^1.0", markers = "sys_platform != 'win32'" }
 nbstripout ="~0.4"
 papermill = "^2.3"
```

### Comparing `datafiles-2.1b4/setup.py` & `datafiles-2.1b5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,157 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: datafiles
+Version: 2.1b5
+Summary: File-based ORM for dataclasses.
+Home-page: https://pypi.org/project/datafiles
+License: MIT
+Keywords: dataclasses,serialization,type-annotations,object-relational mapping,YAML,JSON,TOML
+Author: Jace Browning
+Author-email: jacebrowning@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: cached_property (>=1.5,<2.0)
+Requires-Dist: classproperties (>=0.2,<0.3)
+Requires-Dist: minilog (>=2.1,<3.0)
+Requires-Dist: parse (>=1.12,<2.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
+Project-URL: Documentation, https://datafiles.readthedocs.io
+Project-URL: Repository, https://github.com/jacebrowning/datafiles
+Description-Content-Type: text/markdown
+
+# Datafiles: A file-based ORM for Python dataclasses
+
+Datafiles is a bidirectional serialization library for Python [dataclasses](https://docs.python.org/3/library/dataclasses.html) to synchronize objects to the filesystem using type annotations. It supports a variety of file formats with round-trip preservation of formatting and comments, where possible. Object changes are automatically saved to disk and only include the minimum data needed to restore each object.
+
+[![Travis CI](https://img.shields.io/travis/com/jacebrowning/datafiles/main.svg?label=unix)](https://travis-ci.com/jacebrowning/datafiles)
+[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)
+[![Coveralls](https://img.shields.io/coveralls/jacebrowning/datafiles.svg)](https://coveralls.io/r/jacebrowning/datafiles)
+[![PyPI License](https://img.shields.io/pypi/l/datafiles.svg)](https://pypi.org/project/datafiles)
+[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg)](https://pypi.org/project/datafiles)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/datafiles.svg?color=orange)](https://pypistats.org/packages/datafiles)
+[![Gitter](https://img.shields.io/gitter/room/jacebrowning/datafiles?color=D0164E)](https://gitter.im/jacebrowning/datafiles)
+
+Some common use cases include:
+
+- Coercing user-editable files into the proper Python types
+- Storing program configuration and data in version control
+- Loading data fixtures for demonstration or testing purposes
+- Synchronizing application state using file sharing services
+- Prototyping data models agnostic of persistence backends
+
+Watch [my lightning talk](https://www.youtube.com/watch?v=moYkuNrmc1I&feature=youtu.be&t=1225) for a demo of this in action!
+
+## Overview
+
+Take an existing dataclass such as [this example](https://docs.python.org/3/library/dataclasses.html#module-dataclasses) from the documentation:
+
+```python
+from dataclasses import dataclass
+
+@dataclass
+class InventoryItem:
+    """Class for keeping track of an item in inventory."""
+
+    name: str
+    unit_price: float
+    quantity_on_hand: int = 0
+
+    def total_cost(self) -> float:
+        return self.unit_price * self.quantity_on_hand
+```
+
+and decorate it with a directory pattern to synchronize instances:
+
+```python
+from datafiles import datafile
+
+@datafile("inventory/items/{self.name}.yml")
+class InventoryItem:
+    ...
+```
+
+Then, work with instances of the class as normal:
+
+```python
+>>> item = InventoryItem("widget", 3)
+```
+
+```yaml
+# inventory/items/widget.yml
+
+unit_price: 3.0
+```
+
+Changes to the object are automatically saved to the filesystem:
+
+```python
+>>> item.quantity_on_hand += 100
+```
+
+```yaml
+# inventory/items/widget.yml
+
+unit_price: 3.0
+quantity_on_hand: 100
+```
+
+Changes to the filesystem are automatically reflected in the object:
+
+```yaml
+# inventory/items/widget.yml
+
+unit_price: 2.5 # <= manually changed from "3.0"
+quantity_on_hand: 100
+```
+
+```python
+>>> item.unit_price
+2.5
+```
+
+Objects can also be restored from the filesystem:
+
+```python
+>>> from datafiles import Missing
+>>> item = InventoryItem("widget", Missing)
+>>> item.unit_price
+2.5
+>>> item.quantity_on_hand
+100
+```
+
+## Installation
+
+Install this library directly into an activated virtual environment:
+
+```
+$ pip install datafiles
+```
+
+or add it to your [Poetry](https://poetry.eustace.io/) project:
+
+```
+$ poetry add datafiles
+```
 
-packages = \
-['datafiles', 'datafiles.converters', 'datafiles.tests']
+## Documentation
 
-package_data = \
-{'': ['*']}
+To see additional synchronization and formatting options, please consult the [full documentation](https://datafiles.readthedocs.io).
 
-install_requires = \
-['cached_property>=1.5,<2.0',
- 'classproperties>=0.2,<0.3',
- 'minilog>=2.1,<3.0',
- 'parse>=1.12,<2.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'tomlkit>=0.10.1,<0.11.0']
-
-setup_kwargs = {
-    'name': 'datafiles',
-    'version': '2.1b4',
-    'description': 'File-based ORM for dataclasses.',
-    'long_description': '# Datafiles: A file-based ORM for Python dataclasses\n\nDatafiles is a bidirectional serialization library for Python [dataclasses](https://docs.python.org/3/library/dataclasses.html) to synchronize objects to the filesystem using type annotations. It supports a variety of file formats with round-trip preservation of formatting and comments, where possible. Object changes are automatically saved to disk and only include the minimum data needed to restore each object.\n\n[![Travis CI](https://img.shields.io/travis/com/jacebrowning/datafiles/main.svg?label=unix)](https://travis-ci.com/jacebrowning/datafiles)\n[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)\n[![Coveralls](https://img.shields.io/coveralls/jacebrowning/datafiles.svg)](https://coveralls.io/r/jacebrowning/datafiles)\n[![PyPI License](https://img.shields.io/pypi/l/datafiles.svg)](https://pypi.org/project/datafiles)\n[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg)](https://pypi.org/project/datafiles)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/datafiles.svg?color=orange)](https://pypistats.org/packages/datafiles)\n[![Gitter](https://img.shields.io/gitter/room/jacebrowning/datafiles?color=D0164E)](https://gitter.im/jacebrowning/datafiles)\n\nSome common use cases include:\n\n- Coercing user-editable files into the proper Python types\n- Storing program configuration and data in version control\n- Loading data fixtures for demonstration or testing purposes\n- Synchronizing application state using file sharing services\n- Prototyping data models agnostic of persistence backends\n\nWatch [my lightning talk](https://www.youtube.com/watch?v=moYkuNrmc1I&feature=youtu.be&t=1225) for a demo of this in action!\n\n## Overview\n\nTake an existing dataclass such as [this example](https://docs.python.org/3/library/dataclasses.html#module-dataclasses) from the documentation:\n\n```python\nfrom dataclasses import dataclass\n\n@dataclass\nclass InventoryItem:\n    """Class for keeping track of an item in inventory."""\n\n    name: str\n    unit_price: float\n    quantity_on_hand: int = 0\n\n    def total_cost(self) -> float:\n        return self.unit_price * self.quantity_on_hand\n```\n\nand decorate it with a directory pattern to synchronize instances:\n\n```python\nfrom datafiles import datafile\n\n@datafile("inventory/items/{self.name}.yml")\nclass InventoryItem:\n    ...\n```\n\nThen, work with instances of the class as normal:\n\n```python\n>>> item = InventoryItem("widget", 3)\n```\n\n```yaml\n# inventory/items/widget.yml\n\nunit_price: 3.0\n```\n\nChanges to the object are automatically saved to the filesystem:\n\n```python\n>>> item.quantity_on_hand += 100\n```\n\n```yaml\n# inventory/items/widget.yml\n\nunit_price: 3.0\nquantity_on_hand: 100\n```\n\nChanges to the filesystem are automatically reflected in the object:\n\n```yaml\n# inventory/items/widget.yml\n\nunit_price: 2.5 # <= manually changed from "3.0"\nquantity_on_hand: 100\n```\n\n```python\n>>> item.unit_price\n2.5\n```\n\nObjects can also be restored from the filesystem:\n\n```python\n>>> from datafiles import Missing\n>>> item = InventoryItem("widget", Missing)\n>>> item.unit_price\n2.5\n>>> item.quantity_on_hand\n100\n```\n\n## Installation\n\nInstall this library directly into an activated virtual environment:\n\n```\n$ pip install datafiles\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```\n$ poetry add datafiles\n```\n\n## Documentation\n\nTo see additional synchronization and formatting options, please consult the [full documentation](https://datafiles.readthedocs.io).\n',
-    'author': 'Jace Browning',
-    'author_email': 'jacebrowning@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/datafiles',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

