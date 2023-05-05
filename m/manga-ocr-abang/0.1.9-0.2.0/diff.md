# Comparing `tmp/manga-ocr-abang-0.1.9.tar.gz` & `tmp/manga-ocr-abang-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga-ocr-abang-0.1.9.tar", last modified: Wed May  3 09:16:53 2023, max compression
+gzip compressed data, was "manga-ocr-abang-0.2.0.tar", last modified: Fri May  5 04:38:11 2023, max compression
```

## Comparing `manga-ocr-abang-0.1.9.tar` & `manga-ocr-abang-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.572686 manga-ocr-abang-0.1.9/
--rw-rw-rw-   0        0        0    11558 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       28 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      570 2023-05-03 09:16:53.572686 manga-ocr-abang-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.552620 manga-ocr-abang-0.1.9/assets/
--rw-rw-rw-   0        0        0    56623 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/assets/example.jpg
-drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.555974 manga-ocr-abang-0.1.9/manga_ocr/
--rw-rw-rw-   0        0        0       61 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/__init__.py
--rw-rw-rw-   0        0        0      127 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/__main__.py
--rw-rw-rw-   0        0        0     2161 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/ocr.py
--rw-rw-rw-   0        0        0     3947 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.569686 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/
--rw-rw-rw-   0        0        0      570 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:16:53.573751 manga-ocr-abang-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1068 2023-05-03 09:16:45.000000 manga-ocr-abang-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.570685 manga-ocr-abang-0.1.9/tests/
--rw-rw-rw-   0        0        0      424 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/tests/test_ocr.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:38:11.274497 manga-ocr-abang-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1788 2023-05-05 04:38:11.273193 manga-ocr-abang-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6558 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 04:38:11.246385 manga-ocr-abang-0.2.0/assets/
+-rw-rw-rw-   0        0        0    56623 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/assets/example.jpg
+drwxrwxrwx   0        0        0        0 2023-05-05 04:38:11.250385 manga-ocr-abang-0.2.0/manga_ocr/
+-rw-rw-rw-   0        0        0       61 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/manga_ocr/__init__.py
+-rw-rw-rw-   0        0        0      127 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/manga_ocr/__main__.py
+-rw-rw-rw-   0        0        0     2161 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/manga_ocr/ocr.py
+-rw-rw-rw-   0        0        0     3947 2023-05-05 04:21:36.000000 manga-ocr-abang-0.2.0/manga_ocr/run.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:38:11.271773 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/
+-rw-rw-rw-   0        0        0     1788 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 04:38:11.000000 manga-ocr-abang-0.2.0/manga_ocr_abang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 04:38:11.274497 manga-ocr-abang-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-05-05 04:24:12.000000 manga-ocr-abang-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:38:11.273193 manga-ocr-abang-0.2.0/tests/
+-rw-rw-rw-   0        0        0      424 2023-05-05 04:20:54.000000 manga-ocr-abang-0.2.0/tests/test_ocr.py
```

### Comparing `manga-ocr-abang-0.1.9/LICENSE` & `manga-ocr-abang-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.9/assets/example.jpg` & `manga-ocr-abang-0.2.0/assets/example.jpg`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.9/manga_ocr/ocr.py` & `manga-ocr-abang-0.2.0/manga_ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.9/manga_ocr/run.py` & `manga-ocr-abang-0.2.0/manga_ocr/run.py`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.9/setup.py` & `manga-ocr-abang-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="manga-ocr-abang",
-    version='0.1.9',
+    version='0.2.0',
     description="OCR for Japanese manga",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AbangTanYiHan/manga-ocr-abang",
-    author="Maciej Budyś",
+    author="Abang",
     author_email="shinichiconan1997@gmail.com",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=['manga_ocr'],
     include_package_data=True,
@@ -29,11 +29,11 @@
         "sentencepiece",
         "torch>=1.0",
         "transformers>=4.12.5",
         "unidic_lite",
     ],
     entry_points={
         "console_scripts": [
-            "manga_ocr_abang=manga_ocr.__main__:main",
+            "manga_ocr=manga_ocr.__main__:main",
         ]
     },
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

