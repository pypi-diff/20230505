# Comparing `tmp/tomato-engine-1.8.2.tar.gz` & `tmp/tomato-engine-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-engine-1.8.2.tar", last modified: Mon Oct 17 18:09:12 2022, max compression
+gzip compressed data, was "tomato-engine-1.8.3.tar", last modified: Thu May  4 22:52:20 2023, max compression
```

## Comparing `tomato-engine-1.8.2.tar` & `tomato-engine-1.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.460577 tomato-engine-1.8.2/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3044 2022-10-17 18:09:12.460577 tomato-engine-1.8.2/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2412 2022-06-23 17:52:28.000000 tomato-engine-1.8.2/README.md
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2022-10-17 18:09:12.460577 tomato-engine-1.8.2/setup.cfg
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2022-10-17 18:07:59.000000 tomato-engine-1.8.2/setup.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.452577 tomato-engine-1.8.2/src/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.456577 tomato-engine-1.8.2/src/tomato/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       48 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.456577 tomato-engine-1.8.2/src/tomato/classes/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       25 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/classes/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    11178 2022-10-17 01:48:20.000000 tomato-engine-1.8.2/src/tomato/classes/board.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-17 06:22:46.000000 tomato-engine-1.8.2/src/tomato/classes/cell.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4241 2022-10-17 01:48:20.000000 tomato-engine-1.8.2/src/tomato/classes/cellmatrix.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3554 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/classes/window.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.456577 tomato-engine-1.8.2/src/tomato/functions/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/functions/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/functions/display.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-10-17 18:03:59.000000 tomato-engine-1.8.2/src/tomato/functions/file_io.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-17 06:11:40.000000 tomato-engine-1.8.2/src/tomato/functions/utils.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.460577 tomato-engine-1.8.2/src/tomato/rules/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-06-20 23:52:07.000000 tomato-engine-1.8.2/src/tomato/rules/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-17 07:32:26.000000 tomato-engine-1.8.2/src/tomato/rules/colorful.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-17 07:16:00.000000 tomato-engine-1.8.2/src/tomato/rules/colorful_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2022-10-17 17:30:15.000000 tomato-engine-1.8.2/src/tomato/rules/cyclic.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-17 17:25:05.000000 tomato-engine-1.8.2/src/tomato/rules/cyclic_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2022-10-17 07:09:33.000000 tomato-engine-1.8.2/src/tomato/rules/game_of_life.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-17 07:15:45.000000 tomato-engine-1.8.2/src/tomato/rules/game_of_life_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2022-10-17 17:53:21.000000 tomato-engine-1.8.2/src/tomato/rules/toothpick_fractal.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2022-10-17 17:53:18.000000 tomato-engine-1.8.2/src/tomato/rules/toothpick_fractal_demo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-10-17 18:09:12.460577 tomato-engine-1.8.2/src/tomato_engine.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3044 2022-10-17 18:09:12.000000 tomato-engine-1.8.2/src/tomato_engine.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2022-10-17 18:09:12.000000 tomato-engine-1.8.2/src/tomato_engine.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2022-10-17 18:09:12.000000 tomato-engine-1.8.2/src/tomato_engine.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2022-10-17 18:09:12.000000 tomato-engine-1.8.2/src/tomato_engine.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2022-10-17 18:09:12.000000 tomato-engine-1.8.2/src/tomato_engine.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/README.md
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-05-04 22:52:20.334214 tomato-engine-1.8.3/setup.cfg
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-05-04 22:50:25.000000 tomato-engine-1.8.3/setup.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/tomato/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       48 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/tomato/classes/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       25 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/classes/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/classes/board.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/classes/cell.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4569 2023-05-03 22:45:39.000000 tomato-engine-1.8.3/src/tomato/classes/cellmatrix.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-04 17:41:57.000000 tomato-engine-1.8.3/src/tomato/classes/window.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato/functions/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/functions/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.3/src/tomato/functions/display.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.3/src/tomato/functions/file_io.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/functions/utils.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato/rules/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/rules/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/colorful.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/colorful_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/cyclic.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/cyclic_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.3/src/tomato/rules/game_of_life.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/game_of_life_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal_demo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato_engine.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/top_level.txt
```

### Comparing `tomato-engine-1.8.2/LICENSE` & `tomato-engine-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/PKG-INFO` & `tomato-engine-1.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.2
+Version: 1.8.3
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: rulesets
 License-File: LICENSE
 
-
 # tomato-engine
 
 **Engine for prototyping and playing with cellular automata.**
 
 ## Motivation
 
 Tomato-engine aims to be an easy to use, extensible and hackable
 framework for running cellular automata simulations controlled
 via Python.
 
 It handles much of the overhead involved in getting a simple
- realtime visualization of the cellular automata to run, while
- providing an object oriented interface through which the user
- can easily craft their own cellular automata ruleset, and leave
- tomato-engine to handle all the rest.
+realtime visualization of the cellular automata to run, while
+providing an object oriented interface through which the user
+can easily craft their own cellular automata ruleset, and leave
+tomato-engine to handle all the rest.
 
 ## Installation
 
 ```
 pip3 install tomato-engine
 ```
 
 ## Example and basic usage
 
 New rules are implemented on a Python module, which must contain
 the class Cell, which inherits from CellTemplate and specifies
 how the cell should update on each iteration through the function
 Cell.update.
 
-For simple, binary automata rulesets such as the Conway's Game of
+For simple, binary totalistic automata rulesets such as the Conway's Game of
 Life, the class can be as simple as this:
 
 ```python
 from tomato.classes import cell
 
 class Cell(cell.CellTemplate):
     def update(self, state_matrix):
@@ -73,15 +72,15 @@
 
     @property
     def live_neighbors(self):
         return sum(self.neighbors)
 ```
 
 This module is then imported and passed to the Board class, which
-provides the user interface. 
+provides the user interface.
 
 ```python
 import tomato as tt
 from tomato.functions import utils
 
 from my_rules import game_of_life as rule
```

### Comparing `tomato-engine-1.8.2/README.md` & `tomato-engine-1.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-
 # tomato-engine
 
 **Engine for prototyping and playing with cellular automata.**
 
 ## Motivation
 
 Tomato-engine aims to be an easy to use, extensible and hackable
 framework for running cellular automata simulations controlled
 via Python.
 
 It handles much of the overhead involved in getting a simple
- realtime visualization of the cellular automata to run, while
- providing an object oriented interface through which the user
- can easily craft their own cellular automata ruleset, and leave
- tomato-engine to handle all the rest.
+realtime visualization of the cellular automata to run, while
+providing an object oriented interface through which the user
+can easily craft their own cellular automata ruleset, and leave
+tomato-engine to handle all the rest.
 
 ## Installation
 
 ```
 pip3 install tomato-engine
 ```
 
 ## Example and basic usage
 
 New rules are implemented on a Python module, which must contain
 the class Cell, which inherits from CellTemplate and specifies
 how the cell should update on each iteration through the function
 Cell.update.
 
-For simple, binary automata rulesets such as the Conway's Game of
+For simple, binary totalistic automata rulesets such as the Conway's Game of
 Life, the class can be as simple as this:
 
 ```python
 from tomato.classes import cell
 
 class Cell(cell.CellTemplate):
     def update(self, state_matrix):
@@ -57,15 +56,15 @@
 
     @property
     def live_neighbors(self):
         return sum(self.neighbors)
 ```
 
 This module is then imported and passed to the Board class, which
-provides the user interface. 
+provides the user interface.
 
 ```python
 import tomato as tt
 from tomato.functions import utils
 
 from my_rules import game_of_life as rule
```

### Comparing `tomato-engine-1.8.2/setup.cfg` & `tomato-engine-1.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tomato-engine
-version = 1.8.2
+version = 1.8.3
 author = Eduardo Lopes Dias, Murilo Melhem
 author_email = eduardotogpi@usp.br
 description = Engine for prototyping and playing with cellular automata.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://codeberg.org/eduardotogpi/tomato-engine
 project_urls =
```

### Comparing `tomato-engine-1.8.2/setup.py` & `tomato-engine-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomato-engine",
-    version="1.8.2",
+    version="1.8.3",
     author="Eduardo Lopes Dias, Murilo Melhem",
     author_email="eduardosprp@usp.br",
     description="Engine for prototyping and playing with cellular automata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeberg.org/eduardotogpi/tomato-engine",
     project_urls={
```

### Comparing `tomato-engine-1.8.2/src/tomato/classes/board.py` & `tomato-engine-1.8.3/src/tomato/classes/board.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         if self.inline:
             show_window = False
 
         if self.generate_gif:
             self.generate_figures = True
             if self.generations is None:
                 raise TypeError(
-                    f"You must specify the number of generations for the gif to be created."
+                    "You must specify the number of generations for the gif to "
+                    "be created."
                 )
 
         if self.generate_figures:
             self.check_dir(self.generate_figures_dir)
 
         self.load_state(state_matrix, cell_args, multithreaded)
         self.cellMatrix.simulation_start(state_matrix, cell_args)
@@ -90,17 +91,15 @@
 
     def resume(self, **kwargs):
         # {{{
         """
         Continua a simulação de onde ela parou.
         """
 
-        cell_args = kwargs.get("cell_args", None)
         show_window = kwargs.get("show_window", True)
-        multithreaded = kwargs.get("multithreaded", False)
         self.paused = kwargs.get("paused", False)
         self.generations = kwargs.get("generations", None)
         self.inline = kwargs.get("inline", False)
         self.generate_figures = kwargs.get("generate_figures", False)
         self.generate_figures_dir = kwargs.get(
             "generate_figures_dir", f"{self.title}{os.path.sep}"
         )
@@ -110,15 +109,16 @@
         if self.inline is True:
             show_window = False
 
         if self.generate_gif:
             self.generate_figures = True
             if self.generations is None:
                 raise TypeError(
-                    f"You must specify the number of generations for the gif to be created."
+                    "You must specify the number of generations for the gif to "
+                    "be created."
                 )
 
         if self.generate_figures:
             self.check_dir(self.generate_figures_dir)
 
         if show_window:
             self.show_window()
@@ -138,17 +138,15 @@
                 if self.step is None:
                     self.save_png()
                 else:
                     if self.generation % self.step == 0:
                         self.save_png()
             if self.inline:
                 display.clear_output(wait=True)
-                display.display(
-                    file_io.img(self.display_matrix, self.cell_size)
-                )
+                display.display(file_io.img(self.display_matrix, self.cell_size))
         except AttributeError:
             pass
         if not self.debug:
             self.cellMatrix.update(*args, **kwargs)
         else:
             initial_time = time()
             self.cellMatrix.update()
@@ -250,17 +248,15 @@
         else:
             CellMatrix = CellMatrixUnthreaded
 
         self.generation = 0
 
         if isinstance(state_matrix, str):
             png_matrix = file_io.load_png(state_matrix, size=self.cell_size)
-            self.cellMatrix = CellMatrix.from_display(
-                png_matrix, self.rule, cell_args
-            )
+            self.cellMatrix = CellMatrix.from_display(png_matrix, self.rule, cell_args)
         elif isinstance(state_matrix, np.ndarray):
             self.cellMatrix = CellMatrix(state_matrix, self.rule, cell_args)
         elif isinstance(state_matrix, list):
             state_matrix = np.array(state_matrix)
             self.cellMatrix = CellMatrix(state_matrix, self.rule, cell_args)
         else:
             raise TypeError(
@@ -313,17 +309,15 @@
             path = f"{self.generate_figures_dir}{self.generation}.png"
         elif isinstance(path, str):
             if path.endswith(f"{os.path.sep}"):
                 path = f"{path}{self.generation}.png"
             elif not path.endswith(".png"):
                 path = f"{path}{os.path.sep}{self.generation}.png"
 
-        file_io.save_png(
-            path, self.display_matrix, self.cell_size, print_output=False
-        )
+        file_io.save_png(path, self.display_matrix, self.cell_size, print_output=False)
 
     # }}}
 
     def save_gif(self, path=None, max_fps=60):
         # {{{
         """
         Salva o estado da cellMatrix em uma png, para
@@ -333,46 +327,43 @@
             path = f"{self.generate_figures_dir}"
 
         file_io.save_gif(path, fps=self.max_fps)
 
     # }}}
 
     def check_dir(self, add=0):
-# {{{
+        # {{{
         """
         Função para checar se o diretório existe e renomear
         com números inteiros em sequência para a criação de outro diretório.
         """
         i = 1
         dir = self.generate_figures_dir
         if dir is None:
             dir = f"{self.title}{os.path.sep}"
         if not dir.endswith(f"{os.path.sep}"):
             dir = f"{dir}{os.path.sep}"
         while os.path.isdir(dir):
             num = "%03d" % i
-            dir = (
-                dir.split(f"{os.path.sep}")[0].split("_")[0]
-                + "_"
-                + f"{num}"
-                + f"{os.path.sep}"
-            )
+            dir = f"{dir.split(os.path.sep)[0].split('_')[0]}_{num}{os.path.sep}"
             i += 1
         os.mkdir(dir)
         self.generate_figures_dir = dir
-# }}}
+
+    # }}}
 
     def current_time_millis(self):
-# {{{
+        # {{{
         """
         Função auxiliar para retornar o tempo UNIX em milissegundos
         arredondado.
         """
         return round(time() * 1000)
-# }}}
+
+    # }}}
 
     @property
     def state_matrix(self):
         # {{{
         """
         Propriedade de conveniência para acessar a matriz de estados.
         """
```

### Comparing `tomato-engine-1.8.2/src/tomato/classes/cell.py` & `tomato-engine-1.8.3/src/tomato/classes/cell.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/classes/cellmatrix.py` & `tomato-engine-1.8.3/src/tomato/classes/cellmatrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-import numpy as np
-from multiprocessing import Pool
 from functools import partial
+from multiprocessing import Pool
+from types import ModuleType
+
+import numpy as np
+
+from .cell import CellTemplate
 
 """
 Estrutura de dados para a matriz que contém todos os autômatos.
 """
 
 
 class CellMatrix:
@@ -12,15 +16,24 @@
     def __init__(self, state_matrix, rule, cell_args=None):
         # {{{
         """
         Cria a matriz de autômatos a partir de uma regra e a
         matriz de estado inicial.
         """
 
-        self.Cell = rule.Cell
+        if isinstance(rule, ModuleType):
+            self.Cell = rule.Cell
+        elif rule in CellTemplate.__subclasses__():
+            self.Cell = rule
+        else:
+            raise TypeError(
+                f"Tipo {type(rule)} inválido para o parâmetro rule. "
+                "Tipos válidos são 'Cell' e 'module'"
+            )
+
         self.state_matrix = state_matrix.copy()
 
         if cell_args is not None:
             self.cell_matrix = np.array(
                 [
                     self.Cell(value, (lin_num, col_num), cell_args)
                     for lin_num, lin in enumerate(self.state_matrix)
@@ -97,28 +110,24 @@
     # {{{
     def update(self, *args, **kwargs):
         # {{{
 
         old_state_matrix = self.state_matrix
 
         update_cell = partial(
-            self.update_cell,
-            old_state_matrix=old_state_matrix,
-            *args, **kwargs
+            self.update_cell, old_state_matrix=old_state_matrix, *args, **kwargs
         )
 
         with Pool() as p:
             new_state_matrix = p.map(update_cell, self.cell_matrix)
 
         for cell, new_value in zip(self.cell_matrix, new_state_matrix):
             cell.value = new_value
 
-        self.state_matrix = np.array(new_state_matrix).reshape(
-            old_state_matrix.shape
-        )
+        self.state_matrix = np.array(new_state_matrix).reshape(old_state_matrix.shape)
 
         return self.state_matrix
 
     # }}}
 
     @staticmethod
     def update_cell(cell, old_state_matrix, *args, **kwargs):
```

### Comparing `tomato-engine-1.8.2/src/tomato/classes/window.py` & `tomato-engine-1.8.3/src/tomato/classes/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from ..functions import display
 import pygame
 from time import time
 from numpy import mean, std
 
+from os import environ
+environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 
 class Window:
 
     """
     Uma classe para ser a representação da janelinha da simulação
     no projeto. Sim, porque não temos overhead suficiente.
```

### Comparing `tomato-engine-1.8.2/src/tomato/functions/display.py` & `tomato-engine-1.8.3/src/tomato/functions/display.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/functions/file_io.py` & `tomato-engine-1.8.3/src/tomato/functions/file_io.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/functions/utils.py` & `tomato-engine-1.8.3/src/tomato/functions/utils.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/rules/colorful.py` & `tomato-engine-1.8.3/src/tomato/rules/colorful.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/rules/cyclic.py` & `tomato-engine-1.8.3/src/tomato/rules/cyclic.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/rules/game_of_life.py` & `tomato-engine-1.8.3/src/tomato/rules/game_of_life.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato/rules/toothpick_fractal.py` & `tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.2/src/tomato_engine.egg-info/PKG-INFO` & `tomato-engine-1.8.3/src/tomato_engine.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.2
+Version: 1.8.3
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: rulesets
 License-File: LICENSE
 
-
 # tomato-engine
 
 **Engine for prototyping and playing with cellular automata.**
 
 ## Motivation
 
 Tomato-engine aims to be an easy to use, extensible and hackable
 framework for running cellular automata simulations controlled
 via Python.
 
 It handles much of the overhead involved in getting a simple
- realtime visualization of the cellular automata to run, while
- providing an object oriented interface through which the user
- can easily craft their own cellular automata ruleset, and leave
- tomato-engine to handle all the rest.
+realtime visualization of the cellular automata to run, while
+providing an object oriented interface through which the user
+can easily craft their own cellular automata ruleset, and leave
+tomato-engine to handle all the rest.
 
 ## Installation
 
 ```
 pip3 install tomato-engine
 ```
 
 ## Example and basic usage
 
 New rules are implemented on a Python module, which must contain
 the class Cell, which inherits from CellTemplate and specifies
 how the cell should update on each iteration through the function
 Cell.update.
 
-For simple, binary automata rulesets such as the Conway's Game of
+For simple, binary totalistic automata rulesets such as the Conway's Game of
 Life, the class can be as simple as this:
 
 ```python
 from tomato.classes import cell
 
 class Cell(cell.CellTemplate):
     def update(self, state_matrix):
@@ -73,15 +72,15 @@
 
     @property
     def live_neighbors(self):
         return sum(self.neighbors)
 ```
 
 This module is then imported and passed to the Board class, which
-provides the user interface. 
+provides the user interface.
 
 ```python
 import tomato as tt
 from tomato.functions import utils
 
 from my_rules import game_of_life as rule
```

### Comparing `tomato-engine-1.8.2/src/tomato_engine.egg-info/SOURCES.txt` & `tomato-engine-1.8.3/src/tomato_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

