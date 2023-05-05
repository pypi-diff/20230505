# Comparing `tmp/trackplot-0.2.2.tar.gz` & `tmp/trackplot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.2.tar", last modified: Fri May  5 02:17:30 2023, max compression
+gzip compressed data, was "trackplot-0.2.3.tar", last modified: Fri May  5 05:00:06 2023, max compression
```

## Comparing `trackplot-0.2.2.tar` & `trackplot-0.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.483409 trackplot-0.2.2/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.2/LICENSE
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6781 2023-05-05 02:17:30.483153 trackplot-0.2.2/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.2/Pipfile
--rw-r--r--   0 zhangyiming   (501) staff       (20)    95508 2023-05-05 02:05:45.000000 trackplot-0.2.2/Pipfile.lock
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6595 2023-03-05 02:34:19.000000 trackplot-0.2.2/README.md
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1135 2023-05-04 09:50:39.000000 trackplot-0.2.2/pyproject.toml
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-05-05 02:17:30.483490 trackplot-0.2.2/setup.cfg
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-05-05 02:09:30.000000 trackplot-0.2.2/setup.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.472984 trackplot-0.2.2/trackplot/
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/__init__.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.475731 trackplot-0.2.2/trackplot/anno/
--rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/anno/AxLabel.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/anno/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/anno/theme.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.478433 trackplot-0.2.2/trackplot/base/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/CoordinateMap.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.2/trackplot/base/GenomicLoci.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/Protein.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8074 2023-05-04 09:29:01.000000 trackplot-0.2.2/trackplot/base/ReadDepth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.2/trackplot/base/Readder.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/Stroke.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/Transcript.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/base/pyUniprot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-05-04 09:50:39.000000 trackplot-0.2.2/trackplot/cli.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.479505 trackplot-0.2.2/trackplot/conf/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/conf/DomainSetting.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/conf/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/conf/config.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/conf/drawing.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.482872 trackplot-0.2.2/trackplot/file/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.2/trackplot/file/ATAC.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.2/trackplot/file/Bam.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/BedGraph.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/Bigwig.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/Depth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/Fasta.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.2/trackplot/file/File.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.2/trackplot/file/Motif.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.2/trackplot/file/ReadSegments.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    21780 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/Reference.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/file/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    45287 2023-02-25 16:01:18.000000 trackplot-0.2.2/trackplot/plot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.2/trackplot/plot_func.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.2/trackplot/plot_tests.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 02:17:30.474983 trackplot-0.2.2/trackplot.egg-info/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6781 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/entry_points.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 01:34:01.000000 trackplot-0.2.2/trackplot.egg-info/not-zip-safe
--rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/requires.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-05-05 02:17:30.000000 trackplot-0.2.2/trackplot.egg-info/top_level.txt
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.853056 trackplot-0.2.3/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.3/LICENSE
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-05 05:00:06.852759 trackplot-0.2.3/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.3/Pipfile
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    95508 2023-05-05 02:05:45.000000 trackplot-0.2.3/Pipfile.lock
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6521 2023-05-05 03:12:18.000000 trackplot-0.2.3/README.md
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1135 2023-05-04 09:50:39.000000 trackplot-0.2.3/pyproject.toml
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-05-05 05:00:06.853149 trackplot-0.2.3/setup.cfg
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-05-05 04:58:29.000000 trackplot-0.2.3/setup.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.836518 trackplot-0.2.3/trackplot/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/__init__.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.840298 trackplot-0.2.3/trackplot/anno/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/AxLabel.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/theme.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.844079 trackplot-0.2.3/trackplot/base/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/CoordinateMap.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.3/trackplot/base/GenomicLoci.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Protein.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8274 2023-05-05 03:48:03.000000 trackplot-0.2.3/trackplot/base/ReadDepth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.3/trackplot/base/Readder.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Stroke.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Transcript.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/pyUniprot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-05-05 04:58:29.000000 trackplot-0.2.3/trackplot/cli.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.845806 trackplot-0.2.3/trackplot/conf/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/DomainSetting.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/config.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/drawing.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.852406 trackplot-0.2.3/trackplot/file/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.3/trackplot/file/ATAC.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.3/trackplot/file/Bam.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/BedGraph.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Bigwig.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Depth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Fasta.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.3/trackplot/file/File.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.3/trackplot/file/Motif.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.3/trackplot/file/ReadSegments.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.3/trackplot/file/Reference.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    45287 2023-02-25 16:01:18.000000 trackplot-0.2.3/trackplot/plot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.3/trackplot/plot_func.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/plot_tests.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.839065 trackplot-0.2.3/trackplot.egg-info/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/entry_points.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 01:34:01.000000 trackplot-0.2.3/trackplot.egg-info/not-zip-safe
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/requires.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/top_level.txt
```

### Comparing `trackplot-0.2.2/LICENSE` & `trackplot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/PKG-INFO` & `trackplot-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
 
@@ -207,9 +207,9 @@
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
 If you use Sashimi.py in your publication, please cite Sashimi.py by
 
-[Zhang et al. Sashimi.py: a flexible toolkit for combinatorial analysis of genomic data. bioRxiv 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
+[Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.2/Pipfile.lock` & `trackplot-0.2.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/README.md` & `trackplot-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -199,9 +199,9 @@
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
 If you use Sashimi.py in your publication, please cite Sashimi.py by
 
-[Zhang et al. Sashimi.py: a flexible toolkit for combinatorial analysis of genomic data. bioRxiv 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
+[Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.2/pyproject.toml` & `trackplot-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/setup.py` & `trackplot-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from configparser import ConfigParser
 from setuptools import setup, find_packages
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def locate_packages():
     __dir__ = os.path.dirname(os.path.abspath(__file__))
     pipfile = os.path.join(__dir__, "Pipfile")
```

### Comparing `trackplot-0.2.2/trackplot/anno/theme.py` & `trackplot-0.2.3/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/CoordinateMap.py` & `trackplot-0.2.3/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/GenomicLoci.py` & `trackplot-0.2.3/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/Junction.py` & `trackplot-0.2.3/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/Protein.py` & `trackplot-0.2.3/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/ReadDepth.py` & `trackplot-0.2.3/trackplot/base/ReadDepth.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,23 @@
         self.site_plus = site_plus
         self.site_minus = site_minus * -1 if site_minus is not None else site_minus
 
         self._number_of_merged_ = 1
 
     @property
     def plus(self) -> Optional[np.array]:
-        return self._plus_ / self._number_of_merged_
+        if self._plus_ is not None and self._number_of_merged_ > 0:
+            return self._plus_ / self._number_of_merged_
+        return self._plus_
 
     @property
     def minus(self) -> Optional[np.array]:
-        return self._minus_ / self._number_of_merged_
+        if self._minus_ is not None and self._number_of_merged_ > 0:
+            return self._minus_ / self._number_of_merged_
+        return self._minus_
 
     @property
     def wiggle(self) -> np.array:
         if (self._plus_ is None or not self._plus_.any()) and self._minus_ is not None:
             return self.minus
 
         if self._plus_ is not None and self._minus_ is not None:
```

### Comparing `trackplot-0.2.2/trackplot/base/Readder.py` & `trackplot-0.2.3/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/Stroke.py` & `trackplot-0.2.3/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/Transcript.py` & `trackplot-0.2.3/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/base/pyUniprot.py` & `trackplot-0.2.3/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/cli.py` & `trackplot-0.2.3/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
 from trackplot.plot import Plot
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def decode_region(region: str):
     regions = region.split(":")
```

### Comparing `trackplot-0.2.2/trackplot/conf/DomainSetting.py` & `trackplot-0.2.3/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/conf/config.py` & `trackplot-0.2.3/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/conf/drawing.py` & `trackplot-0.2.3/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/ATAC.py` & `trackplot-0.2.3/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Bam.py` & `trackplot-0.2.3/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/BedGraph.py` & `trackplot-0.2.3/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Bigwig.py` & `trackplot-0.2.3/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Depth.py` & `trackplot-0.2.3/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Fasta.py` & `trackplot-0.2.3/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/File.py` & `trackplot-0.2.3/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.3/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Junction.py` & `trackplot-0.2.3/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Motif.py` & `trackplot-0.2.3/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/ReadSegments.py` & `trackplot-0.2.3/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/file/Reference.py` & `trackplot-0.2.3/trackplot/file/Reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,26 +331,22 @@
                 pysam.tabix_index(
                     output_gtf,
                     preset="gff",
                     force=True,
                     keep_original=True
                 )
             except OSError as err:
-                logger.error(err)
-                logger.error("Guess gtf needs to be sorted")
+                logger.warning(f"Guess gtf needs to be sorted: {err}")
 
                 sorted_gtf = re.sub(r"\.gtf(.gz)?$", "", input_gtf) + ".sorted.gtf.gz"
                 if os.path.exists(sorted_gtf) and os.path.exists(sorted_gtf + ".tbi"):
                     return sorted_gtf
 
                 cls.sort_gtf(input_gtf, sorted_gtf)
-                pysam.tabix_index(
-                    sorted_gtf, preset="gff",
-                    force=True, keep_original=True
-                )
+                pysam.tabix_index(sorted_gtf, preset="gff", force=True, keep_original=True)
                 return sorted_gtf
         elif os.path.getctime(output_gtf) < os.path.getctime(output_gtf):
             logger.info("the tbi index is older than the gtf file")
 
         return output_gtf
 
     def __load_gtf__(self, region: GenomicLoci) -> List[Transcript]:
@@ -438,19 +434,17 @@
                     start=read.reference_start + 1 if read.reference_start + 1 > region.start else region.start,
                     end=read.reference_end + 1 if read.reference_end + 1 < region.end else region.end,
                     strand=strand,
                     exons=exons_in_read
                 )
                 transcripts[t] = transcripts.get(t, 0) + 1
         except IOError as err:
-            logger.error('There is no .bam file at {0}'.format(self.path))
-            logger.error(err)
+            logger.warning(f"There is no .bam file at {self.path}: {err}")
         except ValueError as err:
-            logger.error(self.path)
-            logger.error(err)
+            logger.warning(f"{self.path}: {err}")
 
         return sorted([x for x, y in transcripts.items() if y > threshold_of_reads])
 
     def __load_bed__(self, region: GenomicLoci) -> List[Transcript]:
         transcripts = []
         try:
             for rec in Reader.read_gtf(self.path, region=region, bed=True):
@@ -498,19 +492,17 @@
                 )
                 if read.start < self.region.start or read.end > self.region.end:
                     continue
 
                 transcripts.append(read)
 
         except IOError as err:
-            logger.error('There is no .bed file at {0}'.format(self.path))
-            logger.error(err)
+            logger.warning(f"There is no .bed file at {self.path}: {err}")
         except ValueError as err:
-            logger.error(self.path)
-            logger.error(err)
+            logger.warning(f"{self.path}: {err}")
         return transcripts
 
     def load(self, region: GenomicLoci, threshold_of_reads: int = 0, **kwargs):
         u"""
         Load transcripts inside of region
         :param region: target region
         :param threshold_of_reads: used for bam file, only kept reads with minimum frequency
```

### Comparing `trackplot-0.2.2/trackplot/plot.py` & `trackplot-0.2.3/trackplot/plot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/plot_func.py` & `trackplot-0.2.3/trackplot/plot_func.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot/plot_tests.py` & `trackplot-0.2.3/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.2/trackplot.egg-info/PKG-INFO` & `trackplot-0.2.3/trackplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
 
@@ -207,9 +207,9 @@
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
 If you use Sashimi.py in your publication, please cite Sashimi.py by
 
-[Zhang et al. Sashimi.py: a flexible toolkit for combinatorial analysis of genomic data. bioRxiv 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
+[Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.2/trackplot.egg-info/SOURCES.txt` & `trackplot-0.2.3/trackplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

