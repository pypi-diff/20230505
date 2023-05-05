# Comparing `tmp/musegan-0.0.2.tar.gz` & `tmp/musegan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.0.2.tar", last modified: Fri May  5 06:26:47 2023, max compression
+gzip compressed data, was "musegan-0.0.3.tar", last modified: Fri May  5 06:50:33 2023, max compression
```

## Comparing `musegan-0.0.2.tar` & `musegan-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:26:47.808422 musegan-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      884 2023-05-05 06:26:47.808422 musegan-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-04-26 09:44:28.000000 musegan-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:26:47.792701 musegan-0.0.2/musegan/
--rw-rw-rw-   0        0        0      382 2023-04-26 07:08:57.000000 musegan-0.0.2/musegan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:26:47.808422 musegan-0.0.2/musegan.egg-info/
--rw-rw-rw-   0        0        0      884 2023-05-05 06:26:47.000000 musegan-0.0.2/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-05 06:26:47.000000 musegan-0.0.2/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:26:47.000000 musegan-0.0.2/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-05 06:26:47.000000 musegan-0.0.2/musegan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 06:26:47.000000 musegan-0.0.2/musegan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-05 06:26:47.808422 musegan-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1797 2023-05-05 06:26:13.000000 musegan-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:50:33.615162 musegan-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      884 2023-05-05 06:50:33.616159 musegan-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-04-26 09:44:28.000000 musegan-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:50:33.606424 musegan-0.0.3/musegan/
+-rw-rw-rw-   0        0        0      382 2023-04-26 07:08:57.000000 musegan-0.0.3/musegan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:50:33.614157 musegan-0.0.3/musegan.egg-info/
+-rw-rw-rw-   0        0        0      884 2023-05-05 06:50:32.000000 musegan-0.0.3/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-05 06:50:33.000000 musegan-0.0.3/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:50:32.000000 musegan-0.0.3/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 06:50:33.000000 musegan-0.0.3/musegan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 06:50:33.000000 musegan-0.0.3/musegan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-05 06:50:33.617671 musegan-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-05 06:48:53.000000 musegan-0.0.3/setup.py
```

### Comparing `musegan-0.0.2/LICENSE` & `musegan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.0.2/PKG-INFO` & `musegan-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytorch implimentation of musegan by https://github.com/salu133445
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz
 Author: cliffordkleinsr
 Author-email: cnjoroge925@gmail.com
 License: MIT
 Keywords: pytorch,music,generative adverserial networks
```

### Comparing `musegan-0.0.2/README.md` & `musegan-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `musegan-0.0.2/musegan.egg-info/PKG-INFO` & `musegan-0.0.3/musegan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytorch implimentation of musegan by https://github.com/salu133445
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz
 Author: cliffordkleinsr
 Author-email: cnjoroge925@gmail.com
 License: MIT
 Keywords: pytorch,music,generative adverserial networks
```

### Comparing `musegan-0.0.2/setup.py` & `musegan-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'musegan',         # How you named your package folder (MyLib)
   packages = ['musegan'],   # Chose the same as "name"
-  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  version = '0.0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A pytorch implimentation of musegan by https://github.com/salu133445',   # Give a short description about your library
   author = 'cliffordkleinsr',                   # Type in your name
   author_email = 'cnjoroge925@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/cliffordkleinsr/musegan-pytorch',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz',    # I explain this later on
   keywords = ['pytorch', 'music', 'generative adverserial networks'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'music21',
-          'SharedArray',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

