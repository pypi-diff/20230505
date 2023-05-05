# Comparing `tmp/HumanCursor-0.0.4.tar.gz` & `tmp/HumanCursor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.4.tar", last modified: Fri May  5 15:17:21 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.5.tar", last modified: Fri May  5 15:45:41 2023, max compression
```

## Comparing `HumanCursor-0.0.4.tar` & `HumanCursor-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.040648 HumanCursor-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.004715 HumanCursor-0.0.4/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5040 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5040 2023-05-05 15:17:21.040648 HumanCursor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.017508 HumanCursor-0.0.4/humancursor/
--rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.4/humancursor/__init__.py
--rw-rw-rw-   0        0        0     2027 2023-05-05 14:49:34.000000 HumanCursor-0.0.4/humancursor/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.024793 HumanCursor-0.0.4/humancursor/test/
--rw-rw-rw-   0        0        0        0 2023-05-05 14:50:29.000000 HumanCursor-0.0.4/humancursor/test/__init__.py
--rw-rw-rw-   0        0        0      266 2023-05-05 15:01:17.000000 HumanCursor-0.0.4/humancursor/test/system.py
--rw-rw-rw-   0        0        0     1110 2023-05-05 15:01:16.000000 HumanCursor-0.0.4/humancursor/test/web.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.034147 HumanCursor-0.0.4/humancursor/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.4/humancursor/utilities/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.4/humancursor/utilities/calc.py
--rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.4/humancursor/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.4/humancursor/utilities/web_adjuster.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:20.971877 HumanCursor-0.0.4/humancursor/venv/
-drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.037093 HumanCursor-0.0.4/humancursor/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-05-05 13:35:16.000000 HumanCursor-0.0.4/humancursor/venv/Scripts/activate_this.py
--rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.4/humancursor/web_cursor.py
--rw-rw-rw-   0        0        0      643 2023-05-05 15:14:19.000000 HumanCursor-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 15:17:21.042437 HumanCursor-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.959745 HumanCursor-0.0.5/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5384 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5384 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.964646 HumanCursor-0.0.5/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.5/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     2027 2023-05-05 14:49:34.000000 HumanCursor-0.0.5/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.970351 HumanCursor-0.0.5/humancursor/test/
+-rw-rw-rw-   0        0        0      275 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/humancursor/test/system.py
+-rw-rw-rw-   0        0        0     1119 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/humancursor/test/web.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.979754 HumanCursor-0.0.5/humancursor/utilities/
+-rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.5/humancursor/utilities/calc.py
+-rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.5/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.5/humancursor/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.5/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      667 2023-05-05 15:39:56.000000 HumanCursor-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/setup.cfg
```

### Comparing `HumanCursor-0.0.4/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: HumanCursor
-Version: 0.0.4
-Summary: Simulate Human Cursor Movement for Automated Scripts
-Author-email: Flori Batusha <floribatusha0@gmail.com>
-Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HumanCursor: A Python package for simulating human mouse movements
 
 HumanCursor is a Python package that allows you to simulate realistic human mouse movements on the web and the system. It can be used for automating scripts that require mouse interactions, such as web scraping, testing, or gaming.
 
 ## Features
 
 - HumanCursor uses a natural motion algorithm that mimics the way humans move the mouse cursor, with variable speed, acceleration, and curvature.
@@ -90,11 +77,23 @@
 cursor.controll_scroll_bar(element, amount_by_percentage=0.2, orientation='vertical')  # sets a vertical slider to 20% full
 
 cursor.scroll_into_view_of_element(element)  # scrolls into view of element if not already in it
 cursor.show_cursor()  # injects javascript that will display a red dot over the cursor on webpage. Should be called only for visual testing before script and not actual work.
 
 ```
 
+### DEMONSTRATION:
+To quickly check how the cursor moves, you can do this:
+
+```python
+from humancursor.test.system import start_sys_demo
+from humancursor.test.web import start_web_demo
+
+start_sys_demo() # to display a couple of mouse movements with system cursor
+
+start_web_demo() # to visualize how the mouse moves on webpage
+```
+
 
 ## License
 
 HumanCursor is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `HumanCursor-0.0.4/LICENSE` & `HumanCursor-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/PKG-INFO` & `HumanCursor-0.0.5/HumanCursor.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -90,11 +90,23 @@
 cursor.controll_scroll_bar(element, amount_by_percentage=0.2, orientation='vertical')  # sets a vertical slider to 20% full
 
 cursor.scroll_into_view_of_element(element)  # scrolls into view of element if not already in it
 cursor.show_cursor()  # injects javascript that will display a red dot over the cursor on webpage. Should be called only for visual testing before script and not actual work.
 
 ```
 
+### DEMONSTRATION:
+To quickly check how the cursor moves, you can do this:
+
+```python
+from humancursor.test.system import start_sys_demo
+from humancursor.test.web import start_web_demo
+
+start_sys_demo() # to display a couple of mouse movements with system cursor
+
+start_web_demo() # to visualize how the mouse moves on webpage
+```
+
 
 ## License
 
 HumanCursor is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `HumanCursor-0.0.4/README.md` & `HumanCursor-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: HumanCursor
+Version: 0.0.5
+Summary: Simulate Human Cursor Movement for Automated Scripts
+Author-email: Flori Batusha <floribatusha0@gmail.com>
+Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # HumanCursor: A Python package for simulating human mouse movements
 
 HumanCursor is a Python package that allows you to simulate realistic human mouse movements on the web and the system. It can be used for automating scripts that require mouse interactions, such as web scraping, testing, or gaming.
 
 ## Features
 
 - HumanCursor uses a natural motion algorithm that mimics the way humans move the mouse cursor, with variable speed, acceleration, and curvature.
@@ -77,11 +90,23 @@
 cursor.controll_scroll_bar(element, amount_by_percentage=0.2, orientation='vertical')  # sets a vertical slider to 20% full
 
 cursor.scroll_into_view_of_element(element)  # scrolls into view of element if not already in it
 cursor.show_cursor()  # injects javascript that will display a red dot over the cursor on webpage. Should be called only for visual testing before script and not actual work.
 
 ```
 
+### DEMONSTRATION:
+To quickly check how the cursor moves, you can do this:
+
+```python
+from humancursor.test.system import start_sys_demo
+from humancursor.test.web import start_web_demo
+
+start_sys_demo() # to display a couple of mouse movements with system cursor
+
+start_web_demo() # to visualize how the mouse moves on webpage
+```
+
 
 ## License
 
 HumanCursor is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `HumanCursor-0.0.4/humancursor/system_cursor.py` & `HumanCursor-0.0.5/humancursor/system_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/humancursor/test/web.py` & `HumanCursor-0.0.5/humancursor/test/web.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 from humancursor.web_cursor import WebCursor
 
 
-def start():
+def start_web_demo():
     # Disclaimer: This script is for demonstration purposes only and should not be used for any cheating activity.
     driver = webdriver.Chrome()
     cursor = WebCursor(driver)
 
     driver.get('https://humanbenchmark.com/tests/chimp')
     driver.maximize_window()
     cursor.show_cursor()
```

### Comparing `HumanCursor-0.0.4/humancursor/utilities/calc.py` & `HumanCursor-0.0.5/humancursor/utilities/calc.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/humancursor/utilities/human_curve_generator.py` & `HumanCursor-0.0.5/humancursor/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/humancursor/utilities/web_adjuster.py` & `HumanCursor-0.0.5/humancursor/utilities/web_adjuster.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/humancursor/web_cursor.py` & `HumanCursor-0.0.5/humancursor/web_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.4/pyproject.toml` & `HumanCursor-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "selenium >= 4.9.0",
-    "pyautogui >= 0.9.53"
+    "pyautogui >= 0.9.53",
+    "numpy >= 1.24.3"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

