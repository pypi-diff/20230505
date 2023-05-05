# Comparing `tmp/pyUIauto-0.1.2.tar.gz` & `tmp/pyUIauto-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUIauto-0.1.2.tar", max compression
+gzip compressed data, was "pyUIauto-0.1.3.tar", max compression
```

## Comparing `pyUIauto-0.1.2.tar` & `pyUIauto-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.2/LICENSE
--rw-r--r--   0        0        0      905 2023-05-05 08:52:35.811702 pyUIauto-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.2/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.2/pyuiauto/application.py
--rw-r--r--   0        0        0     7054 2023-05-05 08:36:46.552241 pyUIauto-0.1.2/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16286 2023-05-05 08:45:27.938656 pyUIauto-0.1.2/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.2/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.2/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.2/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.2/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    10176 2023-05-02 16:12:27.994623 pyUIauto-0.1.2/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.2/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.2/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.2/pyuiauto/win/application.py
--rw-r--r--   0        0        0     9497 2023-05-05 08:45:47.872926 pyUIauto-0.1.2/pyuiauto/win/components.py
--rw-r--r--   0        0        0     3923 2023-05-05 08:52:41.415706 pyUIauto-0.1.2/README.md
--rw-r--r--   0        0        0     4927 2023-05-05 08:52:57.858415 pyUIauto-0.1.2/setup.py
--rw-r--r--   0        0        0     4802 2023-05-05 08:52:57.858415 pyUIauto-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.3/LICENSE
+-rw-r--r--   0        0        0      905 2023-05-05 09:32:37.754805 pyUIauto-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.3/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.3/pyuiauto/application.py
+-rw-r--r--   0        0        0     7054 2023-05-05 08:36:46.552241 pyUIauto-0.1.3/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16286 2023-05-05 08:45:27.938656 pyUIauto-0.1.3/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.3/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.3/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.3/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.3/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    10332 2023-05-05 09:31:42.558121 pyUIauto-0.1.3/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.3/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.3/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.3/pyuiauto/win/application.py
+-rw-r--r--   0        0        0     9653 2023-05-05 09:30:23.120617 pyUIauto-0.1.3/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     3934 2023-05-05 09:32:16.610049 pyUIauto-0.1.3/README.md
+-rw-r--r--   0        0        0     4938 2023-05-05 09:32:47.343610 pyUIauto-0.1.3/setup.py
+-rw-r--r--   0        0        0     4812 2023-05-05 09:32:47.343610 pyUIauto-0.1.3/PKG-INFO
```

### Comparing `pyUIauto-0.1.2/LICENSE` & `pyUIauto-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyproject.toml` & `pyUIauto-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyUIauto-0.1.2/pyuiauto/base/application.py` & `pyUIauto-0.1.3/pyuiauto/base/application.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/base/components.py` & `pyUIauto-0.1.3/pyuiauto/base/components.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/exceptions.py` & `pyUIauto-0.1.3/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/mac/application.py` & `pyUIauto-0.1.3/pyuiauto/mac/application.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/mac/components.py` & `pyUIauto-0.1.3/pyuiauto/mac/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,17 @@
 
 
 class UIButton(UIBaseComponent, UIButtonWrapper):
     native_control_type: str = "AXButton"
     
     def press(self):
         self.invoke()
+    
+    def setValue(self, value):
+        return super().setValue(value)
 
 class UIRadioButton(UIBaseComponent, UIRadioButtonWrapper):
     native_control_type: str = "AXRadioButton"
 
 class UIText(UIBaseComponent, UITextWrapper):
     native_control_type: str = "AXText"
 
@@ -222,14 +225,17 @@
     native_control_type: str = "AXMenu"
 
 class UIMenuItem(UIBaseComponent, UIMenuItemWrapper):
     native_control_type: str = "AXMenuItem"
 
     def select(self):
         self.invoke()
+    
+    def setValue(self, value):
+        return super().setValue(value)
 
 class UIWindow(UIBaseComponent, UIWindowWrapper):
     native_control_type: str = "AXWindow"
 
     def moveResize(self, x=None, y=None, width=None, height=None):
         left, top, _, _ = self.getCoordinates()
         w, h = self.getSizes()
```

### Comparing `pyUIauto-0.1.2/pyuiauto/wait.py` & `pyUIauto-0.1.3/pyuiauto/wait.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/win/application.py` & `pyUIauto-0.1.3/pyuiauto/win/application.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.2/pyuiauto/win/components.py` & `pyUIauto-0.1.3/pyuiauto/win/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,17 @@
     native_control_type: str = "Button"
 
     def getValue(self):
         return self.component.get_toggle_state()
     
     def press(self):
         self.component.click()
+    
+    def setValue(self, value):
+        return super().setValue(value)
 
 class UIRadioButton(UIBaseComponent, UIRadioButtonWrapper):
     native_control_type: str = "RadioButton"
 
 class UIText(UIBaseComponent, UITextWrapper):
     native_control_type: str = "Text"
 class UISlider(UIBaseComponent, UISliderWrapper):
@@ -215,14 +218,17 @@
         try:
             return bool(self.component.iface_toggle)
         except NoPatternInterfaceError:
             return False
 
     def select(self):
         self.component.select()
+    
+    def setValue(self, value):
+        return super().setValue(value)
 
 class UIWindow(UIBaseComponent, UIWindowWrapper):
     native_control_type: str = "Window"
     
     def moveResize(self, x=None, y=None, width=None, height=None):
         cur_rect = self.component.rectangle()
```

### Comparing `pyUIauto-0.1.2/README.md` & `pyUIauto-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 ## Version History
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
   - 0.1.2
+  - 0.1.3
     - Fixed some issues with setValue() method on buttons and menus
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyUIauto-0.1.2/setup.py` & `pyUIauto-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.2\n    - Fixed some issues with setValue() method on buttons and menus\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.2\n  - 0.1.3\n    - Fixed some issues with setValue() method on buttons and menus\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyUIauto-0.1.2/PKG-INFO` & `pyUIauto-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -104,14 +104,15 @@
 ## Version History
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
   - 0.1.2
+  - 0.1.3
     - Fixed some issues with setValue() method on buttons and menus
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

