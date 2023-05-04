# Comparing `tmp/phamclust-0.1.3.tar.gz` & `tmp/phamclust-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phamclust-0.1.3.tar", last modified: Wed Sep 14 18:22:10 2022, max compression
+gzip compressed data, was "phamclust-1.0.0.tar", last modified: Thu May  4 20:55:41 2023, max compression
```

## Comparing `phamclust-0.1.3.tar` & `phamclust-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-09-14 18:22:10.505993 phamclust-0.1.3/
--rw-r--r--   0 christian   (501) staff       (20)    35148 2022-09-14 18:16:15.000000 phamclust-0.1.3/LICENSE
--rw-r--r--   0 christian   (501) staff       (20)      949 2022-09-14 18:22:10.506063 phamclust-0.1.3/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)       41 2022-09-14 18:16:15.000000 phamclust-0.1.3/README.md
--rw-r--r--   0 christian   (501) staff       (20)       89 2022-09-14 18:16:15.000000 phamclust-0.1.3/pyproject.toml
--rw-r--r--   0 christian   (501) staff       (20)     1097 2022-09-14 18:22:10.506424 phamclust-0.1.3/setup.cfg
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-09-14 18:22:10.502995 phamclust-0.1.3/src/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-09-14 18:22:10.505186 phamclust-0.1.3/src/phamclust/
--rw-r--r--   0 christian   (501) staff       (20)     4043 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/Genome.py
--rw-r--r--   0 christian   (501) staff       (20)     9322 2022-09-14 18:19:41.000000 phamclust-0.1.3/src/phamclust/SymMatrix.py
--rw-r--r--   0 christian   (501) staff       (20)        0 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     5352 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/__main__.py
--rw-r--r--   0 christian   (501) staff       (20)     3447 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/clustering.py
--rw-r--r--   0 christian   (501) staff       (20)     2168 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/multiprocess.py
--rw-r--r--   0 christian   (501) staff       (20)     2496 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/similarity.py
--rw-r--r--   0 christian   (501) staff       (20)     2030 2022-09-14 18:16:15.000000 phamclust-0.1.3/src/phamclust/statistics.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-09-14 18:22:10.505879 phamclust-0.1.3/src/phamclust.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      949 2022-09-14 18:22:10.000000 phamclust-0.1.3/src/phamclust.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)      447 2022-09-14 18:22:10.000000 phamclust-0.1.3/src/phamclust.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2022-09-14 18:22:10.000000 phamclust-0.1.3/src/phamclust.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       54 2022-09-14 18:22:10.000000 phamclust-0.1.3/src/phamclust.egg-info/entry_points.txt
--rw-r--r--   0 christian   (501) staff       (20)       10 2022-09-14 18:22:10.000000 phamclust-0.1.3/src/phamclust.egg-info/top_level.txt
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.780450 phamclust-1.0.0/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2023-05-04 20:48:38.000000 phamclust-1.0.0/LICENSE
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1051 2023-05-04 20:55:41.780557 phamclust-1.0.0/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)       41 2023-05-04 20:48:38.000000 phamclust-1.0.0/README.md
+-rw-r--r--   0 cgauthier   (501) staff       (20)       89 2023-05-04 20:48:38.000000 phamclust-1.0.0/pyproject.toml
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1178 2023-05-04 20:55:41.781096 phamclust-1.0.0/setup.cfg
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.774297 phamclust-1.0.0/src/
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.778957 phamclust-1.0.0/src/phamclust/
+-rw-r--r--   0 cgauthier   (501) staff       (20)       69 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)    16864 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/__main__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     3888 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/blastn.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     5805 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/cli.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1900 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/clustering.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/fasta.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6745 2023-05-04 20:51:42.000000 phamclust-1.0.0/src/phamclust/genome.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2130 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/heatmap.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)    22884 2023-05-04 20:50:58.000000 phamclust-1.0.0/src/phamclust/matrix.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/metrics.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2168 2023-05-04 20:48:38.000000 phamclust-1.0.0/src/phamclust/multiprocess.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/parallel_process.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2496 2023-05-04 20:48:38.000000 phamclust-1.0.0/src/phamclust/similarity.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/statistics.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.780259 phamclust-1.0.0/src/phamclust.egg-info/
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1051 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)      596 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/SOURCES.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)        1 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/dependency_links.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       54 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/entry_points.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       10 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/top_level.txt
```

### Comparing `phamclust-0.1.3/LICENSE` & `phamclust-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phamclust-0.1.3/PKG-INFO` & `phamclust-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 0.1.3
+Version: 1.0.0
 Summary: Cluster genomes based on gene phamily data
-Home-page: https://github.com/chg60/PhamClust
+Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
-Project-URL: Source, https://github.com/chg60/PhamClust
+Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phamclust
 Pham-based genome clustering
```

### Comparing `phamclust-0.1.3/setup.cfg` & `phamclust-1.0.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 name = phamclust
-version = 0.1.3
+version = 1.0.0
 author = Christian Gauthier
 author_email = chg60@pitt.edu
 description = Cluster genomes based on gene phamily data
 long_description = file:README.md
 long_description_content_type = text/markdown
-url = https://github.com/chg60/PhamClust
+url = https://github.com/chg60/phamclust
 project_urls = 
-	Source = https://github.com/chg60/PhamClust
+	Source = https://github.com/chg60/phamclust
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: MacOS
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find:
 install_requires =
```

### Comparing `phamclust-0.1.3/src/phamclust/multiprocess.py` & `phamclust-1.0.0/src/phamclust/multiprocess.py`

 * *Files identical despite different names*

### Comparing `phamclust-0.1.3/src/phamclust/similarity.py` & `phamclust-1.0.0/src/phamclust/similarity.py`

 * *Files identical despite different names*

### Comparing `phamclust-0.1.3/src/phamclust.egg-info/PKG-INFO` & `phamclust-1.0.0/src/phamclust.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 0.1.3
+Version: 1.0.0
 Summary: Cluster genomes based on gene phamily data
-Home-page: https://github.com/chg60/PhamClust
+Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
-Project-URL: Source, https://github.com/chg60/PhamClust
+Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phamclust
 Pham-based genome clustering
```

