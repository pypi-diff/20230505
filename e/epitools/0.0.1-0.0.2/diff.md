# Comparing `tmp/epitools-0.0.1.tar.gz` & `tmp/epitools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epitools-0.0.1.tar", last modified: Thu May  4 14:52:36 2023, max compression
+gzip compressed data, was "epitools-0.0.2.tar", last modified: Fri May  5 08:52:39 2023, max compression
```

## Comparing `epitools-0.0.1.tar` & `epitools-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.510030 epitools-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.494029 epitools-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.498029 epitools-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-04 14:52:23.000000 epitools-0.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 14:52:23.000000 epitools-0.0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-04 14:52:23.000000 epitools-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 14:52:23.000000 epitools-0.0.1/.github/workflows/update_project_board.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-04 14:52:23.000000 epitools-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.498029 epitools-0.0.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 14:52:23.000000 epitools-0.0.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-04 14:52:23.000000 epitools-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-04 14:52:23.000000 epitools-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-04 14:52:36.510030 epitools-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 14:52:23.000000 epitools-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-04 14:52:23.000000 epitools-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.498029 epitools-0.0.1/sample_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.498029 epitools-0.0.1/sample_data/8bitDataset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.506029 epitools-0.0.1/sample_data/8bitDataset/Benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)   223226 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/ProjIm.mat
--rw-r--r--   0 runner    (1001) docker     (123)   219365 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/RegIm.mat
--rw-r--r--   0 runner    (1001) docker     (123)   289918 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/RegIm_wClahe.mat
--rw-r--r--   0 runner    (1001) docker     (123)  3105836 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/SegResults.mat
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/Surfaces.mat
--rw-r--r--   0 runner    (1001) docker     (123)   310533 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/Benchmark/TrackingStart.mat
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/test_image-projected-segmented-seeds.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/test_image-projected-segmented-stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/test_image-projected-segmented.tif
--rw-r--r--   0 runner    (1001) docker     (123)   329123 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/test_image-projected.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1314231 2023-05-04 14:52:23.000000 epitools-0.0.1/sample_data/8bitDataset/test_image.tif
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:52:36.510030 epitools-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.498029 epitools-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.506029 epitools-0.0.1/src/epitools/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.510030 epitools-0.0.1/src/epitools/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/analysis/_skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/analysis/cell_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/analysis/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/analysis/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.510030 epitools-0.0.1/src/epitools/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/widgets/cell_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/widgets/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-04 14:52:23.000000 epitools-0.0.1/src/epitools/widgets/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.510030 epitools-0.0.1/src/epitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 14:52:36.000000 epitools-0.0.1/src/epitools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:36.510030 epitools-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:23.000000 epitools-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-04 14:52:23.000000 epitools-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-04 14:52:23.000000 epitools-0.0.1/tests/test_cell_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 14:52:23.000000 epitools-0.0.1/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-04 14:52:23.000000 epitools-0.0.1/tests/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.973196 epitools-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.957196 epitools-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.957196 epitools-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 08:52:20.000000 epitools-0.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 08:52:20.000000 epitools-0.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-05 08:52:20.000000 epitools-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 08:52:20.000000 epitools-0.0.2/.github/workflows/update_project_board.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-05 08:52:20.000000 epitools-0.0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.957196 epitools-0.0.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-05 08:52:20.000000 epitools-0.0.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-05 08:52:20.000000 epitools-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-05 08:52:20.000000 epitools-0.0.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-05 08:52:39.973196 epitools-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-05 08:52:20.000000 epitools-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-05 08:52:20.000000 epitools-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.957196 epitools-0.0.2/sample_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.961196 epitools-0.0.2/sample_data/8bitDataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.969196 epitools-0.0.2/sample_data/8bitDataset/Benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)   223226 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/ProjIm.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   219365 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/RegIm.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   289918 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/RegIm_wClahe.mat
+-rw-r--r--   0 runner    (1001) docker     (123)  3105836 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/SegResults.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/Surfaces.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   310533 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/Benchmark/TrackingStart.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/test_image-projected-segmented-seeds.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/test_image-projected-segmented-stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   165124 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/test_image-projected-segmented.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   329123 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/test_image-projected.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1314231 2023-05-05 08:52:20.000000 epitools-0.0.2/sample_data/8bitDataset/test_image.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:52:39.973196 epitools-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.957196 epitools-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.969196 epitools-0.0.2/src/epitools/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.969196 epitools-0.0.2/src/epitools/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/analysis/cell_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/analysis/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/analysis/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.969196 epitools-0.0.2/src/epitools/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/widgets/cell_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/widgets/dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/widgets/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-05 08:52:20.000000 epitools-0.0.2/src/epitools/widgets/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.969196 epitools-0.0.2/src/epitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 08:52:39.000000 epitools-0.0.2/src/epitools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:39.973196 epitools-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/test_cell_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/test_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-05 08:52:20.000000 epitools-0.0.2/tests/test_segmentation.py
```

### Comparing `epitools-0.0.1/.github/workflows/deploy.yml` & `epitools-0.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/.github/workflows/linting.yml` & `epitools-0.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/.github/workflows/test.yml` & `epitools-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/.gitignore` & `epitools-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/.napari/DESCRIPTION.md` & `epitools-0.0.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/.pre-commit-config.yaml` & `epitools-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/PKG-INFO` & `epitools-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 Metadata-Version: 2.1
 Name: epitools
-Version: 0.0.1
+Version: 0.0.2
 Summary: EpiTools Plugin
-Author-email: Napari Developer <yourname@example.com>
-License: 
-        Copyright (c) 2022, Napari Developer
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of epitools nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Author-email: "Daniel R. Matthews" <d.matthews@ucl.ac.uk>, Giulia Paci <g.paci@ucl.ac.uk>, "Pablo V. Munuera" <p.munuera@ucl.ac.uk>, "Patrick J. Roddy" <patrick.roddy@ucl.ac.uk>, "Paul J. Smith" <paul.j.smith@ucl.ac.uk>, Yanlan Mao <y.mao@ucl.ac.uk>
+License: BSD 3-Clause Licence
         
-Classifier: Development Status :: 2 - Pre-Alpha
+        Copyright (c) 2022-2023, EpiTools Developers All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+            Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+            Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+            Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Code, https://github.com/epitools/epitools
+Project-URL: Download, https://pypi.org/project/epitools
+Project-URL: Homepage, https://github.com/epitools/epitools
+Project-URL: Issues, https://github.com/epitools/epitools/issues
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -45,72 +33,44 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pyqt
 Provides-Extra: pyside
 Provides-Extra: qt
-License-File: LICENSE
+License-File: LICENCE.md
 
-# epitools
+# EpiTools
 
-[![License](https://img.shields.io/pypi/l/epitools.svg?color=green)](https://raw.githubusercontent.com/epitools/epitools/main/LICENSE)
+[![Licence](https://img.shields.io/pypi/l/epitools.svg?color=green)](https://raw.githubusercontent.com/epitools/epitools/main/LICENCE.md)
 [![PyPI](https://img.shields.io/pypi/v/epitools.svg?color=green)](https://pypi.org/project/epitools)
 [![Python Version](https://img.shields.io/pypi/pyversions/epitools.svg?color=green)](https://python.org)
 [![tests](https://github.com/epitools/epitools/actions/workflows/test.yml/badge.svg)](https://github.com/epitools/epitools/actions/workflows/test.yml)
 [![coverage](https://coveralls.io/repos/github/epitools/epitools/badge.svg?branch=main)](https://coveralls.io/github/epitools/epitools?branch=main)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/epitools)](https://napari-hub.org/plugins/epitools)
 
-EpiTools Plugin
-
----
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/index.html
--->
-
 ## Installation
 
-`epitools` is not yet available to install from PyPI or napari-hub.
-
-To install, please clone the repository and do a local install using `pip`:
+The recommended way to install `EpiTools` is via
+[pip](https://pypi.org/project/pip)
 
+```sh
+python -m pip install epitools
 ```
-git clone https://github.com/epitools/epitools.git
-cd epitools
-python -m pip install .
-```
-
-## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
+To install the latest development version of `EpiTools` clone this repository
+and run
 
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"epitools" is free and open source software
+```sh
+python -m pip install -e .
+```
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please
+[file an issue](https://github.com/epitools/epitools/issues) along with a
+detailed description.
+
+## Contributing
 
-[napari]: https://github.com/napari/napari
-[cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[mit]: http://opensource.org/licenses/MIT
-[bsd-3]: http://opensource.org/licenses/BSD-3-Clause
-[gnu gpl v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[gnu lgpl v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[apache software license 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[mozilla public license 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[pypi]: https://pypi.org/
+Contributions are very welcome. Tests can be run with [tox](https://tox.wiki),
+please ensure the coverage at least stays the same before you submit a pull request.
```

### Comparing `epitools-0.0.1/pyproject.toml` & `epitools-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 requires = [
     "setuptools",
     "setuptools-scm",
 ]
 
 [project]
 authors = [
-    {email = "yourname@example.com", name = "Napari Developer"},
+    {email = "d.matthews@ucl.ac.uk", name = "Daniel R. Matthews"},
+    {email = "g.paci@ucl.ac.uk", name = "Giulia Paci"},
+    {email = "p.munuera@ucl.ac.uk", name = "Pablo V. Munuera"},
+    {email = "patrick.roddy@ucl.ac.uk", name = "Patrick J. Roddy"},
+    {email = "paul.j.smith@ucl.ac.uk", name = "Paul J. Smith"},
+    {email = "y.mao@ucl.ac.uk", name = "Yanlan Mao"},
 ]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
     "Framework :: napari",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
@@ -36,34 +40,31 @@
 description = "EpiTools Plugin"
 dynamic = [
     "version",
 ]
 name = "epitools"
 optional-dependencies = {dev = [
     "black",
-    "flake8",
-    "isort",
-    "napari",
+    "mypy",
     "pre-commit",
     "pyqt5",
-    "pytest",
-    "pytest-cov",
-    "pytest-qt",
+    "ruff",
     "tox",
 ], pyqt = [
     "PyQt5 >= 5.12.3, != 5.15.0",
 ], pyside = [
     "PySide2 >= 5.13.2, != 5.15.0",
 ], qt = [
     "epitools[pyside]",
 ]}
 readme = "README.md"
 requires-python = ">=3.9"
+urls = {Code = "https://github.com/epitools/epitools", Download = "https://pypi.org/project/epitools", Homepage = "https://github.com/epitools/epitools", Issues = "https://github.com/epitools/epitools/issues"}
 entry-points."napari.manifest".epitools = "epitools:napari.yaml"
-license.file = "LICENSE"
+license.file = "LICENCE.md"
 
 [tool.coverage]
 report = {skip_covered = true, sort = "cover"}
 run = {branch = true, parallel = true, source = [
     "epitools",
 ]}
 paths.source = [
@@ -118,14 +119,15 @@
     "SIM",
     "T",
     "TID",
     "UP",
     "W",
     "YTT",
 ]
+target-version = "py39"
 isort.known-first-party = [
     "epitools",
 ]
 isort.section-order = [
     "future",
     "standard-library",
     "third-party",
@@ -136,14 +138,16 @@
 isort.sections.napari = [
     "magicgui",
     "napari",
 ]
 mccabe.max-complexity = 18
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
+write_to = "src/epitools/_version.py"
 
 [tool.tomlsort]
 all = true
 spaces_indent_inline_array = 4
 trailing_comma_inline_array = true
 overrides."project.classifiers".inline_arrays = false
 overrides."tool.coverage.paths.source".inline_arrays = false
```

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/ProjIm.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/ProjIm.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/RegIm.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/RegIm.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/RegIm_wClahe.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/RegIm_wClahe.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/SegResults.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/SegResults.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/Surfaces.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/Surfaces.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/Benchmark/TrackingStart.mat` & `epitools-0.0.2/sample_data/8bitDataset/Benchmark/TrackingStart.mat`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/test_image-projected-segmented-seeds.npy` & `epitools-0.0.2/sample_data/8bitDataset/test_image-projected-segmented-seeds.npy`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/test_image-projected-segmented-stats.csv` & `epitools-0.0.2/sample_data/8bitDataset/test_image-projected-segmented-stats.csv`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/sample_data/8bitDataset/test_image-projected.tif` & `epitools-0.0.2/sample_data/8bitDataset/test_image-projected.tif`

 * *Files 0% similar despite different names*

```diff
@@ -20523,17 +20523,17 @@
 000502a0: 7474 703a 2f2f 7777 772e 6f70 656e 6d69  ttp://www.openmi
 000502b0: 6372 6f73 636f 7079 2e6f 7267 2f53 6368  croscopy.org/Sch
 000502c0: 656d 6173 2f4f 4d45 2f32 3031 362d 3036  emas/OME/2016-06
 000502d0: 2068 7474 703a 2f2f 7777 772e 6f70 656e   http://www.open
 000502e0: 6d69 6372 6f73 636f 7079 2e6f 7267 2f53  microscopy.org/S
 000502f0: 6368 656d 6173 2f4f 4d45 2f32 3031 362d  chemas/OME/2016-
 00050300: 3036 2f6f 6d65 2e78 7364 2220 5555 4944  06/ome.xsd" UUID
-00050310: 3d22 7572 6e3a 7575 6964 3a38 3861 3933  ="urn:uuid:88a93
-00050320: 6330 382d 6539 3963 2d31 3165 642d 3938  c08-e99c-11ed-98
-00050330: 3564 2d61 6364 6534 3830 3031 3132 3222  5d-acde48001122"
+00050310: 3d22 7572 6e3a 7575 6964 3a38 3339 6633  ="urn:uuid:839f3
+00050320: 6632 342d 6561 3961 2d31 3165 642d 3964  f24-ea9a-11ed-9d
+00050330: 3639 2d61 6364 6534 3830 3031 3132 3222  69-acde48001122"
 00050340: 2020 4372 6561 746f 723d 2250 6172 7453    Creator="PartS
 00050350: 6567 223e 3c49 6d61 6765 2049 443d 2249  eg"><Image ID="I
 00050360: 6d61 6765 3a30 2220 4e61 6d65 3d22 496d  mage:0" Name="Im
 00050370: 6167 6522 3e3c 5069 7865 6c73 2049 443d  age"><Pixels ID=
 00050380: 2250 6978 656c 733a 3022 2044 696d 656e  "Pixels:0" Dimen
 00050390: 7369 6f6e 4f72 6465 723d 2258 5943 5a54  sionOrder="XYCZT
 000503a0: 2220 5479 7065 3d22 646f 7562 6c65 2220  " Type="double"
```

### Comparing `epitools-0.0.1/sample_data/8bitDataset/test_image.tif` & `epitools-0.0.2/sample_data/8bitDataset/test_image.tif`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools/_reader.py` & `epitools-0.0.2/src/epitools/_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,19 +87,18 @@
     loader = PartSegCore.analysis.load_functions.LoadStackImage()
     image_stack = loader.load(load_locations=paths)
 
     image_layers = PartSegCore.napari_plugins.loader.project_to_layers(
         project_info=image_stack,
     )
 
+    # Add the YX pixel spacing for all layers - we need this for regionprops
+    # calculations
+    # The slice [-2:] is taken as this corresponds to ZYX[-2:]
     for layer in image_layers:
         layer_data, layer_kwargs, layer_type = layer
         layer_kwargs["metadata"] = {
-            "scale": np.asarray(
-                layer_kwargs.pop("scale")
-            ),  # don't scale the image in the viewer
-            "spacing": np.asarray(
-                image_stack.image.spacing
-            ),  # we need this for regionprops
+            "yx_spacing": np.asarray(
+                image_stack.image.spacing[-2:],
+            ),
         }
-
     return image_layers
```

### Comparing `epitools-0.0.1/src/epitools/_sample_data.py` & `epitools-0.0.2/src/epitools/_sample_data.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools/analysis/cell_statistics.py` & `epitools-0.0.2/src/epitools/analysis/cell_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 import skimage.measure
 
 import napari
 
 logger = logging.getLogger(__name__)
 
 
+FOUR_DIMENSIONAL = 4
+
+
 def calculate_cell_statistics(
     image: napari.types.ImageData,
     labels: napari.types.LabelsData,
     pixel_spacing: tuple[float],
 ) -> tuple[list[dict[str, npt.NDArray]], list[skimage.graph.RAG]]:
     """Calculate the region based properties of a segmented image"""
 
@@ -51,14 +54,18 @@
     labels: napari.types.LabelsData,
     pixel_spacing: tuple[float],
 ) -> list[dict[str, npt.NDArray]]:
     """Calculate cell properties using skimage regionprops"""
 
     properties = ["label", "area", "perimeter", "orientation"]
 
+    # remove z axis if necessary
+    image = image[:, 0] if image.ndim == FOUR_DIMENSIONAL else image
+    labels = labels[:, 0] if labels.ndim == FOUR_DIMENSIONAL else labels
+
     cell_statistics = [
         skimage.measure.regionprops_table(
             label_image=frame_labels,
             intensity_image=frame_image,
             properties=properties,
             spacing=pixel_spacing,
         )
```

### Comparing `epitools-0.0.1/src/epitools/analysis/projection.py` & `epitools-0.0.2/src/epitools/analysis/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 import numpy.typing as npt
 from scipy.interpolate import griddata
 from skimage.filters import gaussian
 
 THREE_DIMENSIONAL = 3
+SINGLE_SLICE = 1
 
 
 def _smooth(
     img: npt.NDArray[np.float64], smoothing_radius: float = 0.3
 ) -> npt.NDArray[np.float64]:
     """Gaussian smoothing of each z plane in the image stack
 
@@ -116,15 +117,17 @@
         # Assume we have a stack of images at a single point in time (ZYX)
         # Expand so we have TZYX
         input_image = np.expand_dims(input_image, axis=0)
 
     t_size, z_size, y_size, x_size = input_image.shape
     smoothed_imstack = _smooth(input_image.astype(np.float64), smoothing_radius)
 
-    t_interp = np.zeros((t_size, y_size, x_size))  # remove the z-axis when projecting
+    # We will always have a single slice in the Z dimension
+    t_interp = np.zeros((t_size, SINGLE_SLICE, y_size, x_size))
+
     for t in range(t_size):
         smoothed_t = smoothed_imstack[t]
         max_intensity = smoothed_t.max(axis=0)
         max_indices = smoothed_t.argmax(axis=0)
 
         confidencemap = z_size * max_intensity / np.sum(smoothed_t, axis=0)
         np.nan_to_num(confidencemap, copy=False)
```

### Comparing `epitools-0.0.1/src/epitools/analysis/segmentation.py` & `epitools-0.0.2/src/epitools/analysis/segmentation.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools/main.py` & `epitools-0.0.2/src/epitools/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ]
 
 logger = logging.getLogger(__name__)
 
 
 THREE_DIMENSIONAL = 3  # ZYX
 FOUR_DIMENSIONAL = 4  # TZYX
+DEFAULT_PIXEL_SPACING = (1e-6, 1e-6)  # 1 um
 
 
 def create_projection_widget() -> magicgui.widgets.Container:
     """Create a widget to project a 4d timeseries (TZYX) along the z dimension"""
 
     projection_widget = epitools.widgets.create_projection_widget()
 
@@ -61,41 +62,23 @@
         image.data,
         smoothing_radius,
         surface_smoothness_1,
         surface_smoothness_2,
         cutoff_distance,
     )
 
-    # Remove z dimension from scale and translate arrays
-    if image.ndim == THREE_DIMENSIONAL:  # ZYX
-        mask = [1, 2]
-    elif image.ndim == FOUR_DIMENSIONAL:  # TZYX
-        mask = [0, 2, 3]
-
-    two_d_scale = image.metadata["scale"][mask]
-    two_d_translate = np.asarray(image.translate)[mask]
-
-    # spacing for regionprops
-    two_d_spacing = (
-        image.metadata["spacing"]
-        if image.ndim == THREE_DIMENSIONAL
-        else image.metadata["spacing"][1:]
-    )
-
-    two_d_metadata = {
-        "scale": two_d_scale,
-        "spacing": two_d_spacing,
-    }
-
     viewer = napari.current_viewer()
     viewer.add_image(
         data=projected_data,
         name="Projection",
-        translate=two_d_translate,
-        metadata=two_d_metadata,
+        scale=image.scale,
+        translate=image.translate,
+        rotate=image.rotate,
+        plane=image.plane,
+        metadata=image.metadata,
     )
 
 
 def create_segmentation_widget() -> magicgui.widgets.Container:
     """Create a widget to segment a 3d (TYZ) timeseries"""
 
     segmentation_widget = epitools.widgets.create_segmentation_widget()
@@ -143,55 +126,55 @@
 
 def run_segmentation(
     image: napari.layers.Image,
     spot_sigma: float,
     outline_sigma: float,
     threshold: float,
 ) -> None:
-    """Segment a 3d timeserise (TYZ) at each frame"""
+    """Segment a 3D timeserise (TZYX) at each frame"""
 
     seeds_data, labels_data = epitools.analysis.calculate_segmentation(
         projection=image.data,
         spot_sigma=spot_sigma,
         outline_sigma=outline_sigma,
         threshold=threshold,
     )
 
-    labels_metadata = {
-        "scale": image.metadata["scale"],
-        "spacing": image.metadata["spacing"],
-    }
-
     viewer = napari.current_viewer()
     viewer.add_labels(
         data=labels_data,
+        scale=image.scale,
         translate=image.translate,
-        metadata=labels_metadata,
+        rotate=image.rotate,
+        plane=image.plane,
         name="Cells",
     )
     viewer.add_points(
         data=seeds_data,
         name="Seeds",
-        size=3,
+        size=3 * image.scale[-2:].mean(),
         edge_color="red",
         face_color="red",
+        scale=image.scale,
+        translate=image.translate,
+        rotate=image.rotate,
     )
 
 
 def create_cell_statistics_widget() -> magicgui.widgets.Container:
     """Create a widget for calculating cell statistics of labelled segmentations."""
 
     cell_statistics_widget = epitools.widgets.create_cell_statistics_widget()
     viewer = napari.current_viewer()
 
     # Update cell_statistics when scrolling through frames
     viewer.dims.events.current_step.connect(
         lambda event: _update_cell_statistics(
             layers=viewer.layers,
-            frame=event.value[0],
+            frame=event.value[0],  # pass in the time frame
         ),
     )
 
     # calculate cell_statistics when pressing 'Run' button
     cell_statistics_widget.run.changed.connect(
         lambda: run_cell_statistics(
             image=cell_statistics_widget.input_image.value,
@@ -253,18 +236,24 @@
 
 def run_cell_statistics(
     image: napari.layers.Image,
     labels: napari.layers.Labels,
 ) -> None:
     """Calculate cell statistics for all frames in the selected Image and Labels"""
 
+    pixel_spacing = (
+        image.metadata["yx_spacing"]
+        if "spacing" in image.metadata
+        else DEFAULT_PIXEL_SPACING
+    )
+
     cell_statistics, graphs = epitools.analysis.calculate_cell_statistics(
         image=image.data,
         labels=labels.data,
-        pixel_spacing=image.metadata["spacing"],
+        pixel_spacing=pixel_spacing,
     )
 
     # We will use these to update the cell stats at each frame
     labels.metadata["cell_statistics"] = cell_statistics
     labels.metadata["graphs"] = graphs
 
     # confirm calculation finished
```

### Comparing `epitools-0.0.1/src/epitools/napari.yaml` & `epitools-0.0.2/src/epitools/napari.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 name: epitools
 display_name: EpiTools
 contributions:
   commands:
     - id: epitools.get_reader
       python_name: epitools._reader:napari_get_reader
-      title: Open data with napari EpiTools
-    - id: epitools.write_multiple
-      python_name: epitools._writer:write_multiple
-      title: Save multi-layer data with napari EpiTools
+      title: Open data with EpiTools
     - id: epitools.write_single_image
       python_name: epitools._writer:write_single_image
-      title: Save image data with napari EpiTools
+      title: Save an image layer with EpiTools
+    - id: epitools.write_single_labels
+      python_name: epitools._writer:write_single_labels
+      title: Save a labels layer with EpiTools
     - id: epitools.load_sample_data
       python_name: epitools._sample_data:load_sample_data
-      title: Load sample data from napari EpiTools
+      title: Load sample data from EpiTools
     - id: epitools.projection_widget
       python_name: epitools.main:create_projection_widget
       title: Epitools Projection Widget
     - id: epitools.segmentation_widget
       python_name: epitools.main:create_segmentation_widget
       title: Epitools Segmentation Widget
     - id: epitools.cell_statistics_widget
       python_name: epitools.main:create_cell_statistics_widget
       title: Epitools cell statistics widget
   readers:
     - command: epitools.get_reader
       accepts_directories: false
       filename_patterns: ["*.tif", "*.tiff"]
   writers:
-    - command: epitools.write_multiple
-      layer_types: ["image*", "labels*"]
-      filename_extensions: []
     - command: epitools.write_single_image
       layer_types: ["image"]
-      filename_extensions: [".npy"]
+      filename_extensions: [".tif", ".tiff"]
+    - command: epitools.write_single_labels
+      layer_types: ["labels"]
+      filename_extensions: [".tif", ".tiff"]
   sample_data:
     - command: epitools.load_sample_data
-      display_name: napari EpiTools
+      display_name: EpiTools
       key: test_image
   widgets:
     - command: epitools.projection_widget
-      # autogenerate: true <- for use with napari-assistant
+      # autogenerate: true <- for use with assistant
       display_name: Projection (selective plane)
     - command: epitools.segmentation_widget
       display_name: Segmentation (local minima seeded watershed)
     - command: epitools.cell_statistics_widget
       display_name: Cell statistics
```

### Comparing `epitools-0.0.1/src/epitools/widgets/cell_statistics.py` & `epitools-0.0.2/src/epitools/widgets/cell_statistics.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools/widgets/projection.py` & `epitools-0.0.2/src/epitools/widgets/projection.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools/widgets/segmentation.py` & `epitools-0.0.2/src/epitools/widgets/segmentation.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/src/epitools.egg-info/PKG-INFO` & `epitools-0.0.2/src/epitools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 Metadata-Version: 2.1
 Name: epitools
-Version: 0.0.1
+Version: 0.0.2
 Summary: EpiTools Plugin
-Author-email: Napari Developer <yourname@example.com>
-License: 
-        Copyright (c) 2022, Napari Developer
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of epitools nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Author-email: "Daniel R. Matthews" <d.matthews@ucl.ac.uk>, Giulia Paci <g.paci@ucl.ac.uk>, "Pablo V. Munuera" <p.munuera@ucl.ac.uk>, "Patrick J. Roddy" <patrick.roddy@ucl.ac.uk>, "Paul J. Smith" <paul.j.smith@ucl.ac.uk>, Yanlan Mao <y.mao@ucl.ac.uk>
+License: BSD 3-Clause Licence
         
-Classifier: Development Status :: 2 - Pre-Alpha
+        Copyright (c) 2022-2023, EpiTools Developers All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+            Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+            Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+            Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Code, https://github.com/epitools/epitools
+Project-URL: Download, https://pypi.org/project/epitools
+Project-URL: Homepage, https://github.com/epitools/epitools
+Project-URL: Issues, https://github.com/epitools/epitools/issues
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -45,72 +33,44 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pyqt
 Provides-Extra: pyside
 Provides-Extra: qt
-License-File: LICENSE
+License-File: LICENCE.md
 
-# epitools
+# EpiTools
 
-[![License](https://img.shields.io/pypi/l/epitools.svg?color=green)](https://raw.githubusercontent.com/epitools/epitools/main/LICENSE)
+[![Licence](https://img.shields.io/pypi/l/epitools.svg?color=green)](https://raw.githubusercontent.com/epitools/epitools/main/LICENCE.md)
 [![PyPI](https://img.shields.io/pypi/v/epitools.svg?color=green)](https://pypi.org/project/epitools)
 [![Python Version](https://img.shields.io/pypi/pyversions/epitools.svg?color=green)](https://python.org)
 [![tests](https://github.com/epitools/epitools/actions/workflows/test.yml/badge.svg)](https://github.com/epitools/epitools/actions/workflows/test.yml)
 [![coverage](https://coveralls.io/repos/github/epitools/epitools/badge.svg?branch=main)](https://coveralls.io/github/epitools/epitools?branch=main)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/epitools)](https://napari-hub.org/plugins/epitools)
 
-EpiTools Plugin
-
----
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/index.html
--->
-
 ## Installation
 
-`epitools` is not yet available to install from PyPI or napari-hub.
-
-To install, please clone the repository and do a local install using `pip`:
+The recommended way to install `EpiTools` is via
+[pip](https://pypi.org/project/pip)
 
+```sh
+python -m pip install epitools
 ```
-git clone https://github.com/epitools/epitools.git
-cd epitools
-python -m pip install .
-```
-
-## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
+To install the latest development version of `EpiTools` clone this repository
+and run
 
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"epitools" is free and open source software
+```sh
+python -m pip install -e .
+```
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please
+[file an issue](https://github.com/epitools/epitools/issues) along with a
+detailed description.
+
+## Contributing
 
-[napari]: https://github.com/napari/napari
-[cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[mit]: http://opensource.org/licenses/MIT
-[bsd-3]: http://opensource.org/licenses/BSD-3-Clause
-[gnu gpl v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[gnu lgpl v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[apache software license 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[mozilla public license 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[pypi]: https://pypi.org/
+Contributions are very welcome. Tests can be run with [tox](https://tox.wiki),
+please ensure the coverage at least stays the same before you submit a pull request.
```

### Comparing `epitools-0.0.1/src/epitools.egg-info/SOURCES.txt` & `epitools-0.0.2/src/epitools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .gitignore
 .pre-commit-config.yaml
-LICENSE
+LICENCE.md
 README.md
 pyproject.toml
 .github/workflows/deploy.yml
 .github/workflows/linting.yml
 .github/workflows/test.yml
 .github/workflows/update_project_board.yml
 .napari/DESCRIPTION.md
@@ -18,30 +18,32 @@
 sample_data/8bitDataset/Benchmark/RegIm_wClahe.mat
 sample_data/8bitDataset/Benchmark/SegResults.mat
 sample_data/8bitDataset/Benchmark/Surfaces.mat
 sample_data/8bitDataset/Benchmark/TrackingStart.mat
 src/epitools/__init__.py
 src/epitools/_reader.py
 src/epitools/_sample_data.py
+src/epitools/_version.py
 src/epitools/_writer.py
 src/epitools/main.py
 src/epitools/napari.yaml
 src/epitools.egg-info/PKG-INFO
 src/epitools.egg-info/SOURCES.txt
 src/epitools.egg-info/dependency_links.txt
 src/epitools.egg-info/entry_points.txt
 src/epitools.egg-info/requires.txt
 src/epitools.egg-info/top_level.txt
 src/epitools/analysis/__init__.py
-src/epitools/analysis/_skeletonize.py
 src/epitools/analysis/cell_statistics.py
 src/epitools/analysis/projection.py
 src/epitools/analysis/segmentation.py
 src/epitools/widgets/__init__.py
 src/epitools/widgets/cell_statistics.py
+src/epitools/widgets/dialogue.py
 src/epitools/widgets/projection.py
 src/epitools/widgets/segmentation.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cell_statistics.py
+tests/test_dialogue.py
 tests/test_projection.py
 tests/test_segmentation.py
```

### Comparing `epitools-0.0.1/tests/conftest.py` & `epitools-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `epitools-0.0.1/tests/test_cell_statistics.py` & `epitools-0.0.2/tests/test_cell_statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
-import pytest
 
 from epitools.analysis import calculate_cell_statistics
 
 if TYPE_CHECKING:
     from typing import Callable
 
     import napari
@@ -65,29 +64,24 @@
     assert cells_layer.features.size == reference_stats[0].size
     assert np.allclose(
         cells_layer.features.to_numpy(),
         reference_stats[0].to_numpy(),
     )
 
 
-@pytest.mark.xfail(
-    raises=NotImplementedError,
-    reason="This test should be fixed by the changes in PR #67",
-    stict=True,
-)
 def test_calculate_cell_statistics(
     projected_image: napari.layers.Image,
     seeds_and_labels: tuple[napari.layers.Points, napari.layers.Labels],
 ):
     reference_seeds, reference_labels = seeds_and_labels
     reference_stats: pd.DataFrame = reference_labels.metadata["cell_statistics"]
 
     cell_statistics, graphs = calculate_cell_statistics(
         image=projected_image.data,
         labels=reference_labels.data,
-        pixel_spacing=reference_labels.metadata["spacing"],
+        pixel_spacing=reference_labels.metadata["yx_spacing"],
     )
 
     assert np.allclose(
         pd.DataFrame.from_dict(cell_statistics[0]).set_index("index").to_numpy(),
-        reference_stats.to_numpy(),
+        reference_stats[0].to_numpy(),
     )
```

### Comparing `epitools-0.0.1/tests/test_projection.py` & `epitools-0.0.2/tests/test_projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from epitools.analysis import calculate_projection
 
 SMOOTHING_RADIUS = 0.2
 SURFACE_SMOOTHNESS_1 = 50
 SURFACE_SMOOTHNESS_2 = 50
 CUT_OFF_DISTANCE = 20
-PROJECTION_NDIM = 3
+PROJECTION_NDIM = 4
 
 
 def test_add_projection_widget(
     make_napari_viewer: Callable,
 ):
     """Checks that the projection widget can be added inside a dock widget."""
 
@@ -68,10 +68,11 @@
         SURFACE_SMOOTHNESS_2,
         CUT_OFF_DISTANCE,
     )
 
     assert projection.ndim == PROJECTION_NDIM
     assert projection.shape == (
         1,  # single frame in the timeseries
+        1,  # single slice in Z
         image.data.shape[2],
         image.data.shape[3],
     )
```

### Comparing `epitools-0.0.1/tests/test_segmentation.py` & `epitools-0.0.2/tests/test_segmentation.py`

 * *Files identical despite different names*

