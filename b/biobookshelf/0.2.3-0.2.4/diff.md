# Comparing `tmp/biobookshelf-0.2.3.tar.gz` & `tmp/biobookshelf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobookshelf-0.2.3.tar", last modified: Tue May  2 03:15:45 2023, max compression
+gzip compressed data, was "biobookshelf-0.2.4.tar", last modified: Fri May  5 13:20:37 2023, max compression
```

## Comparing `biobookshelf-0.2.3.tar` & `biobookshelf-0.2.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/LICENSE
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/MANIFEST.in
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/README.md
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/BA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/BA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/BA/bitarray_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/CLI/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/CLI/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3012 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/CLI/unclassified_programs.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/INT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/INT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/INT/integer.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/IT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/IT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/IT/interval_tree_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/L/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/L/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/L/l_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/MAP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MAP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MAP/mapping.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/MP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MP/multiprocessing_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/ONT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ONT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    63568 2023-05-01 11:20:31.000000 biobookshelf-0.2.3/biobookshelf/ONT/nanopore_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PD/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PD/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PD/pd_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PDB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/PDB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29069 2023-05-01 11:20:31.000000 biobookshelf-0.2.3/biobookshelf/PDB/pdb.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PKG/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PKG/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3096 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PKG/package_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/RNA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/RNA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.3/biobookshelf/RNA/rnaseq.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SAM/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/SAM/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.3/biobookshelf/SAM/sam_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SC/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/SC/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122816 2023-05-01 11:20:34.000000 biobookshelf-0.2.3/biobookshelf/SC/single_cell.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SEQ/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/SEQ/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14816 2023-05-01 11:20:30.000000 biobookshelf-0.2.3/biobookshelf/SEQ/sequence.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/STR/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/STR/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/STR/string.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/UniProt/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/UniProt/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/UniProt/uniprot.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/WEB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/WEB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8722 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/WEB/web_application.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/ZA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ZA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ZA/zarr_utils.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/__main__.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/main/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.3/biobookshelf/main/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   711938 2023-05-01 11:21:08.000000 biobookshelf-0.2.3/biobookshelf/main/unclassified_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf.egg-info/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/SOURCES.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/dependency_links.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/entry_points.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/requires.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/top_level.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-02 03:15:45.434486 biobookshelf-0.2.3/setup.cfg
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/setup.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/LICENSE
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/MANIFEST.in
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/README.md
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.447940 biobookshelf-0.2.4/biobookshelf/
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.463940 biobookshelf-0.2.4/biobookshelf/BA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/BA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/BA/bitarray_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.479941 biobookshelf-0.2.4/biobookshelf/CLI/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/CLI/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3013 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/CLI/unclassified_programs.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.515941 biobookshelf-0.2.4/biobookshelf/INT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/INT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/INT/integer.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.543942 biobookshelf-0.2.4/biobookshelf/IT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/IT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/IT/interval_tree_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.551942 biobookshelf-0.2.4/biobookshelf/L/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/L/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/L/l_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.559942 biobookshelf-0.2.4/biobookshelf/MAP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MAP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MAP/mapping.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.591943 biobookshelf-0.2.4/biobookshelf/MP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MP/multiprocessing_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.595943 biobookshelf-0.2.4/biobookshelf/ONT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ONT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    66087 2023-05-05 08:17:52.000000 biobookshelf-0.2.4/biobookshelf/ONT/nanopore_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.615943 biobookshelf-0.2.4/biobookshelf/PD/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PD/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PD/pd_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.647944 biobookshelf-0.2.4/biobookshelf/PDB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/PDB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29100 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/PDB/pdb.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.667944 biobookshelf-0.2.4/biobookshelf/PKG/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PKG/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3095 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/PKG/package_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.683944 biobookshelf-0.2.4/biobookshelf/RNA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/RNA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.4/biobookshelf/RNA/rnaseq.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.727945 biobookshelf-0.2.4/biobookshelf/SAM/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/SAM/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.4/biobookshelf/SAM/sam_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.775946 biobookshelf-0.2.4/biobookshelf/SC/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/SC/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122849 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/SC/single_cell.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.799946 biobookshelf-0.2.4/biobookshelf/SEQ/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/SEQ/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14831 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/SEQ/sequence.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.835947 biobookshelf-0.2.4/biobookshelf/STR/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/STR/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/STR/string.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.867948 biobookshelf-0.2.4/biobookshelf/UniProt/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/UniProt/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/UniProt/uniprot.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.903948 biobookshelf-0.2.4/biobookshelf/WEB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/WEB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8727 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/WEB/web_application.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.947949 biobookshelf-0.2.4/biobookshelf/ZA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ZA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ZA/zarr_utils.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-05 13:19:35.000000 biobookshelf-0.2.4/biobookshelf/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/__main__.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.967949 biobookshelf-0.2.4/biobookshelf/main/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.4/biobookshelf/main/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   712244 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/main/unclassified_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.447940 biobookshelf-0.2.4/biobookshelf.egg-info/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/SOURCES.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/dependency_links.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/entry_points.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/requires.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/top_level.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/setup.cfg
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-05 13:19:26.000000 biobookshelf-0.2.4/setup.py
```

### Comparing `biobookshelf-0.2.3/LICENSE` & `biobookshelf-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/PKG-INFO` & `biobookshelf-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.3
+Version: 0.2.4
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.3/biobookshelf/BA/bitarray_utils.py` & `biobookshelf-0.2.4/biobookshelf/BA/bitarray_utils.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/CLI/unclassified_programs.py` & `biobookshelf-0.2.4/biobookshelf/CLI/unclassified_programs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from biobookshelf.main import *
 from biobookshelf import PKG
 
+
 # Command line programs
 def Recursively_stop_subprocesses(int_pid):
     if int_pid < 1e3:
         print(
             "ERROR: given PID {} has less than 4 digits. For security reasons, this program failed".format(
                 int_pid
             )
```

### Comparing `biobookshelf-0.2.3/biobookshelf/MAP/mapping.py` & `biobookshelf-0.2.4/biobookshelf/MAP/mapping.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/ONT/nanopore_functions.py` & `biobookshelf-0.2.4/biobookshelf/ONT/nanopore_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     flag_include_failed: bool = True,  # include the failed reads into the fastq output
     int_max_num_reads_for_drawing_size_distribution: int = 100000,  # the maximum number of reads to use to draw a size distribution
     int_max_size_for_displaying_size_distribution: int = 2000,  # max molecule length to display in the histogram
     int_num_bins_for_displaying_size_distribution: int = 200,  # number of bins for drawing histogram
     flag_require_barcodes_both_ends: bool = True,  # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
     flag_rerun_guppy=False,  # rename the the output folder (if it exists) and rerun guppy if the flag is True
 ):
-    """# 2023-04-22 23:54:01
+    """# 2023-05-05 17:16:59 
     l_path_folder_nanopore_sequencing_data : list, # list of folders containing nanopore sequencing data
     l_name_config : Union[ str, List ], # a name of config or a list of name_config
     l_barcoding_kit : Union[ str, List, None ], # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output : str, # a path to the output folder
     dict_name_bc_to_name_sample : Union[ dict, None ], # barcode to name_sample. if not given, exit after combining fastq files.
     dict_name_sample_to_organism : Union[ dict, None ], # define organism for each sample. if not given, does not align reads to genome and transcriptomes
     dict_anno : Union[ dict, None ], # a dictionary containing annotation information for each organism. if not given, does not align reads to genome and transcriptomes
@@ -272,15 +272,15 @@
     ]:
         os.makedirs(path_folder, exist_ok=True)
 
     # align reads
     import concurrent.futures
 
     l_task = []  # initialize the list of tasks
-    int_num_cpus_for_each_alignment = min(
+    int_num_cpus_for_each_alignment = max(
         1, int(int_num_cpus / int_num_samples / 2)
     )  # retrieve approximate number of cpus for each alignment
     for name_sample, path_file_fq in df_fastq.values:  # for each sample
         name_organism = dict_name_sample_to_organism[
             name_sample
         ]  # retrieve the name of the organism
         dict_anno_for_sample = dict_anno[
@@ -378,16 +378,16 @@
             l_l, columns=["gene_name", "length_of_read", "mapping_quality"]
         )
         df["gene_count"] = 1
         # calculate unaligned read count and base count
         int_read_count_unaligned = int_read_count - len(df)
         int_base_pair_count_unaligned = int_base_pair_count - df.length_of_read.sum()
 
-        # compose dataframe of genes
-        df = pd.DataFrame(
+        # compose dataframe of gene counts
+        df_count = pd.DataFrame(
             {
                 "gene_count": df[
                     [
                         "gene_name",
                         "gene_count",
                     ]
                 ]
@@ -407,32 +407,62 @@
                         "mapping_quality",
                     ]
                 ]
                 .groupby("gene_name")
                 .mean()["mapping_quality"],  # calculate 'average_mapping_quality'
             }
         )
-        df.loc["__unaligned_reads__"] = [
+        df_count.loc["__unaligned_reads__"] = [
             int_read_count_unaligned,
             int_base_pair_count_unaligned / int_read_count_unaligned,
             -1,
         ]  # add record of unaligned reads
-        df.sort_values(
+        df_count.sort_values(
             "gene_count", ascending=False, inplace=True
         )  # sort by gene_count
-
         # write result as files
-        df.to_excel(
+        df_count.to_excel(
             f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.xlsx"
         )  # output excel file
-        df.to_csv(
+        df_count.to_csv(
             f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.tsv.gz",
             sep="\t",
         )  # output tsv file
-
+        
+        # calculate accumulated sequencing throughput to determine library diversity
+        s_sequencing_throughput = df_count.gene_count * df_count.average_length_of_read # retrieve total number of base pairs for each entry
+        s_sequencing_throughput_proportion = ( s_sequencing_throughput / s_sequencing_throughput.sum( ) ).sort_values( ascending = False )
+        df_accumulated_throughput = pd.concat( [ 
+            pd.DataFrame( { 
+                'accumulated proportions of sequencing throughput' : [ 0 ], 
+                'number of covered genes' : [ 0 ], 
+                'proportion of sequencing throughput' : [ 0 ], 
+                'gene name' : [ '-' ]
+            } ),
+            pd.DataFrame( { 
+                'accumulated proportions of sequencing throughput' : np.cumsum( s_sequencing_throughput_proportion.values ), 
+                'number of covered genes' : np.arange( len( s_sequencing_throughput_proportion ) ) + 1, 
+                'proportion of sequencing throughput' : s_sequencing_throughput_proportion.values, 
+                'gene name' : s_sequencing_throughput_proportion.index.values
+            } ),
+        ] )
+        # write result as files
+        df_accumulated_throughput.to_excel(
+            f"{path_folder_processed_data}{name_sample}.(supplementary).accumulated_sequencing_throughput.gene_level.xlsx"
+        )  # output excel file
+        df_accumulated_throughput.to_csv(
+            f"{path_folder_processed_data}{name_sample}.(supplementary).accumulated_sequencing_throughput.gene_level.tsv.gz",
+            sep="\t",
+        )  # output tsv file
+        
+        # draw graph
+        float_area_under_the_curve = np.cumsum( s_sequencing_throughput_proportion.values ).mean( ) # calculate area under the curve, which indicates higher library diversity
+        fig = px.line( df_accumulated_throughput, y = 'accumulated proportions of sequencing throughput', x = 'number of covered genes', log_y = False, line_shape='vh', hover_data = [ 'gene name', 'proportion of sequencing throughput' ], title = f"Area Under the Curve (AUC) = {np.round( float_area_under_the_curve, 5 )}<br>(lower AUC indicates higher library diversity)" )
+        os.makedirs( f'{path_folder_graph}accumulated_sequencing_throughput/', exist_ok = True ) # create the output folder
+        fig.write_html( f'{path_folder_graph}accumulated_sequencing_throughput/{name_sample}.accumulated_sequencing_throughput.gene_level.html' ) # write the graph
 
 def Guppy_Run_and_Combine_Output(
     path_folder_nanopore_sequencing_data=None,
     flag_barcoding_was_used=False,
     path_folder_output_fastq=None,
     id_flowcell=None,
     id_lib_prep=None,
```

### Comparing `biobookshelf-0.2.3/biobookshelf/PDB/pdb.py` & `biobookshelf-0.2.4/biobookshelf/PDB/pdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pandas as pd
 from io import StringIO
 import collections  # for external function
 from copy import deepcopy
 
+
 # import internal functions
 def PD_Select(df, deselect=False, **dict_select):
     """Select and filter rows of df according to the given dict_select. If 'deselect' is set to True, deselect rows according to the given dict_select  Usage example : PANDAS_Select( df_meta_imid_ubi, dict(  Data_Type = [ 'Proteome', 'Ubi_Profiling' ], Value_Type = 'log2fc' ) )"""
     for col, query in dict_select.items():
         if type(df) is pd.Series:
             data_values = (
                 df.index.values if col == "index" else df.values
@@ -52,15 +53,16 @@
     duplicate_filter=2,
     dropna=True,
     sort_series_by_values=True,
     convert_tuple_to_string=False,
 ):
     """
     # 20210224
-    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more."""
+    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more.
+    """
     if dropna and isinstance(iterable, pd.Series):
         iterable = (
             iterable.dropna()
         )  # if dropna is set to 'True', dropn NaN values before counting
     if isinstance(next(iterable.__iter__()), (np.ndarray, list)):
         iterable = list(
             map(tuple, iterable)
@@ -170,15 +172,16 @@
 
 
 # In[4]:
 
 
 def Parse_ATOM_or_HETATM_line(line):
     """# 2021-04-27 11:12:31
-    parse a given line (should be ATOM or HETATM records) and return parsed data values as a numpy array (dtype = object) Parse only until xyz coordinates (because later columns are somewhat variable across different docking servers)"""
+    parse a given line (should be ATOM or HETATM records) and return parsed data values as a numpy array (dtype = object) Parse only until xyz coordinates (because later columns are somewhat variable across different docking servers)
+    """
     # parse optional fields based on the length of the entry
     value = "" if len(line) < 60 else line[54:60].strip()
     float_occupancy = np.nan if len(value) == 0 else float(value)
     value = "" if len(line) < 66 else line[60:66].strip()
     float_temperature_factor = np.nan if len(value) == 0 else float(value)
     str_id_segment = "" if len(line) < 76 else line[72:76].strip()
     str_symbol_element = "" if len(line) < 78 else line[76:78].strip()
@@ -210,15 +213,16 @@
 
 
 # In[11]:
 
 
 def Compose_ATOM_or_HETATM_line(arr_values):
     """# 2020-12-14 00:08:19
-    compose a ATOM or HETATM line from the output of 'Parse_ATOM_or_HETATM_line' (it is essentially a reverse operation of 'Parse_ATOM_or_HETATM_line')"""
+    compose a ATOM or HETATM line from the output of 'Parse_ATOM_or_HETATM_line' (it is essentially a reverse operation of 'Parse_ATOM_or_HETATM_line')
+    """
     arr_values = deepcopy(arr_values)
     if len(df_meta_pdb_format) > len(df_meta_pdb_format):
         arr_values = arr_values[: len(df_meta_pdb_format)]
     arr_values[11] = (
         "      "
         if isinstance(arr_values[11], (str)) or np.isnan(arr_values[11])
         else "{:>6.2f}".format(arr_values[11])
@@ -245,15 +249,16 @@
 # In[ ]:
 
 
 def Read_Single_Module(
     path_file, enable_automatic_correction=False, verbose=False
 ):  # 2020-07-07 15:59:00
     """# 2021-04-27 11:25:12
-    Read PDB file with a single module (one chain A and one chain B, etc), and return dataframes of ATOM and HETATM records. If missing chain identifiers are detected, reassign chain identifiers based on chain transitions inferred by residue_numbers"""
+    Read PDB file with a single module (one chain A and one chain B, etc), and return dataframes of ATOM and HETATM records. If missing chain identifiers are detected, reassign chain identifiers based on chain transitions inferred by residue_numbers
+    """
     if "/" in path_file:
         with open(path_file, "r") as file:
             l_lines = file.read().split("\n")
     else:  # if a given 'path_file' is not a directory (does not contain '/') read 'path_file' as a string
         l_lines = path_file.split("\n")
     l_lines = list(
         line for line in l_lines if "HEADER" not in line and "REMARK" not in line
@@ -353,15 +358,16 @@
 
 
 # In[ ]:
 
 
 def Split_Multiple_Models(path_file, path_folder_output=None):  # 2020-11-30 03:07:27
     """read pdb file of 'path_file' containing multiple models (CABS-Dock output 'clus' and 'replica' files) and split the file into individual models without parsing and composing data values.
-    'path_folder_output' : output directory of split files. by default, it is where the pdb file is located"""
+    'path_folder_output' : output directory of split files. by default, it is where the pdb file is located
+    """
     path_folder, name_file = path_file.rsplit("/", 1)
     if path_folder_output is None:
         path_folder_output = path_folder  # set default folder
     path_prefix_output = path_folder_output + name_file.rsplit(".", 1)[0]
     flag_writing = False  # flag for writing
     with open(path_file) as file:
         while True:
@@ -445,15 +451,16 @@
 
 
 # In[ ]:
 
 
 def Identify_Protein_and_Assign_Chain_identifier(df, **dict_identifiable_chains):
     """Input : output dataframe of 'Read_Single_Module' as 'df' and keyworded arguments for desired chain identifier for each identifiable protein (example input: A = { 'start' : { 'ILE' : 47 }, 323 : 'CYS', 326 : 'CYS', 391 : 'CYS', 394 : 'CYS' } )
-    Output : output dataframe of 'Read_Single_Module', but with modified chain identifiers for each identified proteins"""
+    Output : output dataframe of 'Read_Single_Module', but with modified chain identifiers for each identified proteins
+    """
     l_df_a_chain = list()
     for (
         char_chain_identifier
     ) in (
         df.Chain_identifier.unique()
     ):  # resolve merged multiper proteins (for example ACAT1 dimer)
         df_a_chain = PD.Select(df, Chain_identifier=char_chain_identifier)
```

### Comparing `biobookshelf-0.2.3/biobookshelf/PKG/package_util.py` & `biobookshelf-0.2.4/biobookshelf/PKG/package_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         return -1
     path_file_download_flag = pkg_resources.resource_filename(
         name_package, f"{path_file}.gunzip_completed.flag"
     )
     if not os.path.exists(
         path_file_download_flag
     ):  # if gunzip has not been done or not completed
-
         path_file_zipped = pkg_resources.resource_filename(
             name_package, path_file
         )  # absolute directory of gzipped file
         path_file_unzipped = path_file_zipped.rsplit(".", 1)[
             0
         ]  # retrieve directory of an unzipped file
         if os.path.exists(
```

### Comparing `biobookshelf-0.2.3/biobookshelf/RNA/rnaseq.py` & `biobookshelf-0.2.4/biobookshelf/RNA/rnaseq.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/SAM/sam_util.py` & `biobookshelf-0.2.4/biobookshelf/SAM/sam_util.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/SC/single_cell.py` & `biobookshelf-0.2.4/biobookshelf/SC/single_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1427,15 +1427,17 @@
                         sep="\t",
                         header=None,
                         index_col=0,
                     )
                     .iloc[:, 0]
                     .to_dict()
                 )
-            except pd.errors.EmptyDataError:  # handle when the current dictionary is empty
+            except (
+                pd.errors.EmptyDataError
+            ):  # handle when the current dictionary is empty
                 dict_dict[name_dict] = dict()
 
     # return summarized metrics
     return dict_dict
 
 
 def MTX_10X_Retrieve_number_of_rows_columns_and_records(path_folder_mtx_10x_input):
@@ -2412,14 +2414,15 @@
             if flag_output_binary
             else open(path_file_output, "w")
         )
     else:
         flag_output_is_file = False
         flag_output_binary = is_binary_stream(path_file_output)  # detect binary stream
         file_output = path_file_output
+
     # define a function for decorating mtx record
     def __decorate_mtx_file__(file):
         while True:
             line = file.readline()
             if len(line) == 0:
                 break
             """ parse a mtx record """
```

### Comparing `biobookshelf-0.2.3/biobookshelf/SEQ/sequence.py` & `biobookshelf-0.2.4/biobookshelf/SEQ/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     seq,
     start=0,
     append_stop_codon_to_returned_seq=False,
     print_message=True,
     return_error_value_if_stop_codon_not_found=True,
 ):
     """Translate nucleotide sequence until the given seq is end or stop codons are encountered.
-    start = 0 : start position for potential protein sequence (for example, start of ATG start codon.)"""
+    start = 0 : start position for potential protein sequence (for example, start of ATG start codon.)
+    """
     if type(seq) is float:
         return np.nan  # if input is invalid, return np.nan
     length_seq = len(seq)  # it seems the time complexity of the len(str) method is O(1)
     l_aa = list()
     while True:
         if start + 3 > length_seq:
             if print_message:
@@ -133,15 +134,16 @@
         )
     )  # return found ORFs without the dummy ORF at the start of the 2D array.
 
 
 # 2020-05-29 14:28:22
 def ORF_Find_All_Methionine_ORFs_on_Both_Strands(seq, use_1_based_coordinate=True):
     """Find all ORFs start with methionine on both strand of the given sequence by using 'ORF_Find_All_Methionine_ORFs'.
-    use 1-based-coordinate for start and end positions if 'use_1_based_coordinate' is set to True"""
+    use 1-based-coordinate for start and end positions if 'use_1_based_coordinate' is set to True
+    """
     df_plus = ORF_Find_All_Methionine_ORFs(
         seq
     )  # find all ORFs in the sequence and the reverse complement of the sequence
     df_minus = ORF_Find_All_Methionine_ORFs(Reverse_Complement(seq))
     df_plus["strand"] = "+"
     df_minus["strand"] = "-"
     int_length_seq = len(
@@ -168,15 +170,16 @@
     seq,
     from_3_prime_end=True,
     return_length_of_polyA=False,
     str_repeated_base="A",
     int_lookup_window=3,
 ):
     """Trim PolyA sequence from the 3' end of a given sequence (DNA sequence in upper characters) if 'from_3_prime_end' is True or trim polyA from 5' end of the sequence if 'from_3_prime_end' is False
-    if the program encounter base other than 'A', lookup next 'int_lookup_window' number of bases and check weather they are consecutive 'A' bases."""
+    if the program encounter base other than 'A', lookup next 'int_lookup_window' number of bases and check weather they are consecutive 'A' bases.
+    """
     if len(seq) == 0:  # if the given seq is empty
         if return_length_of_polyA:
             return 0
         else:
             return ""
     str_repeated_bases_in_lookup_window = str_repeated_base * int_lookup_window
     seq_polyA_at_5_prime_end = seq[::-1] if from_3_prime_end else seq
```

### Comparing `biobookshelf-0.2.3/biobookshelf/STR/string.py` & `biobookshelf-0.2.4/biobookshelf/STR/string.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/UniProt/uniprot.py` & `biobookshelf-0.2.4/biobookshelf/UniProt/uniprot.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/biobookshelf/WEB/web_application.py` & `biobookshelf-0.2.4/biobookshelf/WEB/web_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     l_col_scientific_notations,
     l_col_typical_notation,
     n_significant_digits_scientific_notation=3,
     n_significant_digits_typical_notation=3,
     inplace=False,
 ):
     """# 2021-07-19 17:38:40
-    round float with a given number of significant digits and convert floating point numbers to strings"""
+    round float with a given number of significant digits and convert floating point numbers to strings
+    """
     if not inplace:
         df = deepcopy(df)
     str_format_scientific_notation = (
         "{:." + str(int(n_significant_digits_scientific_notation)) + "e}"
     )
     str_format_typical_notation = (
         "{:." + str(int(n_significant_digits_typical_notation)) + "f}"
```

### Comparing `biobookshelf-0.2.3/biobookshelf/main/unclassified_functions.py` & `biobookshelf-0.2.4/biobookshelf/main/unclassified_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,15 @@
     7879,
     7905,
     6634,
     7415,
     51699,
 ]
 
+
 # slice functions
 def Slice_to_Range(sl, length):
     """# 2022-06-28 21:47:51
     iterate indices from the given slice
     """
     assert isinstance(sl, slice)  # make sure sl is slice
     # convert slice to integer indices
@@ -541,15 +542,16 @@
 # ### Functions for working with base systems.
 
 # In[ ]:
 
 
 def BASE(number, base, n_numbers=None):  # 2020-07-25 16:08:23
     """return a list of integers representing the number in the given base system.
-    if 'n_numbers' is given and length of the output list is smaller than 'n_numbers', pad zeros and return a list of integers with the length of 'n_numbers'"""
+    if 'n_numbers' is given and length of the output list is smaller than 'n_numbers', pad zeros and return a list of integers with the length of 'n_numbers'
+    """
     if isinstance(number, float):
         number = int(number)
     l_value = list()
     quotient = number
     while True:
         quotient, remainder = divmod(quotient, base)
         l_value.append(remainder)
@@ -568,15 +570,16 @@
 # In[ ]:
 
 
 def Encode_List_of_Strings(
     arr, chr_separator=";", chr_representing_repeated_string="="
 ):  # 2020-08-08 23:47:49
     """Encode list of strings into a string.
-    'chr_representing_repeated_string': Reduce the size of string by representing repeating non-empty, valid string with single 'chr_representing_repeated_string' (default '=') character. To disable this behavior, set 'chr_representing_repeated_string' to None"""
+    'chr_representing_repeated_string': Reduce the size of string by representing repeating non-empty, valid string with single 'chr_representing_repeated_string' (default '=') character. To disable this behavior, set 'chr_representing_repeated_string' to None
+    """
     entry_previous = None
     l_value = list()
     for entry in arr:
         if isinstance(entry, float):
             l_value.append("")
         elif chr_representing_repeated_string is not None and entry_previous == entry:
             l_value.append(chr_representing_repeated_string)
@@ -703,15 +706,16 @@
     n_char=2,
     value_min=0,
     value_max=1,
 ):  # 2020-07-25 18:09:07
     """Encode list of 'list of values' of float datatype with one or more ascii character, and return list of strings (ascii format) (each list of values in the given input will be encoded into a single string). (two ascii characters can encode float value with ~8000 levels)
     ascii_min: (integer) minimum = 33
     ascii_max: (integer) maximum = 126. should be larger than 'ascii_min' + 1. The last value will be used to interpret invalid values
-    value_max: when encoded values are interger or floating number with regular intervalues, correct value_max should be the maximum integer value + step (1 for integer and amount of the regular interval for the float number), since values are floored down to an integer during the encoding process"""
+    value_max: when encoded values are interger or floating number with regular intervalues, correct value_max should be the maximum integer value + step (1 for integer and amount of the regular interval for the float number), since values are floored down to an integer during the encoding process
+    """
     if ascii_max <= 125:
         n_char = 1  # if not all ascii characters are used, use only one ascii character to encode/decode data
     elif n_char > 1:
         ascii_max = 126
     base = (
         ascii_max - ascii_min + 1
     )  # base including ascii characters in l_ascii_to_exclude will be excluded
@@ -917,15 +921,16 @@
             value_max = value
     return key_max, value_max
 
 
 def DICTIONARY_Find_Min(dict_value):
     """
     # 2020-12-06 18:33:24
-    find key value with the maximum value in a given dictionary, and return 'key_min', 'value_min'"""
+    find key value with the maximum value in a given dictionary, and return 'key_min', 'value_min'
+    """
     if len(dict_value) == 0:
         return None, None  # if an empty dictionary is given, return None
     key_min = next(
         dict_value.__iter__()
     )  # retrieve the a key and value from the dictionary as an initial key-value pair with 'max' value
     value_min = dict_value[key_min]
     for key in dict_value:
@@ -934,15 +939,16 @@
             key_min = key
             value_min = value
     return key_min, value_min
 
 
 def DICTIONARY_Find_keys_with_max_value(dict_value):
     """# 2021-11-24 20:44:07
-    find a list of key values with the maximum value in a given dictionary, and return 'l_key_max', 'value_max'"""
+    find a list of key values with the maximum value in a given dictionary, and return 'l_key_max', 'value_max'
+    """
     value_max = None  # initialize max value
     l_key_max = []  # list of key with max_values
     if len(dict_value) != 0:  # if the dictionary is not empty
         for key in dict_value:
             value = dict_value[key]
             if value_max is None:
                 value_max = value
@@ -957,15 +963,16 @@
             ):  # if the another key contains the current max value, add the key to the list of keys with max values
                 l_key_max.append(key)
     return l_key_max, value_max
 
 
 def DICTIONARY_Find_keys_with_min_value(dict_value):
     """# 2022-04-20 18:28:51
-    find a list of key values with the minimum value in a given dictionary, and return 'l_key_min', 'value_min'"""
+    find a list of key values with the minimum value in a given dictionary, and return 'l_key_min', 'value_min'
+    """
     value_min = None  # initialize min value
     l_key_min = []  # list of key with min_values
     if len(dict_value) != 0:  # if the dictionary is not empty
         for key in dict_value:
             value = dict_value[key]
             if value_min is None:
                 value_min = value
@@ -1307,15 +1314,16 @@
     duplicate_filter=2,
     dropna=True,
     sort_series_by_values=True,
     convert_tuple_to_string=False,
 ):
     """
     # 20210224
-    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more."""
+    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more.
+    """
     if dropna and isinstance(iterable, pd.Series):
         iterable = (
             iterable.dropna()
         )  # if dropna is set to 'True', dropn NaN values before counting
     if isinstance(next(iterable.__iter__()), (np.ndarray, list)):
         iterable = list(
             map(tuple, iterable)
@@ -1427,15 +1435,16 @@
 def Search_list_of_strings(
     list_of_strings,
     query="cancer",
     return_mask_matched=False,
     return_location_matched=False,
 ):
     """search list of strings to find strings that contains query string and return the result as a list. if 'return_mask_matched' is True,
-    return list_mask for locations of matched entries (return np.array( search_result, dtype = object ), list_mask_matched)"""
+    return list_mask for locations of matched entries (return np.array( search_result, dtype = object ), list_mask_matched)
+    """
     search_result, list_mask_matched = list(), list()
     list_of_strings = (
         list_of_strings.values
         if type(list_of_strings) is pd.Series
         else list_of_strings
     )  # if type of list_of_strings is pd.Series, even though iterating through pandas series is just fine, to be safe and fast, convert pd.Series to a numpy array
     for (
@@ -1885,15 +1894,16 @@
 # In[ ]:
 
 
 def SEARCH_gene_symbol_name(
     df=None, query_Symbol=None, query_Name=None, negative_query=None
 ):
     """Using df (a subset of HGNC) or full HGNC df by default, search a given query and negative query, and return a DataFrame with genes that
-    have matching Gene_Symbol or Gene_Name to a given query. Give previous search result through an argument 'df' to refine search"""
+    have matching Gene_Symbol or Gene_Name to a given query. Give previous search result through an argument 'df' to refine search
+    """
     if df is None:  # set default df, which is a full HGNC table
         df = df_ID_Symbol
     if query_Symbol is not None:
         search_list, query = df.Approved_Symbol.values, query_Symbol
     elif query_Name is not None:
         search_list, query = df.Approved_Name.values, query_Name
     else:
@@ -2066,15 +2076,16 @@
     interval_2,
     flag_sort_to_retrieve_start_and_end=False,
     flag_0_based_coordinate_system=True,
 ):  # 2020-08-06 20:44:47
     """Fast, basic function for retrieving overlap between two intervals.
     return number of overlapped length between two intervals (each interval is a tuple or list containing start and end position).
     'flag_0_based_coordinate_system': if interval contains float numbers, set 'flag_0_based_coordinate_system' to True.
-    'flag_sort_to_retrieve_start_and_end': if interval is always (start, end), set 'flag_sort_to_retrieve_start_and_end' to False to improve performance. (about 200ns faster)"""
+    'flag_sort_to_retrieve_start_and_end': if interval is always (start, end), set 'flag_sort_to_retrieve_start_and_end' to False to improve performance. (about 200ns faster)
+    """
     if flag_sort_to_retrieve_start_and_end:
         start_1, end_1 = sorted(interval_1)
         start_2, end_2 = sorted(interval_2)
     else:
         start_1, end_1 = interval_1
         start_2, end_2 = interval_2
     if not flag_0_based_coordinate_system:
@@ -2088,15 +2099,16 @@
 # #### Functions for handling outliers
 
 # In[ ]:
 
 
 def OUTLIERS_GET_mask_for_outliers(arr, n_std_for_outliers, outlier_percentile_std=5):
     """for each row of a given numpy array, identify the outliers (outside n_std_for_outliers * std from mean) and return a boolean array
-    that indicates locations of outliers. if 'outlier_percentile_std' is not zero, calculate and mean and std excluding top and bottom 'outlier_percentile_std' percentile for defining outliers"""
+    that indicates locations of outliers. if 'outlier_percentile_std' is not zero, calculate and mean and std excluding top and bottom 'outlier_percentile_std' percentile for defining outliers
+    """
     if outlier_percentile_std == 0:
         arr_mean, arr_std = arr.mean(axis=1), arr.std(
             axis=1
         )  # retrive mean and std of outliers
     else:
         arr_masked = np.ma.masked_array(
             data=arr,
@@ -2243,15 +2255,16 @@
             if len(s) > 0:
                 print("\n👉", col)
                 display(s)
 
 
 def DF_from_Anndata(adata):
     """# 2021-11-17 21:23:10
-    convert Anndata (both in sparse format and dense format) to DataFrame in respective format (either sparse or dense format)"""
+    convert Anndata (both in sparse format and dense format) to DataFrame in respective format (either sparse or dense format)
+    """
     if isinstance(adata.X, scipy.sparse.csr.csr_matrix):
         df = pd.DataFrame.sparse.from_spmatrix(
             adata.X, index=adata.obs.index.values, columns=adata.var.index.values
         )
     else:
         df = adata.to_df()
     return df
@@ -2609,15 +2622,16 @@
     l_col_for_sorting_and_not_for_identifying_duplicates=None,
     dict_kw_sort_values={"ascending": False},
     col_name_for_duplicate_counts="duplicate_counts",
     inplace=False,
     dict_kw_drop_duplicates={"keep": "first"},
 ):  # 2020-08-08 19:58:43  # pandas >= 1.1
     """drop duplicates while counting duplicates. if a column for counting duplicates already exist in the given dataframe, sum values in the columns while dropping duplicates instead of counting duplicates.
-    'l_col_for_sorting_and_not_for_identifying_duplicates': if 'l_col_for_sorting_and_not_for_identifying_duplicates' is given, sort rows using columns given in the order in 'l_col_for_sorting_and_not_for_identifying_duplicates' before dropping duplicates"""
+    'l_col_for_sorting_and_not_for_identifying_duplicates': if 'l_col_for_sorting_and_not_for_identifying_duplicates' is given, sort rows using columns given in the order in 'l_col_for_sorting_and_not_for_identifying_duplicates' before dropping duplicates
+    """
     if not inplace:
         df = deepcopy(df)
     if l_col_for_sorting_and_not_for_identifying_duplicates is not None:
         df.sort_values(
             l_col_for_identifying_duplicates
             + l_col_for_sorting_and_not_for_identifying_duplicates,
             inplace=True,
@@ -2769,15 +2783,16 @@
         set_index = set(set_index)
     return s[list(True if e in set_index else False for e in s.index.values)]
 
 
 def PD_Threshold(df, AND_operation=True, **dict_thresholds):
     """Select rows of a given DataFrame or indices of Series based on a given threshold for each given column or the given series.
     Add 'b' or 'B' at the end of column_label to select rows below the threshold, or add 'a' or 'A' to select rows above the threshold.
-    If 'AND_operation' is true, filter generated from the given threshold will be combined with AND operation before filtering rows of a given dataframe"""
+    If 'AND_operation' is true, filter generated from the given threshold will be combined with AND operation before filtering rows of a given dataframe
+    """
     set_df_columns = set(df.columns.values) if type(df) is pd.DataFrame else set([""])
     mask_filter = (
         np.ones(len(df), dtype=bool) if AND_operation else np.zeros(len(df), dtype=bool)
     )
     for col_direction, threshold in dict_thresholds.items():
         col, direction = col_direction[:-1], col_direction[-1]
         if col not in set_df_columns:
@@ -2960,15 +2975,16 @@
     ignore_case=True,
     verbose=True,
     **dict_search,
 ):
     """# 2021-11-10 01:56:43
     to search index, put 'index' as the name of column in the 'dict_search' argument. To search values in a series, put 'values' as the name of column in the 'dict_search' argument
     To retrive entries matched with all queries, set 'query_AND_operation' to True (perform AND operation during searching), while set 'query_AND_operation' to False to retrive all entries
-    containing at least one of the given queries. Search with multiple columns are always performed with AND operation (will be improved)"""
+    containing at least one of the given queries. Search with multiple columns are always performed with AND operation (will be improved)
+    """
     for col, queries in dict_search.items():
         if type(df) is pd.DataFrame and col not in list(df.columns.values) + [
             "index",
             "columns",
             "col",
         ]:  # print out an error message when invalid column name was given for a dataframe
             if verbose:
@@ -3080,15 +3096,16 @@
 
 
 # In[ ]:
 
 
 def PANDAS_Align_two(df_1, df_2, axis=1):
     """** There is a original method "pandas.align" Use it if possible. **
-    align two dataframe or series. by default, align by columns (axis = 1). if series is given as one of the inputs, align two objects by indices"""
+    align two dataframe or series. by default, align by columns (axis = 1). if series is given as one of the inputs, align two objects by indices
+    """
     if (
         type(df_1) is pd.Series or type(df_2) is pd.Series
     ):  # if series is given as one of the inputs, align two objects by indices
         axis = 0
     if axis == 1:
         cols_shared = LIST_intersection_with_set(
             df_1.columns.values, df_2.columns.values
@@ -3116,15 +3133,16 @@
 
 
 def PANDAS_relation_dataframe_make_symmetric(
     df, data_is_in_lower_tri=True, symmetry_relationship="same", diagonal_data=None
 ):
     """For a given relation dataframe, copy data in lower triangle to upper triangle if 'data_is_in_lower_tri' is True (or copy data in upper triangle into lower triangle if 'data_is_in_lower_tri'
     is False). 'symmetry_relationship' = 'same' or '=' ; 'opposite_sign' or '-' ; 'inverse' or '1/' . 'diagonal_data' : data_value that will be used to the fill diagonal data. If None is given,
-    use the first diagonal value as 'diagonal_data' value ( df.iloc[ 0, 0 ] ). If 'diagonal_data' = 'retain', use the initial diagonal data"""
+    use the first diagonal value as 'diagonal_data' value ( df.iloc[ 0, 0 ] ). If 'diagonal_data' = 'retain', use the initial diagonal data
+    """
     n = len(df)
     if n < 1:
         return -1
     indices_diagonal = np.diag_indices(n)  # define diagnoal indices
     if diagonal_data is None:
         diagonal_data = df.iloc[0, 0]
     elif (
@@ -3482,15 +3500,16 @@
     return_normalized_ratios=False,
     normalization_description="",
 ):
     """Perform Relative Log Expression (RLE) Normalization on DataFrame ( col = sample, index = genes ) for sample_list (default : all columns ) and Gene_Set (default : all indices)
     if 'use_median_ratio' is False, use mean_ratio instead.
     return df and Series with median ratios to pseudoreference (log-averaged for 'sample_list_for_pseudoreference', default : all columns ) for the samples that has been set for normalization.
     When 'return_normalized_ratios' is True, return normalized relative_ratios to pseudoreference instead of normalized data.
-    When 'allow_nan_values' is set to True, use masked array to retrive scaling factors for each sample (if data contains a lot of NaN or zeros, it is better to set this argument to True)"""
+    When 'allow_nan_values' is set to True, use masked array to retrive scaling factors for each sample (if data contains a lot of NaN or zeros, it is better to set this argument to True)
+    """
     Gene_Set = (
         LIST_intersection_with_set(Gene_Set, df.index.values)
         if Gene_Set is not None
         else df.index.values
     )  # by default, Gene_Set is all genes in the df # if Gene_Set has been given, only consider genes that exist in df
     sample_list = (
         LIST_intersection_with_set(sample_list, df.columns.values)
@@ -3618,15 +3637,16 @@
 # In[ ]:
 
 
 def GENE_SET_GET_Gene_Set_by_name(
     Gene_Set_name, return_Gene_Name_Symbol=False, gene_set_background=None
 ):
     """return a Gene_Set (set of Gene_IDs) of a given Gene_Set_name in All Gene_Sets. if 'return_Gene_Name_Symbol' is True, return sorted list of Gene_Name_Symbol of a gene_set. If a
-    background gene_set has been given through 'gene_set_background' argument, return genes that exist in the background gene_set"""
+    background gene_set has been given through 'gene_set_background' argument, return genes that exist in the background gene_set
+    """
     for Gene_Sets_Name in dict_GeneSets_ALL.keys():
         if Gene_Set_name in dict_GeneSets_ALL[Gene_Sets_Name]:
             Gene_Set = dict_GeneSets_ALL[Gene_Sets_Name][Gene_Set_name]
             if (
                 gene_set_background is not None
             ):  # If a background gene_set has been given through 'gene_set_background' argument, return genes that exist in the background gene_set
                 Gene_Set = Gene_Set.intersection(gene_set_background)
@@ -3834,15 +3854,16 @@
 
 
 def ANALYSIS_GSEA__dict_Gene_Sets(
     Gene_IDs, background_Gene_IDs=None, dict_Gene_Sets=None, thres_adj_p_val=0.05
 ):
     """Perform GSEA using gene sets in a given dict_Gene_Sets and return results as two DataFrames
     Calculate adjusted p_value using fdr_bh method
-    filter out entries that have higher adjusted_p_values than a given threshold adj_p_val"""
+    filter out entries that have higher adjusted_p_values than a given threshold adj_p_val
+    """
     background_Gene_IDs = set(background_Gene_IDs)
     Gene_IDs = set(Gene_IDs)
     num_genes = len(Gene_IDs)
     num_background_genes = len(background_Gene_IDs)
     dict_GSEA = (
         {}
     )  # perform GSEA for every gene set in a given dict_Gene_Sets and save result to a dictionary
@@ -3882,15 +3903,16 @@
 
 
 def ANALYSIS_GSEA__MSigDB_Gene_Sets(
     Gene_IDs, background_Gene_IDs=None, thres_adj_p_val=0.05, Gene_Sets_Names=None
 ):
     """Perform GSEA using all available MSigDB gene sets return results as DataFrames in a dictionary
     The list of Gene_Sets_Names can be given though an argument Gene_Sets_Names
-    filter out entries that have higher adjusted_p_values than a given threshold adj_p_val"""
+    filter out entries that have higher adjusted_p_values than a given threshold adj_p_val
+    """
     if background_Gene_IDs is None:
         background_Gene_IDs = PD_Select(
             df_ID_Symbol, Locus_Group="protein-coding gene"
         ).index.values  # set protein-coding genes as a background geneset
     if (
         Gene_Sets_Names is None
     ):  # if a list of Gene_Sets_Names was not given, set default Gene_Sets_Names
@@ -4215,15 +4237,16 @@
     dict_Gene_Sets,
     Gene_IDs=None,
     sample_list_condition_A=None,
     sample_list_condition_B=None,
 ):
     """Calculate Log2FC, t-test p_values, and fdr-bh adjusted p_values for condition 'A' (default: Normal) and condition 'B' (default: Tumor)
     samples for Gene_Sets in 'dict_Gene_Sets' with a given Gene_IDs and return the result as a dataframe. Log2FC is log2( condition B average / condition A average )
-    dropna values to allow pair-wise comparison and calculation of Log2FC of genes in a Gene_Set"""
+    dropna values to allow pair-wise comparison and calculation of Log2FC of genes in a Gene_Set
+    """
     if Gene_IDs is None:  # if Gene_IDs was not given, set indices of df as Gene_IDs
         Gene_IDs = df.index.values
     else:  # if Gene_IDs has been given
         Gene_IDs = set(df.index.values).intersection(
             Gene_IDs
         )  # consider Gene_IDs that exist in df
     if sample_list_condition_A is None:
@@ -4303,15 +4326,16 @@
     label_condition_A="condition_A",
     label_condition_B="condition_B",
     add_Gene_Set_2_df=True,
 ):
     """Calculate Log2FC, t-test p_values, and fdr-bh adjusted p_values for condition 'A' (default: Normal) and condition 'B' (default: Tumor)
     samples for each Gene_Sets in 'dict_Gene_Sets_Name__Gene_Sets' (default : 'dict_GeneSets_ALL' ) with a given Gene_IDs and return the result as a dataframe.
     Log2FC is log2( condition B average / condition A average ). dropna values to allow pair-wise comparison and calculation of Log2FC of genes in a Gene_Set.
-    label columns according to given labels 'label_condition_A' and 'label_condition_B'."""
+    label columns according to given labels 'label_condition_A' and 'label_condition_B'.
+    """
     df = deepcopy(df)  # copy dataframe to avoid changing original content
     if Gene_IDs is None:  # if Gene_IDs was not given, set indices of df as Gene_IDs
         Gene_IDs = df.index.values
     else:  # if Gene_IDs has been given
         Gene_IDs = set(df.index.values).intersection(
             Gene_IDs
         )  # consider Gene_IDs that exist in df
@@ -4578,15 +4602,16 @@
 
 # In[ ]:
 
 
 def GENE_Annotate_df_for_plot(df, gene_list_annotation):
     """gene_list_annotation : if a list of Gene is given through this argument and df is not a list (a single DataFrame), draw annotation of valid genes on the plot. If gene_list_annotation = 'all',
     annotate all genes in a given df. If 'gene_list_annotation' is integer, annotate every 'gene_list_annotation' number of genes in df. if 'gene_list_annotation' is list containing three
-    integers (the list should have at least two integers), annotate [ gene_list_annotation[ 0 ] : gene_list_annotation[ 1 ] : gene_list_annotation[ 2 ] (default : 1) ] genes in df."""
+    integers (the list should have at least two integers), annotate [ gene_list_annotation[ 0 ] : gene_list_annotation[ 1 ] : gene_list_annotation[ 2 ] (default : 1) ] genes in df.
+    """
     if (
         gene_list_annotation is not None
     ):  # if 'gene_list_annotation' is given, retrive valid Gene_IDs and Gene_Symbols from the given list, and retrive positions of the valid genes in the DataFrame
         Gene_IDs, list_positions = df.index.values, np.arange(
             0, len(df.index.values)
         )  # retrive all Gene_IDs and list of positions
         dict_ID_positions = dict(
@@ -4727,15 +4752,16 @@
     linkage_method=None,
     cluster_method="maxclust",
     print_message=False,
 ):
     """Wrapper method of 'recursive_clustering' (recursively cluster and return subcluster-ordered entries) and 'hierarchical_clustering' method (return optimal ordering of entires).
     set 'clustering_type' to 'recursive' or 'rc' for the former method and 'optimal' or 'hc' for the latter
     if list of df is given through 'df' argument, merge the dataframes (DataFrames has to have same indices though they can be in different order) and Clustering the DataFrame
-    For asymmetric data (with different columns and indices), If 'axis' is 0, cluster columns. if 'axis' is 1, cluster indices."""
+    For asymmetric data (with different columns and indices), If 'axis' is 0, cluster columns. if 'axis' is 1, cluster indices.
+    """
     list_df = None  # set a default value of list_df, which will contain list of DataFrame if it has been given through df argument
     if type(df) is not pd.DataFrame:
         cluster_column_too = is_relation_matrix  # store the value of 'is_relation_matrix' separately so that it can be used when returning the clustered result
         list_df, is_relation_matrix = (
             deepcopy(df),
             False,
         )  # set 'is_relation_matrix' False if list of DataFrame has been given so that only indices are used for clustering
@@ -4814,15 +4840,16 @@
     correlation_type="spearman",
     n_std_for_outliers=None,
     min_observation="auto",
 ):
     """Calculate Spearman Correlation Coefficient for each gene-gene pairs and return return df_correl_mat
     default Gene_Set : indices of df (df.index.values)
     correlation_type = { 'pearson', 'kendall', 'spearman' } or lambda function that receive two numpy array
-    it is expected to use require really long time computing when excluding outliers by using 'n_std_for_outliers' to calculate more robust correlation coefficients."""
+    it is expected to use require really long time computing when excluding outliers by using 'n_std_for_outliers' to calculate more robust correlation coefficients.
+    """
     if Gene_Set is None:  # set default Gene_Set
         Gene_Set = set(df.index.values)
     if sample_list is None:  # set default sample_list
         sample_list = set(df.columns.values)
     valid_Gene_Set = set(df.index.values).intersection(
         set(Gene_Set)
     )  # valid Gene_Set is a set of genes that exist in df
@@ -5710,15 +5737,16 @@
 
 def EXPLORE_Cluster(
     df_clus, dict_tree_clus, df_data=None, df_name="", color_map="bwr", add_Log2FC=False
 ):
     """interactive method that can be used to explore clusters of 'df_clus' in 'dict_tree_clus'
     'df_data' is for drawing Log2FC T/N along with the matrix
     it is better and faster to use %matplotlib inline instead of qt, to store all the plots that has been drawn
-    current_cluster_name can be saved and returned at the end of this method as a list"""
+    current_cluster_name can be saved and returned at the end of this method as a list
+    """
     current_tree_node = dict_tree_clus
     list_parent_tree_node = (
         list()
     )  # a stack that will store parant nodes for trace back
     saved_cluster_names = list()
     while True:
         current_cluster_name = current_tree_node["cluster_name"]
@@ -5800,15 +5828,16 @@
 
 
 def PLOT_magnigfied_correl_matrix(
     df, df_data, start, end, show_grid=False, color_limit=1, size="auto"
 ):
     """For clustered relation matrix (let's call ratio matrix or correlation matrix all together as relation matrix),
     Magnify the matrix from 'start' to 'end', and Add Log2FC data at the rightmost column (df_data should be given through an argument)
-    Also, return a DataFrame with indices, Gene_Name_Symbols, and Log2FC so that Two-gene plot can be subsequently drawn"""
+    Also, return a DataFrame with indices, Gene_Name_Symbols, and Log2FC so that Two-gene plot can be subsequently drawn
+    """
     end += 1
     n_genes = end - start  # retrive number of genes
     Gene_IDs = df.index.values[start:end]  # retrive Gene_IDs
     Gene_Name_Symbols = List_Gene_ID__2__List_Gene_Symbol(
         Gene_IDs, add_gene_name=True
     )  # retrive Gene_Name(Gene_Symbol) annotations
     if size == "auto":  # automatically set size of the plot
@@ -6075,15 +6104,16 @@
     color_percentile_lower="b",
     color_percentile_upper="orange",
     thres_n_points=10000,
     **dict_mpl_basic_configure,
 ):
     """(1) Convert iterable data like series or list into np.ndarray using 'TYPE_Convert_NP_Array' (2) Sort, (3) Visualize on a plot using green and red colors
     to visualize deviation from the given threshold. if color_percentile_thres is not None, annotate upper and lower percentiles with the color given by color_percentile arguments
-    if 'data' is pandas.DataFrame with two columns, first sort values in the second column by the first column, visualize, and annotate unique_entries of the first column on the plot. The NaN values in the first column will be ignored."""
+    if 'data' is pandas.DataFrame with two columns, first sort values in the second column by the first column, visualize, and annotate unique_entries of the first column on the plot. The NaN values in the first column will be ignored.
+    """
     bool_flag_sort_using_two_columns = (
         isinstance(data, pd.DataFrame) and len(data.columns.values) == 2
     )  # 'sort_using_two_columns' if a DataFrame with two columns are given as a 'data'.
     if isinstance(
         data, (pd.DataFrame, pd.Series)
     ):  # set default title and y_label by using pandas.Series name if not given
         data_name = data.name if isinstance(data, pd.Series) else data.columns.values[1]
@@ -6377,15 +6407,16 @@
     alpha=0.7,
     figsize=(8.0, 6.0),
     marker="o",
     dict_ax_scatter=dict(),
     **dict_matplotlib_basic_setting,
 ):
     """'arr_coordinates' should be numpy array with 2 columns, x and y coordinates, and 'arr_labels' should be a list-like object containing labels.
-    If arr_labels contains np.nan and it is pd.Series, remove np.nan labels from the given arr_labels and entries with np.nan labels from arr_coordinates"""
+    If arr_labels contains np.nan and it is pd.Series, remove np.nan labels from the given arr_labels and entries with np.nan labels from arr_coordinates
+    """
     if NUMPY_UTIL_Does_contain_NaN(
         arr_labels
     ):  # if arr_labels contains np.nan and it is pd.Series, remove np.nan labels from the given arr_labels and entries with np.nan labels from arr_coordinates
         arr_coordinates = arr_coordinates[~pd.isnull(arr_labels)]
         arr_labels = arr_labels.dropna()
     arr_labels = (
         arr_labels
@@ -6657,15 +6688,16 @@
     save_fig=False,
     show_plot=True,
     name_df="df_proteome_unshared",
     name_Gene_Set="Unnamed",
     name_sample_list="Unnamed",
 ):
     """Calculate Rank of data of samples for each gene, and calculate average rank for each sample, and draw a distribution of ranks of genes in a given set of genes for each sample as a boxplot
-    Return series containing data of arr_sample_ranks_median with sample_list as indices"""
+    Return series containing data of arr_sample_ranks_median with sample_list as indices
+    """
     if Gene_Set is not None:
         df = PANDAS_Subset(df, Gene_Set)
     df = df[sample_list]
     arr_sample_ranks = (
         df.values.argsort(axis=1).argsort(axis=1) / len(sample_list) * 100
     )  # normalize Rank into range from 0 to 100 to aid visualization
     arr_sample_ranks_median = np.median(arr_sample_ranks, axis=0)
@@ -6729,15 +6761,16 @@
     data_label="intensity",
     fontsize_col=12,
     fontsize_index=12,
     fontsize_blot=12,
 ):
     """Plot Grey_scale heatmap of data of a given DataFrame with a given sample_list and Gene_Set, as if showing a image of gel blots (for example, Western Blot) 'data_label' is a label for colorbar label
     'method_data_heatmap' : method used to set colors of heatmap.  'max' = max value become the highest value and 0 becomes lowest value. 'std_positive' = log-average + 2 * std becomes max color
-            and 0 becomes lowest value. 'std_zero' = 2 * std and -2 *std becomes max and min color. A tuple of color limits can be alternatively given when data_heatmap == data"""
+            and 0 becomes lowest value. 'std_zero' = 2 * std and -2 *std becomes max and min color. A tuple of color limits can be alternatively given when data_heatmap == data
+    """
     if df is None:
         df = df_rna
     valid_sample_list = np.array(sample_list)[
         GET_MASK_of_intersection(sample_list, df.columns.values)
     ]  # retrive valid sample_list while preserving the order of a given list of samples
     df = df[valid_sample_list]  # retrive data of valid_sample_list
     df = df.replace(
@@ -7058,15 +7091,16 @@
     colormap_diverging=False,
     graph_folder=None,
 ):
     """Draw interactibe Bokeh volcano plot of a given result dataframe from 'Calculate_Log2FC_p_value__A_vs_B' that calculate Log2FC
     The dataframe should have Gene_ID as its index, and all Gene_IDs has to be valid (that is, it should exist in dict_ID_Symbol)
     color of circle will be set by data of data_label given by 'color', and size of circle will be set by data of data_label given by 'size'
     'show_symbol_filter_kw' keyworded arguments for filtering entries for displaying Approved_Symboles using 'RESULT_filter'.
-    column labels of x_axis, y_axis are given thorugh arguments.    axis type, 'log' or 'linear', is also given thorugh arguments.    tap_callback : 'google' search"""
+    column labels of x_axis, y_axis are given thorugh arguments.    axis type, 'log' or 'linear', is also given thorugh arguments.    tap_callback : 'google' search
+    """
     if (
         x_axis is None
     ):  # if x_axis and y_axis values were not given, automatically set x and y axis values
         x_axis = df.columns.values[5]
     if y_axis is None:
         y_axis = df.columns.values[6]
     if "p_value" in color:
@@ -7192,15 +7226,16 @@
     tap_callback="google",
     graph_folder=None,
 ):
     """Draw interactibe Bokeh volcano plot of a given result dataframe from 'Calculate_Log2FC_p_value__A_vs_B' that calculate Log2FC
     The dataframe should have Gene_ID as its index, and all Gene_IDs has to be valid (that is, it should exist in dict_ID_Symbol)
     column labels of x_axis, y_axis are given thorugh arguments.    axis type, log or linear, is also given thorugh arguments
     tap_callback : 'google' or 'ncbi' search of gene if clicked (default ncbi).
-    Also, annotate a given list of genes in 'show_symbol_gene_ids' if given (dafault is all genes) according to a filter given by 'show_symbol_filter_kw'"""
+    Also, annotate a given list of genes in 'show_symbol_gene_ids' if given (dafault is all genes) according to a filter given by 'show_symbol_filter_kw'
+    """
     dict_shorthand = dict(
         Log2_Fold_Change="Log2FC",
         adjusted_p_value="adj p",
         p_value="p val",
         average_all="avg_all",
     )  # define dictionary of shorthand annotation of possible x and y axes
     df = deepcopy(df)
@@ -7453,15 +7488,16 @@
     x_label="x_axis",
     y_label="y_axis",
     dict_scatter=dict(),
     graph_folder=None,
     **dict_attributes,
 ):
     """'arr_coordinates' should be numpy array with 2 columns, x and y coordinates, and 'arr_labels' should be a list-like object containing labels. Additional information can be given
-    through keyworded arguments, and will be displayed via Bokeh's hover tool. bokeh circle function's additional keywords can be given through 'dict_scatter'"""
+    through keyworded arguments, and will be displayed via Bokeh's hover tool. bokeh circle function's additional keywords can be given through 'dict_scatter'
+    """
     arr_labels = (
         arr_labels
         if isinstance(arr_labels, (np.ndarray))
         else np.array(arr_labels, dtype=object)
     )  # convert arr_labels to a numpy object
     s_label = LIST_COUNT(arr_labels, duplicate_filter=None).sort_values(ascending=False)
     save_html = False
@@ -7560,15 +7596,16 @@
     default df_data is df_proteome
     set data_phospho to True if entries are indices of df_phosphoproteome
     if 'two_plots' = True and both 'df' and 'df_2' are given, draw two plots using both data as subplots to allow comparison
     draw a regression line that go through an origin (with zero intercept) for normal samples if 'add_regression_line_normal' is True
     If 'regression_intercept_zero', draw an regression line that go through an origin
     'show_correl' : if 'N' or 'normal', show correl. for normal samples, 'T' or 'tumor' for tumor, 'NT' or 'TN' or 'A' for all samples.
                     if 'show_correl' = None, do not show correlation coefficient
-    'regression_type' : set type of linear regression line. 'proj' for projection-based least square linear regression, 'th' for Theil-Sen regression, and 'ls' for normal least square linear regression, 0 for normal least linear regression passing the origin"""
+    'regression_type' : set type of linear regression line. 'proj' for projection-based least square linear regression, 'th' for Theil-Sen regression, and 'ls' for normal least square linear regression, 0 for normal least linear regression passing the origin
+    """
     if (
         gene_id_1 is None
     ):  # retrive data (pandas  Series) that will be used in plotting # if external data has been given, used the data
         grade_color = False  # currently grade_color = True option is not available
         series_gene_1_data, series_gene_2_data = (
             external_gene_1_data,
             df[All_samples].loc[gene_id_2],
@@ -7752,15 +7789,16 @@
     Tumor and normal samples are indicated by blue and red colors, respectively.
     normal_type = True, tumor_type = True : when each type is set to True, the group appears on the plot
     default df_data is df_proteome
     set data_phospho to True if entries are indices of df_phosphoproteome
     if df_2' is given, draw two plots using both 'df' and 'df_2' as subplots to allow comparison between two data
     'show_correl' : if 'N' or 'normal', show correl. for normal samples, 'T' or 'tumor' for tumor, 'NT' or 'TN' or 'A' for all samples. if 'show_correl' = None, do not show correlation
     if 'switch_genes' is True, another subplots with swithced genes will be drawn
-    'regression_type' : set type of linear regression line. 'proj' for projection-based least square linear regression, 'th' for Theil-Sen regression, and 'ls' for normal least square linear regression"""
+    'regression_type' : set type of linear regression line. 'proj' for projection-based least square linear regression, 'th' for Theil-Sen regression, and 'ls' for normal least square linear regression
+    """
     if df is None:
         df = df_proteome
         df_name = "Proteome"
     if type(gene_1) is pd.Series:
         gene_id_1, gene_id_2 = None, Gene_2_Gene_ID(gene_2)
         Gene_1_Symbol, Gene_2_Symbol = gene_1.name, dict_ID_Symbol_simple[gene_id_2]
     else:
@@ -8944,15 +8982,16 @@
     n_skip_samples=1,
     show_ref=False,
     Gene_Set_description="Mitochondrial",
 ):
     """subset 'df' with 'Organelle_Gene_Set' to represent an organelle and RLE normalize the data
     With an estimated amount of organelle in each sample, plots boxplots of each samples, along with scatter plots using Gene data (set N_samples as pseudo_reference )
     if 'Gene' is given. If 'plot_normalized' is set to True, boxplots and the scatter plot are drawn using the normalized data
-    external data can be given through 'Gene' argument as a pandas series where index is Sample_ID"""
+    external data can be given through 'Gene' argument as a pandas series where index is Sample_ID
+    """
     df_all_input_genes = deepcopy(df)
     df_normalized, series_organelle_amount = NORMALIZE_Relative_Log_Expression(
         df,
         N_samples,
         Organelle_Gene_Set,
         return_normalized_ratios=True,
         scale_all_genes=True,
@@ -9143,15 +9182,16 @@
 # In[ ]:
 
 
 def PLOT_paired_T_vs_N(
     series_data, list_patients=None, alpha=0.3, linewidth=5, color_by_change=True
 ):
     """Plot data in 'series_data' (where index is Sample_IDs of paired samples) on categorical plots (Normal, Tumor) so that change from
-    tumor to normal can be tracked for individual patients with paired samples. Return fig and ax returned by plt.subplot"""
+    tumor to normal can be tracked for individual patients with paired samples. Return fig and ax returned by plt.subplot
+    """
     if (
         list_patients is None
     ):  # set default list_patients as all patients with paired samples
         list_patients = df_paired_samples.index.values
     else:
         list_patients = set(df_paired_samples.index).intersection(list_patients)
     arr_paired_samples = df_paired_samples.loc[
@@ -9277,15 +9317,16 @@
     method="kendalltau",
 ):
     """Calculate Spearman correlation coefficient (using NUMPY_spearman_correl) between var of in the given df, and return the result as a pandas DataFrame (square matrix)
     df, df_target will be aligned on the given 'axis' (by dafault, aligned )
     if 'df_target' is given, calculate Spearman correlation between df and df_target (index = indices of df, columns = indices of df_target). DataFrame with NaN values are acceptable, but when
     number of valid samples for a var pair is smaller than 'thres_minimum_n_samples', data_value will be np.nan
     when there is no np.nan values in a dataframe and thus there is no need for masking np.nan values, scipy.stats methods are used for calculaating correlation coefficient and p_values
-    'method' : a function name in scipy.stats module. if None is given, a default built-in custum function 'NUMPY_spearman_correl' will be used, which is significantly faster if number of observation is below 100 due to smaller overhead"""
+    'method' : a function name in scipy.stats module. if None is given, a default built-in custum function 'NUMPY_spearman_correl' will be used, which is significantly faster if number of observation is below 100 due to smaller overhead
+    """
     flag_symmetric = (
         True if df_target is None else False
     )  # set a flag to compute only half of a matrix if only one dataframe was given and thus correlation matrix is symmetric
     df_target = (
         df if df_target is None else df_target
     )  # set df as df_target if only one dataframe was given
     if (
@@ -9599,15 +9640,16 @@
     df,
     mask_xy_switched_tril,
     mask_tril,
     fill_diagnal_value,
     method_xy_switch=lambda a, b: a,
 ):
     """a fuction intended to be used in linear regression analysis for selecting values using given masks and makes symmetrix matrix, while filling diagnal entries with 'fill_diagnal_value'
-    'method_xy_switch' is used for calculating values when xy axes are switched (for example, df_slope needs lambda a, b : 1 / a ) 'a' = df, 'b' = a flag that is True when 'a' is df_xy_switched and not selected, False when 'a' is not switched and selected"""
+    'method_xy_switch' is used for calculating values when xy axes are switched (for example, df_slope needs lambda a, b : 1 / a ) 'a' = df, 'b' = a flag that is True when 'a' is df_xy_switched and not selected, False when 'a' is not switched and selected
+    """
     df_xy_switched_tril, df_tril = GET_dataframe_lower_triangle(
         method_xy_switch(df.transpose(), True)
     ), GET_dataframe_lower_triangle(
         df
     )  # retrive inverse (1/s) of slopes where x and y are switched  # remove data above the diagonal line to simplify conputation
     df_selected_tril = df_xy_switched_tril * mask_xy_switched_tril + df_tril * mask_tril
     df_selected_triu = deepcopy(df_selected_tril)
@@ -9821,30 +9863,32 @@
 
 
 # In[ ]:
 
 
 def NUMPY_GET_mean_std(data):
     """calculate mean and standard deviation of a given array of data using np.dot, which involves vector calculation (very fast). when number of elements is small (~100), this method is
-    3 times faster than applying data.mean() and data.std() separately.  calculate sample standard deviation (divided by N - 1 instead of N). return  mean, std"""
+    3 times faster than applying data.mean() and data.std() separately.  calculate sample standard deviation (divided by N - 1 instead of N). return  mean, std
+    """
     N = data.size
     mean = np.dot(data, np.ones(N)) / N
     deviation = data - mean
     std = np.sqrt(
         np.dot(deviation, deviation) / (N - 1)
     )  # calculate sample standard deviation (degree of freedom = 1)
     return mean, std
 
 
 # In[ ]:
 
 
 def NUMPY_spearman_correl(data_1, data_2):
     """Use np.argsort() and np.dot() to reduce computation time. When number of elements is small (~100), it is 50 times faster than scipy.stats.spearmanr method
-    Since np.argsort() give identical values distinct rank, this method can give incorrect spearman correlation coefficient if given data have identical values (for example, multiple zeros)"""
+    Since np.argsort() give identical values distinct rank, this method can give incorrect spearman correlation coefficient if given data have identical values (for example, multiple zeros)
+    """
     N = data_1.size
     rank_1 = (
         data_1.argsort().argsort()
     )  # retrive a rank of given data, assuming all there are no duplicates in the data
     rank_2 = data_2.argsort().argsort()
     diff_of_rank = rank_1 - rank_2
     return 1 - 6 * np.dot(diff_of_rank, diff_of_rank) / (
@@ -9853,15 +9897,16 @@
 
 
 # In[ ]:
 
 
 def NUMPY_least_square_linear_regress(x, y):
     """Perform simple linear regression (least square linear regression), which is implemented in scipy.stats.linregress. When number of elements is moderate ( < 10,000 ),
-    this method is 10 ~ 20 times faster than linregress method. (when n_elements = 100, its 20 times faster than linregress)"""
+    this method is 10 ~ 20 times faster than linregress method. (when n_elements = 100, its 20 times faster than linregress)
+    """
     N = x.size
     arr_ones = np.ones(N)
     sum_x, sum_y, sum_x2, sum_xy = (
         np.dot(arr_ones, x),
         np.dot(arr_ones, y),
         np.dot(x, x),
         np.dot(x, y),
@@ -10003,15 +10048,16 @@
 
 
 def DEVIATION_FROM_NORMAL_CORRELATION_calculation(
     df, Gene_Set=None, n_std_for_outliers=3.5
 ):
     """For each gene pair in Gene_Set (default : all genes in df), perform projection-based least square linear regression for normal data, while masking outliers outside 'n_std_for_outliers'
     from the mean, and calculate mean rejection (Tumor data only since mean rejection in Normal data is 0), standard deviation(std) of rejection, std of projection, correlation between rejections
-    and projections, correlation before projection (Correlation Matrix of df with Spearman's coefficient), and lastly, deviation from origin from the slope and intercept (same sign with intercept)."""
+    and projections, correlation before projection (Correlation Matrix of df with Spearman's coefficient), and lastly, deviation from origin from the slope and intercept (same sign with intercept).
+    """
     if Gene_Set is not None:
         df = PANDAS_Subset(df, Gene_Set)
     n_genes = len(df)
     data = df.values  # row = gene, col = sample
     Gene_IDs = df.index.values
 
     T_data, N_data = (
@@ -10194,15 +10240,16 @@
 # In[ ]:
 
 
 def DEVIATION_NORMAL_CORR_a_gene_pair_with_switching(
     gene_1, gene_2, df=None, n_std_for_outliers=3.5, mask_zero_with_nan=True
 ):
     """calculates 14 metrics for projection-based linear regression analysis for a given pair of genes on 'df' data using 'DEVIATION_NORMAL_CORR_a_gene_pair' method.
-    Return dataframe summarizing the results (swithced and not switched). If 'mask_zero_with_nan' is True, replace near-zero values with np.nan"""
+    Return dataframe summarizing the results (swithced and not switched). If 'mask_zero_with_nan' is True, replace near-zero values with np.nan
+    """
     s_gene_pair = DEVIATION_NORMAL_CORR_a_gene_pair(
         gene_1=gene_1, gene_2=gene_2, df=df, n_std_for_outliers=n_std_for_outliers
     )
     s_gene_pair_switched = DEVIATION_NORMAL_CORR_a_gene_pair(
         gene_1=gene_2, gene_2=gene_1, df=df, n_std_for_outliers=n_std_for_outliers
     )
     df = pd.DataFrame(
@@ -10310,15 +10357,16 @@
 
 
 def LINREGRESS_OPTIMIZE_search_slope_with_minumun_std_of_rejections(
     x, y, x_y_centered, num_probing=5, num_repeat=3
 ):
     """by using double for loop, search a slope that gives minimal standard deviation of rejections for a given data ('x_y_centered').
     in a search space, 'num_probing' number of search points were searched, and magnify the search space, and repeat the search for 'num_repeat' times
-    about 3 times faster than Scipy.optimum.fmin function, though this function is less accurate than the function"""
+    about 3 times faster than Scipy.optimum.fmin function, though this function is less accurate than the function
+    """
     initial_slopes = (
         NUMPY_least_square_linear_regress(x, y)[0],
         1 / NUMPY_least_square_linear_regress(y, x)[0],
     )  # retrive initial slopes using least square linear regression methods
     lower_slope, upper_slope = sorted(
         initial_slopes
     )  # retrive lower and upper slope for setting points in search space using np.arange
@@ -10577,15 +10625,16 @@
 # In[ ]:
 
 
 def TCGA_CALCULATE_KaplanMeierCurve_log_rank_p_value_of_all_genes_in_dataframe(
     df, Gene_Set=None, df_clinical=None, cut_ratio=0.25
 ):
     """For each genes in df (or a subset of df if a 'Gene_Set' is given), calculate log rang p_values for data of 'days_to_death' column in df_clinical (default : df_patients) between
-    two groups of patients, one group with upper n percent and another group with lower n percent of the data given by df"""
+    two groups of patients, one group with upper n percent and another group with lower n percent of the data given by df
+    """
     if df_clinical is None:  # set default df_clinical
         df_clinical = df_patients
     if Gene_Set is not None:  # if 'Gene_Set' is given, subset df with a given Gene_Set
         df = PANDAS_Subset(df, Gene_Set)
     df = df[T_samples]  # select only Tumor samples
     str_percent = str(int(round(cut_ratio * 100, 0)))
     data_1_name, data_2_name = "lower_{}_percent".format(
@@ -10655,15 +10704,16 @@
     df_clinical=None,
     cut_ratio=0.25,
     graph_folder=None,
     save_fig=False,
     show_fig=False,
 ):
     """For a given gene, draw a KaplanMeierCurve between two groups of patients in df_clinical (default : df_patients), one group with upper n percent and another group with lower n percent of the data given by df
-    (default : df_rna). 'show_fig' : if both 'save_fig' and 'show_fig' are True, show the plot, and if 'save_fig' is False, always show the plot"""
+    (default : df_rna). 'show_fig' : if both 'save_fig' and 'show_fig' are True, show the plot, and if 'save_fig' is False, always show the plot
+    """
     if df_clinical is None:  # set default df_clinical
         df_clinical = df_patients
     if df is None:
         df = df_rna
     Gene_ID = Gene_2_Gene_ID(Gene)  # retrive Gene_ID from a given Gene
     if Gene_ID not in df.index.values:
         return -1
@@ -11040,15 +11090,16 @@
     dict_cell_line_set=None,
     gene_for_rna=None,
     size_factor=1,
     thres_n_cell_line=5,
     show_legend=True,
 ):
     """Visualize Gene_Dependency data along with RNA data. bubble size indicates RNA amount (linear), and can be adjusted by 'size_factor'. Sort cell_line_set according to its median gene_dependency
-    value, while excluding cell_line_set if a subset contain less than 'thres_n_cell_line' entries, 'gene_for_rna' : Gene symbol for gene used for retriving RNA-Seq data. by default, the given gene for retriving GD Data"""
+    value, while excluding cell_line_set if a subset contain less than 'thres_n_cell_line' entries, 'gene_for_rna' : Gene symbol for gene used for retriving RNA-Seq data. by default, the given gene for retriving GD Data
+    """
     if dict_cell_line_set is None:
         dict_cell_line_set = dict_ccle__cell_line_sets
     df = (
         df_crispr_gd if data_type.lower() == "crispr" else df_rnai_gd
     )  # set df according to 'data_type'
     Gene_ID, Gene_Symbol = GET_Gene_ID_and_Symbol_from_input_gene(Gene)
     geneid_for_rna = Gene_ID if gene_for_rna is None else Gene_2_Gene_ID(gene_for_rna)
@@ -11448,15 +11499,16 @@
 
 
 # In[ ]:
 
 
 def CRBNPROT_Decompress_metadata(df=None, data_labels=None):
     """Decompress metadata and Create metadata dataframe from columns of the given dataframe containing CRBN_Proteomic profiling dataset. Also see CRBNPROT_Compress_metadata
-    Default data_labels : [ 'Value_Type', 'Data_Type', 'Experiment_System', 'Condition_A', 'Condition_B', 'Replicate', 'Data_Source' ]"""
+    Default data_labels : [ 'Value_Type', 'Data_Type', 'Experiment_System', 'Condition_A', 'Condition_B', 'Replicate', 'Data_Source' ]
+    """
     data_labels = (
         [
             "Value_Type",
             "Data_Type",
             "Experiment_System",
             "Condition_A",
             "Condition_B",
@@ -11475,15 +11527,16 @@
 
 
 # In[ ]:
 
 
 def CRBNPROT_Compress_metadata(df=None, data_labels=None):
     """Compress metadata in the given metadata dataframe (default, df_crbnprot_meta_assays) according to data_labels and return list of labels containing compressed metadata.
-    Default data_labels : [ 'Value_Type', 'Data_Type', 'Experiment_System', 'Condition_A', 'Condition_B', 'Replicate', 'Data_Source' ]. Also see CRBNPROT_Decompress_metadata"""
+    Default data_labels : [ 'Value_Type', 'Data_Type', 'Experiment_System', 'Condition_A', 'Condition_B', 'Replicate', 'Data_Source' ]. Also see CRBNPROT_Decompress_metadata
+    """
     data_labels = (
         [
             "Value_Type",
             "Data_Type",
             "Experiment_System",
             "Condition_A",
             "Condition_B",
@@ -12188,15 +12241,16 @@
 
 
 # from collections import defaultdict
 
 
 def Substring_allow_mismatch(pattern, text):
     """Return True if pattern exist in text allowing upto one mismatch.
-    source : https://stackoverflow.com/questions/2420412/search-for-string-allowing-for-one-mismatch-in-any-location-of-the-string"""
+    source : https://stackoverflow.com/questions/2420412/search-for-string-allowing-for-one-mismatch-in-any-location-of-the-string
+    """
     m = len(pattern)
     S_table = defaultdict(int)
     for i, c in enumerate(pattern):
         S_table[c] |= 1 << i
     R0 = 0
     R1 = 0
     mask = 1 << (m - 1)
@@ -12995,15 +13049,16 @@
     seq,
     start=0,
     append_stop_codon_to_returned_seq=False,
     print_message=True,
     return_error_value_if_stop_codon_not_found=True,
 ):
     """Translate nucleotide sequence until the given seq is end or stop codons are encountered.
-    start = 0 : start position for potential protein sequence (for example, start of ATG start codon.)"""
+    start = 0 : start position for potential protein sequence (for example, start of ATG start codon.)
+    """
     if type(seq) is float:
         return np.nan  # if input is invalid, return np.nan
     length_seq = len(seq)  # it seems the time complexity of the len(str) method is O(1)
     l_aa = list()
     while True:
         if start + 3 > length_seq:
             if print_message:
@@ -13070,15 +13125,16 @@
 
 
 # 2020-05-29 14:28:22
 def NGS_SEQ_ORF_Find_All_Methionine_ORFs_on_Both_Strands(
     seq, use_1_based_coordinate=True
 ):
     """Find all ORFs start with methionine on both strand of the given sequence by using 'NGS_SEQ_ORF_Find_All_Methionine_ORFs'.
-    use 1-based-coordinate for start and end positions if 'use_1_based_coordinate' is set to True"""
+    use 1-based-coordinate for start and end positions if 'use_1_based_coordinate' is set to True
+    """
     df_plus = NGS_SEQ_ORF_Find_All_Methionine_ORFs(
         seq
     )  # find all ORFs in the sequence and the reverse complement of the sequence
     df_minus = NGS_SEQ_ORF_Find_All_Methionine_ORFs(NGS_SEQ_Reverse_Complement(seq))
     df_plus["strand"] = "+"
     df_minus["strand"] = "-"
     int_length_seq = len(
@@ -13105,15 +13161,16 @@
     seq,
     from_3_prime_end=True,
     return_length_of_polyA=False,
     str_repeated_base="A",
     int_lookup_window=3,
 ):
     """Trim PolyA sequence from the 3' end of a given sequence (DNA sequence in upper characters) if 'from_3_prime_end' is True or trim polyA from 5' end of the sequence if 'from_3_prime_end' is False
-    if the program encounter base other than 'A', lookup next 'int_lookup_window' number of bases and check weather they are consecutive 'A' bases."""
+    if the program encounter base other than 'A', lookup next 'int_lookup_window' number of bases and check weather they are consecutive 'A' bases.
+    """
     if len(seq) == 0:  # if the given seq is empty
         if return_length_of_polyA:
             return 0
         else:
             return ""
     str_repeated_bases_in_lookup_window = str_repeated_base * int_lookup_window
     seq_polyA_at_5_prime_end = seq[::-1] if from_3_prime_end else seq
@@ -13388,15 +13445,16 @@
         return dict_header_to_seq
 
 
 def FASTA_Assembly_Stats(
     dict_fasta=None, arr_length=None, flag_arr_length_is_sorted=False
 ):
     """# 2021-09-15 21:52:44
-    return assembly stats for the given fasta file (fasta file containing assembed contigs)"""
+    return assembly stats for the given fasta file (fasta file containing assembed contigs)
+    """
     if dict_fasta is not None:
         dict_fasta = (
             FASTA_Read(dict_fasta) if isinstance(dict_fasta, (str)) else dict_fasta
         )  # read fasta file if path (string) is given, or use given dictionary as a 'dict_fasta'
         int_n_records = len(dict_fasta)
         arr_length = np.zeros(int_n_records)
         for index, header in enumerate(dict_fasta):
@@ -14334,15 +14392,16 @@
                 e.split(" ", 1)[0][1:] for e in df_fq.readname.values
             )  # retrieve qname
         return df_fq
 
 
 def FASTQ_Read_Generator(path_file, return_only_at_index=None):  # 2020-08-18 22:31:31
     """read a given fastq file into list of sequences or a dataframe (gzipped fastq file supported). 'return_only_at_index' is a value between 0 and 3 (0 = readname, 1 = seq, ...)
-    return a generator that return a tuple of 3 length (name, sequence, and quality) or a value at the index given by "return_only_at_index"."""
+    return a generator that return a tuple of 3 length (name, sequence, and quality) or a value at the index given by "return_only_at_index".
+    """
     if return_only_at_index is not None:
         return_only_at_index = (
             return_only_at_index % 4
         )  # 'return_only_at_index' value should be a value between 0 and 3
     bool_flag_file_gzipped = (
         ".gz" in path_file[-3:]
     )  # set a flag indicating whether a file has been gzipped.
@@ -14364,15 +14423,16 @@
 
 # In[ ]:
 
 
 def FASTQ_Write(path_file, dict_seq=None, dict_quality=None, df_fastq=None):
     """
     # 2021-03-07 15:53:19
-    Write FASTQ file with given dataframe or a pair of dict_seq and dict_quality (keys of both dictionaries should be the same)"""
+    Write FASTQ file with given dataframe or a pair of dict_seq and dict_quality (keys of both dictionaries should be the same)
+    """
     if dict_seq is None or dict_quality is None:
         if df_fastq is None:
             print("required inputs are not given, exiting")
             return -1
         else:  # retrieve dictionary of sequences and quality from the dataframe
             df = df_fastq.set_index("readname")
             dict_seq = df.seq.to_dict()
@@ -15081,15 +15141,16 @@
 
 
 # In[ ]:
 
 
 def HMMER_Read_nhmmer_output_with_alignment(path_file):
     """# 2021-02-04 11:20:08
-    Read nhmmer output file with alignment information. read search summary, alignments, and return two dataframes containing the summary and alignment result"""
+    Read nhmmer output file with alignment information. read search summary, alignments, and return two dataframes containing the summary and alignment result
+    """
     bool_flag_new_alignment_start = False  # in case that there is no alignment
     with open(path_file) as file:
         l_l_value__search_result = list()
         l_l_value__alignment_result = list()
         while (
             True
         ):  # retrive a directory to a file containing HMM database in the header
@@ -15974,15 +16035,16 @@
 
 
 # In[ ]:
 
 
 def CIF_Write(path_file, dict_cif):  # 2020-07-13 23:05:05
     """write CIF file in the given 'dict_cif'.
-    *the output file closely resembles standard CIF file, but it does not have line length limit (no value spans multiple lines enclosed by semicolons ';'). This will prevent some CIF readers, such as mkdssp or chimera from reading the metadata (not 3D coordinate data). Therefore, saving only 'atom_site' category is recommended"""
+    *the output file closely resembles standard CIF file, but it does not have line length limit (no value spans multiple lines enclosed by semicolons ';'). This will prevent some CIF readers, such as mkdssp or chimera from reading the metadata (not 3D coordinate data). Therefore, saving only 'atom_site' category is recommended
+    """
     with open(path_file, "w") as file:
         for str_name_data_block in dict_cif:  # for each data block
             dict_data_block = dict_cif[str_name_data_block]
             file.write("data_" + str_name_data_block + "\n")
             for str_name_category in dict_data_block:  # for each category
                 file.write("#\n")
                 data = dict_data_block[
```

### Comparing `biobookshelf-0.2.3/biobookshelf.egg-info/PKG-INFO` & `biobookshelf-0.2.4/biobookshelf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.3
+Version: 0.2.4
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.3/biobookshelf.egg-info/SOURCES.txt` & `biobookshelf-0.2.4/biobookshelf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.3/setup.py` & `biobookshelf-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="biobookshelf",
-    version="0.2.3",
+    version="0.2.4",
     author="Hyunsu An",
     author_email="ahs2202@gm.gist.ac.kr",
     description="a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ahs2202/biobookshelf",
     license="GPLv3",
```

