# Comparing `tmp/gene-ranking-shootout-0.0.0.tar.gz` & `tmp/gene-ranking-shootout-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene-ranking-shootout-0.0.0.tar", last modified: Fri May  5 12:49:08 2023, max compression
+gzip compressed data, was "gene-ranking-shootout-0.1.1.tar", last modified: Fri May  5 13:03:23 2023, max compression
```

## Comparing `gene-ranking-shootout-0.0.0.tar` & `gene-ranking-shootout-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/gene_ranking_shootout/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/gene_ranking_shootout/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 12:49:08.000000 gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 12:49:08.657445 gene-ranking-shootout-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 12:49:03.000000 gene-ranking-shootout-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.495921 gene-ranking-shootout-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.495921 gene-ranking-shootout-0.1.1/docker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/docker/cada/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/docker/cada/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/docker/cada/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/gene_ranking_shootout/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/gene_ranking_shootout/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1439512 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_all_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)   292840 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_cases_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)   871083 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_cases_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)   286957 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_cases_validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)   758682 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_clinvar_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)   680832 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/cada_collaborator_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1546549 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/data/gnomad_counts.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.499921 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 13:03:23.000000 gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-05 13:03:23.511921 gene-ranking-shootout-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.495921 gene-ranking-shootout-0.1.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/tests/data/amelie/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/amelie/query.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/amelie/response.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/tests/data/cada/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/cada/query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/cada/result.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:23.507921 gene-ranking-shootout-0.1.1/tests/data/phen2gene/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/phen2gene/genes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/phen2gene/output_file.associated_gene_list
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/data/phen2gene/terms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 13:03:08.000000 gene-ranking-shootout-0.1.1/tests/test_example.py
```

### Comparing `gene-ranking-shootout-0.0.0/LICENSE` & `gene-ranking-shootout-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.0.0/PKG-INFO` & `gene-ranking-shootout-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-ranking-shootout
-Version: 0.0.0
+Version: 0.1.1
 Summary: Compare gene ranking methods.
 Home-page: https://github.com/bihealth/gene-ranking-shootout
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 Keywords: genes,ranking
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gene-ranking-shootout-0.0.0/README.md` & `gene-ranking-shootout-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.0.0/gene_ranking_shootout/cli/__init__.py` & `gene-ranking-shootout-0.1.1/gene_ranking_shootout/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.0.0/gene_ranking_shootout/models.py` & `gene-ranking-shootout-0.1.1/gene_ranking_shootout/models.py`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.0.0/gene_ranking_shootout/runner.py` & `gene-ranking-shootout-0.1.1/gene_ranking_shootout/runner.py`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.0.0/gene_ranking_shootout.egg-info/PKG-INFO` & `gene-ranking-shootout-0.1.1/gene_ranking_shootout.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-ranking-shootout
-Version: 0.0.0
+Version: 0.1.1
 Summary: Compare gene ranking methods.
 Home-page: https://github.com/bihealth/gene-ranking-shootout
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 Keywords: genes,ranking
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gene-ranking-shootout-0.0.0/setup.cfg` & `gene-ranking-shootout-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 	ranking
 
 [options]
 packages = find:
 python_requires = >= 3.8
 include_package_data = True
 zip_safe = false
+setup_requires = 
+	setuptools_scm
 install_requires = 
 	attrs
 	cattrs
 	click
 	loguru
 	numpy
 	requests
```

