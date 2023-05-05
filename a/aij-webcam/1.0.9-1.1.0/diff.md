# Comparing `tmp/aij-webcam-1.0.9.tar.gz` & `tmp/aij-webcam-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.9.tar", last modified: Thu May  4 10:33:33 2023, max compression
+gzip compressed data, was "aij-webcam-1.1.0.tar", last modified: Fri May  5 12:43:14 2023, max compression
```

## Comparing `aij-webcam-1.0.9.tar` & `aij-webcam-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.9/README.md
--rw-rw-rw-   0        0        0     6452 2023-05-04 10:33:22.000000 aij-webcam-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/webcam/
--rw-rw-rw-   0        0        0    12217 2023-05-04 10:33:32.000000 aij-webcam-1.0.9/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.0/README.md
+-rw-rw-rw-   0        0        0     6368 2023-05-05 12:43:00.000000 aij-webcam-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      175 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 12:43:14.000000 aij-webcam-1.1.0/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.0/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.0/src/news/core.py
+-rw-rw-rw-   0        0        0     3322 2023-05-05 12:17:00.000000 aij-webcam-1.1.0/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.0/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:43:16.000000 aij-webcam-1.1.0/src/webcam/
+-rw-rw-rw-   0        0        0    16936 2023-05-05 12:22:56.000000 aij-webcam-1.1.0/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.9/LICENSE.txt` & `aij-webcam-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.9/PKG-INFO` & `aij-webcam-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.9/README.md` & `aij-webcam-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.9/pyproject.toml` & `aij-webcam-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.9"
+version = "1.1.0"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -95,35 +95,31 @@
 
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
-# import cv2
-# import mediapipe as mp
-# import pandas as pd
-# import threading
-# from gtts import gTTS
-# from pygame import mixer
 dependencies = [
     "requests",
     "setuptools",
     "wheel",
     "pipenv",
     "pylint",
     "autopep8",
     "pyinstaller",
     "pytest",
     "pytest-cov",
     "opencv-python",
     "mediapipe",
     "pandas",
     "gtts",
-    "pygame"
+    "pygame",
+    "cairosvg",
+    "pika"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
@@ -150,15 +146,16 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij-webcam"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-aij-webcam = "webcam:main"
+aijrun = "webcam:main"
+aijnews = "news:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-webcam-1.0.9/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.1.0/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

