# Comparing `tmp/pyqtschema-0.1.9.tar.gz` & `tmp/pyqtschema-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtschema-0.1.9.tar", last modified: Tue Jul 12 20:21:04 2022, max compression
+gzip compressed data, was "pyqtschema-0.2.0.tar", last modified: Fri May  5 21:16:50 2023, max compression
```

## Comparing `pyqtschema-0.1.9.tar` & `pyqtschema-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/
--rw-rw-r--   0 dd        (1000) dd        (1000)     1063 2022-01-28 22:18:31.000000 pyqtschema-0.1.9/LICENSE
--rw-rw-r--   0 dd        (1000) dd        (1000)     3063 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)     1108 2022-02-10 23:35:27.000000 pyqtschema-0.1.9/README.md
--rw-rw-r--   0 dd        (1000) dd        (1000)      134 2022-02-01 23:35:24.000000 pyqtschema-0.1.9/pyproject.toml
--rw-rw-r--   0 dd        (1000) dd        (1000)      689 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/setup.cfg
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2022-07-12 20:21:04.748971 pyqtschema-0.1.9/src/
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/src/pyqtschema/
--rw-rw-r--   0 dd        (1000) dd        (1000)      187 2022-02-01 23:53:00.000000 pyqtschema-0.1.9/src/pyqtschema/__init__.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     4007 2022-02-10 23:35:27.000000 pyqtschema-0.1.9/src/pyqtschema/__main__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)       23 2022-07-12 20:20:05.000000 pyqtschema-0.1.9/src/pyqtschema/__version__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     5103 2022-02-10 23:35:27.000000 pyqtschema-0.1.9/src/pyqtschema/builder.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     2745 2022-07-12 20:20:05.000000 pyqtschema-0.1.9/src/pyqtschema/schema.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     1351 2022-07-12 20:20:05.000000 pyqtschema-0.1.9/src/pyqtschema/utils.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/src/pyqtschema/widgets/
--rwxrwxr-x   0 dd        (1000) dd        (1000)      521 2022-02-09 22:17:21.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     5313 2022-07-04 21:13:16.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/any_of.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     6493 2022-02-07 22:00:54.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/array.py
--rwxrwxr--   0 dd        (1000) dd        (1000)     1912 2022-01-28 23:06:03.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/base.py
--rwxrwxr--   0 dd        (1000) dd        (1000)      443 2022-01-28 23:15:34.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/boolean.py
--rwxrwxr--   0 dd        (1000) dd        (1000)     1738 2022-01-28 23:15:34.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/color.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)      922 2022-07-04 21:13:16.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/enu.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     2954 2022-02-07 22:00:54.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/groups.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     2802 2022-07-12 20:20:05.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/numeric.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     1240 2022-02-09 22:17:21.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/paths.py
--rwxrwxr-x   0 dd        (1000) dd        (1000)     1334 2022-02-07 22:00:54.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/root.py
--rwxrwxr--   0 dd        (1000) dd        (1000)      565 2022-01-28 21:57:57.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/signal.py
--rwxrwxr--   0 dd        (1000) dd        (1000)      966 2022-01-28 23:47:47.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/text.py
--rwxrwxr--   0 dd        (1000) dd        (1000)      406 2022-01-28 21:57:57.000000 pyqtschema-0.1.9/src/pyqtschema/widgets/utils.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2022-07-12 20:21:04.752971 pyqtschema-0.1.9/src/pyqtschema.egg-info/
--rw-rw-r--   0 dd        (1000) dd        (1000)     3063 2022-07-12 20:21:04.000000 pyqtschema-0.1.9/src/pyqtschema.egg-info/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)      843 2022-07-12 20:21:04.000000 pyqtschema-0.1.9/src/pyqtschema.egg-info/SOURCES.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)        1 2022-07-12 20:21:04.000000 pyqtschema-0.1.9/src/pyqtschema.egg-info/dependency_links.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       17 2022-07-12 20:21:04.000000 pyqtschema-0.1.9/src/pyqtschema.egg-info/requires.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       11 2022-07-12 20:21:04.000000 pyqtschema-0.1.9/src/pyqtschema.egg-info/top_level.txt
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.525538 pyqtschema-0.2.0/
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1063 2022-01-28 22:18:31.000000 pyqtschema-0.2.0/LICENSE
+-rw-rw-r--   0 dd        (1000) dd        (1000)     3160 2023-05-05 21:16:50.525538 pyqtschema-0.2.0/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1108 2022-02-10 23:35:27.000000 pyqtschema-0.2.0/README.md
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1559 2023-05-05 21:10:13.000000 pyqtschema-0.2.0/changelog.md
+-rw-rw-r--   0 dd        (1000) dd        (1000)      147 2023-05-05 21:14:58.000000 pyqtschema-0.2.0/pyproject.toml
+-rw-rw-r--   0 dd        (1000) dd        (1000)      695 2023-05-05 21:16:50.525538 pyqtschema-0.2.0/setup.cfg
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.521538 pyqtschema-0.2.0/src/
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.521538 pyqtschema-0.2.0/src/pyqtschema/
+-rw-rw-r--   0 dd        (1000) dd        (1000)      187 2022-02-01 23:53:00.000000 pyqtschema-0.2.0/src/pyqtschema/__init__.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     4005 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/__main__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)       23 2023-05-05 21:08:51.000000 pyqtschema-0.2.0/src/pyqtschema/__version__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     5103 2022-02-10 23:35:27.000000 pyqtschema-0.2.0/src/pyqtschema/builder.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     2745 2022-07-12 20:20:05.000000 pyqtschema-0.2.0/src/pyqtschema/schema.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1410 2023-05-05 20:59:34.000000 pyqtschema-0.2.0/src/pyqtschema/utils.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.521538 pyqtschema-0.2.0/src/pyqtschema/widgets/
+-rwxrwxr-x   0 dd        (1000) dd        (1000)      521 2022-02-09 22:17:21.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     5425 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/any_of.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     6475 2023-05-05 21:01:56.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/array.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     1920 2023-05-05 21:01:43.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/base.py
+-rwxrwxr--   0 dd        (1000) dd        (1000)      442 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/boolean.py
+-rwxrwxr--   0 dd        (1000) dd        (1000)     1727 2023-05-05 21:02:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/color.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)      921 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/enu.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     2952 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/groups.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     2800 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/numeric.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     1239 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/paths.py
+-rwxrwxr-x   0 dd        (1000) dd        (1000)     1333 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/root.py
+-rwxrwxr--   0 dd        (1000) dd        (1000)      965 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/text.py
+-rwxrwxr--   0 dd        (1000) dd        (1000)      405 2023-05-05 21:00:09.000000 pyqtschema-0.2.0/src/pyqtschema/widgets/utils.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.521538 pyqtschema-0.2.0/src/pyqtschema.egg-info/
+-rw-rw-r--   0 dd        (1000) dd        (1000)     3160 2023-05-05 21:16:50.000000 pyqtschema-0.2.0/src/pyqtschema.egg-info/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)      844 2023-05-05 21:16:50.000000 pyqtschema-0.2.0/src/pyqtschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)        1 2023-05-05 21:16:50.000000 pyqtschema-0.2.0/src/pyqtschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       22 2023-05-05 21:16:50.000000 pyqtschema-0.2.0/src/pyqtschema.egg-info/requires.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       11 2023-05-05 21:16:50.000000 pyqtschema-0.2.0/src/pyqtschema.egg-info/top_level.txt
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-05-05 21:16:50.521538 pyqtschema-0.2.0/tests/
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1093 2022-07-04 20:39:46.000000 pyqtschema-0.2.0/tests/test_schema.py
```

### Comparing `pyqtschema-0.1.9/LICENSE` & `pyqtschema-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtschema-0.1.9/PKG-INFO` & `pyqtschema-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtschema
-Version: 0.1.9
+Version: 0.2.0
 Summary: Convert json-schema to QWidgets
 Home-page: https://github.com/amsico/pyqtschema
 Author: Amsico
 Author-email: amsico@eclipso.eu
 Project-URL: Bug Tracker, https://github.com/amsico/pyqtschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,18 @@
 `pyqtschema` is inspired by [qt-jsonschema-form](https://github.com/agoose77/qt-jsonschema-form). Due to the author's
 lack of [time](https://github.com/agoose77/qt-jsonschema-form/pull/1#issuecomment-595491242) and the missing
 [anyOf-support](https://github.com/agoose77/qt-jsonschema-form/blob/ca71ddbf10c2b309c3eb9c4fda6b054a0cb573dd/README.md?plain=1#L10)
 , this project was started.
 
 # Changelog
 
+### Version 0.2.0 (2023-05-05)
+
+* use [QtPy](https://pypi.org/project/QtPy/) instead of `PyQt5`
+
 ### Version 0.1.9 (2022-07-12)
 
 * FIX: default calculation for simple AllOf-cases
 * New example for ui_schema usage
 * New example for simple AllOf case
 
 ### Version 0.1.8 (2022-07-04)
```

### Comparing `pyqtschema-0.1.9/README.md` & `pyqtschema-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqtschema-0.1.9/src/pyqtschema/__main__.py` & `pyqtschema-0.2.0/src/pyqtschema/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from json import load
 from pathlib import Path
 from typing import Dict, Callable, Optional
 
-from PyQt5.QtGui import QIcon
-from PyQt5.QtWidgets import QApplication, QMainWindow, QMenu, QAction, QScrollArea, QStyle, QMessageBox, QFileDialog
+from qtpy.QtGui import QIcon
+from qtpy.QtWidgets import QApplication, QMainWindow, QMenu, QAction, QScrollArea, QStyle, QMessageBox, QFileDialog
 
 from .__version__ import version
 from .builder import WidgetBuilder
 from .schema import schema_from_json
 from .utils import json_dump
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/builder.py` & `pyqtschema-0.2.0/src/pyqtschema/builder.py`

 * *Files identical despite different names*

### Comparing `pyqtschema-0.1.9/src/pyqtschema/schema.py` & `pyqtschema-0.2.0/src/pyqtschema/schema.py`

 * *Files identical despite different names*

### Comparing `pyqtschema-0.1.9/src/pyqtschema/utils.py` & `pyqtschema-0.2.0/src/pyqtschema/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from enum import Enum
 from json import JSONEncoder, dump
 from typing import Dict, Any
 
-from PyQt5.QtWidgets import QApplication, QScrollArea, QWidget
+from qtpy.QtWidgets import QApplication, QScrollArea, QWidget
 
 from pyqtschema.builder import WidgetBuilder
 
 
 def build_example_widget(schema: Dict, ui_schema=None) -> QWidget:
     builder = WidgetBuilder(schema)
     form = builder.create_form(ui_schema=ui_schema)
@@ -18,14 +18,16 @@
     app = QApplication(sys.argv)
     widget = form = build_example_widget(schema, ui_schema=ui_schema)
     if scrollbar:
         widget = QScrollArea()
         widget.setWidget(form)
         widget.setWidgetResizable(True)
 
+    form.widget.on_changed.connect(lambda xxx: print(xxx))
+
     widget.show()
     app.exec_()
 
 
 class Encoder(JSONEncoder):
     def default(self, o: Any) -> Any:
         if isinstance(o, Enum):
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/__init__.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/any_of.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/any_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 from functools import partial
 from typing import Dict, List
 
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QComboBox, QGroupBox
+from qtpy.QtWidgets import QWidget, QVBoxLayout, QComboBox, QGroupBox
 
 from ..schema import Schema
 from .base import state_property, SchemaWidgetMixin
 from .utils import iter_layout_widgets
 
 CHECKER_KEY = 'checker'
 
@@ -109,14 +109,16 @@
     @state.setter
     def state(self, state: dict):
         # assumption:
         #   state is dict => set the state to the current selection
         #   state is a list => set state to all widgets
         # Background:
         #   the function may be called after initializing the form including all defaults for any possible item
+        # Problem:
+        #   TODO: E.g. AnyOf may provide a Sting-object and a List-of-sting objects. Assuming
         _widgets = self.widgets
         if isinstance(state, (list, tuple)):
             for idx, _dat in enumerate(state):
                 if idx >= len(_widgets):
                     break
                 _widgets[idx].state = _dat
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/array.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from functools import partial
 from typing import List, Tuple, Optional
 
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QPushButton, QStyle, QGroupBox
+from qtpy.QtCore import Signal
+from qtpy.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QPushButton, QStyle, QGroupBox
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 from pyqtschema.widgets.utils import iter_layout_widgets, is_concrete_schema
 
 
 class ArrayControlsWidget(QWidget):
-    on_delete = pyqtSignal()
-    on_move_up = pyqtSignal()
-    on_move_down = pyqtSignal()
+    on_delete = Signal()
+    on_move_up = Signal()
+    on_move_down = Signal()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         style = self.style()
 
         self.up_button = QPushButton()
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/base.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import wraps
 from typing import Tuple
 
-from PyQt5.QtGui import QColor
-
-from .signal import Signal
+from qtpy.QtCore import Signal
+from qtpy.QtGui import QColor
 
 
 class StateProperty(property):
 
     def setter(self, fset):
         @wraps(fset)
         def _setter(*args):
@@ -18,15 +17,15 @@
         return super().setter(_setter)
 
 
 state_property = StateProperty
 
 
 class SchemaWidgetMixin:
-    on_changed = Signal()
+    on_changed = Signal(object)
 
     VALID_COLOUR = '#ffffff'
     INVALID_COLOUR = '#f6989d'
 
     def __init__(self, schema: dict, ui_schema: dict, widget_builder: 'IBuilder', **kwargs):
         super().__init__(**kwargs)
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/color.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/color.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from PyQt5.QtCore import pyqtSignal, Qt
-from PyQt5.QtGui import QColor
-from PyQt5.QtWidgets import QPushButton, QColorDialog
+from qtpy.QtCore import Signal, Qt
+from qtpy.QtGui import QColor
+from qtpy.QtWidgets import QPushButton, QColorDialog
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 
 
 class QColorButton(QPushButton):
     """Color picker widget QPushButton subclass.
 
     Implementation derived from https://martinfitzpatrick.name/article/qcolorbutton-a-color-selector-tool-for-pyqt/
     """
 
-    colorChanged = pyqtSignal()
+    colorChanged = Signal()
 
     def __init__(self, *args, **kwargs):
         super(QColorButton, self).__init__(*args, **kwargs)
 
         self._color = None
         self.pressed.connect(self.onColorPicker)
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/enu.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/enu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 
-from PyQt5.QtWidgets import QComboBox
+from qtpy.QtWidgets import QComboBox
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 
 
 class EnumSchemaWidget(SchemaWidgetMixin, QComboBox):
 
     @state_property
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/groups.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict
 from functools import partial
 from typing import Tuple, Dict
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QGroupBox, QWidget, QGridLayout, QLabel, QVBoxLayout, QComboBox, QHBoxLayout, QSizePolicy
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QGroupBox, QWidget, QGridLayout, QLabel, QVBoxLayout, QComboBox, QHBoxLayout, QSizePolicy
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 from pyqtschema.widgets.utils import iter_layout_widgets
 
 
 class ObjectSchemaWidget(SchemaWidgetMixin, QGroupBox):
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/numeric.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/numeric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QDoubleSpinBox, QSpinBox, QSlider
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QDoubleSpinBox, QSpinBox, QSlider
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 
 
 def range_from_schema(schema: dict):
     # https://json-schema.org/understanding-json-schema/reference/numeric.html#range
     # there should be an exclusive-minimum OR a minimum
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/paths.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QFileDialog, QHBoxLayout, QLineEdit, QPushButton, QWidget
+from qtpy.QtWidgets import QFileDialog, QHBoxLayout, QLineEdit, QPushButton, QWidget
 
 from pyqtschema.widgets.base import SchemaWidgetMixin, state_property
 
 
 class FilepathSchemaWidget(SchemaWidgetMixin, QWidget):
 
     def __init__(self, schema: dict, ui_schema: dict, widget_builder: 'WidgetBuilder', **kwargs):
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/root.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/root.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QGroupBox, QLabel
+from qtpy.QtWidgets import QWidget, QVBoxLayout, QGroupBox, QLabel
 
 from pyqtschema.widgets.base import SchemaWidgetMixin
 
 
 class FormWidget(QWidget):
 
     def __init__(self, widget: SchemaWidgetMixin, *args, **kwargs):
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema/widgets/text.py` & `pyqtschema-0.2.0/src/pyqtschema/widgets/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QLineEdit, QTextEdit
+from qtpy.QtWidgets import QLineEdit, QTextEdit
 
 from .base import SchemaWidgetMixin, state_property
 
 
 class TextSchemaWidget(SchemaWidgetMixin, QLineEdit):
     """ """
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema.egg-info/PKG-INFO` & `pyqtschema-0.2.0/src/pyqtschema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtschema
-Version: 0.1.9
+Version: 0.2.0
 Summary: Convert json-schema to QWidgets
 Home-page: https://github.com/amsico/pyqtschema
 Author: Amsico
 Author-email: amsico@eclipso.eu
 Project-URL: Bug Tracker, https://github.com/amsico/pyqtschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,18 @@
 `pyqtschema` is inspired by [qt-jsonschema-form](https://github.com/agoose77/qt-jsonschema-form). Due to the author's
 lack of [time](https://github.com/agoose77/qt-jsonschema-form/pull/1#issuecomment-595491242) and the missing
 [anyOf-support](https://github.com/agoose77/qt-jsonschema-form/blob/ca71ddbf10c2b309c3eb9c4fda6b054a0cb573dd/README.md?plain=1#L10)
 , this project was started.
 
 # Changelog
 
+### Version 0.2.0 (2023-05-05)
+
+* use [QtPy](https://pypi.org/project/QtPy/) instead of `PyQt5`
+
 ### Version 0.1.9 (2022-07-12)
 
 * FIX: default calculation for simple AllOf-cases
 * New example for ui_schema usage
 * New example for simple AllOf case
 
 ### Version 0.1.8 (2022-07-04)
```

### Comparing `pyqtschema-0.1.9/src/pyqtschema.egg-info/SOURCES.txt` & `pyqtschema-0.2.0/src/pyqtschema.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+changelog.md
 pyproject.toml
 setup.cfg
 src/pyqtschema/__init__.py
 src/pyqtschema/__main__.py
 src/pyqtschema/__version__.py
 src/pyqtschema/builder.py
 src/pyqtschema/schema.py
@@ -20,10 +21,10 @@
 src/pyqtschema/widgets/boolean.py
 src/pyqtschema/widgets/color.py
 src/pyqtschema/widgets/enu.py
 src/pyqtschema/widgets/groups.py
 src/pyqtschema/widgets/numeric.py
 src/pyqtschema/widgets/paths.py
 src/pyqtschema/widgets/root.py
-src/pyqtschema/widgets/signal.py
 src/pyqtschema/widgets/text.py
-src/pyqtschema/widgets/utils.py
+src/pyqtschema/widgets/utils.py
+tests/test_schema.py
```

