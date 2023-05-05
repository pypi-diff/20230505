# Comparing `tmp/textbook_nvim-0.2.0.tar.gz` & `tmp/textbook_nvim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbook_nvim-0.2.0.tar", last modified: Fri May  5 05:38:26 2023, max compression
+gzip compressed data, was "textbook_nvim-0.3.0.tar", last modified: Fri May  5 05:40:06 2023, max compression
```

## Comparing `textbook_nvim-0.2.0.tar` & `textbook_nvim-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.2.0/LICENSE
--rw-r--r--   0        0        0     3666 2023-05-05 05:38:10.293987 textbook_nvim-0.2.0/README.md
--rw-r--r--   0        0        0  2231045 2023-05-05 05:38:04.657243 textbook_nvim-0.2.0/docs/example1.gif
--rw-r--r--   0        0        0      517 2023-05-05 05:38:10.293987 textbook_nvim-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6826 2023-05-05 05:38:10.293987 textbook_nvim-0.2.0/rplugin/python3/textbook.py
--rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.2.0/src/textbook_nvim/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-03 19:13:19.864580 textbook_nvim-0.2.0/src/textbook_nvim/cli.py
--rw-r--r--   0        0        0     1714 2023-05-03 19:13:19.867914 textbook_nvim-0.2.0/src/textbook_nvim/parser.py
--rw-r--r--   0        0        0     4656 2023-05-05 05:38:04.657243 textbook_nvim-0.2.0/src/textbook_nvim/render.py
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 textbook_nvim-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3734 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/README.md
+-rw-r--r--   0        0        0      517 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6826 2023-05-05 05:38:10.293987 textbook_nvim-0.3.0/rplugin/python3/textbook.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/src/textbook_nvim/__init__.py
+-rw-r--r--   0        0        0     1247 2023-05-03 19:13:19.864580 textbook_nvim-0.3.0/src/textbook_nvim/cli.py
+-rw-r--r--   0        0        0     1714 2023-05-03 19:13:19.867914 textbook_nvim-0.3.0/src/textbook_nvim/parser.py
+-rw-r--r--   0        0        0     6966 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/src/textbook_nvim/render.py
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 textbook_nvim-0.3.0/PKG-INFO
```

### Comparing `textbook_nvim-0.2.0/LICENSE` & `textbook_nvim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.2.0/README.md` & `textbook_nvim-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 # textbook.nvim
 
-This plugin allows management and rendering of `jupyter` notebooks inside of `neovim` through `jupytext` format and `rich` components.
+This plugin allows management and rendering of `jupyter` notebooks inside of `neovim` through the `jupytext` format and `rich` components.
 
-![example1](docs/example1.gif)
+Click on the following image to see a demo:
+
+[![Alt text](https://img.youtube.com/vi/mC8kZa93uhg/0.jpg)](https://www.youtube.com/watch?v=mC8kZa93uhg)
 
 ## Installation
 
-You'll have to install some utilities and dependencies through `pip`:
+You'll need to install some utilities and dependencies through `pip`:
 
 ```sh
 pip install textbook_nvim
 ```
 
-Then you can install the plugin, for instance, with `packer`:
+After that, you can install the plugin using `packer`, for instance:
 
 ```lua
 use {"juselara1/textbook.nvim", run = ":UpdateRemotePlugins"}
 ```
 
 ## Usage
 
-The idea of `textbook` is to offer a non-intrusive way to edit notebook files defined as plain text. By default it uses the percent format as a cell separator but you can define a regex to parse any kind of format.
+The idea behind `textbook` is to offer a non-intrusive way to edit notebook files defined as plain text. By default, it uses the percent format as a cell separator, but you can define a regex to parse any kind of format.
 
-For instance, the following text defines python notebook:
+For instance, the following text defines a Python notebook:
 
 ```python
 # %% [markdown]
 # Markdown code...
 
 # %% [raw]
-print("hello world")
+print("Hello, world!")
 ```
 
-Where `# %% [markdown]` represents a markdown cell and `# %% [raw]` a code cell. To render this file you should run the following command to specify the current buffer as the source:
+To render this file, you should run the following command to specify the current buffer as the source:
 
 ```vim
 :TextBookBuffer
 ```
 
-Then you should open the render view:
+Then, you should open the render view:
 
 ```vim
 :TextBookOpen
 ```
 
-This will spawn a new buffer with the rendered text, there you have the following options:
+This will spawn a new buffer with the rendered text. There, you will have the following options:
 
 - `:TextBookSync`: syncs the cursor position in the same cell as the plain text file.
-- `:TextBookSelectCell [cell_id]`: when no arguments are passed selects the cell under the cursor, otherwise, selects the cell of the `cell_id`.
+- `:TextBookSelectCell [cell_id]`: when no arguments are passed, selects the cell under the cursor. Otherwise, selects the cell of the `cell_id`.
 - `:TextBookNextCell`: selects the next cell.
 - `:TextBookPrevCell`: selects the previous cell.
 - `:TextBookAddCell cell_type after`: creates a cell of type `cell_type` (`raw` or `markdown`) and can be before (`0`) or after (`1`) the cell under the cursor.
 - `:TextBookConfig`: reloads the configuration.
 - `:TextBookClose`: closes the rendered view and places the cursor in the same cell as the rendered view.
 
 ## Configuration
@@ -75,15 +77,15 @@
     {bind="<Leader>to", command=":TextBookOpen<CR>"},
     {bind="<Leader>tr", command=":TextBookSync<CR>"},
     {bind="<Leader>ti", command=":TextBookBuffer<CR>"},
     {bind="<Leader>ts", command=":TextBookSelectCell<CR>"},
     {bind="<Leader>tg", command=":TextBookSelectCell"},
     {bind="<Leader>tj", command=":TextBookSelectNextCell<CR>"},
     {bind="<Leader>tk", command=":TextBookSelectPrevCell<CR>"},
-    {bind="<Leader>tc", command=":TextBookClose<CR>"},
+    {bind="<Leader>tq", command=":TextBookClose<CR>"},
     {bind="<Leader>tma", command=":TextBookAddCell markdown 1<CR>"},
     {bind="<Leader>tmb", command=":TextBookAddCell markdown 0<CR>"},
     {bind="<Leader>tra", command=":TextBookAddCell raw 1<CR>"},
     {bind="<Leader>trb", command=":TextBookAddCell raw 0<CR>"},
 }
 
 for _, value in ipairs(binds) do
```

### Comparing `textbook_nvim-0.2.0/pyproject.toml` & `textbook_nvim-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textbook_nvim"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{name = "Juan Lara", email = "julara@unal.edu.co"}]
 description = "Main python package for the textbook.nvim plugin."
 requires-python = ">3.8"
 dependencies = [
     "pydantic", "pynvim", "rich", "click"
 ]
```

### Comparing `textbook_nvim-0.2.0/rplugin/python3/textbook.py` & `textbook_nvim-0.3.0/rplugin/python3/textbook.py`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.2.0/src/textbook_nvim/cli.py` & `textbook_nvim-0.3.0/src/textbook_nvim/cli.py`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.2.0/src/textbook_nvim/parser.py` & `textbook_nvim-0.3.0/src/textbook_nvim/parser.py`

 * *Files identical despite different names*

