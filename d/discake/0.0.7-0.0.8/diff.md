# Comparing `tmp/discake-0.0.7.tar.gz` & `tmp/discake-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discake-0.0.7.tar", last modified: Tue Apr 25 11:47:39 2023, max compression
+gzip compressed data, was "discake-0.0.8.tar", last modified: Fri May  5 07:49:01 2023, max compression
```

## Comparing `discake-0.0.7.tar` & `discake-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:47:39.621023 discake-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 11:47:27.000000 discake-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 11:47:39.621023 discake-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 11:47:27.000000 discake-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:47:39.617023 discake-0.0.7/discake/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 11:47:27.000000 discake-0.0.7/discake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:47:39.621023 discake-0.0.7/discake/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-25 11:47:27.000000 discake-0.0.7/discake/paginator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:47:39.621023 discake-0.0.7/discake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:47:27.000000 discake-0.0.7/discake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-25 11:47:27.000000 discake-0.0.7/discake/utils/paginate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:47:39.621023 discake-0.0.7/discake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 11:47:39.000000 discake-0.0.7/discake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 11:47:39.000000 discake-0.0.7/discake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:47:39.000000 discake-0.0.7/discake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 11:47:39.000000 discake-0.0.7/discake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 11:47:39.000000 discake-0.0.7/discake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:47:39.621023 discake-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-25 11:47:27.000000 discake-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 07:48:49.000000 discake-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 07:49:01.808116 discake-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-05 07:48:49.000000 discake-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 07:48:49.000000 discake-0.0.8/discake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-05 07:48:49.000000 discake-0.0.8/discake/paginator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 07:48:49.000000 discake-0.0.8/discake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-05 07:48:49.000000 discake-0.0.8/discake/utils/paginate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:49:01.808116 discake-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 07:48:49.000000 discake-0.0.8/setup.py
```

### Comparing `discake-0.0.7/LICENSE` & `discake-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `discake-0.0.7/PKG-INFO` & `discake-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.7
+Version: 0.0.8
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,19 +21,19 @@
 
 discake
 ==========
 
 .. image:: https://discord.com/api/guilds/815886477066108968/embed.png
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Discord server invite
-.. image:: https://img.shields.io/pypi/v/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/v/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/pyversions/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI supported Python versions
 
 A discord py util library.
 
 Key Features
 -------------
 
@@ -87,8 +87,16 @@
     
     
     client.run('TOKEN')
 
 Links
 ------
 
-- `Official Discord Server <https://discord.gg/egvmz5NjSZ>`_
+.. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Support Server
+
+Author
+------
+.. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Author Info
```

### Comparing `discake-0.0.7/README.rst` & `discake-0.0.8/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 discake
 ==========
 
 .. image:: https://discord.com/api/guilds/815886477066108968/embed.png
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Discord server invite
-.. image:: https://img.shields.io/pypi/v/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/v/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/pyversions/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI supported Python versions
 
 A discord py util library.
 
 Key Features
 -------------
 
@@ -66,8 +66,16 @@
     
     
     client.run('TOKEN')
 
 Links
 ------
 
-- `Official Discord Server <https://discord.gg/egvmz5NjSZ>`_
+.. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Support Server
+
+Author
+------
+.. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Author Info
```

### Comparing `discake-0.0.7/discake/paginator/__init__.py` & `discake-0.0.8/discake/paginator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from cgitb import grey
 
 from typing import TYPE_CHECKING, Literal, Union, List, Any, Optional
 
 from discord import Embed, Interaction
 from discord.ext.commands import Context
 
 from discake.utils import ButtonsView
@@ -58,14 +57,20 @@
         self._pages = []
         self._index = 0
         self.timeout = timeout
         self.color = color
         self.entries: Any = entries
     
     async def send(self, interaction: Union[Context, Interaction]):
+        """
+        Sends or starts the paginator
+
+        Attributes:
+        interaction (Union[Context, Interaction): The Interaction or Context to respond to.
+        """
         if not self.entries:
             raise AttributeError('You must provide atleast one entry or page for pagination.') 
             
         self.author = interaction.user if isinstance(interaction, Interaction) else interaction.author
         entries = self.entries
         for chunk in entries:
             self._pages.append(chunk)
```

### Comparing `discake-0.0.7/discake/utils/paginate.py` & `discake-0.0.8/discake/utils/paginate.py`

 * *Files identical despite different names*

### Comparing `discake-0.0.7/discake.egg-info/PKG-INFO` & `discake-0.0.8/discake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.7
+Version: 0.0.8
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,19 +21,19 @@
 
 discake
 ==========
 
 .. image:: https://discord.com/api/guilds/815886477066108968/embed.png
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Discord server invite
-.. image:: https://img.shields.io/pypi/v/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/v/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI version info
-.. image:: https://img.shields.io/pypi/pyversions/discord.py.svg
-   :target: https://pypi.python.org/pypi/discord.py
+.. image:: https://img.shields.io/pypi/pyversions/discake.svg
+   :target: https://pypi.python.org/pypi/discake
    :alt: PyPI supported Python versions
 
 A discord py util library.
 
 Key Features
 -------------
 
@@ -87,8 +87,16 @@
     
     
     client.run('TOKEN')
 
 Links
 ------
 
-- `Official Discord Server <https://discord.gg/egvmz5NjSZ>`_
+.. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Support Server
+
+Author
+------
+.. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
+   :target: https://discord.gg/egvmz5NjSZ
+   :alt: Author Info
```

### Comparing `discake-0.0.7/setup.py` & `discake-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.rst', 'r') as file:
     readme = file.read()
     
 setup(
     name='discake',
     author='Carlos',
     url='https://github.com/lollipop-69/discake',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     description='A discord py support library containing utilities.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     install_requires=[
         'discord.py'
     ],
```

