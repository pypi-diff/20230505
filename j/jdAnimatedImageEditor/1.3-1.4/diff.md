# Comparing `tmp/jdAnimatedImageEditor-1.3.tar.gz` & `tmp/jdAnimatedImageEditor-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdAnimatedImageEditor-1.3.tar", last modified: Mon Jul 18 19:55:22 2022, max compression
+gzip compressed data, was "jdAnimatedImageEditor-1.4.tar", last modified: Fri May  5 12:50:18 2023, max compression
```

## Comparing `jdAnimatedImageEditor-1.3.tar` & `jdAnimatedImageEditor-1.4.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-18 19:55:22.982029 jdAnimatedImageEditor-1.3/
--rw-rw-rw-   0 root         (0) root         (0)      164 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1556 2022-07-18 19:55:22.981029 jdAnimatedImageEditor-1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-18 19:55:22.979029 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/
--rw-rw-rw-   0 root         (0) root         (0)      585 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/AboutDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2585 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/AboutDialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     2249 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Environment.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/FFmpegHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     4365 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Icon.svg
--rw-rw-rw-   0 root         (0) root         (0)    17577 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/MainWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     9181 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/MainWindow.ui
--rw-rw-rw-   0 root         (0) root         (0)     1565 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4138 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/SettingsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/SettingsDialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     1720 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        4 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-18 19:55:22.981029 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1556 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-07-18 19:55:22.000000 jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-18 19:55:22.982029 jdAnimatedImageEditor-1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3262 2022-07-18 19:54:53.000000 jdAnimatedImageEditor-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:50:18.019409 jdAnimatedImageEditor-1.4/
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35079 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-05-05 12:50:18.019409 jdAnimatedImageEditor-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3791 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:50:18.015409 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Environment.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/FFmpegHandler.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    17656 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:50:18.019409 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/translations/
+-rw-r--r--   0 root         (0) root         (0)    17354 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/translations/jdAnimatedImageEditor_de.ts
+-rw-r--r--   0 root         (0) root         (0)    16844 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/translations/jdAnimatedImageEditor_nl.ts
+-rw-r--r--   0 root         (0) root         (0)    16551 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/translations/jdAnimatedImageEditor_sv.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:50:18.019409 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:50:18.015409 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-05 12:50:18.000000 jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-05-05 12:49:13.000000 jdAnimatedImageEditor-1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 12:50:18.019409 jdAnimatedImageEditor-1.4/setup.cfg
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/AboutDialog.ui` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/AboutDialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/AboutDialog.ui` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/AboutDialog.ui`

```diff
@@ -65,15 +65,15 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="label_3">
           <property name="text">
-            <string notr="true">Copyright © 2022 JakobDev</string>
+            <string notr="true">Copyright © 2022-2023 JakobDev</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Environment.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
         self.recent_files = read_json_file(os.path.join(self.data_dir, "recentfiles.json"), [])
 
         self.ffmpeg_handler = FFmpegHandler(self)
 
     def _get_data_path(self) -> str:
         if platform.system() == "Windows":
-            return os.path.join(os.getenv("APPDATA"), "jdAnimatedImageEditor")
+            return os.path.join(os.getenv("APPDATA"), "JakobDev", "jdAnimatedImageEditor")
         elif platform.system() == "Darwin":
-            return os.path.join(str(Path.home()), "Library", "Application Support", "jdAnimatedImageEditor")
+            return os.path.join(str(Path.home()), "Library", "Application Support", "JakobDev", "jdAnimatedImageEditor")
         elif platform.system() == "Haiku":
-            return os.path.join(str(Path.home()), "config", "settings", "jdAnimatedImageEditor")
+            return os.path.join(str(Path.home()), "config", "settings", "JakobDev", "jdAnimatedImageEditor")
         else:
             if os.getenv("XDG_DATA_HOME"):
-                return os.path.join(os.getenv("XDG_DATA_HOME"), "jdAnimatedImageEditor")
+                return os.path.join(os.getenv("XDG_DATA_HOME"), "JakobDev", "jdAnimatedImageEditor")
             else:
-                return os.path.join(str(Path.home()), ".local", "share", "jdAnimatedImageEditor")
+                return os.path.join(str(Path.home()), ".local", "share", "JakobDev", "jdAnimatedImageEditor")
 
     def save_recent_files(self):
         try:
             os.makedirs(self.data_dir)
         except Exception:
             pass
         with open(os.path.join(self.data_dir, "recentfiles.json"), "w", encoding="utf-8") as f:
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/FFmpegHandler.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/FFmpegHandler.py`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Functions.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Functions.py`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Icon.svg` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/MainWindow.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from .Functions import get_logical_table_row_list, clear_table_widget, get_url_from_clipboard, get_sender_table_row, get_pillow_file_extensions, get_qt_file_filter, get_temp_path
 from PyQt6.QtWidgets import QMainWindow, QApplication, QLabel, QPushButton, QFileDialog, QMessageBox, QInputDialog, QHeaderView
 from PyQt6.QtCore import QCoreApplication, QByteArray, QBuffer, QIODevice
+from .ui_compiled.MainWindow import Ui_MainWindow
 from PyQt6.QtGui import QPixmap, QMovie, QAction
+from typing import Optional, TYPE_CHECKING
 from .SettingsDialog import SettingsDialog
 from .AboutDialog import AboutDialog
-from typing import Optional
 import PIL.ImageSequence
-from PyQt6 import uic
 import PIL.ImageDraw
 import PIL.Image
 import traceback
 import requests
 import shutil
 import sys
 import io
 import os
 
 
+if TYPE_CHECKING:
+    from .Environment import Environment
+
+
 class ImageLabel(QLabel):
     def __init__(self):
         super().__init__()
         self.setScaledContents(True)
 
         self._image = None
 
@@ -30,18 +34,19 @@
         self.setPixmap(pixmap)
         self._image = PIL.Image.open(io.BytesIO(image_bytes))
 
     def get_image(self) -> Optional[PIL.Image.Image]:
         return self._image.copy()
 
 
-class MainWindow(QMainWindow):
-    def __init__(self, env):
+class MainWindow(QMainWindow, Ui_MainWindow):
+    def __init__(self, env: "Environment"):
         super().__init__()
-        uic.loadUi(os.path.join(os.path.dirname(__file__), "MainWindow.ui"), self)
+
+        self.setupUi(self)
 
         self._env = env
         self._modified = False
         self._current_path = None
 
         self._settings_dialog = SettingsDialog(env, self)
         self._about_dialog = AboutDialog(env)
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/MainWindow.ui` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/Settings.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/Settings.py`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/SettingsDialog.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/SettingsDialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 from .Functions import select_combo_box_data, remove_list_duplicates, is_flatpak
+from .ui_compiled.SettingsDialog import Ui_SettingsDialog
 from PyQt6.QtCore import QCoreApplication, QLocale
 from PyQt6.QtWidgets import QDialog, QFileDialog
+from .Languages import get_language_names
+from typing import TYPE_CHECKING
 from .Settings import Settings
-from PyQt6 import uic
+import sys
 import os
 
 
-class SettingsDialog(QDialog):
-    def __init__(self, env, main_window) -> None:
+if TYPE_CHECKING:
+    from .Environment import Environment
+    from .MainWindow import MainWindow
+
+
+class SettingsDialog(QDialog, Ui_SettingsDialog):
+    def __init__(self, env: "Environment", main_window: "MainWindow") -> None:
         super().__init__()
-        uic.loadUi(os.path.join(os.path.dirname(__file__), "SettingsDialog.ui"), self)
+
+        self.setupUi(self)
 
         self._env = env
         self._main_window = main_window
 
+        found_translations = False
+        language_names = get_language_names()
         self.language_box.addItem(QCoreApplication.translate("SettingsDialog", "System language"), "default")
         self.language_box.addItem("English", "en")
         for i in os.listdir(os.path.join(env.program_dir, "translations")):
             if i.endswith(".qm"):
-                self.language_box.addItem(
-                    QLocale.languageToString(QLocale(i.removeprefix("jdAnimatedImageEditor_").removesuffix(".qm")).language()),
-                    i.removeprefix("jdAnimatedImageEditor_").removesuffix(".qm"))
+                lang = i.removeprefix("jdAnimatedImageEditor_").removesuffix(".qm")
+                self.language_box.addItem(language_names.get(lang, lang), lang)
+                found_translations = True
+        if not found_translations:
+             print("No compiled translations found. Please run tools/BuildTranslations to build the Translations.py.", file=sys.stderr)
 
         self.window_title_box.addItem("jdAnimatedImageEditor", "programName")
         self.window_title_box.addItem(QCoreApplication.translate("SettingsDialog", "Filename") + " - jdAnimatedImageEditor", "fileName")
         self.window_title_box.addItem(QCoreApplication.translate("SettingsDialog", "Path") + " - jdAnimatedImageEditor", "filePath")
 
         if is_flatpak():
             # Flatpak should only use the bundled FFmpeg
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/SettingsDialog.ui` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor/__init__.py` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from PyQt6.QtCore import QTranslator, QLocale, QLibraryInfo
 from PyQt6.QtWidgets import QApplication
-from .MainWindow import MainWindow
 from .Environment import Environment
+from .MainWindow import MainWindow
 import PIL.Image
 import sys
 import os
 
 
 def main():
+    if not os.path.isdir(os.path.join(os.path.dirname(__file__), "ui_compiled")):
+        print("Could not find compiled ui files. Please run tools/CompileUI.py first.", file=sys.stderr)
+        sys.exit(1)
+
     app = QApplication(sys.argv)
 
     env = Environment()
 
-    app.setDesktopFileName("com.gitlab.JakobDev.jdAnimatedImageEditor")
+    app.setDesktopFileName("page.codeberg.JakobDev.jdAnimatedImageEditor")
     app.setApplicationName("jdAnimatedImageEditor")
     app.setWindowIcon(env.icon)
 
     app_translator = QTranslator()
     qt_translator = QTranslator()
     app_trans_dir = os.path.join(env.program_dir, "translations")
     qt_trans_dir = QLibraryInfo.path(QLibraryInfo.LibraryPath.TranslationsPath)
```

### Comparing `jdAnimatedImageEditor-1.3/jdAnimatedImageEditor.egg-info/SOURCES.txt` & `jdAnimatedImageEditor-1.4/jdAnimatedImageEditor.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+BuildBackend.py
+LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 jdAnimatedImageEditor/AboutDialog.py
-jdAnimatedImageEditor/AboutDialog.ui
 jdAnimatedImageEditor/Environment.py
 jdAnimatedImageEditor/FFmpegHandler.py
 jdAnimatedImageEditor/Functions.py
 jdAnimatedImageEditor/Icon.svg
+jdAnimatedImageEditor/Languages.py
 jdAnimatedImageEditor/MainWindow.py
-jdAnimatedImageEditor/MainWindow.ui
 jdAnimatedImageEditor/Settings.py
 jdAnimatedImageEditor/SettingsDialog.py
-jdAnimatedImageEditor/SettingsDialog.ui
 jdAnimatedImageEditor/__init__.py
 jdAnimatedImageEditor/version.txt
 jdAnimatedImageEditor.egg-info/PKG-INFO
 jdAnimatedImageEditor.egg-info/SOURCES.txt
 jdAnimatedImageEditor.egg-info/dependency_links.txt
 jdAnimatedImageEditor.egg-info/entry_points.txt
 jdAnimatedImageEditor.egg-info/requires.txt
-jdAnimatedImageEditor.egg-info/top_level.txt
+jdAnimatedImageEditor.egg-info/top_level.txt
+jdAnimatedImageEditor/translations/jdAnimatedImageEditor_de.ts
+jdAnimatedImageEditor/translations/jdAnimatedImageEditor_nl.ts
+jdAnimatedImageEditor/translations/jdAnimatedImageEditor_sv.ts
+jdAnimatedImageEditor/ui/AboutDialog.ui
+jdAnimatedImageEditor/ui/MainWindow.ui
+jdAnimatedImageEditor/ui/SettingsDialog.ui
```

