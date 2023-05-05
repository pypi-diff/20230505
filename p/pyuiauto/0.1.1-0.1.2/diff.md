# Comparing `tmp/pyUIauto-0.1.1.tar.gz` & `tmp/pyUIauto-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUIauto-0.1.1.tar", max compression
+gzip compressed data, was "pyUIauto-0.1.2.tar", max compression
```

## Comparing `pyUIauto-0.1.1.tar` & `pyUIauto-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.1/LICENSE
--rw-r--r--   0        0        0      905 2023-05-02 16:12:27.990637 pyUIauto-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.1/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.1/pyuiauto/application.py
--rw-r--r--   0        0        0     7030 2023-05-02 16:12:27.991633 pyUIauto-0.1.1/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16166 2023-05-02 16:12:27.992630 pyUIauto-0.1.1/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.1/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.1/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.1/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.1/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    10176 2023-05-02 16:12:27.994623 pyUIauto-0.1.1/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.1/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.1/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.1/pyuiauto/win/application.py
--rw-r--r--   0        0        0     9497 2023-05-02 16:12:27.999607 pyUIauto-0.1.1/pyuiauto/win/components.py
--rw-r--r--   0        0        0     3843 2023-05-02 16:12:27.986304 pyUIauto-0.1.1/README.md
--rw-r--r--   0        0        0     4847 2023-05-02 16:12:38.864334 pyUIauto-0.1.1/setup.py
--rw-r--r--   0        0        0     4724 2023-05-02 16:12:38.864334 pyUIauto-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.2/LICENSE
+-rw-r--r--   0        0        0      905 2023-05-05 08:52:35.811702 pyUIauto-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.2/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.2/pyuiauto/application.py
+-rw-r--r--   0        0        0     7054 2023-05-05 08:36:46.552241 pyUIauto-0.1.2/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16286 2023-05-05 08:45:27.938656 pyUIauto-0.1.2/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.2/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.2/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.2/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.2/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    10176 2023-05-02 16:12:27.994623 pyUIauto-0.1.2/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.2/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.2/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.2/pyuiauto/win/application.py
+-rw-r--r--   0        0        0     9497 2023-05-05 08:45:47.872926 pyUIauto-0.1.2/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     3923 2023-05-05 08:52:41.415706 pyUIauto-0.1.2/README.md
+-rw-r--r--   0        0        0     4927 2023-05-05 08:52:57.858415 pyUIauto-0.1.2/setup.py
+-rw-r--r--   0        0        0     4802 2023-05-05 08:52:57.858415 pyUIauto-0.1.2/PKG-INFO
```

### Comparing `pyUIauto-0.1.1/LICENSE` & `pyUIauto-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyproject.toml` & `pyUIauto-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyUIauto-0.1.1/pyuiauto/base/application.py` & `pyUIauto-0.1.2/pyuiauto/base/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     def relaunchApp(self):
         '''Application class relaunch app method\n
         Uses it's context manager __enter__ __exit__ methods to quit and reopen the application.'''
         self.__exit__()
         self.launchApp()
         self.__enter__()
 
-    def __enter__(self):
+    def __enter__(self) -> UIApplicationWrapper:
         self.launchApp()
         self.connectApp()
         return self
     
     def __exit__(self, *args):
         if not self.isAppRunning():
             logging.critical(f"The {self.appName} application may have crashed")
```

### Comparing `pyUIauto-0.1.1/pyuiauto/base/components.py` & `pyUIauto-0.1.2/pyuiauto/base/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,16 @@
     
     def toggle(self, value):
         '''Button toggle method\n
         Performs a button press if the provided value != current value.
         (overrides the setValue method)'''
         return self.press() if self.getValue() != value else None
 
-    setValue = toggle
+    def setValue(self, value):
+        return self.toggle(value)
 
 class UIRadioButtonWrapper(): ...
 
 class UITextWrapper(): ...
 
 class UISliderWrapper(): ...
 
@@ -326,27 +327,29 @@
 class UIMenuWrapper(): ...
 class UIMenuItemWrapper():
     @abstractmethod
     def select(self):
         '''Menu item select method\n
         Similar to the invoke method, selects a menu item without actual mouse movement.'''
     
-    invoke = select
+    def invoke(self):
+        return self.select()
 
     def toggle(self, value) -> bool:
         '''Menu item toggle method\n
         Selects a menu item if the provided value != current value.
         (overrides the setValue method)'''
         if self.getValue() != value:
             self.select()
             return True
         else:
             return False
     
-    setValue = toggle
+    def setValue(self, value):
+        return self.toggle(value)
 
 class UIWindowWrapper():
     @abstractmethod
     def moveResize(self, x: int = None, y: int = None, width: int = None, height: int = None):
         '''Window move resize method\n
         Moves a windows top left corner to the specified pixel points x, y (if provided)
         and resizes the window to the specified pixel width, height (if provided)
```

### Comparing `pyUIauto-0.1.1/pyuiauto/exceptions.py` & `pyUIauto-0.1.2/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyuiauto/mac/application.py` & `pyUIauto-0.1.2/pyuiauto/mac/application.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyuiauto/mac/components.py` & `pyUIauto-0.1.2/pyuiauto/mac/components.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyuiauto/wait.py` & `pyUIauto-0.1.2/pyuiauto/wait.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyuiauto/win/application.py` & `pyUIauto-0.1.2/pyuiauto/win/application.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/pyuiauto/win/components.py` & `pyUIauto-0.1.2/pyuiauto/win/components.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.1/README.md` & `pyUIauto-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -81,13 +81,15 @@
 
 ## Version History
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
+  - 0.1.2
+    - Fixed some issues with setValue() method on buttons and menus
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyUIauto-0.1.1/setup.py` & `pyUIauto-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.2\n    - Fixed some issues with setValue() method on buttons and menus\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyUIauto-0.1.1/PKG-INFO` & `pyUIauto-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -103,14 +103,16 @@
 
 ## Version History
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
+  - 0.1.2
+    - Fixed some issues with setValue() method on buttons and menus
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

